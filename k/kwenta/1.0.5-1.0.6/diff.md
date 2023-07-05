# Comparing `tmp/kwenta-1.0.5.tar.gz` & `tmp/kwenta-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.5.tar", last modified: Thu Jun  8 15:57:50 2023, max compression
+gzip compressed data, was "kwenta-1.0.6.tar", last modified: Wed Jul  5 21:17:38 2023, max compression
```

## Comparing `kwenta-1.0.5.tar` & `kwenta-1.0.6.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 15:57:13.000000 kwenta-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 15:57:50.630359 kwenta-1.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/alerts/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/cli/kwenta_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/contracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/contracts/json/
--rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/json/PerpsV2Market.json
--rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/json/PerpsV2MarketData.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/contracts/json/sUSD.json
--rw-r--r--   0 runner    (1001) docker     (123)    43018 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/pyth/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/pyth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/pyth/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/pyth/pyth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/queries/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/queries/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-08 15:57:13.000000 kwenta-1.0.5/kwenta/queries/queries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:57:50.630359 kwenta-1.0.5/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 15:57:50.000000 kwenta-1.0.5/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:57:50.630359 kwenta-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 15:57:13.000000 kwenta-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 21:17:07.000000 kwenta-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 21:17:38.351922 kwenta-1.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.347922 kwenta-1.0.6/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/cli/kwenta_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/contracts/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2ExchangeRate.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37179 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2Market.json
+-rw-r--r--   0 runner    (1001) docker     (123)    43146 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/PerpsV2MarketData.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/SMAccount.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/SMFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/contracts/json/sUSD.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56577 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/pyth/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-07-05 21:17:07.000000 kwenta-1.0.6/kwenta/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:17:38.351922 kwenta-1.0.6/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-05 21:17:38.000000 kwenta-1.0.6/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:17:38.351922 kwenta-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-05 21:17:07.000000 kwenta-1.0.6/setup.py
```

### Comparing `kwenta-1.0.5/PKG-INFO` & `kwenta-1.0.6/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.5/kwenta/alerts/alerts.py` & `kwenta-1.0.6/kwenta/alerts/alerts.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import requests
 
 
 class Alerts:
     def __init__(self, telegram_token: str = None, telegram_channel_name: str = None):
         if not telegram_token or not telegram_channel_name:
             raise Exception(
-                "Must specify both a `telegram_token` and `telegram_channel_name")
+                "Must specify both a `telegram_token` and `telegram_channel_name"
+            )
 
         self._telegram_token = telegram_token
         self._telegram_channel_name = telegram_channel_name
 
     def send_message(text: str, max_retry: int = 5) -> None:
         """
         Send Message to Telegram Channel
@@ -27,15 +28,15 @@
         """
         url = f"https://api.telegram.org/bot{self._telegram_token}/sendMessage?chat_id={self._telegram_channel_name}&text={text}"
 
         attempt = 1
         while attempt <= max_retry:
             try:
                 request = requests.post(url)
-                if (request.status_code == 200):
+                if request.status_code == 200:
                     break
                 else:
                     attempt += 1
                     time.sleep(1)
                     continue
             except BaseException:
                 attempt += 1
```

### Comparing `kwenta-1.0.5/kwenta/cli/kwenta_cli.py` & `kwenta-1.0.6/kwenta/cli/kwenta_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             telegram_token=kwenta_params["telegram_token"],
             telegram_channel_name=kwenta_params["telegram_channel_name"]
         )
         return kwenta_instance
     except Exception as e:
         print(e)
 
-    
 @click.command()
 @click.argument('token_symbol', type=str)
 @click.pass_context
 def get_market_contract(ctx, token_symbol):
     try:
         market_contract = kwenta_instance.get_market_contract(token_symbol.upper())
         click.echo(f"Market contract for {token_symbol.upper()}: {market_contract.address}")
@@ -109,18 +108,18 @@
         click.echo(f"Current position for {token_symbol.upper()} and wallet {wallet_address}: {position}")
     except Exception as e:
         click.echo(f"Error1: {str(e)}")
 
 @click.command()
 @click.argument('token_symbol', type=str)
 @click.pass_context
-def get_accessible_margin(ctx, token_symbol):
+def get_accessible_margin(ctx, address):
     try:
