# Comparing `tmp/xrpl_py-2.0.0.tar.gz` & `tmp/xrpl-py-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrpl_py-2.0.0.tar", max compression
+gzip compressed data, was "xrpl-py-2.0.0b0.tar", max compression
```

## Comparing `xrpl_py-2.0.0.tar` & `xrpl-py-2.0.0b0.tar`

### file list

```diff
@@ -1,222 +1,223 @@
--rw-r--r--   0        0        0      740 2023-03-27 21:33:33.181289 xrpl_py-2.0.0/LICENSE
--rw-r--r--   0        0        0    16001 2023-07-05 18:29:25.236508 xrpl_py-2.0.0/README.md
--rw-r--r--   0        0        0     2227 2023-07-05 18:48:32.427475 xrpl_py-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      348 2023-03-27 21:33:33.208293 xrpl_py-2.0.0/xrpl/__init__.py
--rw-r--r--   0        0        0      393 2023-07-05 18:29:25.258425 xrpl_py-2.0.0/xrpl/account/__init__.py
--rw-r--r--   0        0        0     3376 2023-07-05 18:29:25.259003 xrpl_py-2.0.0/xrpl/account/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.208607 xrpl_py-2.0.0/xrpl/account/py.typed
--rw-r--r--   0        0        0      776 2023-07-05 18:29:25.259418 xrpl_py-2.0.0/xrpl/account/transaction_history.py
--rw-r--r--   0        0        0      189 2023-03-27 21:33:33.208996 xrpl_py-2.0.0/xrpl/asyncio/__init__.py
--rw-r--r--   0        0        0      415 2023-07-05 18:29:25.259832 xrpl_py-2.0.0/xrpl/asyncio/account/__init__.py
--rw-r--r--   0        0        0     4245 2023-07-05 18:29:25.260231 xrpl_py-2.0.0/xrpl/asyncio/account/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.209363 xrpl_py-2.0.0/xrpl/asyncio/account/py.typed
--rw-r--r--   0        0        0     1170 2023-07-05 18:29:25.260699 xrpl_py-2.0.0/xrpl/asyncio/account/transaction_history.py
--rw-r--r--   0        0        0      705 2023-03-27 21:33:33.209657 xrpl_py-2.0.0/xrpl/asyncio/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-03-27 21:33:33.209787 xrpl_py-2.0.0/xrpl/asyncio/clients/async_client.py
--rw-r--r--   0        0        0      315 2023-03-27 21:33:33.209890 xrpl_py-2.0.0/xrpl/asyncio/clients/async_json_rpc_client.py
--rw-r--r--   0        0        0     7149 2023-05-24 00:47:49.625976 xrpl_py-2.0.0/xrpl/asyncio/clients/async_websocket_client.py
--rw-r--r--   0        0        0     1189 2023-06-28 21:24:17.291182 xrpl_py-2.0.0/xrpl/asyncio/clients/client.py
--rw-r--r--   0        0        0     1083 2023-03-27 21:33:33.210270 xrpl_py-2.0.0/xrpl/asyncio/clients/exceptions.py
--rw-r--r--   0        0        0     1612 2023-03-27 21:33:33.210375 xrpl_py-2.0.0/xrpl/asyncio/clients/json_rpc_base.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.210427 xrpl_py-2.0.0/xrpl/asyncio/clients/py.typed
--rw-r--r--   0        0        0     3341 2023-03-27 21:33:33.210572 xrpl_py-2.0.0/xrpl/asyncio/clients/utils.py
--rw-r--r--   0        0        0     8173 2023-05-24 00:47:49.626225 xrpl_py-2.0.0/xrpl/asyncio/clients/websocket_base.py
--rw-r--r--   0        0        0      328 2023-03-27 21:33:33.210867 xrpl_py-2.0.0/xrpl/asyncio/ledger/__init__.py
--rw-r--r--   0        0        0     3443 2023-03-27 21:33:33.210988 xrpl_py-2.0.0/xrpl/asyncio/ledger/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211039 xrpl_py-2.0.0/xrpl/asyncio/ledger/py.typed
--rw-r--r--   0        0        0     2353 2023-03-27 21:33:33.211142 xrpl_py-2.0.0/xrpl/asyncio/ledger/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211201 xrpl_py-2.0.0/xrpl/asyncio/py.typed
--rw-r--r--   0        0        0      569 2023-07-05 18:29:25.261267 xrpl_py-2.0.0/xrpl/asyncio/transaction/__init__.py
--rw-r--r--   0        0        0    17821 2023-07-05 18:29:25.261786 xrpl_py-2.0.0/xrpl/asyncio/transaction/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211640 xrpl_py-2.0.0/xrpl/asyncio/transaction/py.typed
--rw-r--r--   0        0        0     8210 2023-07-05 18:29:25.262451 xrpl_py-2.0.0/xrpl/asyncio/transaction/reliable_submission.py
--rw-r--r--   0        0        0      219 2023-03-27 21:33:33.211934 xrpl_py-2.0.0/xrpl/asyncio/wallet/__init__.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.211983 xrpl_py-2.0.0/xrpl/asyncio/wallet/py.typed
--rw-r--r--   0        0        0     6614 2023-07-05 18:29:25.262915 xrpl_py-2.0.0/xrpl/asyncio/wallet/wallet_generation.py
--rw-r--r--   0        0        0      656 2023-03-27 21:33:33.212260 xrpl_py-2.0.0/xrpl/clients/__init__.py
--rw-r--r--   0        0        0      295 2023-03-27 21:33:33.212375 xrpl_py-2.0.0/xrpl/clients/json_rpc_client.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.212453 xrpl_py-2.0.0/xrpl/clients/py.typed
--rw-r--r--   0        0        0      705 2023-03-27 21:33:33.212612 xrpl_py-2.0.0/xrpl/clients/sync_client.py
--rw-r--r--   0        0        0     8893 2023-05-24 00:47:49.627983 xrpl_py-2.0.0/xrpl/clients/websocket_client.py
--rw-r--r--   0        0        0     1414 2023-03-27 21:33:33.212831 xrpl_py-2.0.0/xrpl/constants.py
--rw-r--r--   0        0        0      171 2023-03-27 21:33:33.213024 xrpl_py-2.0.0/xrpl/core/__init__.py
--rw-r--r--   0        0        0     1131 2023-07-05 18:29:25.263144 xrpl_py-2.0.0/xrpl/core/addresscodec/__init__.py
--rw-r--r--   0        0        0     7175 2023-03-27 21:33:33.213364 xrpl_py-2.0.0/xrpl/core/addresscodec/codec.py
--rw-r--r--   0        0        0      194 2023-03-27 21:33:33.213467 xrpl_py-2.0.0/xrpl/core/addresscodec/exceptions.py
--rw-r--r--   0        0        0     5735 2023-07-05 18:29:25.263420 xrpl_py-2.0.0/xrpl/core/addresscodec/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.213616 xrpl_py-2.0.0/xrpl/core/addresscodec/py.typed
--rw-r--r--   0        0        0      235 2023-03-27 21:33:33.213716 xrpl_py-2.0.0/xrpl/core/addresscodec/utils.py
--rw-r--r--   0        0        0      488 2023-03-27 21:33:33.213863 xrpl_py-2.0.0/xrpl/core/binarycodec/__init__.py
--rw-r--r--   0        0        0      296 2023-03-27 21:33:33.214024 xrpl_py-2.0.0/xrpl/core/binarycodec/binary_wrappers/__init__.py
--rw-r--r--   0        0        0     9076 2023-03-27 21:33:33.214177 xrpl_py-2.0.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
--rw-r--r--   0        0        0     4650 2023-03-27 21:33:33.214314 xrpl_py-2.0.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
--rw-r--r--   0        0        0     1025 2023-03-27 21:33:33.214520 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/__init__.py
--rw-r--r--   0        0        0    45270 2023-06-28 21:24:17.294480 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/definitions.json
--rw-r--r--   0        0        0     8431 2023-03-27 21:33:33.214831 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/definitions.py
--rw-r--r--   0        0        0     1870 2023-06-13 17:18:50.605201 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_header.py
--rw-r--r--   0        0        0     1192 2023-03-27 21:33:33.215066 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_info.py
--rw-r--r--   0        0        0     1931 2023-03-27 21:33:33.215188 xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_instance.py
--rw-r--r--   0        0        0      191 2023-03-27 21:33:33.215272 xrpl_py-2.0.0/xrpl/core/binarycodec/exceptions.py
--rw-r--r--   0        0        0     3942 2023-03-27 21:33:33.215363 xrpl_py-2.0.0/xrpl/core/binarycodec/field_id_codec.py
--rw-r--r--   0        0        0     3708 2023-06-13 17:18:50.605488 xrpl_py-2.0.0/xrpl/core/binarycodec/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.215490 xrpl_py-2.0.0/xrpl/core/binarycodec/py.typed
--rw-r--r--   0        0        0     1255 2023-06-13 17:18:50.605779 xrpl_py-2.0.0/xrpl/core/binarycodec/types/__init__.py
--rw-r--r--   0        0        0     2956 2023-03-27 21:33:33.215738 xrpl_py-2.0.0/xrpl/core/binarycodec/types/account_id.py
--rw-r--r--   0        0        0    11513 2023-05-24 00:47:49.628328 xrpl_py-2.0.0/xrpl/core/binarycodec/types/amount.py
--rw-r--r--   0        0        0     1950 2023-03-27 21:33:33.215995 xrpl_py-2.0.0/xrpl/core/binarycodec/types/blob.py
--rw-r--r--   0        0        0     4347 2023-03-27 21:33:33.216127 xrpl_py-2.0.0/xrpl/core/binarycodec/types/currency.py
--rw-r--r--   0        0        0     2640 2023-03-27 21:33:33.216255 xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash.py
--rw-r--r--   0        0        0     1494 2023-05-24 00:47:49.628558 xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash128.py
--rw-r--r--   0        0        0      571 2023-03-27 21:33:33.216531 xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash160.py
--rw-r--r--   0        0        0      572 2023-03-27 21:33:33.216629 xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash256.py
--rw-r--r--   0        0        0     9067 2023-03-27 21:33:33.216726 xrpl_py-2.0.0/xrpl/core/binarycodec/types/path_set.py
--rw-r--r--   0        0        0     2493 2023-03-27 21:33:33.216814 xrpl_py-2.0.0/xrpl/core/binarycodec/types/serialized_type.py
--rw-r--r--   0        0        0     3301 2023-03-27 21:33:33.216902 xrpl_py-2.0.0/xrpl/core/binarycodec/types/st_array.py
--rw-r--r--   0        0        0     8392 2023-05-24 00:47:49.628841 xrpl_py-2.0.0/xrpl/core/binarycodec/types/st_object.py
--rw-r--r--   0        0        0     3383 2023-03-27 21:33:33.217092 xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint.py
--rw-r--r--   0        0        0     2063 2023-03-27 21:33:33.217191 xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint16.py
--rw-r--r--   0        0        0     2283 2023-03-27 21:33:33.217268 xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint32.py
--rw-r--r--   0        0        0     2854 2023-03-27 21:33:33.217357 xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint64.py
--rw-r--r--   0        0        0     1994 2023-03-27 21:33:33.217433 xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint8.py
--rw-r--r--   0        0        0     2905 2023-03-27 21:33:33.217534 xrpl_py-2.0.0/xrpl/core/binarycodec/types/vector256.py
--rw-r--r--   0        0        0      447 2023-03-27 21:33:33.217683 xrpl_py-2.0.0/xrpl/core/keypairs/__init__.py
--rw-r--r--   0        0        0     1275 2023-03-27 21:33:33.217784 xrpl_py-2.0.0/xrpl/core/keypairs/crypto_implementation.py
--rw-r--r--   0        0        0     3662 2023-07-05 18:29:25.263845 xrpl_py-2.0.0/xrpl/core/keypairs/ed25519.py
--rw-r--r--   0        0        0      182 2023-03-27 21:33:33.218030 xrpl_py-2.0.0/xrpl/core/keypairs/exceptions.py
--rw-r--r--   0        0        0      893 2023-03-27 21:33:33.218146 xrpl_py-2.0.0/xrpl/core/keypairs/helpers.py
--rw-r--r--   0        0        0     4881 2023-07-05 18:29:25.264355 xrpl_py-2.0.0/xrpl/core/keypairs/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218330 xrpl_py-2.0.0/xrpl/core/keypairs/py.typed
--rw-r--r--   0        0        0     7480 2023-03-27 21:33:33.218476 xrpl_py-2.0.0/xrpl/core/keypairs/secp256k1.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218546 xrpl_py-2.0.0/xrpl/core/py.typed
--rw-r--r--   0        0        0      314 2023-03-27 21:33:33.218727 xrpl_py-2.0.0/xrpl/ledger/__init__.py
--rw-r--r--   0        0        0     2283 2023-03-27 21:33:33.218825 xrpl_py-2.0.0/xrpl/ledger/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.218878 xrpl_py-2.0.0/xrpl/ledger/py.typed
--rw-r--r--   0        0        0      858 2023-06-13 17:18:50.606769 xrpl_py-2.0.0/xrpl/models/__init__.py
--rw-r--r--   0        0        0      497 2023-03-27 21:33:33.219179 xrpl_py-2.0.0/xrpl/models/amounts/__init__.py
--rw-r--r--   0        0        0     1377 2023-03-27 21:33:33.219264 xrpl_py-2.0.0/xrpl/models/amounts/amount.py
--rw-r--r--   0        0        0     1349 2023-03-27 21:33:33.219368 xrpl_py-2.0.0/xrpl/models/amounts/issued_currency_amount.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.219418 xrpl_py-2.0.0/xrpl/models/amounts/py.typed
--rw-r--r--   0        0        0    10682 2023-06-13 17:18:50.607347 xrpl_py-2.0.0/xrpl/models/base_model.py
--rw-r--r--   0        0        0      371 2023-03-27 21:33:33.219720 xrpl_py-2.0.0/xrpl/models/currencies/__init__.py
--rw-r--r--   0        0        0      319 2023-06-20 18:04:32.828627 xrpl_py-2.0.0/xrpl/models/currencies/currency.py
--rw-r--r--   0        0        0     2237 2023-03-27 21:33:33.219871 xrpl_py-2.0.0/xrpl/models/currencies/issued_currency.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.219913 xrpl_py-2.0.0/xrpl/models/currencies/py.typed
--rw-r--r--   0        0        0     2716 2023-07-05 18:29:25.264811 xrpl_py-2.0.0/xrpl/models/currencies/xrp.py
--rw-r--r--   0        0        0      171 2023-03-27 21:33:33.220096 xrpl_py-2.0.0/xrpl/models/exceptions.py
--rw-r--r--   0        0        0     4126 2023-07-05 18:29:25.265065 xrpl_py-2.0.0/xrpl/models/flags.py
--rw-r--r--   0        0        0     2462 2023-03-27 21:33:33.220298 xrpl_py-2.0.0/xrpl/models/nested_model.py
--rw-r--r--   0        0        0     2088 2023-03-27 21:33:33.220387 xrpl_py-2.0.0/xrpl/models/path.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.220444 xrpl_py-2.0.0/xrpl/models/py.typed
--rw-r--r--   0        0        0     3607 2023-06-13 17:18:50.607886 xrpl_py-2.0.0/xrpl/models/requests/__init__.py
--rw-r--r--   0        0        0     1549 2023-06-28 21:24:17.296026 xrpl_py-2.0.0/xrpl/models/requests/account_channels.py
--rw-r--r--   0        0        0     1134 2023-06-28 21:24:17.296337 xrpl_py-2.0.0/xrpl/models/requests/account_currencies.py
--rw-r--r--   0        0        0     1088 2023-06-28 21:24:17.296558 xrpl_py-2.0.0/xrpl/models/requests/account_info.py
--rw-r--r--   0        0        0     1323 2023-06-28 21:24:17.296815 xrpl_py-2.0.0/xrpl/models/requests/account_lines.py
--rw-r--r--   0        0        0     1216 2023-06-28 21:24:17.297206 xrpl_py-2.0.0/xrpl/models/requests/account_nfts.py
--rw-r--r--   0        0        0     1738 2023-06-28 21:24:17.297455 xrpl_py-2.0.0/xrpl/models/requests/account_objects.py
--rw-r--r--   0        0        0     1161 2023-06-28 21:24:17.297683 xrpl_py-2.0.0/xrpl/models/requests/account_offers.py
--rw-r--r--   0        0        0     1207 2023-06-28 21:24:17.297912 xrpl_py-2.0.0/xrpl/models/requests/account_tx.py
--rw-r--r--   0        0        0     1024 2023-06-28 21:24:17.298185 xrpl_py-2.0.0/xrpl/models/requests/book_offers.py
--rw-r--r--   0        0        0     3020 2023-06-13 17:18:50.608358 xrpl_py-2.0.0/xrpl/models/requests/channel_authorize.py
--rw-r--r--   0        0        0     1130 2023-06-13 17:18:50.608584 xrpl_py-2.0.0/xrpl/models/requests/channel_verify.py
--rw-r--r--   0        0        0     1145 2023-06-28 21:24:17.298415 xrpl_py-2.0.0/xrpl/models/requests/deposit_authorized.py
--rw-r--r--   0        0        0      775 2023-03-27 21:33:33.222125 xrpl_py-2.0.0/xrpl/models/requests/fee.py
--rw-r--r--   0        0        0     1076 2023-06-28 21:24:17.298642 xrpl_py-2.0.0/xrpl/models/requests/gateway_balances.py
--rw-r--r--   0        0        0     3068 2023-03-27 21:33:33.222393 xrpl_py-2.0.0/xrpl/models/requests/generic_request.py
--rw-r--r--   0        0        0      887 2023-06-28 21:24:17.298934 xrpl_py-2.0.0/xrpl/models/requests/ledger.py
--rw-r--r--   0        0        0      944 2023-03-27 21:33:33.222656 xrpl_py-2.0.0/xrpl/models/requests/ledger_closed.py
--rw-r--r--   0        0        0      726 2023-03-27 21:33:33.222760 xrpl_py-2.0.0/xrpl/models/requests/ledger_current.py
--rw-r--r--   0        0        0     1190 2023-06-28 21:24:17.299176 xrpl_py-2.0.0/xrpl/models/requests/ledger_data.py
--rw-r--r--   0        0        0     5171 2023-06-28 21:24:17.299427 xrpl_py-2.0.0/xrpl/models/requests/ledger_entry.py
--rw-r--r--   0        0        0      853 2023-03-27 21:33:33.223038 xrpl_py-2.0.0/xrpl/models/requests/manifest.py
--rw-r--r--   0        0        0      809 2023-06-28 21:24:17.299678 xrpl_py-2.0.0/xrpl/models/requests/nft_buy_offers.py
--rw-r--r--   0        0        0     1184 2023-06-28 21:24:17.299933 xrpl_py-2.0.0/xrpl/models/requests/nft_history.py
--rw-r--r--   0        0        0      772 2023-06-28 21:24:17.300172 xrpl_py-2.0.0/xrpl/models/requests/nft_info.py
--rw-r--r--   0        0        0      816 2023-06-28 21:24:17.300459 xrpl_py-2.0.0/xrpl/models/requests/nft_sell_offers.py
--rw-r--r--   0        0        0     1446 2023-06-28 21:24:17.300713 xrpl_py-2.0.0/xrpl/models/requests/no_ripple_check.py
--rw-r--r--   0        0        0     4347 2023-03-27 21:33:33.223485 xrpl_py-2.0.0/xrpl/models/requests/path_find.py
--rw-r--r--   0        0        0      547 2023-03-27 21:33:33.223601 xrpl_py-2.0.0/xrpl/models/requests/ping.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.223670 xrpl_py-2.0.0/xrpl/models/requests/py.typed
--rw-r--r--   0        0        0      579 2023-03-27 21:33:33.223830 xrpl_py-2.0.0/xrpl/models/requests/random.py
--rw-r--r--   0        0        0     6234 2023-06-28 21:24:17.300971 xrpl_py-2.0.0/xrpl/models/requests/request.py
--rw-r--r--   0        0        0     2280 2023-06-28 21:24:17.301222 xrpl_py-2.0.0/xrpl/models/requests/ripple_path_find.py
--rw-r--r--   0        0        0      618 2023-03-27 21:33:33.224173 xrpl_py-2.0.0/xrpl/models/requests/server_info.py
--rw-r--r--   0        0        0     1194 2023-03-27 21:33:33.224272 xrpl_py-2.0.0/xrpl/models/requests/server_state.py
--rw-r--r--   0        0        0     4034 2023-03-27 21:33:33.224362 xrpl_py-2.0.0/xrpl/models/requests/sign.py
--rw-r--r--   0        0        0     5062 2023-03-27 21:33:33.224471 xrpl_py-2.0.0/xrpl/models/requests/sign_and_submit.py
--rw-r--r--   0        0        0     3274 2023-03-27 21:33:33.224567 xrpl_py-2.0.0/xrpl/models/requests/sign_for.py
--rw-r--r--   0        0        0     3758 2023-03-27 21:33:33.224651 xrpl_py-2.0.0/xrpl/models/requests/submit.py
--rw-r--r--   0        0        0     2478 2023-03-27 21:33:33.224732 xrpl_py-2.0.0/xrpl/models/requests/submit_multisigned.py
--rw-r--r--   0        0        0     2842 2023-03-27 21:33:33.224803 xrpl_py-2.0.0/xrpl/models/requests/submit_only.py
--rw-r--r--   0        0        0     2103 2023-03-27 21:33:33.224904 xrpl_py-2.0.0/xrpl/models/requests/subscribe.py
--rw-r--r--   0        0        0     1200 2023-06-28 21:24:17.301450 xrpl_py-2.0.0/xrpl/models/requests/transaction_entry.py
--rw-r--r--   0        0        0      817 2023-03-27 21:33:33.225166 xrpl_py-2.0.0/xrpl/models/requests/tx.py
--rw-r--r--   0        0        0     1595 2023-03-27 21:33:33.225289 xrpl_py-2.0.0/xrpl/models/requests/unsubscribe.py
--rw-r--r--   0        0        0      251 2023-03-27 21:33:33.225598 xrpl_py-2.0.0/xrpl/models/required.py
--rw-r--r--   0        0        0     3617 2023-03-27 21:33:33.225707 xrpl_py-2.0.0/xrpl/models/response.py
--rw-r--r--   0        0        0     3341 2023-07-05 18:29:25.265333 xrpl_py-2.0.0/xrpl/models/transactions/__init__.py
--rw-r--r--   0        0        0     1333 2023-03-27 21:33:33.225958 xrpl_py-2.0.0/xrpl/models/transactions/account_delete.py
--rw-r--r--   0        0        0     9705 2023-07-05 18:29:25.265597 xrpl_py-2.0.0/xrpl/models/transactions/account_set.py
--rw-r--r--   0        0        0     1101 2023-03-27 21:33:33.226157 xrpl_py-2.0.0/xrpl/models/transactions/check_cancel.py
--rw-r--r--   0        0        0     1993 2023-03-27 21:33:33.226245 xrpl_py-2.0.0/xrpl/models/transactions/check_cash.py
--rw-r--r--   0        0        0     1934 2023-03-27 21:33:33.226387 xrpl_py-2.0.0/xrpl/models/transactions/check_create.py
--rw-r--r--   0        0        0     1598 2023-03-27 21:33:33.226509 xrpl_py-2.0.0/xrpl/models/transactions/deposit_preauth.py
--rw-r--r--   0        0        0     1069 2023-06-13 17:18:50.609915 xrpl_py-2.0.0/xrpl/models/transactions/escrow_cancel.py
--rw-r--r--   0        0        0     2617 2023-06-13 17:18:50.610202 xrpl_py-2.0.0/xrpl/models/transactions/escrow_create.py
--rw-r--r--   0        0        0     2114 2023-03-27 21:33:33.226807 xrpl_py-2.0.0/xrpl/models/transactions/escrow_finish.py
--rw-r--r--   0        0        0     3163 2023-05-24 00:47:49.631283 xrpl_py-2.0.0/xrpl/models/transactions/metadata.py
--rw-r--r--   0        0        0     4537 2023-03-27 21:33:33.226988 xrpl_py-2.0.0/xrpl/models/transactions/nftoken_accept_offer.py
--rw-r--r--   0        0        0     1769 2023-03-27 21:33:33.227079 xrpl_py-2.0.0/xrpl/models/transactions/nftoken_burn.py
--rw-r--r--   0        0        0     2015 2023-03-27 21:33:33.227174 xrpl_py-2.0.0/xrpl/models/transactions/nftoken_cancel_offer.py
--rw-r--r--   0        0        0     4324 2023-03-27 21:33:33.227282 xrpl_py-2.0.0/xrpl/models/transactions/nftoken_create_offer.py
--rw-r--r--   0        0        0     4762 2023-03-27 21:33:33.227403 xrpl_py-2.0.0/xrpl/models/transactions/nftoken_mint.py
--rw-r--r--   0        0        0     1045 2023-03-27 21:33:33.227515 xrpl_py-2.0.0/xrpl/models/transactions/offer_cancel.py
--rw-r--r--   0        0        0     3866 2023-03-27 21:33:33.227812 xrpl_py-2.0.0/xrpl/models/transactions/offer_create.py
--rw-r--r--   0        0        0     5861 2023-03-27 21:33:33.227972 xrpl_py-2.0.0/xrpl/models/transactions/payment.py
--rw-r--r--   0        0        0     3917 2023-06-13 17:18:50.610472 xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_claim.py
--rw-r--r--   0        0        0     2367 2023-06-13 17:18:50.610721 xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_create.py
--rw-r--r--   0        0        0     1614 2023-06-13 17:18:50.610980 xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_fund.py
--rw-r--r--   0        0        0      575 2023-03-27 21:33:33.228483 xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/__init__.py
--rw-r--r--   0        0        0     3651 2023-03-27 21:33:33.228597 xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
--rw-r--r--   0        0        0     1366 2023-03-27 21:33:33.228692 xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
--rw-r--r--   0        0        0     1874 2023-03-27 21:33:33.228789 xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/set_fee.py
--rw-r--r--   0        0        0     2262 2023-03-27 21:33:33.228920 xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.228990 xrpl_py-2.0.0/xrpl/models/transactions/py.typed
--rw-r--r--   0        0        0      959 2023-03-27 21:33:33.229144 xrpl_py-2.0.0/xrpl/models/transactions/set_regular_key.py
--rw-r--r--   0        0        0     5113 2023-06-01 20:44:07.712202 xrpl_py-2.0.0/xrpl/models/transactions/signer_list_set.py
--rw-r--r--   0        0        0      959 2023-03-27 21:33:33.229383 xrpl_py-2.0.0/xrpl/models/transactions/ticket_create.py
--rw-r--r--   0        0        0    15851 2023-06-28 21:24:17.302588 xrpl_py-2.0.0/xrpl/models/transactions/transaction.py
--rw-r--r--   0        0        0     2425 2023-03-27 21:33:33.229646 xrpl_py-2.0.0/xrpl/models/transactions/trust_set.py
--rw-r--r--   0        0        0      275 2023-03-27 21:33:33.229800 xrpl_py-2.0.0/xrpl/models/transactions/types/__init__.py
--rw-r--r--   0        0        0      287 2023-03-27 21:33:33.229903 xrpl_py-2.0.0/xrpl/models/transactions/types/pseudo_transaction_type.py
--rw-r--r--   0        0        0     1069 2023-06-13 17:18:50.611538 xrpl_py-2.0.0/xrpl/models/transactions/types/transaction_type.py
--rw-r--r--   0        0        0      749 2023-03-27 21:33:33.230152 xrpl_py-2.0.0/xrpl/models/types.py
--rw-r--r--   0        0        0     2196 2023-05-24 00:47:49.631890 xrpl_py-2.0.0/xrpl/models/utils.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.230311 xrpl_py-2.0.0/xrpl/py.typed
--rw-r--r--   0        0        0      645 2023-07-05 18:29:25.266122 xrpl_py-2.0.0/xrpl/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2023-07-05 18:29:25.266841 xrpl_py-2.0.0/xrpl/transaction/main.py
--rw-r--r--   0        0        0     1216 2023-06-28 21:24:17.303445 xrpl_py-2.0.0/xrpl/transaction/multisign.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.230897 xrpl_py-2.0.0/xrpl/transaction/py.typed
--rw-r--r--   0        0        0     2092 2023-07-05 18:29:25.267498 xrpl_py-2.0.0/xrpl/transaction/reliable_submission.py
--rw-r--r--   0        0        0      839 2023-05-24 00:47:49.633295 xrpl_py-2.0.0/xrpl/utils/__init__.py
--rw-r--r--   0        0        0     4220 2023-05-24 00:47:49.633438 xrpl_py-2.0.0/xrpl/utils/get_nftoken_id.py
--rw-r--r--   0        0        0     3412 2023-03-27 21:33:33.231476 xrpl_py-2.0.0/xrpl/utils/parse_nftoken_id.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.231524 xrpl_py-2.0.0/xrpl/utils/py.typed
--rw-r--r--   0        0        0      788 2023-03-27 21:33:33.231728 xrpl_py-2.0.0/xrpl/utils/str_conversions.py
--rw-r--r--   0        0        0     4202 2023-03-27 21:33:33.231821 xrpl_py-2.0.0/xrpl/utils/time_conversions.py
--rw-r--r--   0        0        0      350 2023-03-27 21:33:33.231975 xrpl_py-2.0.0/xrpl/utils/txn_parser/__init__.py
--rw-r--r--   0        0        0     1717 2023-03-27 21:33:33.232058 xrpl_py-2.0.0/xrpl/utils/txn_parser/get_balance_changes.py
--rw-r--r--   0        0        0     1446 2023-03-27 21:33:33.232179 xrpl_py-2.0.0/xrpl/utils/txn_parser/get_final_balances.py
--rw-r--r--   0        0        0      641 2023-06-20 18:02:15.682794 xrpl_py-2.0.0/xrpl/utils/txn_parser/get_order_book_changes.py
--rw-r--r--   0        0        0      627 2023-03-27 21:33:33.232493 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/__init__.py
--rw-r--r--   0        0        0     5218 2023-03-27 21:33:33.232602 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/balance_parser.py
--rw-r--r--   0        0        0     2518 2023-03-27 21:33:33.232692 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/nodes.py
--rw-r--r--   0        0        0     6191 2023-03-27 21:33:33.232824 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/order_book_parser.py
--rw-r--r--   0        0        0     1192 2023-06-23 20:25:14.082758 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/parser.py
--rw-r--r--   0        0        0     1404 2023-03-27 21:33:33.233075 xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/types.py
--rw-r--r--   0        0        0     3476 2023-06-23 20:12:58.674281 xrpl_py-2.0.0/xrpl/utils/xrp_conversions.py
--rw-r--r--   0        0        0      269 2023-03-27 21:33:33.233321 xrpl_py-2.0.0/xrpl/wallet/__init__.py
--rw-r--r--   0        0        0     9207 2023-07-05 18:29:25.268300 xrpl_py-2.0.0/xrpl/wallet/main.py
--rw-r--r--   0        0        0        0 2023-03-27 21:33:33.233455 xrpl_py-2.0.0/xrpl/wallet/py.typed
--rw-r--r--   0        0        0     1639 2023-06-28 21:24:17.304334 xrpl_py-2.0.0/xrpl/wallet/wallet_generation.py
--rw-r--r--   0        0        0    17289 1970-01-01 00:00:00.000000 xrpl_py-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      740 2021-07-28 20:35:08.759607 xrpl-py-2.0.0b0/LICENSE
+-rw-r--r--   0        0        0    15971 2022-12-15 20:10:31.004701 xrpl-py-2.0.0b0/README.md
+-rw-r--r--   0        0        0     2234 2022-12-15 20:19:30.899020 xrpl-py-2.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0      348 2021-07-28 20:35:08.796326 xrpl-py-2.0.0b0/xrpl/__init__.py
+-rw-r--r--   0        0        0      588 2022-09-15 21:17:14.712442 xrpl-py-2.0.0b0/xrpl/account/__init__.py
+-rw-r--r--   0        0        0     4410 2022-12-15 20:10:31.050399 xrpl-py-2.0.0b0/xrpl/account/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923644 xrpl-py-2.0.0b0/xrpl/account/py.typed
+-rw-r--r--   0        0        0     2692 2022-12-15 20:10:31.051202 xrpl-py-2.0.0b0/xrpl/account/transaction_history.py
+-rw-r--r--   0        0        0      189 2021-07-28 20:35:08.798278 xrpl-py-2.0.0b0/xrpl/asyncio/__init__.py
+-rw-r--r--   0        0        0      610 2021-07-28 20:35:08.798757 xrpl-py-2.0.0b0/xrpl/asyncio/account/__init__.py
+-rw-r--r--   0        0        0     5885 2022-12-15 20:10:31.052617 xrpl-py-2.0.0b0/xrpl/asyncio/account/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923758 xrpl-py-2.0.0b0/xrpl/asyncio/account/py.typed
+-rw-r--r--   0        0        0     3432 2022-12-15 20:10:31.053536 xrpl-py-2.0.0b0/xrpl/asyncio/account/transaction_history.py
+-rw-r--r--   0        0        0      705 2022-04-05 18:02:24.758557 xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py
+-rw-r--r--   0        0        0      692 2022-12-15 20:10:31.054509 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py
+-rw-r--r--   0        0        0      315 2021-07-28 20:35:08.800248 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_json_rpc_client.py
+-rw-r--r--   0        0        0     7099 2022-12-15 20:10:31.055584 xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py
+-rw-r--r--   0        0        0     1066 2022-12-15 20:10:31.056911 xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py
+-rw-r--r--   0        0        0     1083 2021-07-28 20:35:08.801049 xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py
+-rw-r--r--   0        0        0     1612 2022-12-15 20:10:31.057676 xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923862 xrpl-py-2.0.0b0/xrpl/asyncio/clients/py.typed
+-rw-r--r--   0        0        0     3341 2021-12-07 22:32:02.034730 xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py
+-rw-r--r--   0        0        0     7431 2022-12-15 20:10:31.058266 xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py
+-rw-r--r--   0        0        0      328 2021-07-28 20:35:08.802964 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/__init__.py
+-rw-r--r--   0        0        0     3443 2022-12-15 20:10:31.059029 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.923951 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/py.typed
+-rw-r--r--   0        0        0     2353 2022-04-26 22:13:55.274282 xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924038 xrpl-py-2.0.0b0/xrpl/asyncio/py.typed
+-rw-r--r--   0        0        0      956 2022-12-15 20:10:31.059741 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py
+-rw-r--r--   0        0        0     2077 2022-12-15 20:10:31.060567 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/ledger.py
+-rw-r--r--   0        0        0    12247 2022-12-15 20:10:31.061290 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924123 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/py.typed
+-rw-r--r--   0        0        0     3606 2022-12-15 20:10:31.062028 xrpl-py-2.0.0b0/xrpl/asyncio/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      219 2021-07-28 20:35:08.805165 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924197 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/py.typed
+-rw-r--r--   0        0        0     5657 2022-12-15 20:10:31.062888 xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py
+-rw-r--r--   0        0        0      656 2021-07-28 20:35:08.805912 xrpl-py-2.0.0b0/xrpl/clients/__init__.py
+-rw-r--r--   0        0        0      295 2021-07-28 20:35:08.806161 xrpl-py-2.0.0b0/xrpl/clients/json_rpc_client.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924276 xrpl-py-2.0.0b0/xrpl/clients/py.typed
+-rw-r--r--   0        0        0      705 2022-12-15 20:10:31.064928 xrpl-py-2.0.0b0/xrpl/clients/sync_client.py
+-rw-r--r--   0        0        0     8780 2022-12-15 20:10:31.065768 xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py
+-rw-r--r--   0        0        0     1414 2022-07-28 00:01:58.132202 xrpl-py-2.0.0b0/xrpl/constants.py
+-rw-r--r--   0        0        0      171 2021-07-28 20:35:08.807482 xrpl-py-2.0.0b0/xrpl/core/__init__.py
+-rw-r--r--   0        0        0     1131 2022-12-15 20:10:31.067161 xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py
+-rw-r--r--   0        0        0     7175 2022-08-23 17:19:34.990879 xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py
+-rw-r--r--   0        0        0      194 2021-07-28 20:35:08.808480 xrpl-py-2.0.0b0/xrpl/core/addresscodec/exceptions.py
+-rw-r--r--   0        0        0     5735 2022-12-15 20:10:31.067991 xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924387 xrpl-py-2.0.0b0/xrpl/core/addresscodec/py.typed
+-rw-r--r--   0        0        0      235 2021-07-28 20:35:08.808987 xrpl-py-2.0.0b0/xrpl/core/addresscodec/utils.py
+-rw-r--r--   0        0        0      488 2021-07-28 20:35:08.809400 xrpl-py-2.0.0b0/xrpl/core/binarycodec/__init__.py
+-rw-r--r--   0        0        0      296 2021-07-28 20:35:08.809791 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/__init__.py
+-rw-r--r--   0        0        0     9076 2021-07-28 20:35:08.810078 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py
+-rw-r--r--   0        0        0     4650 2021-12-07 22:32:02.051210 xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py
+-rw-r--r--   0        0        0     1025 2021-07-28 20:35:08.810736 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py
+-rw-r--r--   0        0        0    44971 2022-08-23 17:19:34.991511 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json
+-rw-r--r--   0        0        0     8431 2021-07-28 20:35:08.811725 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py
+-rw-r--r--   0        0        0     1870 2021-07-28 20:35:08.812068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py
+-rw-r--r--   0        0        0     1192 2021-07-28 20:35:08.812380 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py
+-rw-r--r--   0        0        0     1931 2022-07-05 22:56:20.051355 xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py
+-rw-r--r--   0        0        0      191 2021-07-28 20:35:08.813180 xrpl-py-2.0.0b0/xrpl/core/binarycodec/exceptions.py
+-rw-r--r--   0        0        0     3942 2021-07-28 20:35:08.813524 xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py
+-rw-r--r--   0        0        0     3708 2022-07-05 22:56:20.052317 xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924565 xrpl-py-2.0.0b0/xrpl/core/binarycodec/py.typed
+-rw-r--r--   0        0        0     1255 2022-07-05 22:56:20.053538 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/__init__.py
+-rw-r--r--   0        0        0     2956 2022-01-20 00:05:30.497701 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py
+-rw-r--r--   0        0        0    11234 2021-12-17 23:17:45.558659 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py
+-rw-r--r--   0        0        0     1950 2021-07-28 20:35:08.815354 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py
+-rw-r--r--   0        0        0     4347 2021-12-07 22:32:02.058589 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py
+-rw-r--r--   0        0        0     2640 2021-12-07 22:32:02.059722 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py
+-rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816233 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash128.py
+-rw-r--r--   0        0        0      571 2021-07-28 20:35:08.816481 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py
+-rw-r--r--   0        0        0      572 2021-07-28 20:35:08.816714 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash256.py
+-rw-r--r--   0        0        0     9067 2021-07-28 20:35:08.817068 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py
+-rw-r--r--   0        0        0     2493 2022-07-05 22:56:20.055452 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py
+-rw-r--r--   0        0        0     3301 2022-07-05 22:56:20.055743 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py
+-rw-r--r--   0        0        0     8394 2022-07-05 22:56:20.056024 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py
+-rw-r--r--   0        0        0     3383 2021-07-28 20:35:08.818405 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py
+-rw-r--r--   0        0        0     2063 2021-07-28 20:35:08.818693 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py
+-rw-r--r--   0        0        0     2283 2021-07-28 20:35:08.819029 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py
+-rw-r--r--   0        0        0     2854 2022-01-20 00:05:30.500382 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py
+-rw-r--r--   0        0        0     1994 2021-07-28 20:35:08.819489 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py
+-rw-r--r--   0        0        0     2905 2021-07-28 20:35:08.819794 xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py
+-rw-r--r--   0        0        0      447 2022-12-15 20:10:31.069734 xrpl-py-2.0.0b0/xrpl/core/keypairs/__init__.py
+-rw-r--r--   0        0        0     1275 2021-07-28 20:35:08.820427 xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py
+-rw-r--r--   0        0        0     3662 2022-12-15 20:10:31.070556 xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py
+-rw-r--r--   0        0        0      182 2021-07-28 20:35:08.820941 xrpl-py-2.0.0b0/xrpl/core/keypairs/exceptions.py
+-rw-r--r--   0        0        0      893 2022-12-15 20:10:31.071456 xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py
+-rw-r--r--   0        0        0     4788 2022-12-15 20:10:31.072827 xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924715 xrpl-py-2.0.0b0/xrpl/core/keypairs/py.typed
+-rw-r--r--   0        0        0     7480 2022-07-28 00:01:58.132708 xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924787 xrpl-py-2.0.0b0/xrpl/core/py.typed
+-rw-r--r--   0        0        0      314 2021-07-28 20:35:08.822692 xrpl-py-2.0.0b0/xrpl/ledger/__init__.py
+-rw-r--r--   0        0        0     2283 2022-04-26 22:13:55.277744 xrpl-py-2.0.0b0/xrpl/ledger/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924863 xrpl-py-2.0.0b0/xrpl/ledger/py.typed
+-rw-r--r--   0        0        0      858 2021-12-17 21:23:35.552124 xrpl-py-2.0.0b0/xrpl/models/__init__.py
+-rw-r--r--   0        0        0      497 2021-12-17 23:17:45.561082 xrpl-py-2.0.0b0/xrpl/models/amounts/__init__.py
+-rw-r--r--   0        0        0     1377 2021-12-17 23:17:45.561971 xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py
+-rw-r--r--   0        0        0     1349 2021-12-17 21:23:35.554848 xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.924950 xrpl-py-2.0.0b0/xrpl/models/amounts/py.typed
+-rw-r--r--   0        0        0    10663 2022-07-05 22:56:20.059672 xrpl-py-2.0.0b0/xrpl/models/base_model.py
+-rw-r--r--   0        0        0      371 2021-07-28 20:35:08.825266 xrpl-py-2.0.0b0/xrpl/models/currencies/__init__.py
+-rw-r--r--   0        0        0      319 2021-07-28 20:35:08.825634 xrpl-py-2.0.0b0/xrpl/models/currencies/currency.py
+-rw-r--r--   0        0        0     2237 2021-12-17 21:23:35.557608 xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925039 xrpl-py-2.0.0b0/xrpl/models/currencies/py.typed
+-rw-r--r--   0        0        0     2500 2021-12-17 21:23:35.558615 xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py
+-rw-r--r--   0        0        0      171 2021-07-28 20:35:08.826501 xrpl-py-2.0.0b0/xrpl/models/exceptions.py
+-rw-r--r--   0        0        0     4300 2022-04-25 18:39:06.767427 xrpl-py-2.0.0b0/xrpl/models/flags.py
+-rw-r--r--   0        0        0     2462 2022-12-15 20:10:31.074348 xrpl-py-2.0.0b0/xrpl/models/nested_model.py
+-rw-r--r--   0        0        0     2088 2021-07-28 20:35:08.826856 xrpl-py-2.0.0b0/xrpl/models/path.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925126 xrpl-py-2.0.0b0/xrpl/models/py.typed
+-rw-r--r--   0        0        0     3428 2022-06-02 20:58:35.644160 xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py
+-rw-r--r--   0        0        0     1599 2021-07-28 20:35:08.828304 xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py
+-rw-r--r--   0        0        0     1213 2021-07-28 20:35:08.828881 xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py
+-rw-r--r--   0        0        0     1166 2021-07-28 20:35:08.829260 xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py
+-rw-r--r--   0        0        0     1373 2021-07-28 20:35:08.829871 xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py
+-rw-r--r--   0        0        0     1170 2021-12-17 23:17:45.563593 xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py
+-rw-r--r--   0        0        0     1760 2021-07-28 20:35:08.830168 xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py
+-rw-r--r--   0        0        0     1211 2021-07-28 20:35:08.830415 xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py
+-rw-r--r--   0        0        0     1257 2021-07-28 20:35:08.830671 xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py
+-rw-r--r--   0        0        0     1074 2021-07-28 20:35:08.830942 xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py
+-rw-r--r--   0        0        0     3020 2021-07-28 20:35:08.831227 xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py
+-rw-r--r--   0        0        0     1130 2021-07-28 20:35:08.831559 xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py
+-rw-r--r--   0        0        0     1204 2021-07-28 20:35:08.831844 xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py
+-rw-r--r--   0        0        0      625 2022-04-05 18:02:24.759920 xrpl-py-2.0.0b0/xrpl/models/requests/federator_info.py
+-rw-r--r--   0        0        0      775 2021-07-28 20:35:08.832085 xrpl-py-2.0.0b0/xrpl/models/requests/fee.py
+-rw-r--r--   0        0        0     1119 2021-07-28 20:35:08.832292 xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py
+-rw-r--r--   0        0        0     3068 2022-06-02 20:58:35.644917 xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py
+-rw-r--r--   0        0        0      832 2021-07-28 20:35:08.832476 xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py
+-rw-r--r--   0        0        0      944 2021-07-28 20:35:08.832645 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py
+-rw-r--r--   0        0        0      726 2021-07-28 20:35:08.832891 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py
+-rw-r--r--   0        0        0     1135 2021-07-28 20:35:08.833259 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py
+-rw-r--r--   0        0        0     4643 2021-07-28 20:35:08.833563 xrpl-py-2.0.0b0/xrpl/models/requests/ledger_entry.py
+-rw-r--r--   0        0        0      853 2021-07-28 20:35:08.833795 xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py
+-rw-r--r--   0        0        0      763 2022-04-25 18:39:06.768162 xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py
+-rw-r--r--   0        0        0      770 2022-04-25 18:39:06.768739 xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py
+-rw-r--r--   0        0        0     1496 2021-07-28 20:35:08.834038 xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py
+-rw-r--r--   0        0        0     4347 2021-07-28 20:35:08.834320 xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py
+-rw-r--r--   0        0        0      547 2021-07-28 20:35:08.834534 xrpl-py-2.0.0b0/xrpl/models/requests/ping.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925225 xrpl-py-2.0.0b0/xrpl/models/requests/py.typed
+-rw-r--r--   0        0        0      579 2021-07-28 20:35:08.834709 xrpl-py-2.0.0b0/xrpl/models/requests/random.py
+-rw-r--r--   0        0        0     5646 2022-07-05 22:56:20.061515 xrpl-py-2.0.0b0/xrpl/models/requests/request.py
+-rw-r--r--   0        0        0     2330 2021-07-28 20:35:08.835181 xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py
+-rw-r--r--   0        0        0      618 2021-07-28 20:35:08.835452 xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py
+-rw-r--r--   0        0        0     1194 2021-07-28 20:35:08.835707 xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py
+-rw-r--r--   0        0        0     4034 2022-07-05 22:56:20.063692 xrpl-py-2.0.0b0/xrpl/models/requests/sign.py
+-rw-r--r--   0        0        0     5062 2022-07-05 22:56:20.065263 xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py
+-rw-r--r--   0        0        0     3274 2022-07-05 22:56:20.066563 xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py
+-rw-r--r--   0        0        0     3758 2022-07-05 22:56:20.068102 xrpl-py-2.0.0b0/xrpl/models/requests/submit.py
+-rw-r--r--   0        0        0     2478 2022-07-05 22:56:20.069204 xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py
+-rw-r--r--   0        0        0     2842 2021-07-28 20:35:08.836916 xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py
+-rw-r--r--   0        0        0     2103 2021-07-28 20:35:08.837120 xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py
+-rw-r--r--   0        0        0     1278 2021-07-28 20:35:08.837698 xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py
+-rw-r--r--   0        0        0      817 2021-07-28 20:35:08.838021 xrpl-py-2.0.0b0/xrpl/models/requests/tx.py
+-rw-r--r--   0        0        0     1595 2021-07-28 20:35:08.838365 xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py
+-rw-r--r--   0        0        0      251 2021-07-28 20:35:08.838692 xrpl-py-2.0.0b0/xrpl/models/required.py
+-rw-r--r--   0        0        0     3617 2021-12-07 22:32:02.066250 xrpl-py-2.0.0b0/xrpl/models/response.py
+-rw-r--r--   0        0        0     3293 2022-06-02 20:58:35.645480 xrpl-py-2.0.0b0/xrpl/models/transactions/__init__.py
+-rw-r--r--   0        0        0     1333 2021-07-28 20:35:08.839736 xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py
+-rw-r--r--   0        0        0     8629 2022-04-25 18:40:11.716081 xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py
+-rw-r--r--   0        0        0     1101 2021-07-28 20:35:08.840429 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py
+-rw-r--r--   0        0        0     1993 2021-07-28 20:35:08.840706 xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py
+-rw-r--r--   0        0        0     1934 2021-07-28 20:35:08.841015 xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py
+-rw-r--r--   0        0        0     1598 2021-07-28 20:35:08.841280 xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py
+-rw-r--r--   0        0        0     1069 2021-07-28 20:35:08.841539 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py
+-rw-r--r--   0        0        0     2617 2021-07-28 20:35:08.841747 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py
+-rw-r--r--   0        0        0     2114 2021-07-28 20:35:08.841923 xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py
+-rw-r--r--   0        0        0     1923 2022-12-15 20:10:31.075374 xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py
+-rw-r--r--   0        0        0     4537 2022-04-25 18:39:06.770393 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py
+-rw-r--r--   0        0        0     1769 2022-04-25 18:39:06.771370 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py
+-rw-r--r--   0        0        0     2015 2022-04-25 18:39:06.771874 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py
+-rw-r--r--   0        0        0     4324 2022-04-25 18:40:20.537837 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py
+-rw-r--r--   0        0        0     4762 2022-04-25 18:40:11.718521 xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py
+-rw-r--r--   0        0        0     1045 2021-07-28 20:35:08.842102 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py
+-rw-r--r--   0        0        0     3866 2022-04-25 18:40:11.719936 xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py
+-rw-r--r--   0        0        0     5861 2022-04-25 18:40:11.721475 xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py
+-rw-r--r--   0        0        0     3917 2022-04-25 18:40:11.722725 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py
+-rw-r--r--   0        0        0     2367 2021-07-28 20:35:08.843065 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py
+-rw-r--r--   0        0        0     1614 2021-07-28 20:35:08.843590 xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py
+-rw-r--r--   0        0        0      575 2022-04-05 18:02:24.769631 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py
+-rw-r--r--   0        0        0     3651 2022-04-05 18:02:24.770653 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py
+-rw-r--r--   0        0        0     1366 2021-07-28 20:35:08.845018 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py
+-rw-r--r--   0        0        0     1874 2021-07-28 20:35:08.845329 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py
+-rw-r--r--   0        0        0     2262 2021-07-28 20:35:08.845606 xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925358 xrpl-py-2.0.0b0/xrpl/models/transactions/py.typed
+-rw-r--r--   0        0        0      959 2021-07-28 20:35:08.845886 xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py
+-rw-r--r--   0        0        0     4747 2022-09-15 21:17:23.562048 xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py
+-rw-r--r--   0        0        0      959 2021-12-07 22:32:02.070889 xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py
+-rw-r--r--   0        0        0    14500 2022-09-15 21:17:23.562911 xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py
+-rw-r--r--   0        0        0     2425 2022-04-25 18:40:11.724215 xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py
+-rw-r--r--   0        0        0      275 2021-07-28 20:35:08.847122 xrpl-py-2.0.0b0/xrpl/models/transactions/types/__init__.py
+-rw-r--r--   0        0        0      287 2021-07-28 20:35:08.847388 xrpl-py-2.0.0b0/xrpl/models/transactions/types/pseudo_transaction_type.py
+-rw-r--r--   0        0        0     1069 2021-12-17 23:17:45.570774 xrpl-py-2.0.0b0/xrpl/models/transactions/types/transaction_type.py
+-rw-r--r--   0        0        0      749 2021-12-17 23:17:45.571050 xrpl-py-2.0.0b0/xrpl/models/types.py
+-rw-r--r--   0        0        0     2174 2021-12-17 21:23:35.561520 xrpl-py-2.0.0b0/xrpl/models/utils.py
+-rw-r--r--   0        0        0        0 2021-12-07 22:32:02.074339 xrpl-py-2.0.0b0/xrpl/py.typed
+-rw-r--r--   0        0        0      958 2022-12-15 20:10:31.076208 xrpl-py-2.0.0b0/xrpl/transaction/__init__.py
+-rw-r--r--   0        0        0     1951 2022-12-15 20:10:31.079134 xrpl-py-2.0.0b0/xrpl/transaction/ledger.py
+-rw-r--r--   0        0        0     3896 2022-12-15 20:10:31.080226 xrpl-py-2.0.0b0/xrpl/transaction/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925547 xrpl-py-2.0.0b0/xrpl/transaction/py.typed
+-rw-r--r--   0        0        0     1163 2021-12-07 22:32:02.077113 xrpl-py-2.0.0b0/xrpl/transaction/reliable_submission.py
+-rw-r--r--   0        0        0      933 2022-08-23 17:19:34.993522 xrpl-py-2.0.0b0/xrpl/utils/__init__.py
+-rw-r--r--   0        0        0     3412 2022-04-25 18:39:06.775209 xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925715 xrpl-py-2.0.0b0/xrpl/utils/py.typed
+-rw-r--r--   0        0        0     1537 2022-07-05 22:56:20.074990 xrpl-py-2.0.0b0/xrpl/utils/sidechain.py
+-rw-r--r--   0        0        0      788 2021-12-17 21:23:35.563169 xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py
+-rw-r--r--   0        0        0     4202 2022-07-28 00:01:58.134040 xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py
+-rw-r--r--   0        0        0      350 2022-08-23 17:19:34.994080 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/__init__.py
+-rw-r--r--   0        0        0     1717 2022-07-05 22:56:20.082815 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py
+-rw-r--r--   0        0        0     1446 2022-07-05 22:56:20.083098 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py
+-rw-r--r--   0        0        0      641 2022-08-23 17:19:34.994400 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py
+-rw-r--r--   0        0        0      627 2022-08-23 17:19:34.995150 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py
+-rw-r--r--   0        0        0     5218 2022-08-23 17:19:34.995970 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py
+-rw-r--r--   0        0        0     2518 2022-12-15 20:10:31.082062 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py
+-rw-r--r--   0        0        0     6191 2022-08-23 17:19:34.996288 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py
+-rw-r--r--   0        0        0     1192 2022-08-23 17:19:34.996460 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py
+-rw-r--r--   0        0        0     1404 2022-12-15 20:10:31.082853 xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py
+-rw-r--r--   0        0        0     3476 2022-07-28 00:01:58.134766 xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py
+-rw-r--r--   0        0        0      269 2021-07-28 20:35:08.852350 xrpl-py-2.0.0b0/xrpl/wallet/__init__.py
+-rw-r--r--   0        0        0     8321 2022-12-15 20:10:31.083718 xrpl-py-2.0.0b0/xrpl/wallet/main.py
+-rw-r--r--   0        0        0        0 2021-11-09 22:17:07.925867 xrpl-py-2.0.0b0/xrpl/wallet/py.typed
+-rw-r--r--   0        0        0     1370 2022-04-05 18:02:24.775775 xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py
+-rw-r--r--   0        0        0    18248 2022-12-15 20:19:48.363167 xrpl-py-2.0.0b0/setup.py
+-rw-r--r--   0        0        0    17208 2022-12-15 20:19:48.364332 xrpl-py-2.0.0b0/PKG-INFO
```

### Comparing `xrpl_py-2.0.0/LICENSE` & `xrpl-py-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/README.md` & `xrpl-py-2.0.0b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 # create a wallet on the testnet
 from xrpl.wallet import generate_faucet_wallet
 test_wallet = generate_faucet_wallet(client)
 print(test_wallet)
 public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
 private_key: -HIDDEN-
