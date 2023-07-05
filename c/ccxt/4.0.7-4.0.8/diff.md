# Comparing `tmp/ccxt-4.0.7.tar.gz` & `tmp/ccxt-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ccxt-4.0.7.tar", last modified: Tue Jul  4 14:58:12 2023, max compression
+gzip compressed data, was "dist/ccxt-4.0.8.tar", last modified: Wed Jul  5 06:16:25 2023, max compression
```

## Comparing `ccxt-4.0.7.tar` & `ccxt-4.0.8.tar`

### file list

```diff
@@ -1,474 +1,474 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.273276 ccxt-4.0.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-07-04 14:58:04.000000 ccxt-4.0.7/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-07-04 14:31:21.000000 ccxt-4.0.7/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)   113165 2023-07-04 14:58:12.277276 ccxt-4.0.7/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-07-04 14:31:21.000000 ccxt-4.0.7/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.121264 ccxt-4.0.7/ccxt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15341 2023-07-04 14:58:03.000000 ccxt-4.0.7/ccxt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.153267 ccxt-4.0.7/ccxt/abstract/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/abstract/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11197 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34928 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8397 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24027 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74318 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9298 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14890 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2507 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7216 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28171 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28171 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25398 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25398 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7866 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-07-04 14:32:42.000000 ccxt-4.0.7/ccxt/abstract/zonda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41372 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33434 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   132518 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.201270 ccxt-4.0.7/ccxt/async_support/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15114 2023-07-04 14:58:03.000000 ccxt-4.0.7/ccxt/async_support/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41596 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/ace.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33580 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   133150 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/ascendex.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.201270 ccxt-4.0.7/ccxt/async_support/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   140818 2023-07-04 14:58:03.000000 ccxt-4.0.7/ccxt/async_support/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/throttler.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.201270 ccxt-4.0.7/ccxt/async_support/base/ws/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/aiohttp_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/fast_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/future.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/base/ws/order_book_side.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79734 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   391701 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35726 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39541 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46269 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69830 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   112043 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38067 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32388 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   226741 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42834 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   132147 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   112719 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65841 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87826 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    90075 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69066 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84835 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17966 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    96414 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    80149 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74658 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16396 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47537 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35428 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22707 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48940 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22365 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35615 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   404940 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65326 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129993 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74334 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34425 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   195376 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39790 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35485 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88146 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18957 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125940 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82616 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85251 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119781 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152858 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89459 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   251121 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75041 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62700 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117105 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69604 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   365673 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87065 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67764 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30066 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42812 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   103339 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85935 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   170113 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101866 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38033 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70570 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33974 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    98087 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40838 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48840 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34917 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   210807 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106617 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62049 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37452 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   178293 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   286898 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24126 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   198396 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    94174 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76886 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74148 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42681 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65800 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119632 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75966 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110274 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35880 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92720 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   105131 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51896 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28985 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79823 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/async_support/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.217272 ccxt-4.0.7/ccxt/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/base/decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-07-04 14:41:54.000000 ccxt-4.0.7/ccxt/base/errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   180207 2023-07-04 14:58:03.000000 ccxt-4.0.7/ccxt/base/exchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/base/precise.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1406 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/base/types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79336 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bigone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   390455 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35520 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bit2c.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39281 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitbay.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46015 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitbns.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69390 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   111573 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37759 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitflyer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    32164 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitforex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   225849 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42616 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bithumb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   131509 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   112225 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65455 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87374 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    89701 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68680 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitso.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84395 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17820 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitstamp1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    95890 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79721 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74228 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bkex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16286 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bl3p.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    47109 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35150 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/btcalpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22513 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/btcbox.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48590 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/btcmarkets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22219 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/btctradeua.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35397 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/btcturk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   403034 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65000 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   129313 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73828 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34219 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coincheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   194478 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38972 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinfalcon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39542 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinmate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35261 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    87724 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinsph.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18823 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/coinspot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   125362 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    82206 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    84871 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/delta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119239 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   152152 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/digifinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    88917 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/flowbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/fmfwio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   250181 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    74551 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    62266 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   116419 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/hitbtc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    69182 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   364145 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    86583 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    67324 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29830 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42540 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/indodax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   102797 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85615 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   169463 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101396 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37785 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/kuna.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70178 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/latoken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33738 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/lbank.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    97539 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/lbank2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40530 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48538 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/lykke.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34675 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/mercado.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   209761 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   106093 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    61681 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/novadax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37114 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/oceanex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   177829 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/okex5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   285826 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23938 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/paymium.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   197800 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    93674 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    76518 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/poloniexfutures.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.249274 ccxt-4.0.7/ccxt/pro/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6376 2023-07-04 14:58:03.000000 ccxt-4.0.7/ccxt/pro/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26671 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/alpaca.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34555 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/ascendex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bequant.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    77505 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/binance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/binancecoinm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/binanceus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/binanceusdm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitcoincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitfinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42055 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitfinex2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46223 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24488 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitmart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    55612 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitmex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12562 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitopro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    54347 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitpanda.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16239 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitrue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitstamp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36718 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bittrex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26013 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bitvavo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31533 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/blockchaincom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    31150 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/btcex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60522 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/bybit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    44893 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/cex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/coinbaseprime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30100 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/coinbasepro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40963 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/coinex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22981 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/cryptocom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22094 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/currencycom.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    33997 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/deribit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24404 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/exmo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42098 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/gate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/gateio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/gemini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15165 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/hitbtc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21788 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/hollaex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    85593 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/huobi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23057 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/huobijp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/huobipro.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28083 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/idex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11060 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/independentreserve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    56308 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/kraken.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52064 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/krakenfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34134 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/kucoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27783 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/kucoinfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12170 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/luno.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41887 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/mexc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/mexc3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22660 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/ndax.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30238 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/okcoin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/okex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35660 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/okx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    59877 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/phemex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/poloniex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40500 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/poloniexfutures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22621 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/probit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/ripio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9476 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29892 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34479 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25028 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/pro/zb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73756 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/probit.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.249274 ccxt-4.0.7/ccxt/static_dependencies/
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.253275 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/curves.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/der.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/ecdsa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/keys.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/numbertheory.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/rfc6979.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/ecdsa/util.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.253275 ccxt-4.0.7/ccxt/static_dependencies/keccak/
--rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/keccak/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/static_dependencies/keccak/keccak.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.257275 ccxt-4.0.7/ccxt/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.273276 ccxt-4.0.7/ccxt/test/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-07-04 14:41:57.000000 ccxt-4.0.7/ccxt/test/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      980 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_account.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_balance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1797 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_borrow_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_borrow_rate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_calculate_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-07-04 14:41:56.000000 ccxt-4.0.7/ccxt/test/base/test_crypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_currency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2023-07-04 14:41:55.000000 ccxt-4.0.7/ccxt/test/base/test_datetime.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_decimal_to_precision.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_deep_extend.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_deposit_withdrawal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_exchange_datetime_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_funding_rate_history.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2369 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_ledger_entry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_ledger_item.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_leverage_tier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_margin_modification.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11190 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_market.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2023-07-04 14:41:55.000000 ccxt-4.0.7/ccxt/test/base/test_number.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_ohlcv.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_open_interest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_order.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3225 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_order_book.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3985 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_position.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16204 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_shared_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      783 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_throttle.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5658 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_ticker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_trade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2023-07-04 14:42:57.000000 ccxt-4.0.7/ccxt/test/base/test_trading_fee.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/test/base/test_transaction.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26228 2023-07-04 14:41:57.000000 ccxt-4.0.7/ccxt/test/test_async.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25824 2023-07-04 14:41:57.000000 ccxt-4.0.7/ccxt/test/test_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42433 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/tidex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    65468 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/timex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   119288 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/tokocrypto.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    75532 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/upbit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   109730 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/wavesexchange.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35632 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/wazirx.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    92268 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/whitebit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   104529 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/woo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    51612 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/yobit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28803 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/zaif.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    79521 2023-07-04 14:31:21.000000 ccxt-4.0.7/ccxt/zonda.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-04 14:58:12.121264 ccxt-4.0.7/ccxt.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)   113165 2023-07-04 14:58:11.000000 ccxt-4.0.7/ccxt.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    11393 2023-07-04 14:58:12.000000 ccxt-4.0.7/ccxt.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-04 14:58:11.000000 ccxt-4.0.7/ccxt.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-04 14:58:11.000000 ccxt-4.0.7/ccxt.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-07-04 14:58:11.000000 ccxt-4.0.7/ccxt.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8698 2023-07-04 14:58:04.000000 ccxt-4.0.7/package.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-07-04 14:58:12.277276 ccxt-4.0.7/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-07-04 14:31:21.000000 ccxt-4.0.7/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.849480 ccxt-4.0.8/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1068 2023-07-05 06:16:18.000000 ccxt-4.0.8/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2023-07-05 05:50:18.000000 ccxt-4.0.8/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113165 2023-07-05 06:16:25.853481 ccxt-4.0.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102253 2023-07-05 05:50:18.000000 ccxt-4.0.8/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.753471 ccxt-4.0.8/ccxt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15341 2023-07-05 06:16:17.000000 ccxt-4.0.8/ccxt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.777474 ccxt-4.0.8/ccxt/abstract/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/abstract/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1448 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1861 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11197 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76029 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2830 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2606 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4082 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7605 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19171 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3576 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2789 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34928 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2659 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9098 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8397 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2919 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3859 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3648 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4025 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24027 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1987 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9337 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7439 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2638 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1380 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      849 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3690 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1403 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74318 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3311 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9298 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6952 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3417 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14890 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2182 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2507 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7216 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2707 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21126 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7563 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5107 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15499 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9386 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6177 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28171 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28171 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6915 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8376 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10949 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2596 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14331 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95821 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2129 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4165 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2266 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4979 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2867 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20600 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21746 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19005 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7168 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1474 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6930 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3566 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2960 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25398 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25398 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11878 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2565 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1721 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25825 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30191 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2752 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12172 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6301 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4575 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1969 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1953 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5875 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4094 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3463 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18450 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2130 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7934 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7866 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1339 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3935 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5482 2023-07-05 05:51:35.000000 ccxt-4.0.8/ccxt/abstract/zonda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41372 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33434 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   132518 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.809477 ccxt-4.0.8/ccxt/async_support/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15114 2023-07-05 06:16:17.000000 ccxt-4.0.8/ccxt/async_support/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41596 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/ace.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33580 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   133150 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/ascendex.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.813477 ccxt-4.0.8/ccxt/async_support/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   140818 2023-07-05 06:16:17.000000 ccxt-4.0.8/ccxt/async_support/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1847 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/throttler.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.813477 ccxt-4.0.8/ccxt/async_support/base/ws/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1791 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4999 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/aiohttp_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6085 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7289 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/fast_client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1495 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      249 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/future.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2894 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6079 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/base/ws/order_book_side.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1150 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79734 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   391701 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1683 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2165 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2518 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35726 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39541 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46269 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      481 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69830 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   112043 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38067 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32388 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   226741 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42834 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   132147 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   112719 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65841 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87826 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    90075 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69066 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84835 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17966 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    96414 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    80149 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74658 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16396 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47537 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35428 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22707 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48940 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22365 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35615 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   404940 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65326 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129993 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1233 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74334 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34425 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   195376 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39268 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39790 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35485 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88146 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18957 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125940 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82616 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85251 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119781 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152858 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89459 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1252 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   251121 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      459 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75041 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62700 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117105 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69604 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   365673 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87065 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      586 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67764 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30066 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42812 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   103339 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85935 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   170113 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101866 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38033 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70570 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33974 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    98087 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40838 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48840 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34917 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   210807 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106617 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62049 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37452 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   178293 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      455 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   286898 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24126 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   198396 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    94174 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76886 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74281 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42681 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65800 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119632 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75966 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110274 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35880 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92720 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   105131 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51896 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28985 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79823 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/async_support/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.813477 ccxt-4.0.8/ccxt/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1320 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6634 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/base/decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3401 2023-07-05 06:00:43.000000 ccxt-4.0.8/ccxt/base/errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180207 2023-07-05 06:16:17.000000 ccxt-4.0.8/ccxt/base/exchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8565 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/base/precise.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1406 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/base/types.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79336 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bigone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   390455 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1645 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2151 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2480 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35520 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bit2c.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39281 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      448 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitbay.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46015 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitbns.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      467 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69390 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   111573 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37759 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitflyer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32164 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitforex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   225849 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42616 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bithumb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   131509 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   112225 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65455 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87374 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    89701 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68680 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitso.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84395 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17820 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitstamp1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    95890 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79721 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74228 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bkex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16286 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bl3p.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    47109 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35150 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/btcalpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22513 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/btcbox.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48590 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/btcmarkets.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22219 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/btctradeua.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35397 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/btcturk.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   403034 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65000 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   129313 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1219 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73828 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34219 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coincheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   194478 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38972 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinfalcon.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39542 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinmate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35261 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinone.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    87724 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinsph.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18823 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/coinspot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   125362 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    82206 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    84871 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/delta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119239 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   152152 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/digifinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    88917 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1169 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/flowbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1238 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/fmfwio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   250181 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    74551 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    62266 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   116419 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/hitbtc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    69182 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   364145 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    86583 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      572 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    67324 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29830 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42540 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/indodax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   102797 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85615 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   169463 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101396 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37785 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/kuna.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70178 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/latoken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33738 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/lbank.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    97539 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/lbank2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40530 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48538 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/lykke.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34675 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/mercado.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   209761 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   106093 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    61681 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/novadax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37114 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/oceanex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   177829 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      434 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/okex5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   285826 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23938 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/paymium.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   197800 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    93674 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    76518 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/poloniexfutures.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.833479 ccxt-4.0.8/ccxt/pro/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6376 2023-07-05 06:16:17.000000 ccxt-4.0.8/ccxt/pro/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26671 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/alpaca.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34555 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/ascendex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bequant.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    77505 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/binance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      724 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/binancecoinm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2016 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/binanceus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1357 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/binanceusdm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      914 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitcoincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24762 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitfinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42055 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitfinex2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46223 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24488 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitmart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    55612 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitmex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12562 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitopro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54347 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitpanda.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16239 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitrue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20782 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitstamp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36718 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bittrex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26013 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bitvavo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31533 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/blockchaincom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    31150 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/btcex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60522 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/bybit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    44893 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/cex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1121 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/coinbaseprime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30100 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/coinbasepro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40963 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/coinex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22981 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/cryptocom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22094 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/currencycom.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33997 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/deribit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24404 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/exmo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42098 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/gate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      391 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/gateio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25142 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/gemini.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15165 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/hitbtc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21788 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/hollaex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    85593 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/huobi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23057 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/huobijp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      400 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/huobipro.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28083 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/idex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11060 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/independentreserve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    56308 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/kraken.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52064 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/krakenfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34134 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/kucoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    27783 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/kucoinfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12170 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/luno.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41887 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/mexc.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      388 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/mexc3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22660 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/ndax.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30238 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/okcoin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      382 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/okex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35660 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/okx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    59877 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/phemex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    41839 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/poloniex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40500 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/poloniexfutures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22621 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/probit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12104 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/ripio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9476 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29892 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    34479 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25028 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21557 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/pro/zb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    73889 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/probit.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.833479 ccxt-4.0.8/ccxt/static_dependencies/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.837479 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18461 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/curves.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6942 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/der.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11336 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/ecdsa.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5517 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14201 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/keys.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13468 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/numbertheory.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/rfc6979.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10037 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/ecdsa/util.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.837479 ccxt-4.0.8/ccxt/static_dependencies/keccak/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       45 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/keccak/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6934 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/static_dependencies/keccak/keccak.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.841480 ccxt-4.0.8/ccxt/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.849480 ccxt-4.0.8/ccxt/test/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1745 2023-07-05 06:00:45.000000 ccxt-4.0.8/ccxt/test/base/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      980 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_account.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2617 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_balance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1797 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_borrow_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_borrow_rate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1177 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_calculate_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7702 2023-07-05 06:00:44.000000 ccxt-4.0.8/ccxt/test/base/test_crypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3696 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_currency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2023-07-05 06:00:44.000000 ccxt-4.0.8/ccxt/test/base/test_datetime.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20934 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_decimal_to_precision.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_deep_extend.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_deposit_withdrawal.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3592 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_exchange_datetime_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1340 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_funding_rate_history.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2369 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_ledger_entry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2154 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_ledger_item.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1658 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_leverage_tier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1732 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_margin_modification.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11190 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_market.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22083 2023-07-05 06:00:44.000000 ccxt-4.0.8/ccxt/test/base/test_number.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_ohlcv.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1463 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_open_interest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3889 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_order.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3225 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_order_book.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3985 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_position.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16204 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_shared_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      783 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3123 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_throttle.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5658 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_ticker.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_trade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2023-07-05 06:01:43.000000 ccxt-4.0.8/ccxt/test/base/test_trading_fee.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/test/base/test_transaction.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26228 2023-07-05 06:00:45.000000 ccxt-4.0.8/ccxt/test/test_async.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25824 2023-07-05 06:00:45.000000 ccxt-4.0.8/ccxt/test/test_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    42433 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/tidex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    65468 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/timex.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   119288 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/tokocrypto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    75532 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/upbit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   109730 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/wavesexchange.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35632 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/wazirx.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    92268 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/whitebit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   104529 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/woo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    51612 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/yobit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28803 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/zaif.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    79521 2023-07-05 05:50:18.000000 ccxt-4.0.8/ccxt/zonda.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-05 06:16:25.757472 ccxt-4.0.8/ccxt.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   113165 2023-07-05 06:16:25.000000 ccxt-4.0.8/ccxt.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11393 2023-07-05 06:16:25.000000 ccxt-4.0.8/ccxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-05 06:16:25.000000 ccxt-4.0.8/ccxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      162 2023-07-05 06:16:25.000000 ccxt-4.0.8/ccxt.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        5 2023-07-05 06:16:25.000000 ccxt-4.0.8/ccxt.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8698 2023-07-05 06:16:18.000000 ccxt-4.0.8/package.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      205 2023-07-05 06:16:25.853481 ccxt-4.0.8/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2891 2023-07-05 05:50:18.000000 ccxt-4.0.8/setup.py
```

### Comparing `ccxt-4.0.7/LICENSE.txt` & `ccxt-4.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/PKG-INFO` & `ccxt-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.0.7
+Version: 4.0.8
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.0.7/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.0.7/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.0.8/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.0.8/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.0.7/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.0.8/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.0.7/README.rst` & `ccxt-4.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/__init__.py` & `ccxt-4.0.8/ccxt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.0.7'
+__version__ = '4.0.8'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.base.exchange import Exchange                     # noqa: F401
 from ccxt.base.precise import Precise                       # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