-        result = kwenta_instance.get_accessible_margin(token_symbol.upper())
-        click.echo(f"Accessible margin for {token_symbol.upper()}: {result}")
+        result = kwenta_instance.get_accessible_margin(address)
+        click.echo(f"Accessible margin for {address}: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.argument('token_symbol', type=str)
 @click.option('--wallet-address', help='The wallet address to check (optional).')
 @click.pass_context
@@ -165,17 +164,17 @@
         result = kwenta_instance.get_market_skew(token_symbol.upper())
         click.echo(f"Market skew for {token_symbol.upper()}: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.pass_context
-def get_susd_balance(ctx):
+def get_susd_balance(ctx,wallet_address):
     try:
-        result = kwenta_instance.get_susd_balance()
+        result = kwenta_instance.get_susd_balance(wallet_address)
         click.echo(f"sUSD balance: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 
 @click.command()
 @click.argument("token_symbol", type=str)
@@ -190,50 +189,50 @@
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.argument("token_symbol", type=str)
 @click.argument("token_amount", type=int)
 @click.option("--execute_now", is_flag=True)
 @click.pass_context
-def transfer_margin(ctx, token_symbol, token_amount, execute_now):
+def transfer_margin(ctx, token_symbol, token_amount, skip_approval:bool =False,execute_now:bool =False,withdrawal_all:bool =False):
     try:
-        result = kwenta_instance.transfer_margin(token_symbol.upper(), token_amount, execute_now)
+        result = kwenta_instance.transfer_margin(token_symbol.upper(), token_amount, execute_now=execute_now,withdrawal_all=withdrawal_all)
         if execute_now:
             click.echo(f"Token transfer Tx id: {result}")
         else:
             click.echo(f"Token transfer data: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.argument("token_symbol", type=str)
 @click.argument("size_delta", type=float)
 @click.option("--slippage", type=float, default=DEFAULT_SLIPPAGE)
 @click.option("--execute_now", is_flag=True)
 @click.option("--self_execute", is_flag=True)
 @click.pass_context
-def modify_position(ctx, token_symbol, size_delta, slippage, execute_now, self_execute):
+def modify_position(ctx, token_symbol, size_delta, slippage,wallet_address, execute_now:bool = False, self_execute:bool = False):
     try:
-        result = kwenta_instance.modify_position(token_symbol.upper(), size_delta, slippage, execute_now, self_execute)
+        result = kwenta_instance.modify_position(token_symbol.upper(), size_delta, slippage, wallet_address,execute_now, self_execute)
         if execute_now:
             click.echo(f"Modify position Tx id: {result}")
         else:
             click.echo(f"Modify position data: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.argument("token_symbol", type=str)
 @click.option("--slippage", type=float, default=DEFAULT_SLIPPAGE)
 @click.option("--execute_now", is_flag=True)
 @click.option("--self_execute", is_flag=True)
 @click.pass_context
-def close_position(ctx, token_symbol, slippage, execute_now, self_execute):
+def close_position(ctx, token_symbol, slippage, wallet_address, execute_now, self_execute):
     try:
-        result = kwenta_instance.close_position(token_symbol.upper(), slippage, execute_now, self_execute)
+        result = kwenta_instance.close_position(token_symbol.upper(), slippage,wallet_address, execute_now, self_execute)
         if execute_now:
             click.echo(f"Close position Tx id: {result}")
         else:
             click.echo(f"Close position data: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
@@ -242,55 +241,65 @@
 @click.option("--short", is_flag=True)
 @click.option("--size_delta", type=float)
 @click.option("--slippage", type=float, default=DEFAULT_SLIPPAGE)
 @click.option("--leverage_multiplier", type=float)
 @click.option("--execute_now", is_flag=True)
 @click.option("--self_execute", is_flag=True)
 @click.pass_context
-def open_position(ctx, token_symbol, short, size_delta, slippage, leverage_multiplier, execute_now, self_execute):
+def open_position(ctx, token_symbol,wallet_address, short:bool = False, position_size:float =None, slippage:float = 2, leverage_multiplier:float=None, execute_now:bool = False, self_execute:bool = False):
     try:
-        result = kwenta_instance.open_position(token_symbol.upper(), short, size_delta, slippage, leverage_multiplier, execute_now, self_execute)
+        result = kwenta_instance.open_position(token_symbol.upper(),wallet_address, short=short, position_size=position_size, slippage=slippage, leverage_multiplier=leverage_multiplier, execute_now=execute_now, self_execute=self_execute)
         if execute_now:
             click.echo(f"Open position Tx id: {result}")
         else:
             click.echo(f"Open position data: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
 @click.argument("order_id", type=int)
 @click.option("--execute_now", is_flag=True)
 @click.pass_context
-def cancel_order(ctx, order_id, execute_now):
+def cancel_order(ctx, token_symbol, account,execute_now: bool = False):
     try:
-        result = kwenta_instance.cancel_order(order_id, execute_now)
+        result = kwenta_instance.cancel_order(token_symbol, account,execute_now=execute_now)
         if execute_now:
             click.echo(f"Cancel order Tx id: {result}")
         else:
             click.echo(f"Cancel order data: {result}")
     except Exception as e:
         click.echo(f"Error: {str(e)}")
 
 @click.command()
-@click.argument("token_symbol", type=str)
-@click.argument("order_type", type=click.Choice(["market", "limit"], case_sensitive=False))
-@click.argument("side", type=click.Choice(["buy", "sell"], case_sensitive=False))
-@click.argument("amount", type=float)
-@click.option("--price", type=float, default=None)
-@click.option("--execute_now", is_flag=True)
+@click.argument("sm_accounts", type=int)
 @click.pass_context
-def execute_order(ctx, token_symbol, order_type, side, amount, price, execute_now):
+def sm_accounts(ctx, wallet_address):
     try:
-        result = kwenta_instance.execute_order(token_symbol.upper(), order_type, side, amount, price, execute_now)
-        if execute_now:
-            click.echo(f"Execute order Tx id: {result}")
-        else:
-            click.echo(f"Execute order data: {result}")
+        if wallet_address is None:
+            wallet_address = kwenta_instance.wallet_address
+        accounts = kwenta_instance.get_sm_accounts()
+        click.echo(f"SM Accounts: {accounts}")
     except Exception as e:
-        click.echo(f"Error: {str(e)}")
+        click.echo(f"Error1: {str(e)}")
+
+@click.command()
+@click.argument("create_sm_account", type=int)
+@click.pass_context
+def sm_accounts(ctx, wallet_address,execute_now: bool = False):
+    try:
+        if wallet_address is None:
+            wallet_address = kwenta_instance.wallet_address
+        accounts = kwenta_instance.new_sm_account(wallet_address,execute_now=execute_now)
+        click.echo(f"Creating new SM Account: {accounts}")
+        sm_accounts = kwenta_instance.get_sm_accounts()
+        click.echo(f"SM Accounts: {sm_accounts[-1]}")
+    except Exception as e:
+        click.echo(f"Error1: {str(e)}")
+
+
 
 kwenta_cli.add_command(configure)
 kwenta_cli.add_command(get_market_contract)
 kwenta_cli.add_command(check_delayed_orders)
 kwenta_cli.add_command(get_current_asset_price)
 kwenta_cli.add_command(get_current_position)
 kwenta_cli.add_command(get_accessible_margin)
@@ -301,15 +310,15 @@
 kwenta_cli.add_command(get_susd_balance)
 kwenta_cli.add_command(get_leveraged_amount)
 kwenta_cli.add_command(transfer_margin)
 kwenta_cli.add_command(modify_position)
 kwenta_cli.add_command(close_position)
 kwenta_cli.add_command(open_position)
 kwenta_cli.add_command(cancel_order)
-kwenta_cli.add_command(execute_order)
+kwenta_cli.add_command(sm_accounts)
 
 if __name__ == '__main__':
     try:
         state_file = os.path.join(os.getcwd(), 'kwenta_state.pickle')
         kwenta_instance = load_kwenta_instance(state_file)
         click.echo("Kwenta instance loaded from the state file.")
     except Exception as e:
```

### Comparing `kwenta-1.0.5/kwenta/contracts/contracts.py` & `kwenta-1.0.6/kwenta/contracts/contracts.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,47 @@
 
 # read abi files
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2MarketData.json') as json_file:
     PerpsV2MarketData_abi = json.load(json_file)
 
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2Market.json') as json_file:
     PerpsV2Market_abi = json.load(json_file)
+    
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/PerpsV2ExchangeRate.json') as json_file:
+    PerpsV2ExchangeRate_abi = json.load(json_file)
+
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/SMFactory.json') as json_file:
+    SMFactory_abi = json.load(json_file)
 
 with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/sUSD.json') as json_file:
     sUSD_abi = json.load(json_file)
 
+with open(f'{os.path.dirname(os.path.abspath(__file__))}/json/SMAccount.json') as json_file:
+    SM_Account_abi= json.load(json_file)
+
+
 # create dictionaries
 addresses = {
     "sUSD": {
         10: '0x8c6f28f2f1a3c87f0f938b96d27520d9751ec8d9',
         420: '0xeBaEAAD9236615542844adC5c149F86C36aD1136'
     },
     "PerpsV2MarketData": {
         10: '0x58e6227510F83d3F45B339F2f7A05a699fDEE6D4',
         420: '0xcE2dC389fc8Be231beECED1D900881e38596d7b2',
     },
+    "PerpsV2ExchangeRate": {
+        10: '0x2C15259D4886e2C0946f9aB7a5E389c86b3c3b04',
+    },
+    "SMFactory": {
+        10: '0x8234F990b149Ae59416dc260305E565e5DAfEb54',
+    },
 }
 
 abis = {
     "sUSD": sUSD_abi,
     "PerpsV2Market": PerpsV2Market_abi,
-    "PerpsV2MarketData": PerpsV2MarketData_abi
+    "PerpsV2MarketData": PerpsV2MarketData_abi,
+    "PerpsV2ExchangeRate": PerpsV2ExchangeRate_abi,
+    "SMFactory": SMFactory_abi,
+    "SM_Account":SM_Account_abi
 }
```

### Comparing `kwenta-1.0.5/kwenta/contracts/json/PerpsV2Market.json` & `kwenta-1.0.6/kwenta/contracts/json/PerpsV2Market.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/contracts/json/PerpsV2MarketData.json` & `kwenta-1.0.6/kwenta/contracts/json/PerpsV2MarketData.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/contracts/json/sUSD.json` & `kwenta-1.0.6/kwenta/contracts/json/sUSD.json`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/kwenta.py` & `kwenta-1.0.6/kwenta/kwenta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,74 @@
 import asyncio
 import time
 import warnings
 from web3 import Web3
 from web3.types import TxParams
 from web3.middleware import geth_poa_middleware
 from decimal import Decimal
-from .constants import DEFAULT_NETWORK_ID, DEFAULT_TRACKING_CODE, DEFAULT_SLIPPAGE, DEFAULT_GQL_ENDPOINT_PERPS, DEFAULT_GQL_ENDPOINT_RATES, DEFAULT_PRICE_SERVICE_ENDPOINTS
+from .constants import (
+    DEFAULT_NETWORK_ID,
+    DEFAULT_TRACKING_CODE,
+    DEFAULT_SLIPPAGE,
+    DEFAULT_GQL_ENDPOINT_PERPS,
+    DEFAULT_GQL_ENDPOINT_RATES,
+    DEFAULT_PRICE_SERVICE_ENDPOINTS,
+)
 from .contracts import abis, addresses
 from .alerts import Alerts
 from .queries import Queries
 from .pyth import Pyth
+from eth_abi import encode
 
-warnings.filterwarnings('ignore')
+warnings.filterwarnings("ignore")
 
 
 class Kwenta:
     def __init__(
-            self,
-            provider_rpc: str,
-            wallet_address: str,
-            private_key: str = None,
-            network_id: int = None,
-            use_estimate_gas: bool = True,
-            gql_endpoint_perps: str = None,
-            gql_endpoint_rates: str = None,
-            price_service_endpoint: str = None,
-            telegram_token: str = None,
-            telegram_channel_name: str = None):
+        self,
+        provider_rpc: str,
+        wallet_address: str,
+        sm_address: str = None,
+        private_key: str = None,
+        network_id: int = None,
+        use_estimate_gas: bool = True,
+        gql_endpoint_perps: str = None,
+        gql_endpoint_rates: str = None,
+        price_service_endpoint: str = None,
+        telegram_token: str = None,
+        telegram_channel_name: str = None,
+    ):
         # set default values
         if network_id is None:
             network_id = DEFAULT_NETWORK_ID
 
         # init account variables
         self.private_key = private_key
         self.wallet_address = wallet_address
         self.use_estimate_gas = use_estimate_gas
         self.provider_rpc = provider_rpc
-
         # init provider
-        if provider_rpc.startswith('https'):
+        if provider_rpc.startswith("https"):
             self.provider_class = Web3.HTTPProvider
-        elif provider_rpc.startswith('wss'):
+        elif provider_rpc.startswith("wss"):
             self.provider_class = Web3.WebsocketProvider
         else:
             raise Exception("RPC endpoint is invalid")
 
         self.network_id = network_id
 
         # init contracts
-        self.markets, self.market_contracts, self.susd_token = self._load_markets()
+        (
+            self.markets,
+            self.market_contracts,
+            self.susd_token,
+            self.sm_account,
+        ) = self._load_markets()
+        if sm_address is not None:
+            self.sm_account = sm_address
         self.token_list = list(self.markets.keys())
 
         # init alerts
         if telegram_token and telegram_channel_name:
             self.alerts = Alerts(telegram_token, telegram_channel_name)
 
         # init queries
@@ -61,54 +77,58 @@
 
         if not gql_endpoint_rates:
             gql_endpoint_rates = DEFAULT_GQL_ENDPOINT_RATES[self.network_id]
 
         self.queries = Queries(
             self,
             gql_endpoint_perps=gql_endpoint_perps,
-            gql_endpoint_rates=gql_endpoint_rates)
+            gql_endpoint_rates=gql_endpoint_rates,
+        )
 
         # init pyth
         if not price_service_endpoint:
             price_service_endpoint = DEFAULT_PRICE_SERVICE_ENDPOINTS[self.network_id]
 
-        self.pyth = Pyth(
-            self.network_id, price_service_endpoint=price_service_endpoint)
+        self.pyth = Pyth(self.network_id, price_service_endpoint=price_service_endpoint)
 
     @property
     def web3(self):
         w3 = Web3(self.provider_class(self.provider_rpc))
 
         if w3.eth.chain_id != self.network_id:
             raise Exception("The RPC `chain_id` must match the stored `network_id`")
         else:
             w3.middleware_onion.inject(geth_poa_middleware, layer=0)
-            self.nonce = w3.eth.get_transaction_count(self.wallet_address)
+            # self.nonce = w3.eth.get_transaction_count(self.wallet_address)
             return w3
 
-
     def _load_markets(self):
         """
         Initializes all market contracts
         ...
 
         Attributes
         ----------
         N/A
         """
-        marketdata_contract = self.web3.eth.contract(self.web3.to_checksum_address(
-            addresses['PerpsV2MarketData'][self.network_id]), abi=abis['PerpsV2MarketData'])
+        marketdata_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(
+                addresses["PerpsV2MarketData"][self.network_id]
+            ),
+            abi=abis["PerpsV2MarketData"],
+        )
         allmarketsdata = (
-            marketdata_contract.functions.allProxiedMarketSummaries().call())
+            marketdata_contract.functions.allProxiedMarketSummaries().call()
+        )
         markets = {}
         market_contracts = {}
         for market in allmarketsdata:
             normalized_market = {
                 "market_address": market[0],
-                "asset": market[1].decode('utf-8').strip("\x00"),
+                "asset": market[1].decode("utf-8").strip("\x00"),
                 "key": market[2],
                 "maxLeverage": market[3],
                 "price": market[4],
                 "marketSize": market[5],
                 "marketSkew": market[6],
                 "marketDebt": market[7],
                 "currentFundingRate": market[8],
@@ -116,32 +136,33 @@
                 "takerFee": market[10][0],
                 "makerFee": market[10][1],
                 "takerFeeDelayedOrder": market[10][2],
                 "makerFeeDelayedOrder": market[10][3],
                 "takerFeeOffchainDelayedOrder": market[10][4],
                 "makerFeeOffchainDelayedOrder": market[10][5],
             }
-
             # set them
-            token_symbol = market[2].decode('utf-8').strip("\x00")[1:-4]
+            token_symbol = market[2].decode("utf-8").strip("\x00")[1:-4]
             markets[token_symbol] = normalized_market
             market_contracts[token_symbol] = self.web3.eth.contract(
-                self.web3.to_checksum_address(
-                    normalized_market['market_address']),
-                abi=abis['PerpsV2Market'])
+                self.web3.to_checksum_address(normalized_market["market_address"]),
+                abi=abis["PerpsV2Market"],
+            )
 
         # load sUSD contract
-        susd_token = self.web3.eth.contract(self.web3.to_checksum_address(
-            addresses['sUSD'][self.network_id]), abi=abis['sUSD'])
+        susd_token = self.web3.eth.contract(
+            self.web3.to_checksum_address(addresses["sUSD"][self.network_id]),
+            abi=abis["sUSD"],
+        )
+
+        sm_account = self.get_sm_accounts()[0]
 
-        return markets, market_contracts, susd_token
+        return markets, market_contracts, susd_token, sm_account
 
-    def _get_tx_params(
-        self, value=0, to=None
-    ) -> TxParams:
+    def _get_tx_params(self, value=0, to=None) -> TxParams:
         """
         Get the default tx params
         ...
 
         Attributes
         ----------
         value : int
@@ -150,21 +171,22 @@
             address to send to
 
         Returns
         -------
         params : dict
             transaction parameters to be completed with another function
         """
+
         params: TxParams = {
-            'from': self.wallet_address,
-            'to': to,
-            'chainId': self.network_id,
-            'value': value,
-            'gasPrice': self.web3.eth.gas_price,
-            'nonce': self.nonce
+            "from": self.wallet_address,
+            "to": to,
+            "chainId": self.network_id,
+            "value": value,
+            "gasPrice": self.web3.eth.gas_price,
+            "nonce": self.web3.eth.get_transaction_count(self.wallet_address),
         }
         return params
 
     def get_market_contract(self, token_symbol: str):
         """
         Run checks and return market contract if it exists
         ...
@@ -197,49 +219,103 @@
         if "gas" not in tx_data:
             if self.use_estimate_gas:
                 tx_data["gas"] = int(self.web3.eth.estimate_gas(tx_data) * 1.2)
             else:
                 tx_data["gas"] = 1500000
 
         signed_txn = self.web3.eth.account.sign_transaction(
-            tx_data, private_key=self.private_key)
-        tx_token = self.web3.eth.send_raw_transaction(
-            signed_txn.rawTransaction)
-
-        # increase nonce
-        self.nonce += 1
-
+            tx_data, private_key=self.private_key
+        )
+        tx_token = self.web3.eth.send_raw_transaction(signed_txn.rawTransaction)
+        # increase nonce -- getting directly from wallet
+        # self.nonce += 1
         return self.web3.to_hex(tx_token)
 
-    def check_delayed_orders(self, token_symbol: str, wallet_address: str = None) -> dict:
+    def check_delayed_orders(self, token_symbol: str, sm_address: str = None) -> dict:
         """
         Check if delayed order is in queue
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
-        wallet_address : str
+        sm_address : str
             wallet address to check for delayed order
         """
-        if not wallet_address:
-            wallet_address = self.wallet_address
+        if not sm_address:
+            sm_address = self.sm_account
         market_contract = self.market_contracts[token_symbol]
-        delayed_order = market_contract.functions.delayedOrders(
-            wallet_address).call()
+        delayed_order = market_contract.functions.delayedOrders(sm_address).call()
 
         return {
-            'is_open': True if delayed_order[2] > 0 else False,
-            'size_delta': delayed_order[1],
-            'desired_fill_price': delayed_order[2],
-            'intention_time': int(delayed_order[7]),
-            'executable_time': int(delayed_order[7]) + 15 if int(delayed_order[7]) > 0 else 0,
+            "is_open": True if delayed_order[2] > 0 else False,
+            "position_size": delayed_order[1],
+            "desired_fill_price": delayed_order[2],
+            "intention_time": int(delayed_order[7]),
+            "executable_time": int(delayed_order[7]) + 15
+            if int(delayed_order[7]) > 0
+            else 0,
         }
 
+    def get_sm_accounts(self, wallet_address: str = None) -> dict:
+        """
+        Gets all the smartmargin accounts for the wallet
+        ...
+
+        Attributes
+        ----------
+        wallet_address : str
+        """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+        exch_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(addresses["SMFactory"][self.network_id]),
+            abi=abis["SMFactory"],
+        )
+        sm_accounts = exch_contract.functions.getAccountsOwnedBy(wallet_address).call()
+        return sm_accounts
+
+    def new_sm_account(
+        self, wallet_address: str = None, execute_now: bool = False
+    ) -> dict:
+        """
+        Creates new smart margin account
+        ...
+
+        Attributes
+        ----------
+        token_symbol : str
+            token symbol from list of supported asset
+        wallet_address : str
+            wallet address to check for delayed order
+        """
+        if not wallet_address:
+            wallet_address = self.wallet_address
+        exch_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(addresses["SMFactory"][self.network_id]),
+            abi=abis["SMFactory"],
+        )
+        # new_account = (exch_contract.functions.newAccount().call())
+        data_tx = data_tx = exch_contract.encodeABI(fn_name="newAccount", args=[])
+        tx_params = self._get_tx_params(
+            to=self.web3.to_checksum_address(addresses["SMFactory"][self.network_id])
+        )
+        tx_params["data"] = data_tx
+        # print(tx_params)
+        if execute_now:
+            tx_token = self.execute_transaction(tx_params)
+            print(f"Creating New SM Account")
+            print(f"TX: {tx_token}")
+            time.sleep(4)
+            print(f"SM Accounts: {self.get_sm_accounts()}")
+            return tx_token
+        else:
+            return tx_params
+
     def get_current_asset_price(self, token_symbol: str) -> dict:
         """
         Gets current asset price for config asset.
         ...
 
         Attributes
         ----------
@@ -248,77 +324,82 @@
 
         Returns
         ----------
         Dict with wei and USD price
         """
         market_contract = self.market_contracts[token_symbol.upper()]
         wei_price = (market_contract.functions.assetPrice().call())[0]
-        usd_price = self.web3.from_wei(wei_price, 'ether')
+        usd_price = self.web3.from_wei(wei_price, "ether")
         return {"usd": usd_price, "wei": wei_price}
 
-    def get_current_position(self, token_symbol: str, wallet_address: str = None) -> dict:
+    def get_current_position(
+        self, token_symbol: str, wallet_address: str = None
+    ) -> dict:
         """
         Gets Current Position Data
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: position information
         """
         if not wallet_address:
-            wallet_address = self.wallet_address
+            wallet_address = self.sm_account
 
         market_contract = self.get_market_contract(token_symbol)
-        id, last_funding_index, margin, last_price, size = market_contract.functions.positions(
-            wallet_address).call()
+        (
+            id,
+            last_funding_index,
+            margin,
+            last_price,
+            size,
+        ) = market_contract.functions.positions(wallet_address).call()
         current_asset_price = self.get_current_asset_price(token_symbol)
 
         # clean usd values
         is_short = -1 if size < 0 else 1
-        size_ether = self.web3.from_wei(abs(size), 'ether') * is_short
-        last_price_usd = self.web3.from_wei(last_price, 'ether')
+        size_ether = self.web3.from_wei(abs(size), "ether") * is_short
+        last_price_usd = self.web3.from_wei(last_price, "ether")
 
         # calculate pnl
-        price_diff = current_asset_price['usd'] - last_price_usd
+        price_diff = current_asset_price["usd"] - last_price_usd
         pnl = size_ether * price_diff * is_short
 
         positions_data = {
             "id": id,
             "last_funding_index": last_funding_index,
             "margin": margin,
             "last_price": last_price,
             "size": size,
-            "pnl_usd": pnl}
+            "pnl_usd": pnl,
+        }
         return positions_data
 
-    def get_accessible_margin(self, token_symbol: str) -> dict:
+    def get_accessible_margin(self, address: str) -> dict:
         """
-        Gets available account margin
+        Gets available NON-MARKET account margin
         ...
 
         Attributes
         ----------
         wallet_address : str
             wallet_address of wallet to check
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: Margin remaining in wei and usd
         """
-        market_contract = self.get_market_contract(token_symbol)
-        margin_allowed = (market_contract.functions.accessibleMargin(
-            self.wallet_address).call())[0]
-        margin_usd = self.web3.from_wei(margin_allowed, 'ether')
-        return {"margin_remaining": margin_allowed,
-                "margin_remaining_usd": margin_usd}
+        margin_allowed = self.get_susd_balance(address)["balance"]
+        margin_usd = self.web3.from_wei(margin_allowed, "ether")
+        return {"margin_remaining": margin_allowed, "margin_remaining_usd": margin_usd}
 
     def can_liquidate(self, token_symbol: str, wallet_address: str = None) -> dict:
         """
         Checks if Liquidation is possible for wallet
         ...
 
         Attributes
@@ -326,24 +407,31 @@
         token_symbol : str
             token symbol from list of supported asset
         Returns
         ----------
         Dict: Liquidation Data
         """
         if not wallet_address:
-            wallet_address = self.wallet_address
+            wallet_address = self.sm_account
         market_contract = self.get_market_contract(token_symbol)
         liquidation_check = market_contract.functions.canLiquidate(
-            wallet_address).call()
+            wallet_address
+        ).call()
         liquidation_price = market_contract.functions.liquidationPrice(
-            wallet_address).call()
-        return {"liq_possible": liquidation_check,
-                "liq_price": liquidation_price}
-
-    def liquidate_position(self, token_symbol: str, wallet_address: str=None,skip_check:bool=False, execute_now: bool = False) -> dict:
+            wallet_address
+        ).call()
+        return {"liq_possible": liquidation_check, "liq_price": liquidation_price}
+
+    def liquidate_position(
+        self,
+        token_symbol: str,
+        wallet_address: str = None,
+        skip_check: bool = False,
+        execute_now: bool = False,
+    ) -> dict:
         """
         Checks if Liquidation is possible for wallet
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -351,57 +439,61 @@
         wallet_address : str
             Wallet address to liquidate
         Returns
         ----------
         Dict: Liquidation of position
         """
         if not wallet_address:
-            wallet_address = self.wallet_address
+            wallet_address = self.sm_account
         market_contract = self.get_market_contract(token_symbol)
         if skip_check:
             data_tx = market_contract.encodeABI(
-                fn_name='liquidatePosition', args=[wallet_address])
-            tx_params = self._get_tx_params(
-                to=market_contract.address)
-            tx_params['data'] = data_tx
+                fn_name="liquidatePosition", args=[wallet_address]
+            )
+            tx_params = self._get_tx_params(to=market_contract.address)
+            tx_params["data"] = data_tx
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Executing Liquidation for {token_symbol}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {
-                    "token": token_symbol.upper(),
-                    "tx_data": tx_params}
+                return {"token": token_symbol.upper(), "tx_data": tx_params}
         liquidation_check = market_contract.functions.canLiquidate(
-            self.wallet_address).call()
+            self.wallet_address
+        ).call()
         # check for if liquidation is possible
         if liquidation_check == True:
             data_tx = market_contract.encodeABI(
-                fn_name='liquidatePosition', args=[wallet_address])
-            tx_params = self._get_tx_params(
-                to=market_contract.address)
-            tx_params['data'] = data_tx
+                fn_name="liquidatePosition", args=[wallet_address]
+            )
+            tx_params = self._get_tx_params(to=market_contract.address)
+            tx_params["data"] = data_tx
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Executing Liquidation for {token_symbol}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {
-                    "token": token_symbol.upper(),
-                    "tx_data": tx_params}
+                return {"token": token_symbol.upper(), "tx_data": tx_params}
         else:
             return {
                 "token": token_symbol.upper(),
-                "tx_data": "N/A, Cannot Liquidate Position."}
+                "tx_data": "N/A, Cannot Liquidate Position.",
+            }
 
-    def flag_position(self, token_symbol: str, wallet_address: str=None,skip_check:bool=False, execute_now: bool = False) -> dict:
+    def flag_position(
+        self,
+        token_symbol: str,
+        wallet_address: str = None,
+        skip_check: bool = False,
+        execute_now: bool = False,
+    ) -> dict:
         """
         Checks if Liquidation is possible for wallet
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -409,55 +501,53 @@
         wallet_address : str
             Wallet address to flag for liquidation
         Returns
         ----------
         Dict: flag Liquidation of position
         """
         if not wallet_address:
-            wallet_address = self.wallet_address
+            wallet_address = self.sm_account
         market_contract = self.get_market_contract(token_symbol)
         if skip_check:
             data_tx = market_contract.encodeABI(
-                fn_name='flagPosition', args=[wallet_address])
-            tx_params = self._get_tx_params(
-                to=market_contract.address)
-            tx_params['data'] = data_tx
+                fn_name="flagPosition", args=[wallet_address]
+            )
+            tx_params = self._get_tx_params(to=market_contract.address)
+            tx_params["data"] = data_tx
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Executing Flag for {token_symbol}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {
-                    "token": token_symbol.upper(),
-                    "tx_data": tx_params}
+                return {"token": token_symbol.upper(), "tx_data": tx_params}
         liquidation_check = market_contract.functions.canLiquidate(
-            self.wallet_address).call()
+            self.wallet_address
+        ).call()
         # check for if liquidation is possible
         if liquidation_check == True:
             data_tx = market_contract.encodeABI(
-                fn_name='flagPosition', args=[wallet_address])
-            tx_params = self._get_tx_params(
-                to=market_contract.address)
-            tx_params['data'] = data_tx
+                fn_name="flagPosition", args=[wallet_address]
+            )
+            tx_params = self._get_tx_params(to=market_contract.address)
+            tx_params["data"] = data_tx
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
                 print(f"Executing Flag for {token_symbol}")
                 print(f"TX: {tx_token}")
                 time.sleep(1)
                 return tx_token
             else:
-                return {
-                    "token": token_symbol.upper(),
-                    "tx_data": tx_params}
+                return {"token": token_symbol.upper(), "tx_data": tx_params}
         else:
             return {
                 "token": token_symbol.upper(),
-                "tx_data": "N/A, Cannot Flag Position."}
+                "tx_data": "N/A, Cannot Flag Position.",
+            }
 
     def get_market_skew(self, token_symbol: str) -> dict:
         """
         Gets current market long/short market skew
         ...
 
         Attributes
@@ -474,37 +564,41 @@
         total = long + short
         if total == 0:
             percent_long = 0
             percent_short = 0
         else:
             percent_long = long / total * 100
             percent_short = short / total * 100
-        return {"long": long, "short": short,
-                "percent_long": percent_long, "percent_short": percent_short}
+        return {
+            "long": long,
+            "short": short,
+            "percent_long": percent_long,
+            "percent_short": percent_short,
+        }
 
-    def get_susd_balance(self) -> dict:
+    def get_susd_balance(self, address: str) -> dict:
         """
         Gets current sUSD Balance in wallet
         ...
 
         Attributes
         ----------
         wallet_address : str
             wallet_address of wallet to check
         Returns
         ----------
         Dict: wei and usd sUSD balance
         """
-        balance = self.susd_token.functions.balanceOf(
-            self.wallet_address).call()
-        balance_usd = self.web3.from_wei(balance, 'ether')
+        balance = self.susd_token.functions.balanceOf(address).call()
+        balance_usd = self.web3.from_wei(balance, "ether")
         return {"balance": balance, "balance_usd": balance_usd}
 
-    def get_leveraged_amount(self, token_symbol: str,
-                             leverage_multiplier: float) -> dict:
+    def get_leveraged_amount(
+        self, token_symbol: str, leverage_multiplier: float, wallet_address: str = None
+    ) -> dict:
         """
         Get out amount of leverage available for account
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -516,299 +610,489 @@
         ----------
         Dict: amount of leverage available and max amount of leverage available
         """
         if leverage_multiplier is not None:
             if leverage_multiplier > 24.7 or leverage_multiplier < 0.1:
                 print("Leveraged_multiplier must be within the range 0.1 - 24.7!")
                 return None
-        margin = self.get_accessible_margin(token_symbol)
+        if wallet_address is None:
+            wallet_address = self.sm_account
+        margin = (
+            self.get_current_position(token_symbol, wallet_address=wallet_address)
+        )["margin"]
         asset_price = self.get_current_asset_price(token_symbol)
-        print(f"SUSD Available: {margin['margin_remaining_usd']}")
-        print(f"Current Asset Price: {asset_price['usd']}")
+        # print(f"SUSD Available: {margin}")
+        # print(f"Current Asset Price: {asset_price['usd']}")
         # Using 24.7 to cover edge cases
         max_leverage = self.web3.to_wei(
-            (margin['margin_remaining_usd'] /
-             asset_price['usd']) *
-            Decimal(24.7),
-            'ether')
-        print(f"Max Leveraged Asset Amount: {max_leverage}")
-        leveraged_amount = (
-            (margin['margin_remaining'] /
-             asset_price['wei']) *
-            leverage_multiplier)
-        return {"leveraged_amount": leveraged_amount,
-                "max_asset_leverage": max_leverage}
+            (margin / asset_price["usd"]) * Decimal(24.7), "ether"
+        )
+        # print(f"Max Leveraged Asset Amount: {max_leverage}")
+        leveraged_amount = (margin / asset_price["wei"]) * leverage_multiplier
+        return {
+            "leveraged_amount": leveraged_amount,
+            "max_asset_leverage": max_leverage,
+        }
+
+    def approve_susd(self, susd_amount: int, approve_max: bool = False):
+        susd_balance = self.get_susd_balance(self.wallet_address)["balance"]
+        if approve_max:
+            data_tx = self.susd_token.encodeABI(
+                fn_name="approve", args=[self.sm_account, susd_balance]
+            )
+        else:
+            data_tx = self.susd_token.encodeABI(
+                fn_name="approve", args=[self.sm_account, susd_amount]
+            )
+        tx_params = self._get_tx_params(
+            to=self.web3.to_checksum_address(addresses["sUSD"][self.network_id])
+        )
+        tx_params["data"] = data_tx
+        tx_params["gas"] = 1500000
+        print(f"Approving sUSD: {susd_amount}")
+        tx_token = self.execute_transaction(tx_params)
+        print(f"TX: {tx_token}")
+        return tx_token
+
+    def withdrawal_margin(
+        self,
+        token_symbol: str,
+        token_amount: int = 1,
+        withdrawal_all: bool = False,
+        execute_now: bool = False,
+    ):
+        """
+        Withdrawal SUSD from Margin Market to Wallet
+        ...
+
+        Attributes
+        ----------
+        token_amount : int
+            Token amount *in human readable* to send to Margin account
+        token_symbol : str
+            token symbol for market
+        withdrawal_all: bool
+            withdrawal all margin from market
+        Returns
+        ----------
+        str: token transfer Tx id
+        """
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(self.sm_account), abi=abis["SM_Account"]
+        )
+        if token_amount == 0:
+            raise Exception("token_amount Cannot be 0.")
+
+        current_position = self.get_current_position(
+            token_symbol, wallet_address=self.sm_account
+        )["margin"]
+        print(f"Current Position: {current_position}")
+        if token_amount < current_position:
+            is_withdrawal = -1
+            token_amount = self.web3.to_wei(abs(token_amount), "ether") * is_withdrawal
+            if execute_now:
+                if token_amount < 0:
+                    print(f"Withdrawal sUSD to {token_symbol} Market.")
+                    if withdrawal_all:
+                        commandBytes = encode(
+                            ["address"],
+                            [str(self.markets[token_symbol.upper()]["market_address"])],
+                        )
+                        data_tx = sm_account_contract.encodeABI(
+                            fn_name="execute", args=[[3], [commandBytes]]
+                        )
+                    else:
+                        commandBytes = encode(
+                            ["address", "int256"],
+                            [
+                                str(
+                                    self.markets[token_symbol.upper()]["market_address"]
+                                ),
+                                token_amount,
+                            ],
+                        )
+                        data_tx = sm_account_contract.encodeABI(
+                            fn_name="execute", args=[[2], [commandBytes]]
+                        )
+                    tx_params = self._get_tx_params(to=self.sm_account, value=0)
+                    tx_params["data"] = data_tx
+                    tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                        self.wallet_address
+                    )
+                    tx_token = self.execute_transaction(tx_params)
+                    return tx_token
+            else:
+                return {"token_amount": token_amount / (10**18), "tx_data": tx_params}
+        else:
+            print(
+                f"Token amount must be less than Current Position: {current_position}"
+            )
 
-    def transfer_margin(self, token_symbol: str,
-                        token_amount: int, execute_now: bool = False) -> str:
+    def transfer_margin(
+        self,
+        token_symbol: str,
+        token_amount: int,
+        skip_approval: bool = False,
+        withdrawal_all: bool = False,
+        execute_now: bool = False,
+    ) -> str:
         """
         Transfers SUSD from wallet to Margin account
         ...
 
         Attributes
         ----------
         token_amount : int
             Token amount *in human readable* to send to Margin account
         wallet_address : str
             wallet_address of wallet to check
-        token_symbol : str
-            token symbol from list of supported asset
+        skip_approval: bool
+            skip susd approval if amount is already approved
         Returns
         ----------
         str: token transfer Tx id
         """
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(self.sm_account), abi=abis["SM_Account"]
+        )
         if token_amount == 0:
-            raise Exception("Can not transfer 0 margin")
+            raise Exception("token_amount Cannot be 0.")
 
         is_withdrawal = -1 if token_amount < 0 else 1
-        token_amount = self.web3.to_wei(
-            abs(token_amount), 'ether') * is_withdrawal
-
-        susd_balance = self.get_susd_balance()
-        market_contract = self.get_market_contract(token_symbol)
+        token_amount = self.web3.to_wei(abs(token_amount), "ether") * is_withdrawal
+        print(token_amount)
+        if is_withdrawal > 0:
+            susd_balance = self.get_susd_balance(self.wallet_address)
+        else:
+            susd_balance = self.get_susd_balance(self.sm_account)
         print(f"sUSD Balance: {susd_balance['balance_usd']}")
-        if (token_amount < susd_balance['balance']):
-            data_tx = market_contract.encodeABI(
-                fn_name='transferMargin', args=[token_amount])
-
-            tx_params = self._get_tx_params(
-                to=market_contract.address, value=0)
-            tx_params['data'] = data_tx
-
+        if token_amount < susd_balance["balance"]:
             if execute_now:
-                tx_token = self.execute_transaction(tx_params)
-                print(f"Updating Position by {token_amount}")
-                print(f"TX: {tx_token}")
-                return tx_token
+                if (token_amount > 0) and (skip_approval is False):
+                    self.approve_susd(token_amount)
+                    print("Waiting for Approval...")
+                    time.sleep(4.5)
+                if token_amount > 0:
+                    print(f"Adding sUSD to {token_symbol} Market.")
+                    time.sleep(4.5)
+                    print(
+                        f"Market_address: {(self.markets[token_symbol.upper()]['market_address'])}"
+                    )
+                    commandBytes1 = encode(["int256"], [token_amount])
+                    commandBytes2 = encode(
+                        ["address", "int256"],
+                        [
+                            str(self.markets[token_symbol.upper()]["market_address"]),
+                            token_amount,
+                        ],
+                    )
+                    data_tx = sm_account_contract.encodeABI(
+                        fn_name="execute", args=[[0, 2], [commandBytes1, commandBytes2]]
+                    )
+                    tx_params = self._get_tx_params(to=self.sm_account, value=0)
+                    tx_params["data"] = data_tx
+                    tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                        self.wallet_address
+                    )
+                    tx_token = self.execute_transaction(tx_params)
+                    return tx_token
+                else:
+                    # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
+                    # args[0] == Command ID, args[1] == command inputs, in bytes
+                    if withdrawal_all:
+                        token_amount = (
+                            int(
+                                self.get_accessible_margin(self.sm_account)[
+                                    "margin_remaining_usd"
+                                ]
+                            )
+                            * -1
+                        )
+                    commandBytes = encode(["int256"], [token_amount])
+                    data_tx = sm_account_contract.encodeABI(
+                        fn_name="execute", args=[[0], [commandBytes]]
+                    )
+                    tx_params = self._get_tx_params(to=self.sm_account, value=0)
+                    tx_params["data"] = data_tx
+                    tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                        self.wallet_address
+                    )
+                    tx_token = self.execute_transaction(tx_params)
+                    print(f"Adding {token_amount} sUSD to Account.")
+                    print(f"TX: {tx_token}")
+                    return tx_token
             else:
-                return {"token": token_symbol.upper(),
-                        'token_amount': token_amount / (10**18),
-                        "susd_balance": susd_balance,
-                        "tx_data": tx_params}
+                return {
+                    "token_amount": token_amount / (10**18),
+                    "susd_balance": susd_balance,
+                    "tx_data": tx_params,
+                }
 
     def modify_position(
-            self,
-            token_symbol: str,
-            size_delta: float,
-            slippage: float = DEFAULT_SLIPPAGE,
-            execute_now: bool = False,
-            self_execute: bool = False) -> str:
+        self,
+        token_symbol: str,
+        position_size: float,
+        wallet_address: str,
+        slippage: float = DEFAULT_SLIPPAGE,
+        execute_now: bool = False,
+        self_execute: bool = False,
+    ) -> str:
         """
-        Submits a delayed offchain order with a size of `size_delta`
+        Submits a delayed offchain order with a size of `position_size`
         ...
 
         Attributes
         ----------
-        size_delta : float
+        position_size : float
             Position amount *in human readable* as trade asset i.e. 12 SOL == 12*(10**18). Exact position in a direction, with negative values representing short orders.
         token_symbol : str
             token symbol from list of supported asset
         wallet_address : str
             wallet_address of wallet to check
         slippage : float
             slippage percentage
         self_execute : bool
             If True, wait until the order is executable and execute it
 
         Returns
         ----------
         str: token transfer Tx id
         """
-        is_short = -1 if size_delta < 0 else 1
-        market_contract = self.get_market_contract(token_symbol)
-        size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
-
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(wallet_address), abi=abis["SM_Account"]
+        )
+        is_short = -1 if position_size < 0 else 1
+        position_size = self.web3.to_wei(abs(position_size), "ether") * is_short
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
-
         desired_fill_price = int(
-            current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
+            current_price["wei"] + current_price["wei"] * (slippage / 100) * is_short
+        )
 
         print(f"Current Position Size: {current_position['size']}")
-        data_tx = market_contract.encodeABI(
-            fn_name='submitOffchainDelayedOrderWithTracking', args=[
-                int(size_delta), desired_fill_price, DEFAULT_TRACKING_CODE])
-
-        tx_params = self._get_tx_params(to=market_contract.address, value=0)
-        tx_params['data'] = data_tx
-
-        print(f"Updating Position by {size_delta}")
+        commandBytes = encode(
+            ["address", "int256", "int256"],
+            [
+                (self.markets[token_symbol.upper()]["market_address"]),
+                position_size,
+                desired_fill_price,
+            ],
+        )
+        data_tx = sm_account_contract.encodeABI(
+            fn_name="execute", args=[[6], [commandBytes]]
+        )
+        tx_params = self._get_tx_params(to=self.sm_account, value=0)
+        tx_params["data"] = data_tx
+        print(f"Updating Position by {position_size}")
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"TX: {tx_token}")
 
             if self_execute:
                 self._wait_and_execute(tx_token, token_symbol)
             return tx_token
         else:
             return {
                 "token": token_symbol.upper(),
-                'current_position': current_position['size'],
-                "tx_data": tx_params}
+                "current_position": current_position["size"],
+                "tx_data": tx_params,
+            }
 
     def close_position(
-            self,
-            token_symbol: str,
-            slippage: float = DEFAULT_SLIPPAGE,
-            execute_now: bool = False,
-            self_execute: bool = False) -> str:
+        self,
+        token_symbol: str,
+        wallet_address: str,
+        slippage: float = DEFAULT_SLIPPAGE,
+        execute_now: bool = False,
+        self_execute: bool = False,
+    ) -> str:
         """
         Fully closes account position
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
+        wallet_address:str
+            wallet address -- Should be SM account
         slippage : float
             slippage percentage
         self_execute : bool
             If True, wait until the order is executable and execute it
 
         Returns
         ----------
         str: token transfer Tx id
         """
-        market_contract = self.get_market_contract(token_symbol)
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
-
-        is_short = -1 if -current_position['size'] < 0 else 1
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(wallet_address), abi=abis["SM_Account"]
+        )
+        is_short = -1 if -current_position["size"] < 0 else 1
         desired_fill_price = int(
-            current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
-
+            current_price["wei"] + current_price["wei"] * (slippage / 100) * is_short
+        )
         print(f"Current Position Size: {current_position['size']}")
-        if current_position['size'] == 0:
+        if current_position["size"] == 0:
             print("Not in position!")
             return None
         # Flip position size to the opposite direction
-        data_tx = market_contract.encodeABI(
-            fn_name='submitCloseOffchainDelayedOrderWithTracking', args=[
-                desired_fill_price, DEFAULT_TRACKING_CODE])
-
-        tx_params = self._get_tx_params(to=market_contract.address, value=0)
-        tx_params['data'] = data_tx
-
+        # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
+        # args[0] == Command ID, args[1] == command inputs, in bytes
+        commandBytes = encode(
+            ["address", "int256"],
+            [
+                (self.markets[token_symbol.upper()]["market_address"]),
+                desired_fill_price,
+            ],
+        )
+        data_tx = sm_account_contract.encodeABI(
+            fn_name="execute", args=[[9], [commandBytes]]
+        )
+        tx_params = self._get_tx_params(to=self.sm_account, value=0)
+        tx_params["data"] = data_tx
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"Closing Position by {-current_position['size']}")
             print(f"TX: {tx_token}")
             if self_execute:
                 self._wait_and_execute(tx_token, token_symbol)
 
             return tx_token
         else:
             return {
                 "token": token_symbol.upper(),
-                'current_position': current_position['size'],
-                "tx_data": tx_params}
+                "current_position": current_position["size"],
+                "tx_data": tx_params,
+            }
 
     def open_position(
-            self,
-            token_symbol: str,
-            short: bool = False,
-            size_delta: float = None,
-            slippage: float = DEFAULT_SLIPPAGE,
-            leverage_multiplier: float = None,
-            execute_now: bool = False,
-            self_execute: bool = False) -> str:
+        self,
+        token_symbol: str,
+        wallet_address: str,
+        short: bool = False,
+        position_size: float = None,
+        slippage: float = DEFAULT_SLIPPAGE,
+        leverage_multiplier: float = None,
+        execute_now: bool = False,
+        self_execute: bool = False,
+    ) -> str:
         """
         Open account position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
+        wallet_address : str
+            Wallet Address to open position in. Should be SM account.
         short : bool, optional
             set to True when creating a short. (Implemented to double check side)
-        size_delta : int, optional
+        position_size : int, optional
             position amount in human readable format as trade asset i.e. 12 SOL. Exact position in a direction (Sign this It WILL MATTER).
         leverage_multiplier :
             Multiplier of Leverage to use when creating order. Based on available margin in account.
         slippage : float
             slippage percentage
         self_execute : bool
             If True, wait until the order is executable and execute it
 
-        *Use either size_delta or leverage_multiplier.
+        *Use either position_size or leverage_multiplier.
 
         Returns
         ----------
         str: token transfer Tx id
         """
-        if (size_delta is None) and (leverage_multiplier is None):
-            print("Enter EITHER a size_delta or a leverage_multiplier!")
+        if (position_size is None) and (leverage_multiplier is None):
+            print("Enter EITHER a position_size or a leverage_multiplier!")
             return None
-        elif (size_delta is not None) and (leverage_multiplier is not None):
-            print("Enter EITHER a size_delta or a leverage_multiplier!")
+        elif (position_size is not None) and (leverage_multiplier is not None):
+            print("Enter EITHER a position_size or a leverage_multiplier!")
             return None
 
-        market_contract = self.get_market_contract(token_symbol)
-        current_position = self.get_current_position(token_symbol)
+        current_position = self.get_current_position(
+            token_symbol, wallet_address=wallet_address
+        )
         current_price = self.get_current_asset_price(token_symbol)
-
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(wallet_address), abi=abis["SM_Account"]
+        )
         # starting at zero otherwise use Update position
-        if current_position['size'] != 0:
+        if current_position["size"] != 0:
             print(f"You are already in a position, use modify_position() instead.")
             print(
-                f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}")
+                f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}"
+            )
             return None
+        is_short = -1 if short else 1
         if leverage_multiplier:
             leveraged_amount = self.get_leveraged_amount(
-                token_symbol, leverage_multiplier)
-            max_leverage = leveraged_amount['max_asset_leverage']
-
-            size_delta = leveraged_amount['leveraged_amount']
-            is_short = short
-            size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
-        elif size_delta:
-            max_leverage = self.get_leveraged_amount(
-                token_symbol, 1)['max_asset_leverage']
-
-            is_short = -1 if size_delta < 0 else 1
-            size_delta = self.web3.to_wei(abs(size_delta), 'ether') * is_short
-        # check side
-        if short == True & is_short != True:
-            print(
-                "Position size is Negative & Short set to False! Double Check intention.")
-            return None
+                token_symbol, leverage_multiplier
+            )
+            max_leverage = leveraged_amount["max_asset_leverage"]
+            position_size = leveraged_amount["leveraged_amount"]
+            position_size = self.web3.to_wei(abs(position_size), "ether") * is_short
+        elif position_size:
+            # check side
+            if (short == True & position_size > 0) or (
+                short == False & position_size < 0
+            ):
+                print(
+                    "Position size and Short value do not line up. Double Check intention."
+                )
+                return None
+            max_leverage = self.get_leveraged_amount(token_symbol, 24.7)[
+                "max_asset_leverage"
+            ]
+            position_size = self.web3.to_wei(abs(position_size), "ether") * is_short
         # checking available margin to make sure this is possible
-        if (abs(size_delta) < max_leverage):
+        if abs(position_size) < max_leverage:
             desired_fill_price = int(
-                current_price['wei'] + current_price['wei'] * (slippage / 100) * is_short)
-
-            data_tx = market_contract.encodeABI(
-                fn_name='submitOffchainDelayedOrderWithTracking', args=[
-                    int(size_delta), desired_fill_price, DEFAULT_TRACKING_CODE])
-
-            tx_params = self._get_tx_params(
-                to=market_contract.address, value=0)
-            tx_params['data'] = data_tx
+                current_price["wei"]
+                + current_price["wei"] * (slippage / 100) * is_short
+            )
+            # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
+            # args[0] == Command ID, args[1] == command inputs, in bytes
+            commandBytes = encode(
+                ["address", "int256", "int256"],
+                [
+                    (self.markets[token_symbol.upper()]["market_address"]),
+                    position_size,
+                    desired_fill_price,
+                ],
+            )
+            data_tx = sm_account_contract.encodeABI(
+                fn_name="execute", args=[[6], [commandBytes]]
+            )
+            tx_params = self._get_tx_params(to=self.sm_account, value=0)
+            tx_params["data"] = data_tx
 
             if execute_now:
                 tx_token = self.execute_transaction(tx_params)
-                print(f"Updating Position by {size_delta}")
+                print(f"Updating Position by {position_size}")
                 print(f"TX: {tx_token}")
                 if self_execute:
                     self._wait_and_execute(tx_token, token_symbol)
                 return tx_token
             else:
-                return {"token": token_symbol.upper(),
-                        'position_size': size_delta / (10**18),
-                        'current_position': current_position['size'],
-                        "max_leverage": max_leverage / (10**18),
-                        "leveraged_percent": (size_delta / max_leverage) * 100,
-                        "tx_data": tx_params}
+                return {
+                    "token": token_symbol.upper(),
+                    "position_size": position_size / (10**18),
+                    "current_position": current_position["size"],
+                    "max_leverage": max_leverage / (10**18),
+                    "leveraged_percent": (position_size / max_leverage) * 100,
+                    "tx_data": tx_params,
+                }
 
     def cancel_order(
-            self,
-            token_symbol: str,
-            account: str = None,
-            execute_now: bool = False) -> str:
+        self, token_symbol: str, account: str = None, execute_now: bool = False
+    ) -> str:
         """
         Cancels an open order
         ...
 
         Attributes
         ----------
         account : str
@@ -816,46 +1100,52 @@
         token_symbol : str
             token symbol from list of supported asset
 
         Returns
         ----------
         str: transaction hash for closing the order
         """
-        market_contract = self.get_market_contract(token_symbol)
-        delayed_order = self.check_delayed_orders(token_symbol)
-
         if account is None:
-            account = self.wallet_address
+            account = self.sm_account
+        delayed_order = self.check_delayed_orders(token_symbol)
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(account), abi=abis["SM_Account"]
+        )
 
-        if not delayed_order['is_open']:
+        if not delayed_order["is_open"]:
             print("No open order")
             return None
 
-        data_tx = market_contract.encodeABI(
-            fn_name='cancelOffchainDelayedOrder', args=[self.wallet_address])
-
-        tx_params = self._get_tx_params(to=market_contract.address, value=0)
-        tx_params['data'] = data_tx
-
+        # Execute Commands: https://github.com/Kwenta/smart-margin/wiki/Commands
+        # args[0] == Command ID, args[1] == command inputs, in bytes
+        commandBytes = encode(
+            ["address"], [(self.markets[token_symbol.upper()]["market_address"])]
+        )
+        data_tx = sm_account_contract.encodeABI(
+            fn_name="execute", args=[[1], [commandBytes]]
+        )
+        tx_params = self._get_tx_params(to=self.sm_account, value=0)
+        tx_params["data"] = data_tx
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"Cancelling order for {token_symbol}")
             print(f"TX: {tx_token}")
             return tx_token
         else:
-            return {
-                "token": token_symbol.upper(),
-                "tx_data": tx_params}
+            return {"token": token_symbol.upper(), "tx_data": tx_params}
 
     def execute_order(
-            self,
-            token_symbol: str,
-            account: str = None,
-            execute_now: bool = False,
-            estimate_gas: bool = False) -> str:
+        self,
+        token_symbol: str,
+        account: str = None,
+        execute_now: bool = False,
+        estimate_gas: bool = False,
+        gas_price: int = None,
+        pyth_feed_data: str = None,
+    ) -> str:
         """
         Executes an open order
         ...
 
         Attributes
         ----------
         account : str
@@ -869,47 +1159,52 @@
         """
         if not account:
             account = self.wallet_address
 
         market_contract = self.get_market_contract(token_symbol)
         delayed_order = self.check_delayed_orders(token_symbol, account)
 
-        if not delayed_order['is_open']:
+        if not delayed_order["is_open"]:
             print("No open order")
             return None
 
-        # get price update data
-        price_update_data = self.pyth.price_update_data(token_symbol)
+        if pyth_feed_data is None:
+            # get price update data
+            pyth_feed_data = self.pyth.price_update_data(token_symbol)
 
-        if not price_update_data:
-            raise Exception(
-                "Failed to get price update data from price service")
+        if not pyth_feed_data:
+            raise Exception("Failed to get price update data from price service")
 
         data_tx = market_contract.encodeABI(
-            fn_name='executeOffchainDelayedOrder', args=[account, [price_update_data]])
+            fn_name="executeOffchainDelayedOrder", args=[account, [pyth_feed_data]]
+        )
 
         tx_params = self._get_tx_params(to=market_contract.address, value=1)
-        tx_params['data'] = data_tx
+        tx_params["data"] = data_tx
 
         if execute_now:
             tx_token = self.execute_transaction(tx_params)
             print(f"Executing order for {token_symbol}")
             print(f"TX: {tx_token}")
             return tx_token
+        elif gas_price is not None:
+            tx_params["gasPrice"] = gas_price
+            tx_token = self.execute_transaction(tx_params)
+            print(f"Executing order for {token_symbol}")
+            print(f"TX: {tx_token}")
+            return tx_token
         elif estimate_gas:
             try:
                 gas_estimate = self.web3.eth.estimate_gas(tx_params)
                 return gas_estimate
             except Exception as e:
-                print(f'Error estimating gas: {e}')
+                print(f"Error estimating gas: {e}")
                 return None
         else:
-            return {
-                "token": token_symbol.upper(),
-                "tx_data": tx_params}
+            return {"token": token_symbol.upper(), "tx_data": tx_params}
 
     async def _wait_and_execute(self, tx, token_symbol, retries=3, retry_interval=1):
         """
         Wait for a transaction receipt and execute the order when executable
         ...
 
         Attributes
@@ -926,43 +1221,45 @@
         # wait for receipt
         self.web3.eth.wait_for_transaction_receipt(tx)
 
         # get delayed order
         delayed_order = self.check_delayed_orders(token_symbol)
 
         # wait until executable
-        print('Waiting until order is executable')
-        time.sleep(delayed_order['executable_time'] - time.time())
+        print("Waiting until order is executable")
+        time.sleep(delayed_order["executable_time"] - time.time())
 
         # set up the estimate
         gas_estimate = None
         attempt = 0
 
         # Retry gas estimation multiple times
         while attempt < retries:
             gas_estimate = self.execute_order(token_symbol, estimate_gas=True)
 
             if gas_estimate is not None:
                 break
 
-            print(
-                f'Gas estimation failed, retrying in {retry_interval} seconds...')
+            print(f"Gas estimation failed, retrying in {retry_interval} seconds...")
             time.sleep(retry_interval)
             attempt += 1
 
         # If gas estimation is successful, execute the order
         if gas_estimate:
-            print(f'Gas estimate for executing order: {gas_estimate}')
+            print(f"Gas estimate for executing order: {gas_estimate}")
             tx_execute = self.execute_order(token_symbol, execute_now=True)
-            print(f'Executing tx: {tx_execute}')
+            print(f"Executing tx: {tx_execute}")
         else:
             print(
-                'Gas estimation failed after multiple retries, not executing the order.')
+                "Gas estimation failed after multiple retries, not executing the order."
+            )
 
-    async def execute_for_address(self, token_symbol, wallet_address, retries=5, retry_interval=1):
+    async def execute_for_address(
+        self, token_symbol, wallet_address, retries=5, retry_interval=1
+    ):
         """
         Check an addresses delayed orders and execute the order when executable
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -973,146 +1270,164 @@
         if not wallet_address:
             wallet_address = self.wallet_address
 
         # check delayed orders
         delayed_order = self.check_delayed_orders(token_symbol, wallet_address)
 
         # if no order, exit
-        if not delayed_order['is_open']:
+        if not delayed_order["is_open"]:
             print("No delayed order open")
             return
 
         # wait until executable
-        print('Waiting until order is executable')
-        await asyncio.sleep(delayed_order['executable_time'] - time.time())
+        print("Waiting until order is executable")
+        await asyncio.sleep(delayed_order["executable_time"] - time.time())
 
         # set up the estimate
         gas_estimate = None
         attempt = 0
 
         # Retry gas estimation multiple times
         while attempt < retries:
             gas_estimate = self.execute_order(
-                token_symbol, account=wallet_address, estimate_gas=True)
+                token_symbol, account=wallet_address, estimate_gas=True
+            )
 
             if gas_estimate is not None:
                 break
 
-            print(
-                f'Gas estimation failed, retrying in {retry_interval} seconds...')
+            print(f"Gas estimation failed, retrying in {retry_interval} seconds...")
             await asyncio.sleep(retry_interval)
             attempt += 1
 
         # If gas estimation is successful, execute the order
         if gas_estimate:
-            print(f'Gas estimate for executing order: {gas_estimate}')
+            print(f"Gas estimate for executing order: {gas_estimate}")
             tx_execute = self.execute_order(
-                token_symbol, account=wallet_address, execute_now=True)
-            print(f'Executing tx: {tx_execute}')
+                token_symbol, account=wallet_address, execute_now=True
+            )
+            print(f"Executing tx: {tx_execute}")
         else:
             print(
-                'Gas estimation failed after multiple retries, not executing the order.')
+                "Gas estimation failed after multiple retries, not executing the order."
+            )
 
     def open_limit(
-            self,
-            token_symbol: str,
-            limit_price: float,
-            size_delta: float = None,
-            leverage_multiplier: float = None,
-            slippage: float = DEFAULT_SLIPPAGE,
-            short: bool = False,
-            execute_now: bool = False) -> str:
+        self,
+        token_symbol: str,
+        limit_price: float,
+        wallet_address: str = None,
+        position_size: float = None,
+        leverage_multiplier: float = None,
+        slippage: float = DEFAULT_SLIPPAGE,
+        short: bool = False,
+        execute_now: bool = False,
+    ) -> str:
         """
         Open Limit position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
             token symbol from list of supported asset
         short : bool, optional
             set to True when creating a short. (Implemented to double check side)
         limit_price : float
             limit price in dollars to open position.
-        size_delta : int, optional
+        position_size : int, optional
             position amount in human readable format as trade asset i.e. 12 SOL . Exact position in a direction (Sign this It WILL MATTER).
         leverage_multiplier :
             Multiplier of Leverage to use when creating order. Based on available margin in account.
         slippage : float
             slippage percentage
-        *Use either size_delta or leverage_multiplier.
+        *Use either position_size or leverage_multiplier.
 
         Returns
         ----------
         str: token transfer Tx id
         """
-        if (size_delta is None) and (leverage_multiplier is None):
+        if wallet_address is None:
+            wallet_address = self.sm_account
+        if (position_size is None) and (leverage_multiplier is None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
-        elif (size_delta is not None) and (leverage_multiplier is not None):
+        elif (position_size is not None) and (leverage_multiplier is not None):
             print("Enter EITHER a position amount or a leverage multiplier!")
             return None
 
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
-        if current_position['size'] != 0:
+        if current_position["size"] != 0:
             print(f"You are already in a position, use modify_position() instead.")
             print(
-                f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}")
+                f"Current Position Size: {self.web3.from_wei(current_position['size'], 'ether')}"
+            )
             return None
 
         # Case for position_amount manually set
-        if size_delta is not None:
+        if position_size is not None:
             # check Short Position
             if short:
-                if current_price['usd'] >= limit_price:
+                if current_price["usd"] >= limit_price:
                     return self.open_position(
                         token_symbol,
+                        wallet_address,
                         short=True,
                         slippage=slippage,
-                        size_delta=size_delta,
-                        execute_now=execute_now)
+                        position_size=position_size,
+                        execute_now=execute_now,
+                    )
             else:
-                if current_price['usd'] <= limit_price:
+                if current_price["usd"] <= limit_price:
                     return self.open_position(
                         token_symbol,
+                        wallet_address,
                         short=False,
                         slippage=slippage,
-                        size_delta=size_delta,
-                        execute_now=execute_now)
+                        position_size=position_size,
+                        execute_now=execute_now,
+                    )
 
         # Case for Leverage Multiplier
         else:
             if short:
-                if current_price['usd'] >= limit_price:
+                if current_price["usd"] >= limit_price:
                     return self.open_position(
                         token_symbol,
+                        wallet_address,
                         short=True,
                         slippage=slippage,
                         leverage_multiplier=leverage_multiplier,
-                        execute_now=execute_now)
+                        execute_now=execute_now,
+                    )
             else:
-                if current_price['usd'] <= limit_price:
+                if current_price["usd"] <= limit_price:
                     return self.open_position(
                         token_symbol,
+                        wallet_address,
                         short=False,
                         slippage=slippage,
                         leverage_multiplier=leverage_multiplier,
-                        execute_now=execute_now)
+                        execute_now=execute_now,
+                    )
         print(
-            f"Limit not reached current : {current_price} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}")
+            f"Limit not reached current : {current_price} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}"
+        )
         return None
 
     def close_limit(
-            self,
-            token_symbol: str,
-            limit_price: float,
-            slippage: float = DEFAULT_SLIPPAGE,
-            execute_now: bool = False):
+        self,
+        token_symbol: str,
+        limit_price: float,
+        wallet_address: str = None,
+        slippage: float = DEFAULT_SLIPPAGE,
+        execute_now: bool = False,
+    ):
         """
         Close Limit position in a direction
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -1121,41 +1436,54 @@
             limit price in *dollars* to open position.
         slippage : float
             slippage percentage
         Returns
         ----------
         str: token transfer Tx id
         """
+        if wallet_address is None:
+            wallet_address = self.sm_account
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
 
         # Check if you are in Position
-        if current_position['size'] == 0:
+        if current_position["size"] == 0:
             print("Not in position!")
             return None
 
-        short = True if current_position['size'] < 0 else False
+        short = True if current_position["size"] < 0 else False
         if short:
-            if current_price['usd'] <= limit_price:
+            if current_price["usd"] <= limit_price:
                 return self.close_position(
-                    token_symbol, slippage=slippage, execute_now=execute_now)
+                    token_symbol,
+                    wallet_address,
+                    slippage=slippage,
+                    execute_now=execute_now,
+                )
         else:
-            if current_price['usd'] >= limit_price:
+            if current_price["usd"] >= limit_price:
                 return self.close_position(
-                    token_symbol, slippage=slippage, execute_now=execute_now)
+                    token_symbol,
+                    wallet_address,
+                    slippage=slippage,
+                    execute_now=execute_now,
+                )
         print(
-            f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}")
+            f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price}"
+        )
         return None
 
     def close_stop_limit(
-            self,
-            token_symbol: str,
-            limit_price: float,
-            stop_price: float,
-            slippage: float = DEFAULT_SLIPPAGE) -> str:
+        self,
+        token_symbol: str,
+        limit_price: float,
+        stop_price: float,
+        wallet_address: str = None,
+        slippage: float = DEFAULT_SLIPPAGE,
+    ) -> str:
         """
         Close Limit position in a direction with Stop price
         ...
 
         Attributes
         ----------
         token_symbol : str
@@ -1166,28 +1494,83 @@
             Set to stop price incase of bad position, will exit position if triggered
         slippage : float
             slippage percentage
         Returns
         ----------
         str: token transfer Tx id
         """
+        if wallet_address is None:
+            wallet_address = self.sm_account
         current_position = self.get_current_position(token_symbol)
         current_price = self.get_current_asset_price(token_symbol)
         # Check if you are in Position
-        if current_position['size'] == 0:
+        if current_position["size"] == 0:
             print("Not in position!")
             return None
 
-        short = True if current_position['size'] < 0 else False
+        short = True if current_position["size"] < 0 else False
         if short:
-            if current_price['usd'] <= limit_price:
-                return self.close_position(token_symbol, slippage=slippage)
-            elif current_price['usd'] >= stop_price:
-                return self.close_position(token_symbol, slippage=slippage)
+            if current_price["usd"] <= limit_price:
+                return self.close_position(
+                    token_symbol, wallet_address, slippage=slippage
+                )
+            elif current_price["usd"] >= stop_price:
+                return self.close_position(
+                    token_symbol, wallet_address, slippage=slippage
+                )
         else:
-            if current_price['usd'] >= limit_price:
-                return self.close_position(token_symbol, slippage=slippage)
-            elif current_price['usd'] <= stop_price:
-                return self.close_position(token_symbol, slippage=slippage)
+            if current_price["usd"] >= limit_price:
+                return self.close_position(
+                    token_symbol, wallet_address, slippage=slippage
+                )
+            elif current_price["usd"] <= stop_price:
+                return self.close_position(
+                    token_symbol, wallet_address, slippage=slippage
+                )
         print(
-            f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price} | Stop Limit: {stop_price}")
+            f"Limit not reached current : {current_price['usd']} | Entry: {current_position['last_price']/(10**18)} | Limit: {limit_price} | Stop Limit: {stop_price}"
+        )
         return None
+
+    def execute_chain(
+        self, command_list: list, wallet_address: str = None, execute_now: bool = False
+    ) -> str:
+        """
+        Excecute Kwenta Command Chain. Advanced Usage.
+        ...
+        Attributes
+        ----------
+        command_list : list
+            list of commands to execute with command details
+            Example format:
+                token_amount = 55000000
+                market = "SOL"
+                command_list = []
+                command_list.append(kwenta_account.ACCOUNT_COMMANDS['ACCOUNT_MODIFY_MARGIN'],[token_amount])
+                command_list.append(kwenta_account.ACCOUNT_COMMANDS['PERPS_V2_MODIFY_MARGIN'],[market, token_amount])
+        Returns
+        ----------
+        str: token transfer Tx id
+        """
+        if wallet_address is None:
+            wallet_address = self.sm_account
+        sm_account_contract = self.web3.eth.contract(
+            self.web3.to_checksum_address(self.sm_account), abi=abis["SM_Account"]
+        )
+        if execute_now:
+            command_ids = []
+            command_data = []
+            for command in command_list:
+                command_ids.append(command[0])
+                command_data.append(command[1])
+            data_tx = sm_account_contract.encodeABI(
+                fn_name="execute", args=[command_ids, command_data]
+            )
+            tx_params = self._get_tx_params(to=self.sm_account, value=0)
+            tx_params["data"] = data_tx
+            tx_params["nonce"] = self.web3.eth.get_transaction_count(
+                self.wallet_address
+            )
+            tx_token = self.execute_transaction(tx_params)
+            return tx_token
+        else:
+            return {"command_list": command_list, "tx_data": tx_params}
```

### Comparing `kwenta-1.0.5/kwenta/pyth/constants.py` & `kwenta-1.0.6/kwenta/pyth/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/pyth/pyth.py` & `kwenta-1.0.6/kwenta/pyth/pyth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import base64
 import requests
 from .constants import PRICE_FEED_IDS
+import json
 
-
-class Pyth:
+class Pyth:            
     def __init__(self, network_id: int, price_service_endpoint: str = None):
         self._price_service_endpoint = price_service_endpoint
         self.price_feed_ids = PRICE_FEED_IDS[network_id]
-
+        
     def price_update_data(self, token_symbol):
         """
         Request price update data from the pyth price service
         ...
 
         Attributes
         ----------
```

### Comparing `kwenta-1.0.5/kwenta/queries/config.py` & `kwenta-1.0.6/kwenta/queries/config.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/queries/gql.py` & `kwenta-1.0.6/kwenta/queries/gql.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta/queries/queries.py` & `kwenta-1.0.6/kwenta/queries/queries.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.5/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.6/kwenta.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.5/kwenta.egg-info/SOURCES.txt` & `kwenta-1.0.6/kwenta.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 kwenta.egg-info/top_level.txt
 kwenta/alerts/__init__.py
 kwenta/alerts/alerts.py
 kwenta/cli/__init__.py
 kwenta/cli/kwenta_cli.py
 kwenta/contracts/__init__.py
 kwenta/contracts/contracts.py
+kwenta/contracts/json/PerpsV2ExchangeRate.json
 kwenta/contracts/json/PerpsV2Market.json
 kwenta/contracts/json/PerpsV2MarketData.json
+kwenta/contracts/json/SMAccount.json
+kwenta/contracts/json/SMFactory.json
 kwenta/contracts/json/__init__.py
 kwenta/contracts/json/sUSD.json
 kwenta/pyth/__init__.py
 kwenta/pyth/constants.py
 kwenta/pyth/pyth.py
 kwenta/queries/__init__.py
 kwenta/queries/config.py
```

### Comparing `kwenta-1.0.5/setup.py` & `kwenta-1.0.6/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 from setuptools import setup, find_packages
+
 setup(
-    name='kwenta',
-    version='1.0.5',
-    description='Python SDK for Kwenta',
-    long_description='Python SDK for Kwenta',
-    author='Kwenta DAO',
+    name="kwenta",
+    version="1.0.6",
+    description="Python SDK for Kwenta",
+    long_description="Python SDK for Kwenta",
+    author="Kwenta DAO",
     packages=[
-        'kwenta',
-        'kwenta.alerts',
-        'kwenta.cli',
-        'kwenta.contracts',
-        'kwenta.contracts.json',
-        'kwenta.pyth',
-        'kwenta.queries'
-    ],
-    install_requires=[
-        "numpy",
-        "pandas",
-        "requests",
-        "web3>=6.0.0",
-        "gql"
+        "kwenta",
+        "kwenta.alerts",
+        "kwenta.cli",
+        "kwenta.contracts",
+        "kwenta.contracts.json",
+        "kwenta.pyth",
+        "kwenta.queries",
     ],
+    install_requires=["numpy", "pandas", "requests", "web3>=6.0.0", "gql"],
     classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     python_requires=">=3.8",
     package_data={"kwenta": ["json/*"]},
     include_package_data=True,
     entry_points={
-        'console_scripts': [
-            'kwenta = kwenta.cli.kwenta_cli:kwenta_cli',
+        "console_scripts": [
+            "kwenta = kwenta.cli.kwenta_cli:kwenta_cli",
         ],
     },
 )
```