-address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
+classic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
 
 # look up account info
-from xrpl.models import AccountInfo
+from xrpl.models.requests.account_info import AccountInfo
 acct_info = AccountInfo(
     account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
     ledger_index="current",
     queue=True,
     strict=True,
 )
 response = client.request(acct_info)
@@ -99,26 +99,26 @@
 #### `xrpl.wallet`
 
 Use the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).
 
 To create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):
 
 ```py
-wallet_from_seed = xrpl.wallet.Wallet.from_seed(seed)
+wallet_from_seed = xrpl.wallet.Wallet(seed, 0)
 print(wallet_from_seed)
 # pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0
 # priv_key: -HIDDEN-
-# address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
+# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
 ```
 
 To create a wallet from a Testnet faucet:
 
 ```py
 test_wallet = generate_faucet_wallet(client)
-test_account = test_wallet.address
+test_account = test_wallet.classic_address
 print("Classic address:", test_account)
 # Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw
 ```
 
 #### `xrpl.core.keypairs`
 
 Use the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.
@@ -153,41 +153,41 @@
 
 Use the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:
 
 * [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.
 
 * [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.
 
-* [`submit_and_wait`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.submit_and_wait) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
+* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
 
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import sign, submit_and_wait
+from xrpl.transaction import sign, send_reliable_submission
 from xrpl.ledger import get_latest_validated_ledger_sequence
 from xrpl.account import get_next_valid_seq_number
 
 current_validated_ledger = get_latest_validated_ledger_sequence(client)
 
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.address,
+    account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
     last_ledger_sequence=current_validated_ledger + 20,
-    sequence=get_next_valid_seq_number(test_wallet.address, client),
+    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),
     fee="10",
 )
 # sign the transaction
 my_tx_payment_signed = sign(my_tx_payment,test_wallet)
 
 # submit the transaction