```

### Comparing `ccxt-4.0.7/ccxt/abstract/ace.py` & `ccxt-4.0.8/ccxt/abstract/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/alpaca.py` & `ccxt-4.0.8/ccxt/abstract/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/ascendex.py` & `ccxt-4.0.8/ccxt/abstract/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bequant.py` & `ccxt-4.0.8/ccxt/abstract/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bigone.py` & `ccxt-4.0.8/ccxt/abstract/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/binance.py` & `ccxt-4.0.8/ccxt/abstract/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/binancecoinm.py` & `ccxt-4.0.8/ccxt/abstract/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/binanceus.py` & `ccxt-4.0.8/ccxt/abstract/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/binanceusdm.py` & `ccxt-4.0.8/ccxt/abstract/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bit2c.py` & `ccxt-4.0.8/ccxt/abstract/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitbank.py` & `ccxt-4.0.8/ccxt/abstract/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitbay.py` & `ccxt-4.0.8/ccxt/abstract/bitbay.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitbns.py` & `ccxt-4.0.8/ccxt/abstract/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitcoincom.py` & `ccxt-4.0.8/ccxt/abstract/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitfinex.py` & `ccxt-4.0.8/ccxt/abstract/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitfinex2.py` & `ccxt-4.0.8/ccxt/abstract/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitflyer.py` & `ccxt-4.0.8/ccxt/abstract/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitforex.py` & `ccxt-4.0.8/ccxt/abstract/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitget.py` & `ccxt-4.0.8/ccxt/abstract/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bithumb.py` & `ccxt-4.0.8/ccxt/abstract/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitmart.py` & `ccxt-4.0.8/ccxt/abstract/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitmex.py` & `ccxt-4.0.8/ccxt/abstract/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitopro.py` & `ccxt-4.0.8/ccxt/abstract/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitpanda.py` & `ccxt-4.0.8/ccxt/abstract/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitrue.py` & `ccxt-4.0.8/ccxt/abstract/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitso.py` & `ccxt-4.0.8/ccxt/abstract/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitstamp.py` & `ccxt-4.0.8/ccxt/abstract/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitstamp1.py` & `ccxt-4.0.8/ccxt/abstract/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bittrex.py` & `ccxt-4.0.8/ccxt/abstract/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bitvavo.py` & `ccxt-4.0.8/ccxt/abstract/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bkex.py` & `ccxt-4.0.8/ccxt/abstract/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bl3p.py` & `ccxt-4.0.8/ccxt/abstract/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/blockchaincom.py` & `ccxt-4.0.8/ccxt/abstract/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/btcalpha.py` & `ccxt-4.0.8/ccxt/abstract/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/btcbox.py` & `ccxt-4.0.8/ccxt/abstract/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/btcmarkets.py` & `ccxt-4.0.8/ccxt/abstract/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/btctradeua.py` & `ccxt-4.0.8/ccxt/abstract/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/btcturk.py` & `ccxt-4.0.8/ccxt/abstract/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/bybit.py` & `ccxt-4.0.8/ccxt/abstract/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/cex.py` & `ccxt-4.0.8/ccxt/abstract/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinbase.py` & `ccxt-4.0.8/ccxt/abstract/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinbaseprime.py` & `ccxt-4.0.8/ccxt/abstract/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinbasepro.py` & `ccxt-4.0.8/ccxt/abstract/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coincheck.py` & `ccxt-4.0.8/ccxt/abstract/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinex.py` & `ccxt-4.0.8/ccxt/abstract/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinfalcon.py` & `ccxt-4.0.8/ccxt/abstract/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinmate.py` & `ccxt-4.0.8/ccxt/abstract/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinone.py` & `ccxt-4.0.8/ccxt/abstract/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinsph.py` & `ccxt-4.0.8/ccxt/abstract/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/coinspot.py` & `ccxt-4.0.8/ccxt/abstract/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/cryptocom.py` & `ccxt-4.0.8/ccxt/abstract/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/currencycom.py` & `ccxt-4.0.8/ccxt/abstract/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/delta.py` & `ccxt-4.0.8/ccxt/abstract/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/deribit.py` & `ccxt-4.0.8/ccxt/abstract/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/digifinex.py` & `ccxt-4.0.8/ccxt/abstract/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/exmo.py` & `ccxt-4.0.8/ccxt/abstract/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/fmfwio.py` & `ccxt-4.0.8/ccxt/abstract/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/gate.py` & `ccxt-4.0.8/ccxt/abstract/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/gateio.py` & `ccxt-4.0.8/ccxt/abstract/gateio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/gemini.py` & `ccxt-4.0.8/ccxt/abstract/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/hitbtc.py` & `ccxt-4.0.8/ccxt/abstract/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/hitbtc3.py` & `ccxt-4.0.8/ccxt/abstract/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/hollaex.py` & `ccxt-4.0.8/ccxt/abstract/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/huobi.py` & `ccxt-4.0.8/ccxt/abstract/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/huobijp.py` & `ccxt-4.0.8/ccxt/abstract/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/huobipro.py` & `ccxt-4.0.8/ccxt/abstract/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/idex.py` & `ccxt-4.0.8/ccxt/abstract/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/independentreserve.py` & `ccxt-4.0.8/ccxt/abstract/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/indodax.py` & `ccxt-4.0.8/ccxt/abstract/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/kraken.py` & `ccxt-4.0.8/ccxt/abstract/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/krakenfutures.py` & `ccxt-4.0.8/ccxt/abstract/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/kucoin.py` & `ccxt-4.0.8/ccxt/abstract/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/kucoinfutures.py` & `ccxt-4.0.8/ccxt/abstract/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/kuna.py` & `ccxt-4.0.8/ccxt/abstract/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/latoken.py` & `ccxt-4.0.8/ccxt/abstract/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/lbank.py` & `ccxt-4.0.8/ccxt/abstract/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/lbank2.py` & `ccxt-4.0.8/ccxt/abstract/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/luno.py` & `ccxt-4.0.8/ccxt/abstract/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/lykke.py` & `ccxt-4.0.8/ccxt/abstract/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/mercado.py` & `ccxt-4.0.8/ccxt/abstract/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/mexc.py` & `ccxt-4.0.8/ccxt/abstract/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/mexc3.py` & `ccxt-4.0.8/ccxt/abstract/mexc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/ndax.py` & `ccxt-4.0.8/ccxt/abstract/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/novadax.py` & `ccxt-4.0.8/ccxt/abstract/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/oceanex.py` & `ccxt-4.0.8/ccxt/abstract/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/okcoin.py` & `ccxt-4.0.8/ccxt/abstract/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/okex.py` & `ccxt-4.0.8/ccxt/abstract/okex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/okex5.py` & `ccxt-4.0.8/ccxt/abstract/okex5.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/okx.py` & `ccxt-4.0.8/ccxt/abstract/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/paymium.py` & `ccxt-4.0.8/ccxt/abstract/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/phemex.py` & `ccxt-4.0.8/ccxt/abstract/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/poloniex.py` & `ccxt-4.0.8/ccxt/abstract/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/poloniexfutures.py` & `ccxt-4.0.8/ccxt/abstract/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/probit.py` & `ccxt-4.0.8/ccxt/abstract/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/tidex.py` & `ccxt-4.0.8/ccxt/abstract/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/timex.py` & `ccxt-4.0.8/ccxt/abstract/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/tokocrypto.py` & `ccxt-4.0.8/ccxt/abstract/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/upbit.py` & `ccxt-4.0.8/ccxt/abstract/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/wavesexchange.py` & `ccxt-4.0.8/ccxt/abstract/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/wazirx.py` & `ccxt-4.0.8/ccxt/abstract/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/whitebit.py` & `ccxt-4.0.8/ccxt/abstract/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/woo.py` & `ccxt-4.0.8/ccxt/abstract/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/yobit.py` & `ccxt-4.0.8/ccxt/abstract/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/zaif.py` & `ccxt-4.0.8/ccxt/abstract/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/abstract/zonda.py` & `ccxt-4.0.8/ccxt/abstract/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/ace.py` & `ccxt-4.0.8/ccxt/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/alpaca.py` & `ccxt-4.0.8/ccxt/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/ascendex.py` & `ccxt-4.0.8/ccxt/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/__init__.py` & `ccxt-4.0.8/ccxt/async_support/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.0.7'
+__version__ = '4.0.8'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange                   # noqa: F401
 
 from ccxt.base.decimal_to_precision import decimal_to_precision  # noqa: F401
 from ccxt.base.decimal_to_precision import TRUNCATE              # noqa: F401
