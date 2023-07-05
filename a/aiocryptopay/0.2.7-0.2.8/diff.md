# Comparing `tmp/aiocryptopay-0.2.7.tar.gz` & `tmp/aiocryptopay-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocryptopay-0.2.7.tar", max compression
+gzip compressed data, was "aiocryptopay-0.2.8.tar", max compression
```

## Comparing `aiocryptopay-0.2.7.tar` & `aiocryptopay-0.2.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2022-12-05 16:03:04.838812 aiocryptopay-0.2.7/LICENSE
--rw-r--r--   0        0        0     1784 2022-12-05 16:03:04.839813 aiocryptopay-0.2.7/README.md
--rw-r--r--   0        0        0       82 2023-05-08 12:47:23.802151 aiocryptopay-0.2.7/aiocryptopay/__init__.py
--rw-r--r--   0        0        0    12716 2023-05-08 12:46:57.658276 aiocryptopay-0.2.7/aiocryptopay/api.py
--rw-r--r--   0        0        0     2136 2023-03-20 12:28:03.059079 aiocryptopay-0.2.7/aiocryptopay/base.py
--rw-r--r--   0        0        0      839 2023-05-08 12:41:06.571903 aiocryptopay-0.2.7/aiocryptopay/const.py
--rw-r--r--   0        0        0      131 2022-12-05 16:07:52.984529 aiocryptopay-0.2.7/aiocryptopay/exceptions/__init__.py
--rw-r--r--   0        0        0     1551 2023-03-20 12:28:03.065080 aiocryptopay-0.2.7/aiocryptopay/exceptions/factory.py
--rw-r--r--   0        0        0        0 2022-12-05 16:03:04.844812 aiocryptopay-0.2.7/aiocryptopay/models/__init__.py
--rw-r--r--   0        0        0      141 2022-12-05 16:07:52.995530 aiocryptopay-0.2.7/aiocryptopay/models/balance.py
--rw-r--r--   0        0        0      224 2023-03-21 18:17:03.290716 aiocryptopay-0.2.7/aiocryptopay/models/currencies.py
--rw-r--r--   0        0        0      793 2022-12-05 16:07:53.022044 aiocryptopay-0.2.7/aiocryptopay/models/invoice.py
--rw-r--r--   0        0        0      130 2022-12-05 16:07:53.002531 aiocryptopay-0.2.7/aiocryptopay/models/profile.py
--rw-r--r--   0        0        0      169 2022-12-05 16:47:13.745316 aiocryptopay-0.2.7/aiocryptopay/models/rates.py
--rw-r--r--   0        0        0      322 2022-12-05 16:07:53.015528 aiocryptopay-0.2.7/aiocryptopay/models/transfer.py
--rw-r--r--   0        0        0      206 2022-12-05 16:07:53.018668 aiocryptopay-0.2.7/aiocryptopay/models/update.py
--rw-r--r--   0        0        0       46 2022-12-05 16:42:12.806836 aiocryptopay-0.2.7/aiocryptopay/utils/__init__.py
--rw-r--r--   0        0        0      793 2022-12-05 16:47:13.754826 aiocryptopay-0.2.7/aiocryptopay/utils/exchange.py
--rw-r--r--   0        0        0      720 2023-05-08 12:41:06.580901 aiocryptopay-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 aiocryptopay-0.2.7/setup.py
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 aiocryptopay-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 16:03:04.838812 aiocryptopay-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1789 2023-07-05 19:41:30.284416 aiocryptopay-0.2.8/README.md
+-rw-r--r--   0        0        0       82 2023-07-05 19:44:31.835418 aiocryptopay-0.2.8/aiocryptopay/__init__.py
+-rw-r--r--   0        0        0    12716 2023-05-08 12:46:57.658276 aiocryptopay-0.2.8/aiocryptopay/api.py
+-rw-r--r--   0        0        0     2136 2023-03-20 12:28:03.059079 aiocryptopay-0.2.8/aiocryptopay/base.py
+-rw-r--r--   0        0        0      855 2023-07-05 19:41:48.800418 aiocryptopay-0.2.8/aiocryptopay/const.py
+-rw-r--r--   0        0        0      131 2022-12-05 16:07:52.984529 aiocryptopay-0.2.8/aiocryptopay/exceptions/__init__.py
+-rw-r--r--   0        0        0     1551 2023-03-20 12:28:03.065080 aiocryptopay-0.2.8/aiocryptopay/exceptions/factory.py
+-rw-r--r--   0        0        0        0 2022-12-05 16:03:04.844812 aiocryptopay-0.2.8/aiocryptopay/models/__init__.py
+-rw-r--r--   0        0        0      141 2022-12-05 16:07:52.995530 aiocryptopay-0.2.8/aiocryptopay/models/balance.py
+-rw-r--r--   0        0        0      224 2023-03-21 18:17:03.290716 aiocryptopay-0.2.8/aiocryptopay/models/currencies.py
+-rw-r--r--   0        0        0      793 2022-12-05 16:07:53.022044 aiocryptopay-0.2.8/aiocryptopay/models/invoice.py
+-rw-r--r--   0        0        0      130 2022-12-05 16:07:53.002531 aiocryptopay-0.2.8/aiocryptopay/models/profile.py
+-rw-r--r--   0        0        0      169 2022-12-05 16:47:13.745316 aiocryptopay-0.2.8/aiocryptopay/models/rates.py
+-rw-r--r--   0        0        0      322 2022-12-05 16:07:53.015528 aiocryptopay-0.2.8/aiocryptopay/models/transfer.py
+-rw-r--r--   0        0        0      206 2022-12-05 16:07:53.018668 aiocryptopay-0.2.8/aiocryptopay/models/update.py
+-rw-r--r--   0        0        0       46 2022-12-05 16:42:12.806836 aiocryptopay-0.2.8/aiocryptopay/utils/__init__.py
+-rw-r--r--   0        0        0      793 2022-12-05 16:47:13.754826 aiocryptopay-0.2.8/aiocryptopay/utils/exchange.py
+-rw-r--r--   0        0        0      720 2023-07-05 19:44:42.348416 aiocryptopay-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 aiocryptopay-0.2.8/setup.py
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 aiocryptopay-0.2.8/PKG-INFO
```

### Comparing `aiocryptopay-0.2.7/LICENSE` & `aiocryptopay-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/README.md` & `aiocryptopay-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 web_app = web.Application()
 crypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)
 
 
 @crypto.pay_handler()