-tx_response = submit_and_wait(my_tx_payment_signed, client)
+tx_response = send_reliable_submission(my_tx_payment_signed, client)
 ```
 
 #### Get fee from the XRP Ledger
 
 
 In most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:
 
@@ -200,27 +200,27 @@
 
 #### Auto-filled fields
 
 The `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import submit_and_wait, autofill_and_sign
+from xrpl.transaction import send_reliable_submission, autofill_and_sign
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.address,
+    account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"
 )
 
 # sign the transaction with the autofill method
 # (this will auto-populate the fee, sequence, and last_ledger_sequence)
-my_tx_payment_signed = autofill_and_sign(my_tx_payment, client, test_wallet)
+my_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)
 print(my_tx_payment_signed)
 # Payment(
 #     account='rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz',
 #     transaction_type=<TransactionType.PAYMENT: 'Payment'>,
 #     fee='10',
 #     sequence=16034065,
 #     account_txn_id=None,
@@ -237,26 +237,26 @@
 #     invoice_id=None,
 #     paths=None,
 #     send_max=None,
 #     deliver_min=None
 # )
 
 # submit the transaction
-tx_response = submit_and_wait(my_tx_payment_signed, client)
+tx_response = send_reliable_submission(my_tx_payment_signed, client)
 ```
 
 
 ### Subscribe to ledger updates
 
 You can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.
 
 ```py
 from xrpl.clients import WebsocketClient
 url = "wss://s.altnet.rippletest.net/"
-from xrpl.models import Subscribe, StreamParameter
+from xrpl.models.requests import Subscribe, StreamParameter
 req = Subscribe(streams=[StreamParameter.LEDGER])
 # NOTE: this code will run forever without a timeout, until the process is killed
 with WebsocketClient(url) as client:
     client.send(req)
     for message in client:
         print(message)
 # {'result': {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': '7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0', 'ledger_index': 18183504, 'ledger_time': 676412962, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'validated_ledgers': '17469391-18183504'}, 'status': 'success', 'type': 'response'}
@@ -271,37 +271,40 @@
 This library supports Python's [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.
 
 This sample code is the asynchronous equivalent of the above section on submitting a transaction.
 
 ```py
 import asyncio
 from xrpl.models.transactions import Payment
-from xrpl.asyncio.transaction import sign, submit_and_wait
+from xrpl.asyncio.transaction import sign, send_reliable_submission
 from xrpl.asyncio.ledger import get_latest_validated_ledger_sequence
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import AsyncJsonRpcClient
 
 async_client = AsyncJsonRpcClient(JSON_RPC_URL)
 
 async def submit_sample_transaction():
     current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
 
     # prepare the transaction
     # the amount is expressed in drops, not XRP
     # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
     my_tx_payment = Payment(
-        account=test_wallet.address,
+        account=test_wallet.classic_address,
         amount="2200000",
         destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
         last_ledger_sequence=current_validated_ledger + 20,
-        sequence=await get_next_valid_seq_number(test_wallet.address, async_client),
+        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),
         fee="10",
     )
-    # sign and submit the transaction
-    tx_response = await submit_and_wait(my_tx_payment_signed, async_client, test_wallet)
+    # sign the transaction
+    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)
+
+    # submit the transaction
+    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)
 
 asyncio.run(submit_sample_transaction())
 ```
 
 ### Encode addresses
 
 Use [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).
@@ -323,26 +326,22 @@
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
 
-We have a low-traffic mailing list for announcements of new `xrpl-py` releases. (About 1 email per week)
+We have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)
 
 + [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)
 
 If you're using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.
 
 + [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)
 