```

### Comparing `ccxt-4.0.7/ccxt/async_support/ace.py` & `ccxt-4.0.8/ccxt/async_support/ace.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/alpaca.py` & `ccxt-4.0.8/ccxt/async_support/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/ascendex.py` & `ccxt-4.0.8/ccxt/async_support/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/exchange.py` & `ccxt-4.0.8/ccxt/async_support/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.0.7'
+__version__ = '4.0.8'
 
 # -----------------------------------------------------------------------------
 
 import asyncio
 import concurrent.futures
 import socket
 import certifi
```

### Comparing `ccxt-4.0.7/ccxt/async_support/base/throttler.py` & `ccxt-4.0.8/ccxt/async_support/base/throttler.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/__init__.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/aiohttp_client.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/cache.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/cache.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/client.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/fast_client.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/fast_client.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/functions.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/order_book.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/base/ws/order_book_side.py` & `ccxt-4.0.8/ccxt/async_support/base/ws/order_book_side.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bequant.py` & `ccxt-4.0.8/ccxt/async_support/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bigone.py` & `ccxt-4.0.8/ccxt/async_support/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/binance.py` & `ccxt-4.0.8/ccxt/async_support/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/binancecoinm.py` & `ccxt-4.0.8/ccxt/async_support/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/binanceus.py` & `ccxt-4.0.8/ccxt/async_support/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/binanceusdm.py` & `ccxt-4.0.8/ccxt/async_support/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bit2c.py` & `ccxt-4.0.8/ccxt/async_support/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitbank.py` & `ccxt-4.0.8/ccxt/async_support/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitbns.py` & `ccxt-4.0.8/ccxt/async_support/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitfinex.py` & `ccxt-4.0.8/ccxt/async_support/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitfinex2.py` & `ccxt-4.0.8/ccxt/async_support/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitflyer.py` & `ccxt-4.0.8/ccxt/async_support/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitforex.py` & `ccxt-4.0.8/ccxt/async_support/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitget.py` & `ccxt-4.0.8/ccxt/async_support/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bithumb.py` & `ccxt-4.0.8/ccxt/async_support/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitmart.py` & `ccxt-4.0.8/ccxt/async_support/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitmex.py` & `ccxt-4.0.8/ccxt/async_support/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitopro.py` & `ccxt-4.0.8/ccxt/async_support/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitpanda.py` & `ccxt-4.0.8/ccxt/async_support/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitrue.py` & `ccxt-4.0.8/ccxt/async_support/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitso.py` & `ccxt-4.0.8/ccxt/async_support/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitstamp.py` & `ccxt-4.0.8/ccxt/async_support/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitstamp1.py` & `ccxt-4.0.8/ccxt/async_support/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bittrex.py` & `ccxt-4.0.8/ccxt/async_support/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bitvavo.py` & `ccxt-4.0.8/ccxt/async_support/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bkex.py` & `ccxt-4.0.8/ccxt/async_support/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bl3p.py` & `ccxt-4.0.8/ccxt/async_support/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/blockchaincom.py` & `ccxt-4.0.8/ccxt/async_support/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/btcalpha.py` & `ccxt-4.0.8/ccxt/async_support/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/btcbox.py` & `ccxt-4.0.8/ccxt/async_support/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/btcmarkets.py` & `ccxt-4.0.8/ccxt/async_support/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/btctradeua.py` & `ccxt-4.0.8/ccxt/async_support/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/btcturk.py` & `ccxt-4.0.8/ccxt/async_support/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/bybit.py` & `ccxt-4.0.8/ccxt/async_support/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/cex.py` & `ccxt-4.0.8/ccxt/async_support/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinbase.py` & `ccxt-4.0.8/ccxt/async_support/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinbaseprime.py` & `ccxt-4.0.8/ccxt/async_support/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinbasepro.py` & `ccxt-4.0.8/ccxt/async_support/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coincheck.py` & `ccxt-4.0.8/ccxt/async_support/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinex.py` & `ccxt-4.0.8/ccxt/async_support/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinfalcon.py` & `ccxt-4.0.8/ccxt/async_support/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinmate.py` & `ccxt-4.0.8/ccxt/async_support/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinone.py` & `ccxt-4.0.8/ccxt/async_support/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinsph.py` & `ccxt-4.0.8/ccxt/async_support/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/coinspot.py` & `ccxt-4.0.8/ccxt/async_support/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/cryptocom.py` & `ccxt-4.0.8/ccxt/async_support/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/currencycom.py` & `ccxt-4.0.8/ccxt/async_support/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/delta.py` & `ccxt-4.0.8/ccxt/async_support/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/deribit.py` & `ccxt-4.0.8/ccxt/async_support/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/digifinex.py` & `ccxt-4.0.8/ccxt/async_support/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/exmo.py` & `ccxt-4.0.8/ccxt/async_support/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/flowbtc.py` & `ccxt-4.0.8/ccxt/async_support/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/fmfwio.py` & `ccxt-4.0.8/ccxt/async_support/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/gate.py` & `ccxt-4.0.8/ccxt/async_support/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/gemini.py` & `ccxt-4.0.8/ccxt/async_support/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/hitbtc.py` & `ccxt-4.0.8/ccxt/async_support/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/hitbtc3.py` & `ccxt-4.0.8/ccxt/async_support/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/hollaex.py` & `ccxt-4.0.8/ccxt/async_support/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/huobi.py` & `ccxt-4.0.8/ccxt/async_support/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/huobijp.py` & `ccxt-4.0.8/ccxt/async_support/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/huobipro.py` & `ccxt-4.0.8/ccxt/async_support/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/idex.py` & `ccxt-4.0.8/ccxt/async_support/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/independentreserve.py` & `ccxt-4.0.8/ccxt/async_support/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/indodax.py` & `ccxt-4.0.8/ccxt/async_support/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/kraken.py` & `ccxt-4.0.8/ccxt/async_support/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/krakenfutures.py` & `ccxt-4.0.8/ccxt/async_support/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/kucoin.py` & `ccxt-4.0.8/ccxt/async_support/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/kucoinfutures.py` & `ccxt-4.0.8/ccxt/async_support/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/kuna.py` & `ccxt-4.0.8/ccxt/async_support/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/latoken.py` & `ccxt-4.0.8/ccxt/async_support/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/lbank.py` & `ccxt-4.0.8/ccxt/async_support/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/lbank2.py` & `ccxt-4.0.8/ccxt/async_support/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/luno.py` & `ccxt-4.0.8/ccxt/async_support/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/lykke.py` & `ccxt-4.0.8/ccxt/async_support/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/mercado.py` & `ccxt-4.0.8/ccxt/async_support/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/mexc.py` & `ccxt-4.0.8/ccxt/async_support/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/ndax.py` & `ccxt-4.0.8/ccxt/async_support/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/novadax.py` & `ccxt-4.0.8/ccxt/async_support/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/oceanex.py` & `ccxt-4.0.8/ccxt/async_support/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/okcoin.py` & `ccxt-4.0.8/ccxt/async_support/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/okx.py` & `ccxt-4.0.8/ccxt/async_support/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/paymium.py` & `ccxt-4.0.8/ccxt/async_support/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/phemex.py` & `ccxt-4.0.8/ccxt/async_support/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/poloniex.py` & `ccxt-4.0.8/ccxt/async_support/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/poloniexfutures.py` & `ccxt-4.0.8/ccxt/async_support/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/probit.py` & `ccxt-4.0.8/ccxt/async_support/probit.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 'fetchBorrowRates': False,
                 'fetchBorrowRatesPerSymbol': False,
                 'fetchClosedOrders': True,
                 'fetchCurrencies': True,
                 'fetchDepositAddress': True,
                 'fetchDepositAddresses': True,
                 'fetchDeposits': True,