-async def invoice_paid(update: Update) -> None:
+async def invoice_paid(update: Update, app) -> None:
     print(update)
 
 async def create_invoice(app) -> None:
     invoice = await crypto.create_invoice(asset='TON', amount=1.5)
     print(invoice.pay_url)
 
 async def close_session(app) -> None:
```

### Comparing `aiocryptopay-0.2.7/aiocryptopay/api.py` & `aiocryptopay-0.2.8/aiocryptopay/api.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/aiocryptopay/base.py` & `aiocryptopay-0.2.8/aiocryptopay/base.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/aiocryptopay/const.py` & `aiocryptopay-0.2.8/aiocryptopay/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     BTC = "BTC"
     TON = "TON"
     ETH = "ETH"
     USDT = "USDT"
     USDC = "USDC"
     BUSD = "BUSD"
     BNB = "BNB"
+    TRX = "TRX"
 
     @classmethod
     def values(cls):
         return list(map(lambda asset: asset.value, cls))
 
 
 class PaidButtons(StrEnum):
```

### Comparing `aiocryptopay-0.2.7/aiocryptopay/exceptions/factory.py` & `aiocryptopay-0.2.8/aiocryptopay/exceptions/factory.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/aiocryptopay/models/invoice.py` & `aiocryptopay-0.2.8/aiocryptopay/models/invoice.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/aiocryptopay/utils/exchange.py` & `aiocryptopay-0.2.8/aiocryptopay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `aiocryptopay-0.2.7/pyproject.toml` & `aiocryptopay-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocryptopay"
-version = "0.2.7"
+version = "0.2.8"
 description = "@cryptobot api asynchronous python wrapper"
 authors = ["layerqa"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/layerqa/aiocryptopay"
 documentation = "https://help.crypt.bot/crypto-pay-api"
 keywords = [
```