-### Code Samples
-- For samples of common use cases, see the [XRPL.org Code Samples](https://xrpl.org/code-samples.html) page.
-- You can also browse those samples [directly on GitHub](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples).
-
 ### Report an issue
 
 Experienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).
 
 ## License
 
 The `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.
```

### Comparing `xrpl_py-2.0.0/pyproject.toml` & `xrpl-py-2.0.0b0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xrpl-py"
-version = "2.0.0"
+version = "2.0.0-beta.0"
 description = "A complete Python library for interacting with the XRP ledger"
 readme = "README.md"
 repository = "https://github.com/XRPLF/xrpl-py"
 authors = [
   "Mayukha Vadari <mvadari@ripple.com>",
   "Greg Weisbrod <gweisbrod@ripple.com>",
   "Amie Corso <acorso@ripple.com>",
@@ -30,41 +30,41 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 base58 = "^2.1.0"
 ECPy = "^1.2.5"
 typing-extensions = "^4.2.0"
-httpx = ">=0.18.1,<0.25.0"
+httpx = ">=0.18.1,<0.24.0"
 websockets = [
     {version = ">=9.0.1 <11.0", python = ">= 3.7, < 3.10"},
     {version = "^10.0", python = "^3.10"}
 ]
 Deprecated = "^1.2.13"
 types-Deprecated = "^1.2.9"
 pycryptodome = "^3.16.0"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^3.8.4"
-black = "23.3.0"
-flake8-black = "^0.3.6"
-flake8-docstrings = "^1.7.0"
-mypy = "^1"
-isort = "^5.11.5"
-flake8-isort = "^6.0.0"
+black = "22.10.0"
+flake8-black = "^0.3.3"
+flake8-docstrings = "^1.5.0"
+mypy = "^0"
+isort = "^5.7.0"
+flake8-isort = "^5.0.0"
 flake8-annotations = "2.7.0"
 flake8-absolute-import = "^1.0"
 darglint = "^1.5.8"
-sphinx-rtd-theme = "^1.2.1"
+sphinx-rtd-theme = "^0.5.1"
 aiounittest = "^1.4.0"
-coverage = "^7.2.7"
+coverage = "^6.5.0"
 Jinja2 = "^3.1.2"
-MarkupSafe = "2.1.2"
+MarkupSafe = "2.1.1"
 Sphinx = "^5.3.0"
-poethepoet = "^0.19.0"
+poethepoet = "^0.16.5"
 
 [tool.isort]
 # Make sure that isort's settings line up with black
 profile = "black"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `xrpl_py-2.0.0/xrpl/account/main.py` & `xrpl-py-2.0.0b0/xrpl/account/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """High-level methods to obtain information about accounts."""
 
 import asyncio
 from typing import Dict, Union
 
+from deprecated.sphinx import deprecated
+
 from xrpl.asyncio.account import main
 from xrpl.clients.sync_client import SyncClient
+from xrpl.models.response import Response
 
 
 def does_account_exist(
     address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
 ) -> bool:
     """
     Query the ledger for whether the account exists.
@@ -84,7 +87,34 @@
             closed-and-proposed version), or "validated" (the most recent version
             validated by consensus). The default is "validated".
 
     Returns:
         The AccountRoot dictionary for the address.
     """
     return asyncio.run(main.get_account_root(address, client, ledger_index))
+
+
+@deprecated(
+    reason="Sending an AccountInfo request directly is just as easy to use.",
+    version="1.8.0",
+)
+def get_account_info(
+    address: str, client: SyncClient, ledger_index: Union[str, int] = "validated"
+) -> Response:
+    """
+    Query the ledger for account info of given address.
+
+    Args:
+        address: the account to query.
+        client: the network client used to make network calls.
+        ledger_index: The ledger index to use for the request. Must be an integer
+            ledger value or "current" (the current working version), "closed" (for the
+            closed-and-proposed version), or "validated" (the most recent version
+            validated by consensus). The default is "validated".
+
+    Returns:
+        The account info for the address.
+
+    Raises:
+        XRPLRequestFailureException: if the rippled API call fails.
+    """
+    return asyncio.run(main.get_account_info(address, client, ledger_index))
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/account/main.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/account/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """High-level methods to obtain information about accounts."""
 
 from typing import Dict, Union, cast
 
+from deprecated.sphinx import deprecated
+
 from xrpl.asyncio.clients import Client, XRPLRequestFailureException
+from xrpl.constants import XRPLException
 from xrpl.core.addresscodec import is_valid_xaddress, xaddress_to_classic_address
 from xrpl.models.requests import AccountInfo
+from xrpl.models.response import Response
 
 
 async def does_account_exist(
     address: str, client: Client, ledger_index: Union[str, int] = "validated"
 ) -> bool:
     """
     Query the ledger for whether the account exists.
@@ -24,15 +28,15 @@
     Returns:
         Whether the account exists on the ledger.
 
     Raises:
         XRPLRequestFailureException: if the transaction fails.
     """
     try:
-        await get_account_root(address, client, ledger_index=ledger_index)
+        await get_account_info(address, client)
         return True
     except XRPLRequestFailureException as e:
         if e.error == "actNotFound":
             # error code for if the account is not found on the ledger
             return False
         raise
 
@@ -72,17 +76,15 @@
             ledger value or "current" (the current working version), "closed" (for the
             closed-and-proposed version), or "validated" (the most recent version
             validated by consensus). The default is "validated".
 
     Returns:
         The balance of the address.
     """
-    return int(
-        (await get_account_root(address, client, ledger_index=ledger_index))["Balance"]
-    )
+    return int((await get_account_root(address, client))["Balance"])
 
 
 async def get_account_root(
     address: str, client: Client, ledger_index: Union[str, int] = "validated"
 ) -> Dict[str, Union[int, str]]:
     """
     Query the ledger for the AccountRoot object associated with a given address.
@@ -113,7 +115,56 @@
         )
     )
 
     if not account_info.is_successful():
         raise XRPLRequestFailureException(account_info.result)
 
     return cast(Dict[str, Union[int, str]], account_info.result["account_data"])
+
+
+@deprecated(
+    reason="Sending an AccountInfo request directly is just as easy to use.",
+    version="1.8.0",
+)
+async def get_account_info(
+    address: str, client: Client, ledger_index: Union[str, int] = "validated"
+) -> Response:
+    """
+    Query the ledger for account info of given address.
+
+    Args:
+        address: the account to query.
+        client: the network client used to make network calls.
+        ledger_index: The ledger index to use for the request. Must be an integer
+            ledger value or "current" (the current working version), "closed" (for the
+            closed-and-proposed version), or "validated" (the most recent version
+            validated by consensus). The default is "validated".
+
+    Returns:
+        The account info for the address.
+
+    Raises:
+        XRPLException: If the ledger_index value is invalid.
+        XRPLRequestFailureException: if the rippled API call fails.
+    """
+    if is_valid_xaddress(address):
+        address, _, _ = xaddress_to_classic_address(address)
+
+    if isinstance(ledger_index, str) and ledger_index not in {
+        "validated",
+        "current",
+        "closed",
+    }:
+        raise XRPLException(
+            "`ledger_index` is not valid - must be an `int` or one of {'validated', "
+            "'current', 'closed'}."
+        )
+    response = await client._request_impl(
+        AccountInfo(
+            account=address,
+            ledger_index=ledger_index,
+        )
+    )
+    if response.is_successful():
+        return response
+
+    raise XRPLRequestFailureException(response.result)
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/__init__.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/async_client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/async_websocket_client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/async_websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,21 +112,23 @@
             # remember to run your entire program within a
             # `asyncio.run` call.
             asyncio.run(main())
     """
 
     async def open(self: AsyncWebsocketClient) -> None:
         """Connects the client to the Web Socket API at the given URL."""
-        if not self.is_open():
-            await self._do_open()
+        if self.is_open():
+            return
+        await self._do_open()
 
     async def close(self: AsyncWebsocketClient) -> None:
         """Closes the connection."""
-        if self.is_open():
-            await self._do_close()
+        if not self.is_open():
+            return
+        await self._do_close()
 
     async def __aenter__(self: AsyncWebsocketClient) -> AsyncWebsocketClient:
         """
         Enters an async context after opening itself.
 
         Returns:
             The opened client.
@@ -140,20 +142,15 @@
         _exc_val: BaseException,
         _trace: TracebackType,
     ) -> None:
         """Exits an async context after closing itself."""
         await self.close()
 
     async def __aiter__(self: AsyncWebsocketClient) -> AsyncIterator[Dict[str, Any]]:
-        """
-        Iterate on received messages.
-
-        Yields:
-            Message at the top of the queue.
-        """
+        """Iterate on received messages."""
         while self.is_open():
             yield await self._do_pop_message()
 
     async def send(self: AsyncWebsocketClient, request: Request) -> None:
         """
         Submit the request represented by the request to the
         rippled node specified by this client's URL. Unlike ``request``,
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/client.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Interface for all network clients to follow."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Optional
 
 from xrpl.models.requests.request import Request
 from xrpl.models.response import Response
 
 
 class Client(ABC):
     """
@@ -19,16 +18,14 @@
         """
         Initializes a client.
 
         Arguments:
             url: The url to which this client will connect
         """
         self.url = url
-        self.network_id: Optional[int] = None
-        self.build_version: Optional[str] = None
 
     @abstractmethod
     async def _request_impl(self: Client, request: Request) -> Response:
         """
         This is the actual driver for a given Client's request. It must be
         async because all of the helper functions in this library are
         async-first. Implement this in a given Client.
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/exceptions.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/exceptions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/json_rpc_base.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/json_rpc_base.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/utils.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/clients/websocket_base.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/clients/websocket_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A client for interacting with the rippled WebSocket API."""
 from __future__ import annotations
 
-import asyncio
 import json
+from asyncio import Future, Queue, Task, create_task, get_running_loop
 from random import randrange
 from typing import TYPE_CHECKING, Any, Dict, Optional, cast
 
 from typing_extensions import Final
 from websockets.legacy.client import WebSocketClientProtocol, connect
 
 from xrpl.asyncio.clients.client import Client
@@ -15,34 +15,28 @@
 from xrpl.models.requests.request import Request
 from xrpl.models.response import Response
 
 _REQ_ID_MAX: Final[int] = 1_000_000
 # the types from asyncio are not implemented as generics in python 3.8 and
 # lower, so we need to only subscript them when running typechecking.
 if TYPE_CHECKING:
-    _REQUESTS_TYPE = Dict[str, asyncio.Future[Dict[str, Any]]]
-    _MESSAGES_TYPE = asyncio.Queue[Dict[str, Any]]
-    _HANDLER_TYPE = asyncio.Task[None]
+    _REQUESTS_TYPE = Dict[str, Future[Dict[str, Any]]]
+    _MESSAGES_TYPE = Queue[Dict[str, Any]]
+    _HANDLER_TYPE = Task[None]
 else:
-    _REQUESTS_TYPE = Dict[str, asyncio.Future]
-    _MESSAGES_TYPE = asyncio.Queue
-    _HANDLER_TYPE = asyncio.Task
+    _REQUESTS_TYPE = Dict[str, Future]
+    _MESSAGES_TYPE = Queue
+    _HANDLER_TYPE = Task
 
 
 def _inject_request_id(request: Request) -> Request:
     """
     Given a Request with an ID, return the same Request.
 
     Given a Request without an ID, make a copy with a randomly generated ID.
-
-    Arguments:
-        request: The request to inject an ID into.
-
-    Returns:
-        The request with an ID injected into it.
     """
     if request.id is not None:
         return request
     request_dict = request.to_dict()
     request_dict["id"] = f"{request.method}_{randrange(_REQ_ID_MAX)}"
     return Request.from_dict(request_dict)
 
@@ -87,18 +81,18 @@
 
     async def _do_open(self: WebsocketBase) -> None:
         """Connects the client to the Web Socket API at its URL."""
         # open the connection
         self._websocket = await connect(self.url)
 
         # make a message queue
-        self._messages = asyncio.Queue()
+        self._messages = Queue()
 
         # start the handler
-        self._handler_task = asyncio.create_task(self._handler())
+        self._handler_task = create_task(self._handler())
 
     async def _do_close(self: WebsocketBase) -> None:
         """Closes the connection."""
         # cancel the handler
         cast(_HANDLER_TYPE, self._handler_task).cancel()
         self._handler_task = None
 
@@ -137,65 +131,41 @@
             cast(_MESSAGES_TYPE, self._messages).put_nowait(response_dict)
 
     def _set_up_future(self: WebsocketBase, request: Request) -> None:
         """
         Only to be called from the public send and _request_impl functions.
         Given a request with an ID, ensure that that ID is backed by an open
         Future in self._open_requests.
-
-        Arguments:
-            request: The request with which to set up a future.
-
-        Raises:
-            XRPLWebsocketException: if there is already a request with this ID
-                in progress.
         """
         if request.id is None:
             return
         request_str = str(request.id)
         if (
             request_str in self._open_requests
             and not self._open_requests[request_str].done()
         ):
             raise XRPLWebsocketException(
                 f"Request {request_str} is already in progress."
             )
-        self._open_requests[request_str] = asyncio.get_running_loop().create_future()
+        self._open_requests[request_str] = get_running_loop().create_future()
 
     async def _do_send_no_future(self: WebsocketBase, request: Request) -> None:
-        """
-        Base websocket send function
-
-        Arguments:
-            request: The request to send.
-        """
         await cast(WebSocketClientProtocol, self._websocket).send(
             json.dumps(
                 request_to_websocket(request),
             ),
         )
 
     async def _do_send(self: WebsocketBase, request: Request) -> None:
-        """
-        Websocket send function that should be used by
-        any inherited classes.
-
-        Arguments:
-            request: The request to send.
-        """
         # we need to set up a future here, even if no one cares about it, so
         # that if a user submits a few requests with the same ID they fail.
         self._set_up_future(request)
         await self._do_send_no_future(request)
 
     async def _do_pop_message(self: WebsocketBase) -> Dict[str, Any]:
-        """
-        Returns:
-            The top message from the queue
-        """
         msg = await cast(_MESSAGES_TYPE, self._messages).get()
         cast(_MESSAGES_TYPE, self._messages).task_done()
         return msg
 
     async def _do_request_impl(self: WebsocketBase, request: Request) -> Response:
         """
         Base ``_request_impl`` implementation for websockets.
@@ -213,13 +183,13 @@
         # if no ID on this request, generate and inject one, and ensure it
         # is backed by a future
         request_with_id = _inject_request_id(request)
         request_str = str(request_with_id.id)
         self._set_up_future(request_with_id)
 
         # fire-and-forget the send, and await the Future
-        asyncio.create_task(self._do_send_no_future(request_with_id))
+        create_task(self._do_send_no_future(request_with_id))
         raw_response = await self._open_requests[request_str]
 
         # remove the resolved Future, hopefully getting it garbage colleted
         del self._open_requests[request_str]
         return websocket_to_response(raw_response)
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/ledger/main.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/ledger/utils.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/ledger/utils.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/transaction/__init__.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/transaction/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 """Async methods for working with transactions on the XRP Ledger."""
+from xrpl.asyncio.transaction.ledger import get_transaction_from_hash
 from xrpl.asyncio.transaction.main import (
     autofill,
     autofill_and_sign,
+    safe_sign_and_autofill_transaction,
+    safe_sign_and_submit_transaction,
+    safe_sign_transaction,
     sign,
     sign_and_submit,
     submit,
+    submit_transaction,
     transaction_json_to_binary_codec_form,
 )
 from xrpl.asyncio.transaction.reliable_submission import (
     XRPLReliableSubmissionException,
-    submit_and_wait,
+    send_reliable_submission,
 )
 
 __all__ = [
     "autofill",
     "autofill_and_sign",
+    "get_transaction_from_hash",
+    "safe_sign_transaction",
+    "safe_sign_and_autofill_transaction",
+    "safe_sign_and_submit_transaction",
     "sign",
     "sign_and_submit",
     "submit",
-    "submit_and_wait",
+    "submit_transaction",
     "transaction_json_to_binary_codec_form",
+    "send_reliable_submission",
     "XRPLReliableSubmissionException",
 ]
```

### Comparing `xrpl_py-2.0.0/xrpl/asyncio/wallet/wallet_generation.py` & `xrpl-py-2.0.0b0/xrpl/asyncio/wallet/wallet_generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,20 +9,18 @@
 from xrpl.asyncio.clients import Client, XRPLRequestFailureException
 from xrpl.constants import XRPLException
 from xrpl.wallet.main import Wallet
 
 _TEST_FAUCET_URL: Final[str] = "https://faucet.altnet.rippletest.net/accounts"
 _DEV_FAUCET_URL: Final[str] = "https://faucet.devnet.rippletest.net/accounts"
 _AMM_DEV_FAUCET_URL: Final[str] = "https://ammfaucet.devnet.rippletest.net/accounts"
-_HOOKS_V3_TEST_FAUCET_URL: Final[
+_NFT_DEV_FAUCET_URL: Final[str] = "https://faucet-nft.ripple.com/accounts"
+_HOOKS_V2_TEST_FAUCET_URL: Final[
     str
-] = "https://hooks-testnet-v3.xrpl-labs.com/accounts"
-_SIDECHAIN_DEVNET_FAUCET_URL: Final[
-    str
-] = "https://sidechain-faucet.devnet.rippletest.net/accounts"
+] = "https://hooks-testnet-v2.xrpl-labs.com/accounts"
 
 _TIMEOUT_SECONDS: Final[int] = 40
 
 
 class XRPLFaucetException(XRPLException):
     """Faucet generation exception."""
 
@@ -30,32 +28,24 @@
 
 
 async def generate_faucet_wallet(
     client: Client,
     wallet: Optional[Wallet] = None,
     debug: bool = False,
     faucet_host: Optional[str] = None,
-    usage_context: Optional[str] = None,
-    user_agent: Optional[str] = "xrpl-py",
 ) -> Wallet:
     """
     Generates a random wallet and funds it using the XRPL Testnet Faucet.
 
     Args:
         client: the network client used to make network calls.
         wallet: the wallet to fund. If omitted or `None`, a new wallet is created.
         debug: Whether to print debug information as it creates the wallet.
         faucet_host: A custom host to use for funding a wallet. In environments other
             than devnet and testnet, this parameter is required.
-        usage_context: The intended use case for the funding request
-            (for example, testing). This information  will be included
-            in the json body of the HTTP request to the faucet.
-        user_agent: A string representing the user agent (software/ client used)
-            for the HTTP request. Default is "xrpl-py".
-
 
     Returns:
         A Wallet on the testnet that contains some amount of XRP.
 
     Raises:
         XRPLFaucetException: if an address could not be funded with the faucet.
         XRPLRequestFailureException: if a request to the ledger fails.
@@ -64,24 +54,24 @@
     .. # noqa: DAR402 exception raised in private method
     """
     faucet_url = get_faucet_url(client.url, faucet_host)
 
     if wallet is None:
         wallet = Wallet.create()
 
-    address = wallet.address
+    address = wallet.classic_address
     # The faucet *can* be flakey... by printing info about this it's easier to
     # understand if tests are actually failing, or if it was just a faucet failure.
     if debug:
         print("Attempting to fund address {}".format(address))
     # Balance prior to asking for more funds
     starting_balance = await _check_wallet_balance(address, client)
 
     # Ask the faucet to send funds to the given address
-    await _request_funding(faucet_url, address, usage_context, user_agent)
+    await _request_funding(faucet_url, address)
     # Wait for the faucet to fund our account or until timeout
     # Waits one second checks if balance has changed
     # If balance doesn't change it will attempt again until _TIMEOUT_SECONDS
     is_funded = False
     for _ in range(_TIMEOUT_SECONDS):
         await asyncio.sleep(1)
         if not is_funded:  # faucet transaction hasn't been validated yet
@@ -116,29 +106,24 @@
         The URL of the matching faucet.
 
     Raises:
         XRPLFaucetException: if the provided URL is not for the testnet or devnet.
     """
     if faucet_host is not None:
         return f"https://{faucet_host}/accounts"
-    if "hooks-testnet-v3" in url:  # hooks v3 testnet
-        return _HOOKS_V3_TEST_FAUCET_URL
+    if "hooks-testnet-v2" in url:  # hooks v2 testnet
+        return _HOOKS_V2_TEST_FAUCET_URL
     if "altnet" in url or "testnet" in url:  # testnet
         return _TEST_FAUCET_URL
     if "amm" in url:  # amm devnet
         return _AMM_DEV_FAUCET_URL
-    if "sidechain-net1" in url:  # sidechain devnet
-        return _SIDECHAIN_DEVNET_FAUCET_URL
-    elif "sidechain-net2" in url:  # sidechain issuing chain devnet
-        raise XRPLFaucetException(
-            "Cannot fund an account on an issuing chain. Accounts must be created via "
-            "the bridge."
-        )
     if "devnet" in url:  # devnet
         return _DEV_FAUCET_URL
+    if "xls20-sandbox" in url:  # nft devnet
+        return _NFT_DEV_FAUCET_URL
     raise XRPLFaucetException(
         "Cannot fund an account with a client that is not on the testnet or devnet."
     )
 
 
 async def _check_wallet_balance(address: str, client: Client) -> int:
     try:
@@ -146,25 +131,17 @@
     except XRPLRequestFailureException as e:
         if e.error == "actNotFound":  # transaction has not gone through
             return 0
         # some other error
         raise
 
 
-async def _request_funding(
-    url: str,
-    address: str,
-    usage_context: Optional[str] = None,
-    user_agent: Optional[str] = None,
-) -> None:
+async def _request_funding(url: str, address: str) -> None:
     async with httpx.AsyncClient() as http_client:
-        json_body = {"destination": address, "userAgent": user_agent}
-        if usage_context is not None:
-            json_body["usageContext"] = usage_context
-        response = await http_client.post(url=url, json=json_body)
+        response = await http_client.post(url=url, json={"destination": address})
     if not response.status_code == httpx.codes.OK:
         response.raise_for_status()
 
 
 async def _try_to_get_next_seq(address: str, client: Client) -> Optional[int]:
     try:
         return await get_next_valid_seq_number(address, client)
```

### Comparing `xrpl_py-2.0.0/xrpl/clients/__init__.py` & `xrpl-py-2.0.0b0/xrpl/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/clients/sync_client.py` & `xrpl-py-2.0.0b0/xrpl/clients/sync_client.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/clients/websocket_client.py` & `xrpl-py-2.0.0b0/xrpl/clients/websocket_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A sync client for interacting with the rippled WebSocket API."""
 from __future__ import annotations
 
-import asyncio
+from asyncio import AbstractEventLoop, new_event_loop, run_coroutine_threadsafe
 from concurrent.futures import CancelledError, TimeoutError
 from threading import Thread
 from types import TracebackType
 from typing import Any, Dict, Iterator, Optional, Type, Union, cast
 
 from xrpl.asyncio.clients.exceptions import XRPLWebsocketException
 from xrpl.asyncio.clients.websocket_base import WebsocketBase
@@ -73,15 +73,15 @@
         Arguments:
             url: The URL of the rippled node to submit requests to.
             timeout: Maximum seconds to wait for a new message when
                 iterating. A value of 0 or None will result in no limit.
                 If this limit is met, iteration will stop.
         """
         self.timeout = timeout
-        self._loop: Optional[asyncio.AbstractEventLoop] = None
+        self._loop: Optional[AbstractEventLoop] = None
         self._thread: Optional[Thread] = None
         super().__init__(url)
 
     def is_open(self: WebsocketClient) -> bool:
         """
         Returns whether the client is currently open.
 
@@ -92,47 +92,47 @@
 
     def open(self: WebsocketClient) -> None:
         """Connects the client to the Web Socket API at the given URL."""
         if self.is_open():
             return
 
         # make a new asyncio event loop
-        self._loop = asyncio.new_event_loop()
+        self._loop = new_event_loop()
 
         # create and start a thread to run that event loop
         self._thread = Thread(
             target=self._loop.run_forever,
             daemon=True,
         )
         self._thread.start()
 
         # run WebsocketBase._do_open on the event loop of the child thread and
         # wait for it to finish
-        asyncio.run_coroutine_threadsafe(self._do_open(), self._loop).result()
+        run_coroutine_threadsafe(self._do_open(), self._loop).result()
 
     def close(self: WebsocketClient) -> None:
         """Closes the connection."""
         if not self.is_open():
             return
 
         # run WebsocketBase._do_close on the event loop of the child thread and
         # wait for it to finish
-        asyncio.run_coroutine_threadsafe(
-            self._do_close(), cast(asyncio.AbstractEventLoop, self._loop)
+        run_coroutine_threadsafe(
+            self._do_close(), cast(AbstractEventLoop, self._loop)
         ).result()
 
         # request the child thread to stop the loop and wait for it to
         # terminate
-        cast(asyncio.AbstractEventLoop, self._loop).call_soon_threadsafe(
-            cast(asyncio.AbstractEventLoop, self._loop).stop
+        cast(AbstractEventLoop, self._loop).call_soon_threadsafe(
+            cast(AbstractEventLoop, self._loop).stop
         )
         cast(Thread, self._thread).join()
 
         # close the stopped loop
-        cast(asyncio.AbstractEventLoop, self._loop).close()
+        cast(AbstractEventLoop, self._loop).close()
 
         # clear state
         self._loop = None
         self._thread = None
 
     def __enter__(self: WebsocketClient) -> WebsocketClient:
         """
@@ -156,21 +156,18 @@
     def __iter__(self: WebsocketClient) -> Iterator[Dict[str, Any]]:
         """
         Iterate on received messages. This iterator will block until
         a message is received. If no message is received within
         `self.timeout` seconds then the iterator will exit. If
         `self.timeout` is `None` or `0` then the iterator will block
         indefinetly for the next messsage.
-
-        Yields:
-            The message at the top of the queue.
         """
         while self.is_open():
-            future = asyncio.run_coroutine_threadsafe(
-                self._do_pop_message(), cast(asyncio.AbstractEventLoop, self._loop)
+            future = run_coroutine_threadsafe(
+                self._do_pop_message(), cast(AbstractEventLoop, self._loop)
             )
             try:
                 yield future.result(self.timeout)
             except TimeoutError:
                 # in this case, the future reached its timeout. we can safely
                 # cancel and stop listening
                 future.cancel()
@@ -192,16 +189,16 @@
 
         Raises:
             XRPLWebsocketException: If there is already an open request by the
                 request's ID, or if this WebsocketClient is not open.
         """
         if not self.is_open():
             raise XRPLWebsocketException("Websocket is not open")
-        asyncio.run_coroutine_threadsafe(
-            self._do_send(request), cast(asyncio.AbstractEventLoop, self._loop)
+        run_coroutine_threadsafe(
+            self._do_send(request), cast(AbstractEventLoop, self._loop)
         ).result()
 
     async def _request_impl(self: WebsocketClient, request: Request) -> Response:
         """
         ``_request_impl`` implementation for sync websockets that ensures the
         ``WebsocketBase._do_request_impl`` implementation is run on the other thread.
 
@@ -227,11 +224,11 @@
         # is a sync client we want to completely block until the request is
         # complete. also, `asyncio.run_coroutine_threadsafe` returns a
         # concurrent.futures.Future which is not awaitable.
         #
         # when this is run via `await client._request_impl`, it will
         # completely block the main thread until completed,
         # just as if it were not async.
-        return asyncio.run_coroutine_threadsafe(
+        return run_coroutine_threadsafe(
             self._do_request_impl(request),
-            cast(asyncio.AbstractEventLoop, self._loop),
+            cast(AbstractEventLoop, self._loop),
         ).result()
```

### Comparing `xrpl_py-2.0.0/xrpl/constants.py` & `xrpl-py-2.0.0b0/xrpl/constants.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/addresscodec/__init__.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/addresscodec/codec.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/codec.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/addresscodec/main.py` & `xrpl-py-2.0.0b0/xrpl/core/addresscodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/binary_wrappers/binary_serializer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/__init__.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/definitions.json` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972894959166432%*

 * *Differences: {"'FIELDS'": '{delete: [27]}',*

 * * "'TRANSACTION_RESULTS'": "{delete: ['telWRONG_NETWORK', 'telREQUIRES_NETWORK_ID', "*

 * *                          "'telNETWORK_ID_MAKES_TX_NON_CANONICAL']}"}*

```diff
@@ -267,24 +267,14 @@
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 20,
                 "type": "UInt16"
             }
         ],
         [
-            "NetworkID",
-            {
-                "isSerialized": true,
-                "isSigningField": true,
-                "isVLEncoded": false,
-                "nth": 1,
-                "type": "UInt32"
-            }
-        ],
-        [
             "Flags",
             {
                 "isSerialized": true,
                 "isSigningField": true,
                 "isVLEncoded": false,
                 "nth": 2,
                 "type": "UInt32"
@@ -2221,18 +2211,15 @@
         "telCAN_NOT_QUEUE_BLOCKED": -389,
         "telCAN_NOT_QUEUE_BLOCKS": -390,
         "telCAN_NOT_QUEUE_FEE": -388,
         "telCAN_NOT_QUEUE_FULL": -387,
         "telFAILED_PROCESSING": -395,
         "telINSUF_FEE_P": -394,
         "telLOCAL_ERROR": -399,
-        "telNETWORK_ID_MAKES_TX_NON_CANONICAL": -384,
         "telNO_DST_PARTIAL": -393,
-        "telREQUIRES_NETWORK_ID": -385,
-        "telWRONG_NETWORK": -386,
         "temBAD_AMOUNT": -298,
         "temBAD_CURRENCY": -297,
         "temBAD_EXPIRATION": -296,
         "temBAD_FEE": -295,
         "temBAD_ISSUER": -294,
         "temBAD_LIMIT": -293,
         "temBAD_NFTOKEN_TRANSFER_FEE": -262,
```

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/definitions.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/definitions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_header.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_header.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_info.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_info.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/definitions/field_instance.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/definitions/field_instance.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/field_id_codec.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/field_id_codec.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/main.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/__init__.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/account_id.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/account_id.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/amount.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/amount.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,14 @@
     Raises:
         XRPLBinaryCodecException: If issued_currency_value is invalid.
     """
     decimal_value = Decimal(issued_currency_value)
     if decimal_value.is_zero():
         return
     exponent = decimal_value.as_tuple().exponent
-    if not isinstance(exponent, int):  # NaN, sNaN, Infinity
-        raise XRPLBinaryCodecException(f"Expected exponent to be int, is {exponent}")
     if (
         (_calculate_precision(issued_currency_value) > MAX_IOU_PRECISION)
         or (exponent > MAX_IOU_EXPONENT)
         or (exponent < MIN_IOU_EXPONENT)
     ):
         raise XRPLBinaryCodecException(
             "Decimal precision out of range for issued currency value."
@@ -147,16 +145,14 @@
     decimal_value = Decimal(value)
     if decimal_value.is_zero():
         return _ZERO_CURRENCY_AMOUNT_HEX.to_bytes(8, byteorder="big")
 
     # Convert components to integers ---------------------------------------
     sign, digits, exp = decimal_value.as_tuple()
     mantissa = int("".join([str(d) for d in digits]))
-    if not isinstance(exp, int):  # NaN, sNaN, Infinity
-        raise XRPLBinaryCodecException(f"Expected exp to be int, is {exp}")
 
     # Canonicalize to expected range ---------------------------------------
     while mantissa < MIN_IOU_MANTISSA and exp > MIN_IOU_EXPONENT:
         mantissa *= 10
         exp -= 1
 
     while mantissa > MAX_IOU_MANTISSA:
```

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/blob.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/blob.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/currency.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/currency.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash160.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash160.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/hash256.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/hash256.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/path_set.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/path_set.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/serialized_type.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/serialized_type.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/st_array.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_array.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/st_object.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/st_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         from xrpl.core.binarycodec.binary_wrappers.binary_serializer import (
             BinarySerializer,
         )
 
         serializer = BinarySerializer()
 
         xaddress_decoded = {}
-        for k, v in value.items():
+        for (k, v) in value.items():
             if isinstance(v, str) and is_valid_xaddress(v):
                 handled = _handle_xaddress(k, v)
                 if (
                     _SOURCE_TAG in handled
                     and handled[_SOURCE_TAG] is not None
                     and _SOURCE_TAG in value
                     and value[_SOURCE_TAG] is not None
```

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint16.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint16.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint32.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint32.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint64.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint64.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/uint8.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/uint8.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/binarycodec/types/vector256.py` & `xrpl-py-2.0.0b0/xrpl/core/binarycodec/types/vector256.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/keypairs/crypto_implementation.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/crypto_implementation.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/keypairs/ed25519.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/ed25519.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/keypairs/helpers.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/helpers.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/core/keypairs/main.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Interface for cryptographic key pairs for use with the XRP Ledger."""
 from secrets import token_bytes
-from typing import Dict, Optional, Tuple, Type, Union
+from typing import Dict, Optional, Tuple, Type
 
 from typing_extensions import Final
 
 from xrpl.constants import CryptoAlgorithm
 from xrpl.core import addresscodec
 from xrpl.core.keypairs.crypto_implementation import CryptoImplementation
 from xrpl.core.keypairs.ed25519 import ED25519
@@ -93,27 +93,25 @@
     Returns:
         The classic address corresponding to the given public key.
     """
     account_id = get_account_id(bytes.fromhex(public_key))
     return addresscodec.encode_classic_address(account_id)
 
 
-def sign(message: Union[str, bytes], private_key: str) -> str:
+def sign(message: bytes, private_key: str) -> str:
     """
     Sign a message using a given private key.
 
     Args:
         message: The message to sign, as bytes.
         private_key: The private key to use to sign the message.
 
     Returns:
         Signed message, as hexadecimal.
     """
-    if isinstance(message, str):
-        message = bytes.fromhex(message)
     return (
         _get_module_from_key(private_key)
         .sign(
             message,
             private_key,
         )
         .hex()
```

### Comparing `xrpl_py-2.0.0/xrpl/core/keypairs/secp256k1.py` & `xrpl-py-2.0.0b0/xrpl/core/keypairs/secp256k1.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/ledger/main.py` & `xrpl-py-2.0.0b0/xrpl/ledger/main.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/amounts/amount.py` & `xrpl-py-2.0.0b0/xrpl/models/amounts/amount.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/amounts/issued_currency_amount.py` & `xrpl-py-2.0.0b0/xrpl/models/amounts/issued_currency_amount.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/base_model.py` & `xrpl-py-2.0.0b0/xrpl/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The base class for all model types."""
 
 from __future__ import annotations
 
 import json
 import re
 from abc import ABC
-from dataclasses import dataclass, fields
+from dataclasses import fields
 from enum import Enum
 from typing import Any, Dict, List, Pattern, Type, TypeVar, Union, cast, get_type_hints
 
 from typing_extensions import Final, get_args, get_origin
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.required import REQUIRED
@@ -59,15 +59,14 @@
     if isinstance(value, dict):
         return {_key_to_json(k): _value_to_json(v) for (k, v) in value.items()}
     if isinstance(value, list):
         return [_value_to_json(sub_value) for sub_value in value]
     return value
 
 
-@dataclass(frozen=True)
 class BaseModel(ABC):
     """The base class for all model types."""
 
     @classmethod
     def is_dict_of_model(cls: Type[BM], dictionary: Any) -> bool:
         """
         Checks whether the provided ``dictionary`` is a dictionary representation
@@ -269,15 +268,15 @@
 
         If not overridden, returns the object dict with all non-None values.
 
         Returns:
             The dictionary representation of a BaseModel.
         """
         # mypy doesn't realize that BaseModel has a field called __dataclass_fields__
-        dataclass_fields = self.__dataclass_fields__.keys()
+        dataclass_fields = self.__dataclass_fields__.keys()  # type: ignore
         return {
             key: self._to_dict_elem(getattr(self, key))
             for key in dataclass_fields
             if getattr(self, key) is not None
         }
 
     def _to_dict_elem(self: BaseModel, elem: Any) -> Any:
```

### Comparing `xrpl_py-2.0.0/xrpl/models/currencies/issued_currency.py` & `xrpl-py-2.0.0b0/xrpl/models/currencies/issued_currency.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/currencies/xrp.py` & `xrpl-py-2.0.0b0/xrpl/models/currencies/xrp.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,23 +57,18 @@
         Returns the dictionary representation of an XRP currency object.
 
         Returns:
             The dictionary representation of an XRP currency object.
         """
         return {**super().to_dict(), "currency": "XRP"}
 
-    def to_amount(self: XRP, value: Union[str, int, float]) -> str:
+    def to_amount(self: XRP, value: Union[str, int]) -> str:
         """
         Converts value to XRP.
 
         Args:
             value: The amount of XRP.
 
         Returns:
             A string representation of XRP amount.
         """
-        # import needed here to avoid circular dependency
-        from xrpl.utils.xrp_conversions import xrp_to_drops
-
-        if isinstance(value, str):
-            return xrp_to_drops(float(value))
-        return xrp_to_drops(value)
+        return str(value)
```

### Comparing `xrpl_py-2.0.0/xrpl/models/flags.py` & `xrpl-py-2.0.0b0/xrpl/models/flags.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-"""All transaction flags and utils to build a list of ints from a FlagInterface"""
+"""All transacion flags and utils to build a list of ints from a FlagInterface"""
 
 from typing import Dict, List, Union
 
 from typing_extensions import TypedDict
 
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.transactions.types.pseudo_transaction_type import PseudoTransactionType
 from xrpl.models.transactions.types.transaction_type import TransactionType
 
 TX_FLAGS: Dict[str, Dict[str, int]] = {
     "AccountSet": {
-        "tf_require_dest_tag": 0x00010000,
-        "tf_optional_dest_tag": 0x00020000,
-        "tf_require_auth": 0x00040000,
-        "tf_optional_auth": 0x00080000,
-        "tf_disallow_xrp": 0x00100000,
-        "tf_allow_xrp": 0x00200000,
+        "asf_account_tx_id": 0x00000005,
+        "asf_authorized_nftoken_minter": 0x0000000A,
+        "asf_default_ripple": 0x00000008,
+        "asf_deposit_auth": 0x00000009,
+        "asf_disable_master": 0x00000004,
+        "asf_disallow_xrp": 0x00000003,
+        "asf_global_freeze": 0x00000007,
+        "asf_no_freeze": 0x00000006,
+        "asf_require_auth": 0x00000002,
+        "asf_require_dest": 0x00000001,
     },
     "NFTokenCreateOffer": {
         "tf_sell_token": 0x00000001,
     },
     "NFTokenMint": {
         "tf_burnable": 0x00000001,
         "tf_only_xrp": 0x00000002,
```

### Comparing `xrpl_py-2.0.0/xrpl/models/nested_model.py` & `xrpl-py-2.0.0b0/xrpl/models/nested_model.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/path.py` & `xrpl-py-2.0.0b0/xrpl/models/path.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 from xrpl.models.requests.fee import Fee
 from xrpl.models.requests.gateway_balances import GatewayBalances
 from xrpl.models.requests.generic_request import GenericRequest
 from xrpl.models.requests.ledger import Ledger
 from xrpl.models.requests.ledger_closed import LedgerClosed
 from xrpl.models.requests.ledger_current import LedgerCurrent
 from xrpl.models.requests.ledger_data import LedgerData
-from xrpl.models.requests.ledger_entry import LedgerEntry, LedgerEntryType
+from xrpl.models.requests.ledger_entry import LedgerEntry
 from xrpl.models.requests.manifest import Manifest
 from xrpl.models.requests.nft_buy_offers import NFTBuyOffers
-from xrpl.models.requests.nft_history import NFTHistory
-from xrpl.models.requests.nft_info import NFTInfo
 from xrpl.models.requests.nft_sell_offers import NFTSellOffers
 from xrpl.models.requests.no_ripple_check import NoRippleCheck, NoRippleCheckRole
 from xrpl.models.requests.path_find import PathFind, PathFindSubcommand
 from xrpl.models.requests.ping import Ping
 from xrpl.models.requests.random import Random
 from xrpl.models.requests.request import Request
 from xrpl.models.requests.ripple_path_find import RipplePathFind
@@ -62,20 +60,17 @@
     "GatewayBalances",
     "GenericRequest",
     "Ledger",
     "LedgerClosed",
     "LedgerCurrent",
     "LedgerData",
     "LedgerEntry",
-    "LedgerEntryType",
     "Manifest",
     "NFTBuyOffers",
     "NFTSellOffers",
-    "NFTInfo",
-    "NFTHistory",
     "NoRippleCheck",
     "NoRippleCheckRole",
     "PathFind",
     "PathFindSubcommand",
     "PathStep",
     "Ping",
     "Random",
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_channels.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_channels.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 destination. (A channel's "source" and "owner" are the same.)
 
 All information retrieved is relative to a particular version of the ledger.
 
 `See account_channels <https://xrpl.org/account_channels.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountChannels(Request, LookupByLedgerRequest):
+class AccountChannels(Request):
     """
     This request returns information about an account's Payment Channels. This includes
     only channels where the specified account is the channel's source, not the
     destination. (A channel's "source" and "owner" are the same.)
 
     All information retrieved is relative to a particular version of the ledger.
 
@@ -37,7 +37,9 @@
     """
 
     destination_account: Optional[str] = None
     limit: int = 200
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_currencies.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_currencies.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 This is not a thoroughly confirmed list, but it can be used to populate user
 interfaces.
 
 `See account_currencies <https://xrpl.org/account_currencies.html>`_
 """
 from dataclasses import dataclass, field
+from typing import Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountCurrencies(Request, LookupByLedgerRequest):
+class AccountCurrencies(Request):
     """
     This request retrieves a list of currencies that an account can send or receive,
     based on its trust lines.
 
     This is not a thoroughly confirmed list, but it can be used to populate user
     interfaces.
 
@@ -29,9 +30,12 @@
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
+
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_CURRENCIES, init=False)
     strict: bool = False
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_info.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 balance.
 
 All information retrieved is relative to a particular version of the ledger.
 
 `See account_info <https://xrpl.org/account_info.html>`_
 """
 from dataclasses import dataclass, field
+from typing import Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountInfo(Request, LookupByLedgerRequest):
+class AccountInfo(Request):
     """
     This request retrieves information about an account, its activity, and its XRP
     balance.
 
     All information retrieved is relative to a particular version of the ledger.
 
     `See account_info <https://xrpl.org/account_info.html>`_
@@ -28,11 +29,13 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_INFO, init=False)
     queue: bool = False
     signer_lists: bool = False
     strict: bool = False
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_lines.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_lines.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 This request returns information about an account's trust lines, including balances
 in all non-XRP currencies and assets. All information retrieved is relative to a
 particular version of the ledger.
 
 `See account_lines <https://xrpl.org/account_lines.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountLines(Request, LookupByLedgerRequest):
+class AccountLines(Request):
     """
     This request returns information about an account's trust lines, including balances
     in all non-XRP currencies and assets. All information retrieved is relative to a
     particular version of the ledger.
 
     `See account_lines <https://xrpl.org/account_lines.html>`_
     """
@@ -27,13 +27,15 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_LINES, init=False)
     peer: Optional[str] = None
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_nfts.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_nfts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """This method retrieves all of the NFTs currently owned by the specified account."""
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountNFTs(Request, LookupByLedgerRequest):
+class AccountNFTs(Request):
     """
     This method retrieves all of the NFTs currently owned
     by the specified account.
     """
 
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_NFTS, init=False)
     account: str = REQUIRED  # type: ignore
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_objects.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 For a higher-level view of an account's trust lines and balances, see
 AccountLinesRequest instead.
 
 `See account_objects <https://xrpl.org/account_objects.html>`_
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class AccountObjectType(str, Enum):
     """Represents the object types that an AccountObjectsRequest can ask for."""
 
@@ -22,20 +22,19 @@
     DEPOSIT_PREAUTH = "deposit_preauth"
     ESCROW = "escrow"
     OFFER = "offer"
     PAYMENT_CHANNEL = "payment_channel"
     SIGNER_LIST = "signer_list"
     STATE = "state"
     TICKET = "ticket"
-    NFT_OFFER = "nft_offer"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountObjects(Request, LookupByLedgerRequest):
+class AccountObjects(Request):
     """
     This request returns the raw ledger format for all objects owned by an account.
 
     For a higher-level view of an account's trust lines and balances, see
     AccountLinesRequest instead.
 
     `See account_objects <https://xrpl.org/account_objects.html>`_
@@ -44,14 +43,16 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_OBJECTS, init=False)
     type: Optional[AccountObjectType] = None
     deletion_blockers_only: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_offers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
 This request retrieves a list of offers made by a given account that are
 outstanding as of a particular ledger version.
 
 `See account_offers <https://xrpl.org/account_offers.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountOffers(Request, LookupByLedgerRequest):
+class AccountOffers(Request):
     """
     This request retrieves a list of offers made by a given account that are
     outstanding as of a particular ledger version.
 
     `See account_offers <https://xrpl.org/account_offers.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_OFFERS, init=False)
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
     strict: bool = False
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/account_tx.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/account_tx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """
 This request retrieves from the ledger a list of transactions that involved the
 specified account.
 
 `See account_tx <https://xrpl.org/account_tx.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class AccountTx(Request, LookupByLedgerRequest):
+class AccountTx(Request):
     """
     This request retrieves from the ledger a list of transactions that involved the
     specified account.
 
     `See account_tx <https://xrpl.org/account_tx.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.ACCOUNT_TX, init=False)
     ledger_index_min: Optional[int] = None
     ledger_index_max: Optional[int] = None
     binary: bool = False
     forward: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/book_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/book_offers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 The book_offers method retrieves a list of offers, also known
 as the order book, between two currencies.
 """
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Optional, Union
 
 from xrpl.models.currencies import Currency
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class BookOffers(Request, LookupByLedgerRequest):
+class BookOffers(Request):
     """
     The book_offers method retrieves a list of offers, also known
     as the order book, between two currencies.
     """
 
     taker_gets: Currency = REQUIRED  # type: ignore
     """
@@ -30,9 +30,11 @@
     """
     This field is required.
 
     :meta hide-value:
     """
 
     method: RequestMethod = field(default=RequestMethod.BOOK_OFFERS, init=False)
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     limit: Optional[int] = None
     taker: Optional[str] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/channel_authorize.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/channel_authorize.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/channel_verify.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/channel_verify.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/deposit_authorized.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/deposit_authorized.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 The deposit_authorized command indicates whether one account
 is authorized to send payments directly to another. See
 Deposit Authorization for information on how to require
 authorization to deliver money to your account.
 """
 from dataclasses import dataclass, field
+from typing import Optional
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class DepositAuthorized(Request, LookupByLedgerRequest):
+class DepositAuthorized(Request):
     """
     The deposit_authorized command indicates whether one account
     is authorized to send payments directly to another. See
     Deposit Authorization for information on how to require
     authorization to deliver money to your account.
     """
 
@@ -32,7 +33,9 @@
     """
     This field is required.
 
     :meta hide-value:
     """
 
     method: RequestMethod = field(default=RequestMethod.DEPOSIT_AUTHORIZED, init=False)
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[str] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/fee.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/fee.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/gateway_balances.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/gateway_balances.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 excluding amounts held by operational addresses.
 
 `See gateway_balances <https://xrpl.org/gateway_balances.html>`_
 """
 from dataclasses import dataclass, field
 from typing import List, Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class GatewayBalances(Request, LookupByLedgerRequest):
+class GatewayBalances(Request):
     """
     This request calculates the total balances issued by a given account, optionally
     excluding amounts held by operational addresses.
 
     `See gateway_balances <https://xrpl.org/gateway_balances.html>`_
     """
 
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.GATEWAY_BALANCES, init=False)
     strict: bool = False
     hotwallet: Optional[Union[str, List[str]]] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/generic_request.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/generic_request.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ledger.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """
 Retrieve information about the public ledger.
 `See ledger <https://xrpl.org/ledger.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Optional, Union
 
-from xrpl.models.requests.ledger_entry import LedgerEntryType
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class Ledger(Request, LookupByLedgerRequest):
+class Ledger(Request):
     """
     Retrieve information about the public ledger.
     `See ledger <https://xrpl.org/ledger.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.LEDGER, init=False)
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     full: bool = False
     accounts: bool = False
     transactions: bool = False
     expand: bool = False
     owner_funds: bool = False
     binary: bool = False
     queue: bool = False
-    type: Optional[LedgerEntryType] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ledger_closed.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_closed.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ledger_current.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_current.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ledger_data.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 The ledger_data method retrieves contents of
 the specified ledger. You can iterate through
 several calls to retrieve the entire contents
 of a single ledger version.
 `See ledger data <https://xrpl.org/ledger_data.html>`_
 """
 from dataclasses import dataclass, field
-from typing import Any, Optional
+from typing import Any, Optional, Union
 
-from xrpl.models.requests.ledger_entry import LedgerEntryType
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class LedgerData(Request, LookupByLedgerRequest):
+class LedgerData(Request):
     """
     The ledger_data method retrieves contents of
     the specified ledger. You can iterate through
     several calls to retrieve the entire contents
     of a single ledger version.
     `See ledger data <https://xrpl.org/ledger_data.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.LEDGER_DATA, init=False)
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     binary: bool = False
     limit: Optional[int] = None
     # marker data shape is actually undefined in the spec, up to the
     # implementation of an individual server
     marker: Optional[Any] = None
-    type: Optional[LedgerEntryType] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ledger_entry.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ledger_entry.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,42 +4,22 @@
 See ledger format for information on the
 different types of objects you can retrieve.
 `See ledger entry <https://xrpl.org/ledger_entry.html>`_
 """
 from __future__ import annotations
 
 from dataclasses import dataclass, field
-from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from xrpl.models.base_model import BaseModel
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
-class LedgerEntryType(str, Enum):
-    """Identifiers for on-ledger objects."""
-
-    ACCOUNT = "account"
-    AMENDMENTS = "amendments"
-    CHECK = "check"
-    DEPOSIT_PREAUTH = "deposit_preauth"
-    DIRECTORY = "directory"
-    ESCROW = "escrow"
-    FEE = "fee"
-    HASHES = "hashes"
-    OFFER = "offer"
-    PAYMENT_CHANNEL = "payment_channel"
-    SIGNER_LIST = "signer_list"
-    STATE = "state"
-    TICKET = "ticket"
-    NFT_OFFER = "nft_offer"
-
-
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class DepositPreauth(BaseModel):
     """
     Required fields for requesting a DepositPreauth if not querying by
     object ID.
     """
@@ -170,15 +150,15 @@
 
     :meta hide-value:
     """
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class LedgerEntry(Request, LookupByLedgerRequest):
+class LedgerEntry(Request):
     """
     The ledger_entry method returns a single ledger
     object from the XRP Ledger in its raw format.
     See ledger format for information on the
     different types of objects you can retrieve.
     `See ledger entry <https://xrpl.org/ledger_entry.html>`_
     """
@@ -191,16 +171,16 @@
     directory: Optional[Union[str, Directory]] = None
     escrow: Optional[Union[str, Escrow]] = None
     offer: Optional[Union[str, Offer]] = None
     payment_channel: Optional[str] = None
     ripple_state: Optional[RippleState] = None
     ticket: Optional[Union[str, Ticket]] = None
     binary: bool = False
-    nft_page: Optional[str] = None
-    """Must be the object ID of the NFToken page, as hexadecimal"""
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
 
     def _get_errors(self: LedgerEntry) -> Dict[str, str]:
         errors = super()._get_errors()
         query_params = [
             param
             for param in [
                 self.index,
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/manifest.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/manifest.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/nft_buy_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/nft_buy_offers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 The `nft_buy_offers` method retrieves all of buy offers
 for the specified NFToken.
 """
 from dataclasses import dataclass, field
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NFTBuyOffers(Request, LookupByLedgerRequest):
+class NFTBuyOffers(Request):
     """
     The `nft_buy_offers` method retrieves all of buy offers
     for the specified NFToken.
     """
 
     method: RequestMethod = field(default=RequestMethod.NFT_BUY_OFFERS, init=False)
     nft_id: str = REQUIRED  # type: ignore
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/nft_sell_offers.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/nft_sell_offers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 The `nft_sell_offers` method retrieves all of sell offers
 for the specified NFToken.
 """
 from dataclasses import dataclass, field
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NFTSellOffers(Request, LookupByLedgerRequest):
+class NFTSellOffers(Request):
     """
     The `nft_sell_offers` method retrieves all of sell offers
     for the specified NFToken.
     """
 
     method: RequestMethod = field(default=RequestMethod.NFT_SELL_OFFERS, init=False)
     nft_id: str = REQUIRED  # type: ignore
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/no_ripple_check.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/no_ripple_check.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 for an account and the No Ripple flag of its trust lines, compared with the
 recommended settings.
 
 `See noripple_check <https://xrpl.org/noripple_check.html>`_
 """
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Optional
+from typing import Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 class NoRippleCheckRole(str, Enum):
     """Represents the options for the address role in a NoRippleCheckRequest."""
 
     GATEWAY = "gateway"
     USER = "user"
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class NoRippleCheck(Request, LookupByLedgerRequest):
+class NoRippleCheck(Request):
     """
     This request provides a quick way to check the status of the Default Ripple field
     for an account and the No Ripple flag of its trust lines, compared with the
     recommended settings.
 
     `See noripple_check <https://xrpl.org/noripple_check.html>`_
     """
@@ -35,14 +35,16 @@
     account: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
 
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     method: RequestMethod = field(default=RequestMethod.NO_RIPPLE_CHECK, init=False)
     role: NoRippleCheckRole = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/path_find.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/path_find.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ping.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ping.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/random.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/random.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/request.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,16 +54,14 @@
     LEDGER_CURRENT = "ledger_current"
     LEDGER_DATA = "ledger_data"
     LEDGER_ENTRY = "ledger_entry"
 
     # NFT methods
     NFT_BUY_OFFERS = "nft_buy_offers"
     NFT_SELL_OFFERS = "nft_sell_offers"
-    NFT_INFO = "nft_info"  # clio only
-    NFT_HISTORY = "nft_history"  # clio only
 
     # subscription methods
     SUBSCRIBE = "subscribe"
     UNSUBSCRIBE = "unsubscribe"
 
     # server info methods
     FEE = "fee"
@@ -71,22 +69,26 @@
     SERVER_INFO = "server_info"
     SERVER_STATE = "server_state"
 
     # utility methods
     PING = "ping"
     RANDOM = "random"
 
+    # sidechain methods
+    FEDERATOR_INFO = "federator_info"
+
     # generic unknown/unsupported request
     # (there is no XRPL analog, this model is specific to xrpl-py)
     GENERIC_REQUEST = "zzgeneric_request"
 
 
 R = TypeVar("R", bound="Request")
 
 
+@require_kwargs_on_init
 @dataclass(frozen=True)
 class Request(BaseModel):
     """
     The base class for all network request types.
     Represents fields common to all request types.
     """
 
@@ -155,18 +157,14 @@
             return xrpl.models.requests.NoRippleCheck
         if method == RequestMethod.ACCOUNT_NFTS:
             return xrpl.models.requests.AccountNFTs
         if method == RequestMethod.NFT_BUY_OFFERS:
             return xrpl.models.requests.NFTBuyOffers
         if method == RequestMethod.NFT_SELL_OFFERS:
             return xrpl.models.requests.NFTSellOffers
-        if method == RequestMethod.NFT_INFO:
-            return xrpl.models.requests.NFTInfo
-        if method == RequestMethod.NFT_HISTORY:
-            return xrpl.models.requests.NFTHistory
 
         parsed_name = "".join([word.capitalize() for word in method.split("_")])
         if parsed_name in xrpl.models.requests.__all__:
             return cast(Type[Request], getattr(xrpl.models.requests, parsed_name))
         return xrpl.models.requests.GenericRequest
 
     def to_dict(self: Request) -> Dict[str, Any]:
@@ -175,22 +173,7 @@
 
         Returns:
             The dictionary representation of a Request.
         """
         # we need to override this because method is using ``field``
         # which will not include the value in the object's __dict__
         return {**super().to_dict(), "method": self.method.value}
-
-
-@require_kwargs_on_init
-@dataclass(frozen=True)
-class LookupByLedgerRequest:
-    """Represents requests that need specifying an instance of the ledger"""
-
-    ledger_hash: Optional[str] = None
-    """
-    A 20-byte hex string for the ledger version to use.
-    """
-    ledger_index: Optional[Union[str, int]] = None
-    """
-    The ledger index of the ledger to use, or a shortcut string.
-    """
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/ripple_path_find.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/ripple_path_find.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 updates where possible.
 
 Although the rippled server tries to find the cheapest path or
 combination of paths for making a payment, it is not guaranteed that
 the paths returned by this method are, in fact, the best paths.
 """
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from xrpl.models.amounts import Amount
 from xrpl.models.currencies import Currency
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class RipplePathFind(Request, LookupByLedgerRequest):
+class RipplePathFind(Request):
     """
     The ripple_path_find method is a simplified version of the
     path_find method that provides a single response with a payment
     path you can use right away. It is available in both the WebSocket
     and JSON-RPC APIs. However, the results tend to become outdated as
     time passes. Instead of making multiple calls to stay updated, you
     should instead use the path_find method to subscribe to continued
@@ -58,7 +58,9 @@
 
     :meta hide-value:
     """
 
     method: RequestMethod = field(default=RequestMethod.RIPPLE_PATH_FIND, init=False)
     send_max: Optional[Amount] = None
     source_currencies: Optional[List[Currency]] = None
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/server_info.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/server_info.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/server_state.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/server_state.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/sign.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/sign_and_submit.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign_and_submit.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/sign_for.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/sign_for.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/submit.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/submit_multisigned.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit_multisigned.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/submit_only.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/submit_only.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/subscribe.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/subscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/transaction_entry.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/transaction_entry.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 
 `See transaction_entry <https://xrpl.org/transaction_entry.html>`_
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import Optional, Union
 
-from xrpl.models.requests.request import LookupByLedgerRequest, Request, RequestMethod
+from xrpl.models.requests.request import Request, RequestMethod
 from xrpl.models.required import REQUIRED
 from xrpl.models.utils import require_kwargs_on_init
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
-class TransactionEntry(Request, LookupByLedgerRequest):
+class TransactionEntry(Request):
     """
     The transaction_entry method retrieves information on a single transaction from a
     specific ledger version. (The tx method, by contrast, searches all ledgers for the
     specified transaction. We recommend using that method instead.)
 
     `See transaction_entry <https://xrpl.org/transaction_entry.html>`_
     """
 
     method: RequestMethod = field(default=RequestMethod.TRANSACTION_ENTRY, init=False)
+    ledger_hash: Optional[str] = None
+    ledger_index: Optional[Union[str, int]] = None
     tx_hash: str = REQUIRED  # type: ignore
     """
     This field is required.
 
     :meta hide-value:
     """
```

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/tx.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/tx.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/requests/unsubscribe.py` & `xrpl-py-2.0.0b0/xrpl/models/requests/unsubscribe.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/response.py` & `xrpl-py-2.0.0b0/xrpl/models/response.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Model objects for specific `types of Transactions
 <https://xrpl.org/transaction-types.html>`_ in the XRP Ledger.
 """
 
 from xrpl.models.transactions.account_delete import AccountDelete
 from xrpl.models.transactions.account_set import (
     AccountSet,
-    AccountSetAsfFlag,
     AccountSetFlag,
     AccountSetFlagInterface,
 )
 from xrpl.models.transactions.check_cancel import CheckCancel
 from xrpl.models.transactions.check_cash import CheckCash
 from xrpl.models.transactions.check_create import CheckCreate
 from xrpl.models.transactions.deposit_preauth import DepositPreauth
@@ -54,15 +53,14 @@
     TrustSetFlag,
     TrustSetFlagInterface,
 )
 
 __all__ = [
     "AccountDelete",
     "AccountSet",
-    "AccountSetAsfFlag",
     "AccountSetFlag",
     "AccountSetFlagInterface",
     "CheckCancel",
     "CheckCash",
     "CheckCreate",
     "DepositPreauth",
     "EscrowCancel",
@@ -79,21 +77,21 @@
     "NFTokenMintFlag",
     "NFTokenMintFlagInterface",
     "OfferCancel",
     "OfferCreate",
     "OfferCreateFlag",
     "OfferCreateFlagInterface",
     "Payment",
+    "PaymentFlag",
+    "PaymentFlagInterface",
     "PaymentChannelClaim",
     "PaymentChannelClaimFlag",
     "PaymentChannelClaimFlagInterface",
     "PaymentChannelCreate",
     "PaymentChannelFund",
-    "PaymentFlag",
-    "PaymentFlagInterface",
     "SetRegularKey",
     "Signer",
     "SignerEntry",
     "SignerListSet",
     "TicketCreate",
     "Transaction",
     "TransactionMetadata",
```

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/account_delete.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/account_delete.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/account_set.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/account_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,26 +19,24 @@
 _MIN_TICK_SIZE: Final[int] = 3
 _MAX_TICK_SIZE: Final[int] = 15
 _DISABLE_TICK_SIZE: Final[int] = 0
 
 _MAX_DOMAIN_LENGTH: Final[int] = 256
 
 
-class AccountSetAsfFlag(int, Enum):
+class AccountSetFlag(int, Enum):
     """
-    Enum for AccountSet Flags.
-
     There are several options which can be either enabled or disabled for an account.
     Account options are represented by different types of flags depending on the
     situation. The AccountSet transaction type has several "AccountSet Flags" (prefixed
     `asf`) that can enable an option when passed as the SetFlag parameter, or disable
     an option when passed as the ClearFlag parameter. This enum represents those
     options.
 
-    `See AccountSet asf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
+    `See AccountSet Flags <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     ASF_ACCOUNT_TXN_ID = 5
     """
     Track the ID of this account's most recent transaction. Required for
     `AccountTxnID <https://xrpl.org/transaction-common-fields.html#accounttxnid>`_
     """
@@ -87,93 +85,48 @@
 
     ASF_REQUIRE_DEST = 1
     """Require a destination tag to send transactions to this account."""
 
     ASF_AUTHORIZED_NFTOKEN_MINTER = 10
     """Allow another account to mint and burn tokens on behalf of this account."""
 
-    ASF_DISABLE_INCOMING_NFTOKEN_OFFER = 12
-    """Disallow other accounts from creating NFTokenOffers directed at this account."""
-
-    ASF_DISABLE_INCOMING_CHECK = 13
-    """Disallow other accounts from creating Checks directed at this account."""
-
-    ASF_DISABLE_INCOMING_PAYCHAN = 14
-    """Disallow other accounts from creating PayChannels directed at this account."""
-
-    ASF_DISABLE_INCOMING_TRUSTLINE = 15
-    """Disallow other accounts from creating Trustlines directed at this account."""
-
-
-class AccountSetFlag(int, Enum):
-    """
-    Enum for AccountSet Transaction Flags.
-
-    Transactions of the AccountSet type support additional values in the Flags field.
-    This enum represents those options.
-
-    `See AccountSet tf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
-    """
-
-    TF_REQUIRE_DEST_TAG = 0x00010000
-    """
-    The same as SetFlag: asfRequireDest.
-    """
-
-    TF_OPTIONAL_DEST_TAG = 0x00020000
-    """
-    The same as ClearFlag: asfRequireDest.
-    """
-
-    TF_REQUIRE_AUTH = 0x00040000
-    """
-    The same as SetFlag: asfRequireAuth.
-    """
-
-    TF_OPTIONAL_AUTH = 0x00080000
-    """
-    The same as ClearFlag: asfRequireAuth.
-    """
-
-    TF_DISALLOW_XRP = 0x00100000
-    """
-    The same as SetFlag: asfDisallowXRP.
-    """
-
-    TF_ALLOW_XRP = 0x00200000
-    """
-    The same as ClearFlag: asfDisallowXRP.
-    """
-
 
 class AccountSetFlagInterface(FlagInterface):
     """
-    Transactions of the AccountSet type support additional values in the Flags field.
-    This TypedDict represents those options.
+    There are several options which can be either enabled or disabled for an account.
+    Account options are represented by different types of flags depending on the
+    situation. The AccountSet transaction type has several "AccountSet Flags" (prefixed
+    `asf`) that can enable an option when passed as the SetFlag parameter, or disable
+    an option when passed as the ClearFlag parameter. This TypedDict represents those
+    options.
 
-    `See AccountSet tf Flags <https://xrpl.org/accountset.html#accountset-flags>`_
+    `See AccountSet Flags <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
-    TF_REQUIRE_DEST_TAG: bool
-    TF_OPTIONAL_DEST_TAG: bool
-    TF_REQUIRE_AUTH: bool
-    TF_OPTIONAL_AUTH: bool
-    TF_DISALLOW_XRP: bool
-    TF_ALLOW_XRP: bool
+    ASF_ACCOUNT_TXN_ID: bool
+    ASF_DEFAULT_RIPPLE: bool
+    ASF_DEPOSIT_AUTH: bool
+    ASF_DISABLE_MASTER: bool
+    ASF_DISALLOW_XRP: bool
+    ASF_GLOBAL_FREEZE: bool
+    ASF_NO_FREEZE: bool
+    ASF_REQUIRE_AUTH: bool
+    ASF_REQUIRE_DEST: bool
+    ASF_AUTHORIZED_NFTOKEN_MINTER: bool
 
 
 @require_kwargs_on_init
 @dataclass(frozen=True)
 class AccountSet(Transaction):
     """
     Represents an `AccountSet transaction <https://xrpl.org/accountset.html>`_,
     which modifies the properties of an account in the XRP Ledger.
     """
 
-    clear_flag: Optional[AccountSetAsfFlag] = None
+    clear_flag: Optional[int] = None
     """
     Disable a specific `AccountSet Flag
     <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     domain: Optional[str] = None
     """
@@ -186,15 +139,15 @@
     Set the MD5 Hash to be used for generating an avatar image for this
     account.
     """
 
     message_key: Optional[str] = None
     """Set a public key for sending encrypted messages to this account."""
 
-    set_flag: Optional[AccountSetAsfFlag] = None
+    set_flag: Optional[int] = None
     """
     Enable a specific `AccountSet Flag
     <https://xrpl.org/accountset.html#accountset-flags>`_
     """
 
     transfer_rate: Optional[int] = None
     """
@@ -210,15 +163,15 @@
     <https://xrpl.org/ticksize.html>`_ for details.
     """
 
     nftoken_minter: Optional[str] = None
     """
     Sets an alternate account that is allowed to mint NFTokens on this
     account's behalf using NFTokenMint's `Issuer` field. If set, you must
-    also set the AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER flag.
+    also set the AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER flag.
     """
 
     transaction_type: TransactionType = field(
         default=TransactionType.ACCOUNT_SET,
         init=False,
     )
 
@@ -267,32 +220,29 @@
     def _get_clear_flag_error(self: AccountSet) -> Optional[str]:
         if self.clear_flag is not None and self.clear_flag == self.set_flag:
             return "Must not be equal to the set_flag"
         return None
 
     def _get_nftoken_minter_error(self: AccountSet) -> Optional[str]:
         if (
-            self.set_flag != AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.set_flag != AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is not None
         ):
             return (
                 "Will not set the minter unless "
-                "AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
+                "AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
             )
         if (
-            self.set_flag == AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.set_flag == AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is None
         ):
-            return (
-                "Must be present if AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER "
-                "is set"
-            )
+            return "\
+                Must be present if AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is set"
         if (
-            self.clear_flag == AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
+            self.clear_flag == AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER
             and self.nftoken_minter is not None
         ):
             return (
-                "Must not be present if "
-                "AccountSetAsfFlag.ASF_AUTHORIZED_NFTOKEN_MINTER is unset "
-                "using clear_flag"
+                "Must not be present if AccountSetFlag.ASF_AUTHORIZED_NFTOKEN_MINTER "
+                "is unset using clear_flag"
             )
         return None
```

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/check_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/check_cash.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_cash.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/check_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/check_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/deposit_preauth.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/deposit_preauth.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/escrow_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/escrow_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/escrow_finish.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/escrow_finish.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/metadata.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 """Models for a transaction's metadata."""
 
 from typing import Dict, List, Union
 
-from typing_extensions import Literal, NotRequired, TypeAlias, TypedDict, TypeGuard
+from typing_extensions import Literal, NotRequired, TypedDict
 
 from xrpl.models.amounts.amount import Amount
 
 
-class NFTokenMetadataFields(TypedDict):
-    """Model for NFToken data in metadata."""
-
-    NFTokenID: str
-    URI: str
-
-
-class NFTokenMetadata(TypedDict):
-    """Model what NFTokens look like in metadata."""
-
-    NFToken: NFTokenMetadataFields
-
-
 class Fields(TypedDict):
     """Model for possible fields."""
 
     Flags: int
     Sequence: int
     Account: NotRequired[str]
     LowLimit: NotRequired[Dict[str, str]]
     HighLimit: NotRequired[Dict[str, str]]
     Balance: NotRequired[Union[Dict[str, str], str]]
     TakerGets: NotRequired[Union[Dict[str, str], str]]
     TakerPays: NotRequired[Union[Dict[str, str], str]]
     BookDirectory: NotRequired[str]
     Expiration: NotRequired[int]
-    NFTokens: NotRequired[List[NFTokenMetadata]]
 
 
 class CreatedNodeFields(TypedDict):
     """Fields of a CreatedNode."""
 
     LedgerEntryType: str
     LedgerIndex: str
@@ -87,49 +73,7 @@
 
     AffectedNodes: List[Union[CreatedNode, ModifiedNode, DeletedNode]]
     TransactionIndex: int
     TransactionResult: str
     DeliveredAmount: NotRequired[Amount]
     # "unavailable" possible for transactions before 2014-01-20
     delivered_amount: NotRequired[Union[Amount, Literal["unavailable"]]]
-
-
-Node: TypeAlias = Union[CreatedNode, ModifiedNode, DeletedNode]
-
-
-def isCreatedNode(node: Node) -> TypeGuard[CreatedNode]:
-    """
-    Typeguard for CreatedNode
-
-    Args:
-        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
-
-    Returns:
-        Whether this node is a CreatedNode.
-    """
-    return "CreatedNode" in node
-
-
-def isModifiedNode(node: Node) -> TypeGuard[ModifiedNode]:
-    """
-    Typeguard for ModifiedNode
-
-    Args:
-        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
-
-    Returns:
-        Whether this node is a ModifiedNode.
-    """
-    return "ModifiedNode" in node
-
-
-def isDeletedNode(node: Node) -> TypeGuard[DeletedNode]:
-    """
-    Typeguard for DeletedNode
-
-    Args:
-        node: A node of any type (CreatedNode, ModifiedNode, or DeletedNode)
-
-    Returns:
-        Whether this node is a DeletedNode.
-    """
-    return "DeletedNode" in node
```

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/nftoken_accept_offer.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_accept_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/nftoken_burn.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_burn.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/nftoken_cancel_offer.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_cancel_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/nftoken_create_offer.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_create_offer.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/nftoken_mint.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/nftoken_mint.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/offer_cancel.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_cancel.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/offer_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/offer_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/payment.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_claim.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_claim.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/payment_channel_fund.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/payment_channel_fund.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/__init__.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/enable_amendment.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/pseudo_transaction.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/set_fee.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/set_fee.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/pseudo_transactions/unl_modify.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/pseudo_transactions/unl_modify.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/set_regular_key.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/set_regular_key.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/signer_list_set.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/signer_list_set.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,36 +93,27 @@
                 "Must have a value of zero for `signer_quorum` if the signer list is "
                 "being deleted."
             )
 
         if self.signer_entries is None:  # deletion of the SignerList object
             return errors
 
-        if self.signer_quorum == REQUIRED:
-            errors["signer_quorum"] = "`signer_quorum` is not set."
-        elif self.signer_quorum <= 0:
-            errors["signer_quorum"] = (
-                "`signer_quorum` must be greater than or equal to 0 when not deleting "
-                "signer_list."
-            )
-
-        if not isinstance(self.signer_entries, list):
+        if self.signer_quorum <= 0:
             errors[
-                "signer_entries"
-            ] = "`signer_entries` must be a list of `SignerEntry` objects."
-            return errors
+                "signer_quorum"
+            ] = "`signer_quorum` must be greater than or equal to 0."
 
         if (
             len(self.signer_entries) < 1
             or len(self.signer_entries) > MAX_SIGNER_ENTRIES
         ):
             errors["signer_entries"] = (
-                "`signer_entries` must have at least 1 member and no more than "
-                f"{MAX_SIGNER_ENTRIES} members. If this transaction is deleting the "
-                "SignerList, then this parameter must be omitted."
+                "`signer_entries` must have at least 1 member and no more than {} "
+                "members. If this transaction is deleting the SignerList, then "
+                "this parameter must be omitted.".format(MAX_SIGNER_ENTRIES)
             )
             return errors
 
         account_set = set()
         signer_weight_sum = 0
 
         for signer_entry in self.signer_entries:
```

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/ticket_create.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/ticket_create.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/transaction.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from dataclasses import dataclass
 from hashlib import sha512
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
 from typing_extensions import Final
 
-from xrpl.core.binarycodec import decode, encode
+from xrpl.core.binarycodec import encode
 from xrpl.models.amounts import IssuedCurrencyAmount
 from xrpl.models.base_model import BaseModel
 from xrpl.models.exceptions import XRPLModelException
 from xrpl.models.flags import check_false_flag_definition, interface_to_flag_list
 from xrpl.models.nested_model import NestedModel
 from xrpl.models.requests import PathStep
 from xrpl.models.required import REQUIRED
@@ -251,17 +251,14 @@
 
     txn_signature: Optional[str] = None
     """
     The cryptographic signature from the sender that authorizes this
     transaction. Automatically added during signing.
     """
 
-    network_id: Optional[int] = None
-    """The network id of the transaction."""
-
     def _get_errors(self: Transaction) -> Dict[str, str]:
         errors = super()._get_errors()
         if self.ticket_sequence is not None and (
             (self.sequence is not None and self.sequence != 0)
             or self.account_txn_id is not None
         ):
             errors[
@@ -315,23 +312,14 @@
         based on the Transaction object.
 
         Returns:
             A JSON-like dictionary in the JSON format used by the binary codec.
         """
         return transaction_json_to_binary_codec_form(self.to_dict())
 
-    def blob(self: Transaction) -> str:
-        """
-        Creates the canonical binary format of the Transaction object.
-
-        Returns:
-            The binary-encoded object, as a hexadecimal string.
-        """
-        return encode(self.to_xrpl())
-
     @classmethod
     def from_dict(cls: Type[T], value: Dict[str, Any]) -> T:
         """
         Construct a new Transaction from a dictionary of parameters.
 
         Args:
             value: The value to construct the Transaction from.
@@ -379,44 +367,26 @@
             return flag in interface_to_flag_list(
                 tx_type=self.transaction_type,
                 tx_flags=self.flags,
             )
         else:  # is List[int]
             return flag in self.flags
 
-    def is_signed(self: Transaction) -> bool:
-        """
-        Checks if a transaction has been signed.
-
-        Returns:
-            Whether the transaction has been signed
-        """
-        if self.signers:
-            for signer in self.signers:
-                if (
-                    signer.signing_pub_key is None or len(signer.signing_pub_key) <= 0
-                ) or (signer.txn_signature is None or len(signer.txn_signature) <= 0):
-                    return False
-            return True
-        return (
-            self.signing_pub_key is not None and len(self.signing_pub_key) > 0
-        ) and (self.txn_signature is not None and len(self.txn_signature) > 0)
-
     def get_hash(self: Transaction) -> str:
         """
         Hashes the Transaction object as the ledger does. Only valid for signed
         Transaction objects.
 
         Returns:
             The hash of the Transaction object.
 
         Raises:
             XRPLModelException: if the Transaction is unsigned.
         """
-        if self.txn_signature is None and self.signers is None:
+        if self.txn_signature is None:
             raise XRPLModelException(
                 "Cannot get the hash from an unsigned Transaction."
             )
         prefix = hex(_TRANSACTION_HASH_PREFIX)[2:].upper()
         encoded_str = bytes.fromhex(prefix + encode(self.to_xrpl()))
         return sha512(encoded_str).digest().hex().upper()[:64]
 
@@ -450,20 +420,7 @@
             t.value: getattr(pseudo_transaction_models, t)
             for t in transaction_models.types.PseudoTransactionType
         }
         if transaction_type in pseudo_transaction_types:
             return pseudo_transaction_types[transaction_type]
 
         raise XRPLModelException(f"{transaction_type} is not a valid Transaction type")
-
-    @staticmethod
-    def from_blob(tx_blob: str) -> Transaction:
-        """
-        Decodes a transaction blob.
-
-        Args:
-            tx_blob: the tx blob to decode.
-
-        Returns:
-            The formatted transaction.
-        """
-        return Transaction.from_xrpl(decode(tx_blob))
```

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/trust_set.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/trust_set.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/transactions/types/transaction_type.py` & `xrpl-py-2.0.0b0/xrpl/models/transactions/types/transaction_type.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/types.py` & `xrpl-py-2.0.0b0/xrpl/models/types.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/models/utils.py` & `xrpl-py-2.0.0b0/xrpl/models/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Helper util functions for the models module."""
 
 from dataclasses import is_dataclass
-from typing import Any, Dict, List, Type, TypeVar, cast
+from typing import Any, Dict, List, Type, TypeVar
 
 from xrpl.models.exceptions import XRPLModelException
 
 # Code source for requiring kwargs:
 # https://gist.github.com/mikeholler/4be180627d3f8fceb55704b729464adb
 
 _T = TypeVar("_T")
@@ -58,8 +58,8 @@
                 f"Found the following positional arguments: {args}"
             )
         original_init(self, **kwargs)
 
     # noinspection PyTypeHints
     cls.__init__ = new_init  # type: ignore
 
-    return cast(Type[_T], cls)
+    return cls
```

### Comparing `xrpl_py-2.0.0/xrpl/transaction/main.py` & `xrpl-py-2.0.0b0/xrpl/transaction/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,132 +1,155 @@
 """High-level transaction methods with XRPL transactions."""
 import asyncio
-from typing import Optional
 
 from xrpl.asyncio.transaction import main
 from xrpl.clients.sync_client import SyncClient
 from xrpl.models.response import Response
 from xrpl.models.transactions.transaction import Transaction
 from xrpl.wallet.main import Wallet
 
 
 def sign_and_submit(
     transaction: Transaction,
-    client: SyncClient,
     wallet: Wallet,
+    client: SyncClient,
     autofill: bool = True,
     check_fee: bool = True,
 ) -> Response:
     """
     Signs a transaction (locally, without trusting external rippled nodes) and submits
     it to the XRPL.
 
     Args:
         transaction: the transaction to be signed and submitted.
-        client: the network client with which to submit the transaction.
         wallet: the wallet with which to sign the transaction.
+        client: the network client with which to submit the transaction.
         autofill: whether to autofill the relevant fields. Defaults to True.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
 
     Returns:
         The response from the ledger.
     """
     return asyncio.run(
         main.sign_and_submit(
             transaction,
-            client,
             wallet,
+            client,
             autofill,
             check_fee,
         )
     )
 
 
+safe_sign_and_submit_transaction = sign_and_submit
+
+
 def submit(
     transaction: Transaction,
     client: SyncClient,
-    *,
-    fail_hard: bool = False,
 ) -> Response:
     """
     Submits a transaction to the ledger.
 
     Args:
         transaction: the Transaction to be submitted.
         client: the network client with which to submit the transaction.
-        fail_hard: an optional boolean. If True, and the transaction fails for
-            the initial server, do not retry or relay the transaction to other
-            servers. Defaults to False.
 
     Returns:
         The response from the ledger.
 
     Raises:
         XRPLRequestFailureException: if the rippled API call fails.
     """
     return asyncio.run(
         main.submit(
             transaction,
             client,
-            fail_hard=fail_hard,
         )
     )
 
 
-sign = main.sign
+submit_transaction = submit
+
+
+def sign(
+    transaction: Transaction,
+    wallet: Wallet,
+    check_fee: bool = True,
+) -> Transaction:
+    """
+    Signs a transaction locally, without trusting external rippled nodes.
+
+    Args:
+        transaction: the transaction to be signed.
+        wallet: the wallet with which to sign the transaction.
+        check_fee: whether to check if the fee is higher than the expected transaction
+            type fee. Defaults to True.
+
+    Returns:
+        The signed transaction.
+    """
+    return asyncio.run(
+        main.sign(
+            transaction,
+            wallet,
+            check_fee,
+        )
+    )
+
+
+safe_sign_transaction = sign
 
 
 def autofill_and_sign(
     transaction: Transaction,
-    client: SyncClient,
     wallet: Wallet,
+    client: SyncClient,
     check_fee: bool = True,
 ) -> Transaction:
     """
     Signs a transaction locally, without trusting external rippled nodes. Autofills
     relevant fields.
 
     Args:
         transaction: the transaction to be signed.
-        client: a network client.
         wallet: the wallet with which to sign the transaction.
+        client: a network client.
         check_fee: whether to check if the fee is higher than the expected transaction
             type fee. Defaults to True.
 
     Returns:
         The signed transaction.
     """
     return asyncio.run(
         main.autofill_and_sign(
             transaction,
-            client,
             wallet,
+            client,
             check_fee,
         )
     )
 
 
-def autofill(
-    transaction: Transaction, client: SyncClient, signers_count: Optional[int] = None
-) -> Transaction:
+safe_sign_and_autofill_transaction = autofill_and_sign
+
+
+def autofill(transaction: Transaction, client: SyncClient) -> Transaction:
     """
     Autofills fields in a transaction. This will set `sequence`, `fee`, and
     `last_ledger_sequence` according to the current state of the server this Client is
     connected to. It also converts all X-Addresses to classic addresses.
 
     Args:
         transaction: the transaction to be signed.
         client: a network client.
-        signers_count: the expected number of signers for this transaction.
-            Only used for multisigned transactions.
 
     Returns:
         The autofilled transaction.
     """
     return asyncio.run(
         main.autofill(
             transaction,
             client,
-            signers_count,
         )
     )
```

### Comparing `xrpl_py-2.0.0/xrpl/utils/__init__.py` & `xrpl-py-2.0.0b0/xrpl/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Convenience utilities for the XRP Ledger"""
 
+from xrpl.utils.sidechain import create_cross_chain_payment
 from xrpl.utils.str_conversions import hex_to_str, str_to_hex
 from xrpl.utils.time_conversions import (
     XRPLTimeRangeException,
     datetime_to_ripple_time,
     posix_to_ripple_time,
     ripple_time_to_datetime,
     ripple_time_to_posix,
@@ -22,11 +23,12 @@
     "drops_to_xrp",
     "ripple_time_to_datetime",
     "datetime_to_ripple_time",
     "ripple_time_to_posix",
     "posix_to_ripple_time",
     "XRPRangeException",
     "XRPLTimeRangeException",
+    "create_cross_chain_payment",
     "get_balance_changes",
     "get_final_balances",
     "get_order_book_changes",
 ]
```

### Comparing `xrpl_py-2.0.0/xrpl/utils/parse_nftoken_id.py` & `xrpl-py-2.0.0b0/xrpl/utils/parse_nftoken_id.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/str_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/str_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/time_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/time_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/get_balance_changes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_balance_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/get_final_balances.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_final_balances.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/get_order_book_changes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/get_order_book_changes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/__init__.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/balance_parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/balance_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/nodes.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/nodes.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/order_book_parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/order_book_parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/parser.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/parser.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/txn_parser/utils/types.py` & `xrpl-py-2.0.0b0/xrpl/utils/txn_parser/utils/types.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/utils/xrp_conversions.py` & `xrpl-py-2.0.0b0/xrpl/utils/xrp_conversions.py`

 * *Files identical despite different names*

### Comparing `xrpl_py-2.0.0/xrpl/wallet/main.py` & `xrpl-py-2.0.0b0/xrpl/wallet/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,87 +13,69 @@
     """
     The cryptographic keys needed to control an XRP Ledger account. See
     `Cryptographic Keys <https://xrpl.org/cryptographic-keys.html>`_ for
     details.
     """
 
     @property
-    def address(self: Wallet) -> str:
+    def classic_address(self: Wallet) -> str:
         """
-        The XRPL address that publicly identifies this wallet,
-        as a base58 string. This is the same value as the `classic_address`.
+        The address that publicly identifies this wallet,
+        as a base58 string.
         """  # noqa: DAR201
-        return self._address
+        return self._classic_address
 
-    classic_address = address
+    address = classic_address
     """
-    `classic_address` is the same as `address`. It is called `classic_address` to
-    differentiate it from the x-address standard, which encodes the network,
-    destination tag, and XRPL address into a single value. It's also a base58 string.
+    The address that publicly identifies this wallet, as a base58 string.
     """
 
     def __init__(
         self: Wallet,
         public_key: str,
         private_key: str,
         *,
         master_address: Optional[str] = None,
         seed: Optional[str] = None,
-        algorithm: Optional[CryptoAlgorithm] = None,
     ) -> None:
         """
         Generate a new Wallet.
 
         Args:
             public_key: The public key for the account.
             private_key: The private key used for signing transactions for the account.
             master_address: Include if a Wallet uses a Regular Key Pair. This sets the
                 address that this wallet corresponds to. The default is `None`.
             seed: The seed used to derive the account keys. The default is `None`.
-            algorithm: The algorithm used to encode the keys. Inferred from the seed if
-                not included
         """
-        self.seed = seed
-        """
-        The core value that is used to derive all other information about
-        this wallet. MUST be kept secret!
-        """
-
-        if algorithm is None:
-            if seed is not None and seed.startswith("sEd"):
-                wallet_algorithm = CryptoAlgorithm.ED25519
-            else:
-                wallet_algorithm = CryptoAlgorithm.SECP256K1
-        else:
-            wallet_algorithm = algorithm
-
-        self.algorithm = wallet_algorithm
-        """
-        The algorithm that is used to convert the seed into its public/private keypair.
-        """
-
         self.public_key = public_key
         """
         The public key that is used to identify this wallet's signatures, as
         a hexadecimal string.
         """
 
         self.private_key = private_key
         """
         The private key that is used to create signatures, as a hexadecimal
         string. MUST be kept secret!
         """
 
-        self._address = (
+        self._classic_address = (
             ensure_classic_address(master_address)
             if master_address is not None
             else derive_classic_address(self.public_key)
         )
         """Internal variable for classic_address. Use classic_address instead."""
 
+        self.seed = seed
+        """
+        The core value that is used to derive all other information about
+        this wallet. MUST be kept secret!
+        """
+
     @classmethod
     def create(
         cls: Type[Wallet], algorithm: CryptoAlgorithm = CryptoAlgorithm.ED25519
     ) -> Wallet:
         """
         Generates a new seed and Wallet.
 
@@ -125,21 +107,15 @@
             algorithm: The key-generation algorithm to use when generating the seed.
                 The default is `ED25519`.
 
         Returns:
             The wallet that is generated from the given secret.
         """
         public_key, private_key = derive_keypair(seed, algorithm=algorithm)
-        return cls(
-            public_key,
-            private_key,
-            master_address=master_address,
-            seed=seed,
-            algorithm=algorithm,
-        )
+        return cls(public_key, private_key, master_address=master_address, seed=seed)
 
     from_secret = from_seed
 
     @classmethod
     def from_entropy(
         cls: Type[Wallet],
         entropy: str,
@@ -242,23 +218,23 @@
             tag: The destination tag of the address. Defaults to `None`.
             is_test: Whether the address corresponds to an address on the test network.
                 Defaults to `False`.
 
         Returns:
             The X-Address of the Wallet's account.
         """
-        return classic_address_to_xaddress(self.address, tag, is_test)
+        return classic_address_to_xaddress(self.classic_address, tag, is_test)
 
     def __str__(self: Wallet) -> str:
         """
         Returns a string representation of a Wallet.
 
         Returns:
             A string representation of a Wallet.
         """
         return "\n".join(
             [
                 f"public_key: {self.public_key}",
                 "private_key: -HIDDEN-",
-                f"classic_address: {self.address}",
+                f"classic_address: {self.classic_address}",
             ]
         )
```

### Comparing `xrpl_py-2.0.0/xrpl/wallet/wallet_generation.py` & `xrpl-py-2.0.0b0/xrpl/wallet/wallet_generation.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,35 +8,29 @@
 
 
 def generate_faucet_wallet(
     client: SyncClient,
     wallet: Optional[Wallet] = None,
     debug: bool = False,
     faucet_host: Optional[str] = None,
-    usage_context: Optional[str] = None,
 ) -> Wallet:
     """
     Generates a random wallet and funds it using the XRPL Testnet Faucet.
 
     Args:
         client: the network client used to make network calls.
         wallet: the wallet to fund. If omitted or `None`, a new wallet is created.
         debug: Whether to print debug information as it creates the wallet.
         faucet_host: A custom host to use for funding a wallet. In environments other
             than devnet and testnet, this parameter is required.
-        usage_context: The intended use case for the funding request
-            (for example, testing). This information will be included in json body
-            of the HTTP request to the faucet.
 
     Returns:
         A Wallet on the testnet that contains some amount of XRP.
 
     Raises:
         XRPLFaucetException: if an address could not be funded with the faucet.
         XRPLRequestFailureException: if a request to the ledger fails.
         requests.exceptions.HTTPError: if the request to the faucet fails.
 
     .. # noqa: DAR402 exception raised in private method
     """
-    return asyncio.run(
-        async_generate_faucet_wallet(client, wallet, debug, faucet_host, usage_context)
-    )
+    return asyncio.run(async_generate_faucet_wallet(client, wallet, debug, faucet_host))
```

### Comparing `xrpl_py-2.0.0/PKG-INFO` & `xrpl-py-2.0.0b0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: xrpl-py
-Version: 2.0.0
+Version: 2.0.0b0
 Summary: A complete Python library for interacting with the XRP ledger
 Home-page: https://github.com/XRPLF/xrpl-py
 License: ISC
 Keywords: xrp,xrpl,cryptocurrency
 Author: Mayukha Vadari
 Author-email: mvadari@ripple.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: ECPy (>=1.2.5,<2.0.0)
 Requires-Dist: base58 (>=2.1.0,<3.0.0)
-Requires-Dist: httpx (>=0.18.1,<0.25.0)
+Requires-Dist: httpx (>=0.18.1,<0.24.0)
 Requires-Dist: pycryptodome (>=3.16.0,<4.0.0)
 Requires-Dist: types-Deprecated (>=1.2.9,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
-Requires-Dist: websockets (>=10.0,<11.0) ; python_version >= "3.10" and python_version < "4.0"
-Requires-Dist: websockets (>=9.0.1,<11.0) ; python_version >= "3.7" and python_version < "3.10"
+Requires-Dist: websockets (>=10.0,<11.0); python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: websockets (>=9.0.1,<11.0); python_version >= "3.7" and python_version < "3.10"
 Project-URL: Documentation, https://xrpl-py.readthedocs.io
 Project-URL: Repository, https://github.com/XRPLF/xrpl-py
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/xrpl-py/badge)](https://xrpl-py.readthedocs.io/)
 
 # xrpl-py
@@ -43,18 +42,18 @@
 
 # create a wallet on the testnet
 from xrpl.wallet import generate_faucet_wallet
 test_wallet = generate_faucet_wallet(client)
 print(test_wallet)
 public_key: ED3CC1BBD0952A60088E89FA502921895FC81FBD79CAE9109A8FE2D23659AD5D56
 private_key: -HIDDEN-
-address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
+classic_address: rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo
 
 # look up account info
-from xrpl.models import AccountInfo
+from xrpl.models.requests.account_info import AccountInfo
 acct_info = AccountInfo(
     account="rBtXmAdEYcno9LWRnAGfT9qBxCeDvuVRZo",
     ledger_index="current",
     queue=True,
     strict=True,
 )
 response = client.request(acct_info)
@@ -129,26 +128,26 @@
 #### `xrpl.wallet`
 
 Use the [`xrpl.wallet`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.wallet.html) module to create a wallet from a given seed or or via a [Testnet faucet](https://xrpl.org/xrp-testnet-faucet.html).
 
 To create a wallet from a seed (in this case, the value generated using [`xrpl.keypairs`](#xrpl-keypairs)):
 
 ```py
-wallet_from_seed = xrpl.wallet.Wallet.from_seed(seed)
+wallet_from_seed = xrpl.wallet.Wallet(seed, 0)
 print(wallet_from_seed)
 # pub_key: ED46949E414A3D6D758D347BAEC9340DC78F7397FEE893132AAF5D56E4D7DE77B0
 # priv_key: -HIDDEN-
-# address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
+# classic_address: rG5ZvYsK5BPi9f1Nb8mhFGDTNMJhEhufn6
 ```
 
 To create a wallet from a Testnet faucet:
 
 ```py
 test_wallet = generate_faucet_wallet(client)
-test_account = test_wallet.address
+test_account = test_wallet.classic_address
 print("Classic address:", test_account)
 # Classic address: rEQB2hhp3rg7sHj6L8YyR4GG47Cb7pfcuw
 ```
 
 #### `xrpl.core.keypairs`
 
 Use the [`xrpl.core.keypairs`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.keypairs.html#module-xrpl.core.keypairs) module to generate seeds and derive keypairs and addresses from those seed values.
@@ -183,41 +182,41 @@
 
 Use the [`xrpl.transaction`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html) module to sign and submit transactions. The module offers three ways to do this:
 
 * [`sign_and_submit`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign_and_submit) — Signs a transaction locally, then submits it to the XRP Ledger. This method does not implement [reliable transaction submission](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission) best practices, so only use it for development or testing purposes.
 
 * [`sign`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.sign) — Signs a transaction locally. This method **does  not** submit the transaction to the XRP Ledger.
 
-* [`submit_and_wait`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.submit_and_wait) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
+* [`send_reliable_submission`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.transaction.html#xrpl.transaction.send_reliable_submission) — An implementation of the [reliable transaction submission guidelines](https://xrpl.org/reliable-transaction-submission.html#reliable-transaction-submission), this method submits a signed transaction to the XRP Ledger and then verifies that it has been included in a validated ledger (or has failed to do so). Use this method to submit transactions for production purposes.
 
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import sign, submit_and_wait
+from xrpl.transaction import sign, send_reliable_submission
 from xrpl.ledger import get_latest_validated_ledger_sequence
 from xrpl.account import get_next_valid_seq_number
 
 current_validated_ledger = get_latest_validated_ledger_sequence(client)
 
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.address,
+    account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
     last_ledger_sequence=current_validated_ledger + 20,
-    sequence=get_next_valid_seq_number(test_wallet.address, client),
+    sequence=get_next_valid_seq_number(test_wallet.classic_address, client),
     fee="10",
 )
 # sign the transaction
 my_tx_payment_signed = sign(my_tx_payment,test_wallet)
 
 # submit the transaction
-tx_response = submit_and_wait(my_tx_payment_signed, client)
+tx_response = send_reliable_submission(my_tx_payment_signed, client)
 ```
 
 #### Get fee from the XRP Ledger
 
 
 In most cases, you can specify the minimum [transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) of `"10"` for the `fee` field unless you have a strong reason not to. But if you want to get the [current load-balanced transaction cost](https://xrpl.org/transaction-cost.html#current-transaction-cost) from the network, you can use the `get_fee` function:
 
@@ -230,27 +229,27 @@
 
 #### Auto-filled fields
 
 The `xrpl-py` library automatically populates the `fee`, `sequence` and `last_ledger_sequence` fields when you create transactions. In the example above, you could omit those fields and let the library fill them in for you.
 
 ```py
 from xrpl.models.transactions import Payment
-from xrpl.transaction import submit_and_wait, autofill_and_sign
+from xrpl.transaction import send_reliable_submission, autofill_and_sign
 # prepare the transaction
 # the amount is expressed in drops, not XRP
 # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
 my_tx_payment = Payment(
-    account=test_wallet.address,
+    account=test_wallet.classic_address,
     amount="2200000",
     destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe"
 )
 
 # sign the transaction with the autofill method
 # (this will auto-populate the fee, sequence, and last_ledger_sequence)
-my_tx_payment_signed = autofill_and_sign(my_tx_payment, client, test_wallet)
+my_tx_payment_signed = autofill_and_sign(my_tx_payment, test_wallet, client)
 print(my_tx_payment_signed)
 # Payment(
 #     account='rMPUKmzmDWEX1tQhzQ8oGFNfAEhnWNFwz',
 #     transaction_type=<TransactionType.PAYMENT: 'Payment'>,
 #     fee='10',
 #     sequence=16034065,
 #     account_txn_id=None,
@@ -267,26 +266,26 @@
 #     invoice_id=None,
 #     paths=None,
 #     send_max=None,
 #     deliver_min=None
 # )
 
 # submit the transaction
-tx_response = submit_and_wait(my_tx_payment_signed, client)
+tx_response = send_reliable_submission(my_tx_payment_signed, client)
 ```
 
 
 ### Subscribe to ledger updates
 
 You can send `subscribe` and `unsubscribe` requests only using the WebSocket network client. These request methods allow you to be alerted of certain situations as they occur, such as when a new ledger is declared.
 
 ```py
 from xrpl.clients import WebsocketClient
 url = "wss://s.altnet.rippletest.net/"
-from xrpl.models import Subscribe, StreamParameter
+from xrpl.models.requests import Subscribe, StreamParameter
 req = Subscribe(streams=[StreamParameter.LEDGER])
 # NOTE: this code will run forever without a timeout, until the process is killed
 with WebsocketClient(url) as client:
     client.send(req)
     for message in client:
         print(message)
 # {'result': {'fee_base': 10, 'fee_ref': 10, 'ledger_hash': '7CD50477F23FF158B430772D8E82A961376A7B40E13C695AA849811EDF66C5C0', 'ledger_index': 18183504, 'ledger_time': 676412962, 'reserve_base': 20000000, 'reserve_inc': 5000000, 'validated_ledgers': '17469391-18183504'}, 'status': 'success', 'type': 'response'}
@@ -301,37 +300,40 @@
 This library supports Python's [`asyncio`](https://docs.python.org/3/library/asyncio.html) package, which is used to run asynchronous code. All the async code is in [`xrpl.asyncio`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.asyncio.html) If you are writing asynchronous code, please note that you will not be able to use any synchronous sugar functions, due to how event loops are handled. However, every synchronous method has a corresponding asynchronous method that you can use.
 
 This sample code is the asynchronous equivalent of the above section on submitting a transaction.
 
 ```py
 import asyncio
 from xrpl.models.transactions import Payment
-from xrpl.asyncio.transaction import sign, submit_and_wait
+from xrpl.asyncio.transaction import sign, send_reliable_submission
 from xrpl.asyncio.ledger import get_latest_validated_ledger_sequence
 from xrpl.asyncio.account import get_next_valid_seq_number
 from xrpl.asyncio.clients import AsyncJsonRpcClient
 
 async_client = AsyncJsonRpcClient(JSON_RPC_URL)
 
 async def submit_sample_transaction():
     current_validated_ledger = await get_latest_validated_ledger_sequence(async_client)
 
     # prepare the transaction
     # the amount is expressed in drops, not XRP
     # see https://xrpl.org/basic-data-types.html#specifying-currency-amounts
     my_tx_payment = Payment(
-        account=test_wallet.address,
+        account=test_wallet.classic_address,
         amount="2200000",
         destination="rPT1Sjq2YGrBMTttX4GZHjKu9dyfzbpAYe",
         last_ledger_sequence=current_validated_ledger + 20,
-        sequence=await get_next_valid_seq_number(test_wallet.address, async_client),
+        sequence=await get_next_valid_seq_number(test_wallet.classic_address, async_client),
         fee="10",
     )
-    # sign and submit the transaction
-    tx_response = await submit_and_wait(my_tx_payment_signed, async_client, test_wallet)
+    # sign the transaction
+    my_tx_payment_signed = await sign(my_tx_payment,test_wallet)
+
+    # submit the transaction
+    tx_response = await send_reliable_submission(my_tx_payment_signed, async_client)
 
 asyncio.run(submit_sample_transaction())
 ```
 
 ### Encode addresses
 
 Use [`xrpl.core.addresscodec`](https://xrpl-py.readthedocs.io/en/stable/source/xrpl.core.addresscodec.html) to encode and decode addresses into and from the ["classic" and X-address formats](https://xrpl.org/accounts.html#addresses).
@@ -353,26 +355,22 @@
 
 ## Contributing
 
 If you want to contribute to this project, see [CONTRIBUTING.md].
 
 ### Mailing Lists
 
-We have a low-traffic mailing list for announcements of new `xrpl-py` releases. (About 1 email per week)
+We have a low-traffic mailing list for announcements of new `xrpl.js` releases. (About 1 email per week)
 
 + [Subscribe to xrpl-announce](https://groups.google.com/g/xrpl-announce)
 
 If you're using the XRP Ledger in production, you should run a [rippled server](https://github.com/ripple/rippled) and subscribe to the ripple-server mailing list as well.
 
 + [Subscribe to ripple-server](https://groups.google.com/g/ripple-server)
 
-### Code Samples
-- For samples of common use cases, see the [XRPL.org Code Samples](https://xrpl.org/code-samples.html) page.
-- You can also browse those samples [directly on GitHub](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples).
-
 ### Report an issue
 
 Experienced an issue? Report it [here](https://github.com/XRPLF/xrpl-py/issues/new).
 
 ## License
 
 The `xrpl-py` library is licensed under the ISC License. See [LICENSE] for more information.
```