+                'fetchDepositsWithdrawals': True,
                 'fetchFundingHistory': False,
                 'fetchFundingRate': False,
                 'fetchFundingRateHistory': False,
                 'fetchFundingRates': False,
                 'fetchIndexOHLCV': False,
                 'fetchLeverage': False,
                 'fetchLeverageTiers': False,
@@ -1391,15 +1392,17 @@
             'type': 'withdrawal',
         }
         result = await self.fetch_transactions(code, since, limit, self.extend(request, params))
         return result
 
     async def fetch_transactions(self, code: Optional[str] = None, since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
-        fetch all transactions made to an account
+         * @deprecated
+        use fetchDepositsWithdrawals instead
+        see https://docs-en.probit.com/reference/transferpayment
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch transactions for
         :param int [limit]: the maximum number of transaction structures to retrieve
         :param dict [params]: extra parameters specific to the probit api endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         await self.load_markets()
```

### Comparing `ccxt-4.0.7/ccxt/async_support/tidex.py` & `ccxt-4.0.8/ccxt/async_support/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/timex.py` & `ccxt-4.0.8/ccxt/async_support/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/tokocrypto.py` & `ccxt-4.0.8/ccxt/async_support/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/upbit.py` & `ccxt-4.0.8/ccxt/async_support/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/wavesexchange.py` & `ccxt-4.0.8/ccxt/async_support/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/wazirx.py` & `ccxt-4.0.8/ccxt/async_support/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/whitebit.py` & `ccxt-4.0.8/ccxt/async_support/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/woo.py` & `ccxt-4.0.8/ccxt/async_support/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/yobit.py` & `ccxt-4.0.8/ccxt/async_support/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/zaif.py` & `ccxt-4.0.8/ccxt/async_support/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/async_support/zonda.py` & `ccxt-4.0.8/ccxt/async_support/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/base/__init__.py` & `ccxt-4.0.8/ccxt/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/base/decimal_to_precision.py` & `ccxt-4.0.8/ccxt/base/decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/base/errors.py` & `ccxt-4.0.8/ccxt/base/errors.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/base/exchange.py` & `ccxt-4.0.8/ccxt/base/exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Base exchange class"""
 
 # -----------------------------------------------------------------------------
 
-__version__ = '4.0.7'
+__version__ = '4.0.8'
 
 # -----------------------------------------------------------------------------
 
 from ccxt.base.errors import ExchangeError
 from ccxt.base.errors import NetworkError
 from ccxt.base.errors import NotSupported
 from ccxt.base.errors import AuthenticationError
```

### Comparing `ccxt-4.0.7/ccxt/base/precise.py` & `ccxt-4.0.8/ccxt/base/precise.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/base/types.py` & `ccxt-4.0.8/ccxt/base/types.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bequant.py` & `ccxt-4.0.8/ccxt/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bigone.py` & `ccxt-4.0.8/ccxt/bigone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/binance.py` & `ccxt-4.0.8/ccxt/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/binancecoinm.py` & `ccxt-4.0.8/ccxt/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/binanceus.py` & `ccxt-4.0.8/ccxt/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/binanceusdm.py` & `ccxt-4.0.8/ccxt/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bit2c.py` & `ccxt-4.0.8/ccxt/bit2c.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitbank.py` & `ccxt-4.0.8/ccxt/bitbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitbns.py` & `ccxt-4.0.8/ccxt/bitbns.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitfinex.py` & `ccxt-4.0.8/ccxt/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitfinex2.py` & `ccxt-4.0.8/ccxt/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitflyer.py` & `ccxt-4.0.8/ccxt/bitflyer.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitforex.py` & `ccxt-4.0.8/ccxt/bitforex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitget.py` & `ccxt-4.0.8/ccxt/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bithumb.py` & `ccxt-4.0.8/ccxt/bithumb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitmart.py` & `ccxt-4.0.8/ccxt/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitmex.py` & `ccxt-4.0.8/ccxt/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitopro.py` & `ccxt-4.0.8/ccxt/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitpanda.py` & `ccxt-4.0.8/ccxt/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitrue.py` & `ccxt-4.0.8/ccxt/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitso.py` & `ccxt-4.0.8/ccxt/bitso.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitstamp.py` & `ccxt-4.0.8/ccxt/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitstamp1.py` & `ccxt-4.0.8/ccxt/bitstamp1.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bittrex.py` & `ccxt-4.0.8/ccxt/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bitvavo.py` & `ccxt-4.0.8/ccxt/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bkex.py` & `ccxt-4.0.8/ccxt/bkex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bl3p.py` & `ccxt-4.0.8/ccxt/bl3p.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/blockchaincom.py` & `ccxt-4.0.8/ccxt/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/btcalpha.py` & `ccxt-4.0.8/ccxt/btcalpha.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/btcbox.py` & `ccxt-4.0.8/ccxt/btcbox.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/btcmarkets.py` & `ccxt-4.0.8/ccxt/btcmarkets.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/btctradeua.py` & `ccxt-4.0.8/ccxt/btctradeua.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/btcturk.py` & `ccxt-4.0.8/ccxt/btcturk.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/bybit.py` & `ccxt-4.0.8/ccxt/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/cex.py` & `ccxt-4.0.8/ccxt/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinbase.py` & `ccxt-4.0.8/ccxt/coinbase.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinbaseprime.py` & `ccxt-4.0.8/ccxt/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinbasepro.py` & `ccxt-4.0.8/ccxt/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coincheck.py` & `ccxt-4.0.8/ccxt/coincheck.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinex.py` & `ccxt-4.0.8/ccxt/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinfalcon.py` & `ccxt-4.0.8/ccxt/coinfalcon.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinmate.py` & `ccxt-4.0.8/ccxt/coinmate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinone.py` & `ccxt-4.0.8/ccxt/coinone.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinsph.py` & `ccxt-4.0.8/ccxt/coinsph.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/coinspot.py` & `ccxt-4.0.8/ccxt/coinspot.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/cryptocom.py` & `ccxt-4.0.8/ccxt/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/currencycom.py` & `ccxt-4.0.8/ccxt/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/delta.py` & `ccxt-4.0.8/ccxt/delta.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/deribit.py` & `ccxt-4.0.8/ccxt/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/digifinex.py` & `ccxt-4.0.8/ccxt/digifinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/exmo.py` & `ccxt-4.0.8/ccxt/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/flowbtc.py` & `ccxt-4.0.8/ccxt/flowbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/fmfwio.py` & `ccxt-4.0.8/ccxt/fmfwio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/gate.py` & `ccxt-4.0.8/ccxt/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/gemini.py` & `ccxt-4.0.8/ccxt/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/hitbtc.py` & `ccxt-4.0.8/ccxt/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/hitbtc3.py` & `ccxt-4.0.8/ccxt/hitbtc3.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/hollaex.py` & `ccxt-4.0.8/ccxt/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/huobi.py` & `ccxt-4.0.8/ccxt/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/huobijp.py` & `ccxt-4.0.8/ccxt/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/huobipro.py` & `ccxt-4.0.8/ccxt/huobipro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/idex.py` & `ccxt-4.0.8/ccxt/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/independentreserve.py` & `ccxt-4.0.8/ccxt/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/indodax.py` & `ccxt-4.0.8/ccxt/indodax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/kraken.py` & `ccxt-4.0.8/ccxt/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/krakenfutures.py` & `ccxt-4.0.8/ccxt/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/kucoin.py` & `ccxt-4.0.8/ccxt/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/kucoinfutures.py` & `ccxt-4.0.8/ccxt/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/kuna.py` & `ccxt-4.0.8/ccxt/kuna.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/latoken.py` & `ccxt-4.0.8/ccxt/latoken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/lbank.py` & `ccxt-4.0.8/ccxt/lbank.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/lbank2.py` & `ccxt-4.0.8/ccxt/lbank2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/luno.py` & `ccxt-4.0.8/ccxt/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/lykke.py` & `ccxt-4.0.8/ccxt/lykke.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/mercado.py` & `ccxt-4.0.8/ccxt/mercado.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/mexc.py` & `ccxt-4.0.8/ccxt/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/ndax.py` & `ccxt-4.0.8/ccxt/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/novadax.py` & `ccxt-4.0.8/ccxt/novadax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/oceanex.py` & `ccxt-4.0.8/ccxt/oceanex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/okcoin.py` & `ccxt-4.0.8/ccxt/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/okx.py` & `ccxt-4.0.8/ccxt/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/paymium.py` & `ccxt-4.0.8/ccxt/paymium.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/phemex.py` & `ccxt-4.0.8/ccxt/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/poloniex.py` & `ccxt-4.0.8/ccxt/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/poloniexfutures.py` & `ccxt-4.0.8/ccxt/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/__init__.py` & `ccxt-4.0.8/ccxt/pro/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """CCXT: CryptoCurrency eXchange Trading Library (Async)"""
 
 # ----------------------------------------------------------------------------
 
-__version__ = '4.0.7'
+__version__ = '4.0.8'
 
 # ----------------------------------------------------------------------------
 
 from ccxt.async_support.base.exchange import Exchange  # noqa: F401
 
 # CCXT Pro exchanges (now this is mainly used for importing exchanges in WS tests)
```

### Comparing `ccxt-4.0.7/ccxt/pro/alpaca.py` & `ccxt-4.0.8/ccxt/pro/alpaca.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/ascendex.py` & `ccxt-4.0.8/ccxt/pro/ascendex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bequant.py` & `ccxt-4.0.8/ccxt/pro/bequant.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/binance.py` & `ccxt-4.0.8/ccxt/pro/binance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/binancecoinm.py` & `ccxt-4.0.8/ccxt/pro/binancecoinm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/binanceus.py` & `ccxt-4.0.8/ccxt/pro/binanceus.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/binanceusdm.py` & `ccxt-4.0.8/ccxt/pro/binanceusdm.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitcoincom.py` & `ccxt-4.0.8/ccxt/pro/bitcoincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitfinex.py` & `ccxt-4.0.8/ccxt/pro/bitfinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitfinex2.py` & `ccxt-4.0.8/ccxt/pro/bitfinex2.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitget.py` & `ccxt-4.0.8/ccxt/pro/bitget.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitmart.py` & `ccxt-4.0.8/ccxt/pro/bitmart.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitmex.py` & `ccxt-4.0.8/ccxt/pro/bitmex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitopro.py` & `ccxt-4.0.8/ccxt/pro/bitopro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitpanda.py` & `ccxt-4.0.8/ccxt/pro/bitpanda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitrue.py` & `ccxt-4.0.8/ccxt/pro/bitrue.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitstamp.py` & `ccxt-4.0.8/ccxt/pro/bitstamp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bittrex.py` & `ccxt-4.0.8/ccxt/pro/bittrex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bitvavo.py` & `ccxt-4.0.8/ccxt/pro/bitvavo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/blockchaincom.py` & `ccxt-4.0.8/ccxt/pro/blockchaincom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/btcex.py` & `ccxt-4.0.8/ccxt/pro/btcex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/bybit.py` & `ccxt-4.0.8/ccxt/pro/bybit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/cex.py` & `ccxt-4.0.8/ccxt/pro/cex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/coinbaseprime.py` & `ccxt-4.0.8/ccxt/pro/coinbaseprime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/coinbasepro.py` & `ccxt-4.0.8/ccxt/pro/coinbasepro.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/coinex.py` & `ccxt-4.0.8/ccxt/pro/coinex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/cryptocom.py` & `ccxt-4.0.8/ccxt/pro/cryptocom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/currencycom.py` & `ccxt-4.0.8/ccxt/pro/currencycom.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/deribit.py` & `ccxt-4.0.8/ccxt/pro/deribit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/exmo.py` & `ccxt-4.0.8/ccxt/pro/exmo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/gate.py` & `ccxt-4.0.8/ccxt/pro/gate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/gemini.py` & `ccxt-4.0.8/ccxt/pro/gemini.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/hitbtc.py` & `ccxt-4.0.8/ccxt/pro/hitbtc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/hollaex.py` & `ccxt-4.0.8/ccxt/pro/hollaex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/huobi.py` & `ccxt-4.0.8/ccxt/pro/huobi.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/huobijp.py` & `ccxt-4.0.8/ccxt/pro/huobijp.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/idex.py` & `ccxt-4.0.8/ccxt/pro/idex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/independentreserve.py` & `ccxt-4.0.8/ccxt/pro/independentreserve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/kraken.py` & `ccxt-4.0.8/ccxt/pro/kraken.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/krakenfutures.py` & `ccxt-4.0.8/ccxt/pro/krakenfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/kucoin.py` & `ccxt-4.0.8/ccxt/pro/kucoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/kucoinfutures.py` & `ccxt-4.0.8/ccxt/pro/kucoinfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/luno.py` & `ccxt-4.0.8/ccxt/pro/luno.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/mexc.py` & `ccxt-4.0.8/ccxt/pro/mexc.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/ndax.py` & `ccxt-4.0.8/ccxt/pro/ndax.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/okcoin.py` & `ccxt-4.0.8/ccxt/pro/okcoin.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/okx.py` & `ccxt-4.0.8/ccxt/pro/okx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/phemex.py` & `ccxt-4.0.8/ccxt/pro/phemex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/poloniex.py` & `ccxt-4.0.8/ccxt/pro/poloniex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/poloniexfutures.py` & `ccxt-4.0.8/ccxt/pro/poloniexfutures.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/probit.py` & `ccxt-4.0.8/ccxt/pro/probit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/ripio.py` & `ccxt-4.0.8/ccxt/pro/ripio.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/upbit.py` & `ccxt-4.0.8/ccxt/pro/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/wazirx.py` & `ccxt-4.0.8/ccxt/pro/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/whitebit.py` & `ccxt-4.0.8/ccxt/pro/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/woo.py` & `ccxt-4.0.8/ccxt/pro/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/pro/zb.py` & `ccxt-4.0.8/ccxt/pro/zb.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/probit.py` & `ccxt-4.0.8/ccxt/probit.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                 'fetchBorrowRates': False,
                 'fetchBorrowRatesPerSymbol': False,
                 'fetchClosedOrders': True,
                 'fetchCurrencies': True,
                 'fetchDepositAddress': True,
                 'fetchDepositAddresses': True,
                 'fetchDeposits': True,
+                'fetchDepositsWithdrawals': True,
                 'fetchFundingHistory': False,
                 'fetchFundingRate': False,
                 'fetchFundingRateHistory': False,
                 'fetchFundingRates': False,
                 'fetchIndexOHLCV': False,
                 'fetchLeverage': False,
                 'fetchLeverageTiers': False,
@@ -1391,15 +1392,17 @@
             'type': 'withdrawal',
         }
         result = self.fetch_transactions(code, since, limit, self.extend(request, params))
         return result
 
     def fetch_transactions(self, code: Optional[str] = None, since: Optional[int] = None, limit: Optional[int] = None, params={}):
         """
-        fetch all transactions made to an account
+         * @deprecated
+        use fetchDepositsWithdrawals instead
+        see https://docs-en.probit.com/reference/transferpayment
         :param str code: unified currency code
         :param int [since]: the earliest time in ms to fetch transactions for
         :param int [limit]: the maximum number of transaction structures to retrieve
         :param dict [params]: extra parameters specific to the probit api endpoint
         :returns dict[]: a list of `transaction structures <https://docs.ccxt.com/#/?id=transaction-structure>`
         """
         self.load_markets()
```

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/__init__.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/_version.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/_version.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/curves.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/curves.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/der.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/der.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/ecdsa.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/ecdsa.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/ellipticcurve.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/ellipticcurve.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/keys.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/keys.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/numbertheory.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/numbertheory.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/rfc6979.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/rfc6979.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/ecdsa/util.py` & `ccxt-4.0.8/ccxt/static_dependencies/ecdsa/util.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/static_dependencies/keccak/keccak.py` & `ccxt-4.0.8/ccxt/static_dependencies/keccak/keccak.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/__init__.py` & `ccxt-4.0.8/ccxt/test/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_account.py` & `ccxt-4.0.8/ccxt/test/base/test_account.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_balance.py` & `ccxt-4.0.8/ccxt/test/base/test_balance.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_borrow_interest.py` & `ccxt-4.0.8/ccxt/test/base/test_borrow_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_borrow_rate.py` & `ccxt-4.0.8/ccxt/test/base/test_borrow_rate.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_calculate_fee.py` & `ccxt-4.0.8/ccxt/test/base/test_calculate_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_crypto.py` & `ccxt-4.0.8/ccxt/test/base/test_crypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_currency.py` & `ccxt-4.0.8/ccxt/test/base/test_currency.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_datetime.py` & `ccxt-4.0.8/ccxt/test/base/test_datetime.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_decimal_to_precision.py` & `ccxt-4.0.8/ccxt/test/base/test_decimal_to_precision.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_deep_extend.py` & `ccxt-4.0.8/ccxt/test/base/test_deep_extend.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_deposit_withdrawal.py` & `ccxt-4.0.8/ccxt/test/base/test_deposit_withdrawal.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_exchange_datetime_functions.py` & `ccxt-4.0.8/ccxt/test/base/test_exchange_datetime_functions.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_funding_rate_history.py` & `ccxt-4.0.8/ccxt/test/base/test_funding_rate_history.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_ledger_entry.py` & `ccxt-4.0.8/ccxt/test/base/test_ledger_entry.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_ledger_item.py` & `ccxt-4.0.8/ccxt/test/base/test_ledger_item.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_leverage_tier.py` & `ccxt-4.0.8/ccxt/test/base/test_leverage_tier.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_margin_modification.py` & `ccxt-4.0.8/ccxt/test/base/test_margin_modification.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_market.py` & `ccxt-4.0.8/ccxt/test/base/test_market.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_number.py` & `ccxt-4.0.8/ccxt/test/base/test_number.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_ohlcv.py` & `ccxt-4.0.8/ccxt/test/base/test_ohlcv.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_open_interest.py` & `ccxt-4.0.8/ccxt/test/base/test_open_interest.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_order.py` & `ccxt-4.0.8/ccxt/test/base/test_order.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_order_book.py` & `ccxt-4.0.8/ccxt/test/base/test_order_book.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_position.py` & `ccxt-4.0.8/ccxt/test/base/test_position.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_shared_methods.py` & `ccxt-4.0.8/ccxt/test/base/test_shared_methods.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_status.py` & `ccxt-4.0.8/ccxt/test/base/test_status.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_throttle.py` & `ccxt-4.0.8/ccxt/test/base/test_throttle.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_ticker.py` & `ccxt-4.0.8/ccxt/test/base/test_ticker.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_trade.py` & `ccxt-4.0.8/ccxt/test/base/test_trade.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_trading_fee.py` & `ccxt-4.0.8/ccxt/test/base/test_trading_fee.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/base/test_transaction.py` & `ccxt-4.0.8/ccxt/test/base/test_transaction.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/test_async.py` & `ccxt-4.0.8/ccxt/test/test_async.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/test/test_sync.py` & `ccxt-4.0.8/ccxt/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/tidex.py` & `ccxt-4.0.8/ccxt/tidex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/timex.py` & `ccxt-4.0.8/ccxt/timex.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/tokocrypto.py` & `ccxt-4.0.8/ccxt/tokocrypto.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/upbit.py` & `ccxt-4.0.8/ccxt/upbit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/wavesexchange.py` & `ccxt-4.0.8/ccxt/wavesexchange.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/wazirx.py` & `ccxt-4.0.8/ccxt/wazirx.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/whitebit.py` & `ccxt-4.0.8/ccxt/whitebit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/woo.py` & `ccxt-4.0.8/ccxt/woo.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/yobit.py` & `ccxt-4.0.8/ccxt/yobit.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/zaif.py` & `ccxt-4.0.8/ccxt/zaif.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt/zonda.py` & `ccxt-4.0.8/ccxt/zonda.py`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/ccxt.egg-info/PKG-INFO` & `ccxt-4.0.8/ccxt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccxt
-Version: 4.0.7
+Version: 4.0.8
 Summary: A JavaScript / TypeScript / Python / C# / PHP cryptocurrency trading library with support for 130+ exchanges
 Home-page: https://ccxt.com
 Author: Igor Kroitor
 Author-email: igor.kroitor@gmail.com
 License: MIT
 Project-URL: Homepage, https://ccxt.com
 Project-URL: Documentation, https://docs.ccxt.com
@@ -222,21 +222,21 @@
         console.log(version, Object.keys(exchanges));
         ```
         
         ### JavaScript (for use with the `<script>` tag):
         
         All-in-one browser bundle (dependencies included), served from a CDN of your choice:
         
-        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.0.7/dist/ccxt.browser.js
-        * unpkg: https://unpkg.com/ccxt@4.0.7/dist/ccxt.browser.js
+        * jsDelivr: https://cdn.jsdelivr.net/npm/ccxt@4.0.8/dist/ccxt.browser.js
+        * unpkg: https://unpkg.com/ccxt@4.0.8/dist/ccxt.browser.js
         
         CDNs are not updated in real-time and may have delays. Defaulting to the most recent version without specifying the version number is not recommended. Please, keep in mind that we are not responsible for the correct operation of those CDN servers.
         
         ```HTML
-        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.0.7/dist/ccxt.browser.js"></script>
+        <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/ccxt@4.0.8/dist/ccxt.browser.js"></script>
         ```
         
         Creates a global `ccxt` object:
         
         ```JavaScript
         console.log (ccxt.exchanges) // print all available exchanges
         ```
```

### Comparing `ccxt-4.0.7/ccxt.egg-info/SOURCES.txt` & `ccxt-4.0.8/ccxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccxt-4.0.7/package.json` & `ccxt-4.0.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'4.0.8'"}*

```diff
@@ -222,9 +222,9 @@
         "update-badges": "node build/update-badges",
         "update-links": "node build/update-links",
         "vss": "node build/vss"
     },
     "type": "module",
     "types": "./js/ccxt.d.ts",
     "unpkg": "dist/ccxt.browser.js",
-    "version": "4.0.7"
+    "version": "4.0.8"
 }
```

### Comparing `ccxt-4.0.7/setup.py` & `ccxt-4.0.8/setup.py`

 * *Files identical despite different names*