### Comparing `aiocryptopay-0.2.7/setup.py` & `aiocryptopay-0.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['aiohttp>=3.8.3,<4.0.0',
  'certifi>=2023.5.7,<2024.0.0',
  'pydantic>=1.10.7,<2.0.0',
  'strenum>=0.4.10,<0.5.0']
 
 setup_kwargs = {
     'name': 'aiocryptopay',
-    'version': '0.2.7',
+    'version': '0.2.8',
     'description': '@cryptobot api asynchronous python wrapper',
-    'long_description': "## **[@cryptobot](https://t.me/CryptoBot) asynchronous api wrapper**\n**Docs:** https://help.crypt.bot/crypto-pay-api\n\n - MainNet - [@CryptoBot](http://t.me/CryptoBot)\n - TestNet - [@CryptoTestnetBot](http://t.me/CryptoTestnetBot)\n\n\n**Install**\n``` bash\npip install aiocryptopay\npoetry add aiocryptopay\n```\n\n**Basic methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\nprofile = await crypto.get_me()\ncurrencies = await crypto.get_currencies()\nbalance = await crypto.get_balance()\nrates = await crypto.get_exchange_rates()\n\nprint(profile, currencies, balance, rates, sep='\\n')\n```\n\n**Create and get invoice methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\ninvoice = await crypto.create_invoice(asset='TON', amount=1.5)\nprint(invoice.pay_url)\n\ninvoices = await crypto.get_invoices(invoice_ids=invoice.invoice_id)\nprint(invoices.status)\n```\n\n**WebHook usage**\n``` python\nfrom aiohttp import web\n\nfrom aiocryptopay import AioCryptoPay, Networks\nfrom aiocryptopay.models.update import Update\n\n\nweb_app = web.Application()\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\n\n@crypto.pay_handler()\nasync def invoice_paid(update: Update) -> None:\n    print(update)\n\nasync def create_invoice(app) -> None:\n    invoice = await crypto.create_invoice(asset='TON', amount=1.5)\n    print(invoice.pay_url)\n\nasync def close_session(app) -> None:\n    await crypto.close()\n\n\nweb_app.add_routes([web.post('/crypto-secret-path', crypto.get_updates)])\nweb_app.on_startup.append(create_invoice)\nweb_app.on_shutdown.append(close_session)\nweb.run_app(app=web_app, host='localhost', port=3001)\n```",
+    'long_description': "## **[@cryptobot](https://t.me/CryptoBot) asynchronous api wrapper**\n**Docs:** https://help.crypt.bot/crypto-pay-api\n\n - MainNet - [@CryptoBot](http://t.me/CryptoBot)\n - TestNet - [@CryptoTestnetBot](http://t.me/CryptoTestnetBot)\n\n\n**Install**\n``` bash\npip install aiocryptopay\npoetry add aiocryptopay\n```\n\n**Basic methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\nprofile = await crypto.get_me()\ncurrencies = await crypto.get_currencies()\nbalance = await crypto.get_balance()\nrates = await crypto.get_exchange_rates()\n\nprint(profile, currencies, balance, rates, sep='\\n')\n```\n\n**Create and get invoice methods**\n``` python\nfrom aiocryptopay import AioCryptoPay, Networks\n\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\ninvoice = await crypto.create_invoice(asset='TON', amount=1.5)\nprint(invoice.pay_url)\n\ninvoices = await crypto.get_invoices(invoice_ids=invoice.invoice_id)\nprint(invoices.status)\n```\n\n**WebHook usage**\n``` python\nfrom aiohttp import web\n\nfrom aiocryptopay import AioCryptoPay, Networks\nfrom aiocryptopay.models.update import Update\n\n\nweb_app = web.Application()\ncrypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)\n\n\n@crypto.pay_handler()\nasync def invoice_paid(update: Update, app) -> None:\n    print(update)\n\nasync def create_invoice(app) -> None:\n    invoice = await crypto.create_invoice(asset='TON', amount=1.5)\n    print(invoice.pay_url)\n\nasync def close_session(app) -> None:\n    await crypto.close()\n\n\nweb_app.add_routes([web.post('/crypto-secret-path', crypto.get_updates)])\nweb_app.on_startup.append(create_invoice)\nweb_app.on_shutdown.append(close_session)\nweb.run_app(app=web_app, host='localhost', port=3001)\n```",
     'author': 'layerqa',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/layerqa/aiocryptopay',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aiocryptopay-0.2.7/PKG-INFO` & `aiocryptopay-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocryptopay
-Version: 0.2.7
+Version: 0.2.8
 Summary: @cryptobot api asynchronous python wrapper
 Home-page: https://github.com/layerqa/aiocryptopay
 License: MIT
 Keywords: aiocryptopay,cryptobot,cryptopay,cryptopay api,cryptobot api
 Author: layerqa
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -70,15 +70,15 @@
 
 
 web_app = web.Application()
 crypto = AioCryptoPay(token='1337:JHigdsaASq', network=Networks.MAIN_NET)
 
 
 @crypto.pay_handler()
-async def invoice_paid(update: Update) -> None:
+async def invoice_paid(update: Update, app) -> None:
     print(update)
 
 async def create_invoice(app) -> None:
     invoice = await crypto.create_invoice(asset='TON', amount=1.5)
     print(invoice.pay_url)
 
 async def close_session(app) -> None:
```

