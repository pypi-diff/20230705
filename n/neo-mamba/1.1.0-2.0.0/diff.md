# Comparing `tmp/neo-mamba-1.1.0.tar.gz` & `tmp/neo-mamba-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-mamba-1.1.0.tar", last modified: Mon Mar  6 14:28:14 2023, max compression
+gzip compressed data, was "neo-mamba-2.0.0.tar", last modified: Wed Jul  5 17:21:02 2023, max compression
```

## Comparing `neo-mamba-1.1.0.tar` & `neo-mamba-2.0.0.tar`

### file list

```diff
@@ -1,165 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.913956 neo-mamba-1.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.921956 neo-mamba-1.1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/advanced.md
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/home.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/mamba-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/smart-contracts.md
--rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/docs/source/wrapper-hierarchy.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.913956 neo-mamba-1.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.921956 neo-mamba-1.1.0/examples/shared/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/coz-wallet.json
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/default.neo-express
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.925956 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v1.nef
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v2.nef
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.925956 neo-mamba-1.1.0/examples/shared/nep11-token/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/compile_instructions.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/go.mod
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/go.sum
--rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/nep11-token.manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/nep11-token.nef
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/nft.go
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep11-token/nft.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.925956 neo-mamba-1.1.0/examples/shared/nep17-token/
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.nef
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/register-candidate.invoke
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/setup-neoxp-for-tests.batch
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/examples/shared/user-wallet.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.925956 neo-mamba-1.1.0/neo3/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.925956 neo-mamba-1.1.0/neo3/api/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.929956 neo-mamba-1.1.0/neo3/api/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/helpers/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/helpers/txbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/helpers/unwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    45432 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/noderpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    55075 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.929956 neo-mamba-1.1.0/neo3/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/callflags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/findoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/nef.py
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/contracts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.929956 neo-mamba-1.1.0/neo3/core/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.929956 neo-mamba-1.1.0/neo3/core/cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/cryptography/bloomfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/cryptography/ecc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/cryptography/merkletree.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.929956 neo-mamba-1.1.0/neo3/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/types/uint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.933956 neo-mamba-1.1.0/neo3/network/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.933956 neo-mamba-1.1.0/neo3/network/convenience/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/flightinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/nodeweight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/requestinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/convenience/syncmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/ipfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/message.py
--rw-r--r--   0 runner    (1001) docker     (123)    27799 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.937956 neo-mamba-1.1.0/neo3/network/payloads/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/address.py
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/consensus.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/extensible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    27420 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/payloads/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/network/relaycache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    23223 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.937956 neo-mamba-1.1.0/neo3/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26642 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/scrypt_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/neo3/wallet/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.937956 neo-mamba-1.1.0/neo_mamba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-06 14:28:14.000000 neo-mamba-1.1.0/neo_mamba.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.937956 neo-mamba-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.941956 neo-mamba-1.1.0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/api/test_noderpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.941956 neo-mamba-1.1.0/tests/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_callflags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_contractstate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_nef.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/contracts/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.941956 neo-mamba-1.1.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/test_biginteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/test_cryptography.py
--rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/core/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/tests/network/convenience/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/convenience/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/convenience/test_nodemanager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/convenience/test_syncmanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/convenience/test_various.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_ipfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    61223 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/network/test_witnessrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:28:14.945956 neo-mamba-1.1.0/tests/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/wallet/rc2-wallet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/wallet/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-03-06 14:27:53.000000 neo-mamba-1.1.0/tests/wallet/test_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.726175 neo-mamba-2.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.730175 neo-mamba-2.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/advanced.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14449 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/mamba-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/smart-contracts.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26776 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/docs/source/wrapper-hierarchy.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.730175 neo-mamba-2.0.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/coz-wallet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/default.neo-express
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.nef
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.nef
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/nep11-token/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/compile_instructions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/go.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/go.sum
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2042 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1756 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.nef
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nft.go
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep11-token/nft.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/examples/shared/nep17-token/
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.nef
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/register-candidate.invoke
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/setup-neoxp-for-tests.batch
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/examples/shared/user-wallet.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/neo3/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.734175 neo-mamba-2.0.0/neo3/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/api/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/txbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/helpers/unwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45820 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/noderpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56625 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/callflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/findoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/nef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/contracts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/bloomfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/cryptography/merkletree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21193 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/types/uint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.738175 neo-mamba-2.0.0/neo3/network/convenience/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/flightinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/nodeweight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/requestinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13641 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/convenience/syncmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/ipfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo3/network/payloads/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/consensus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/extensible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27818 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/payloads/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/network/relaycache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26371 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo3/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27088 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/scrypt_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15843 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/neo3/wallet/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/neo_mamba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 17:21:02.000000 neo-mamba-2.0.0/neo_mamba.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 17:21:02.750176 neo-mamba-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.742175 neo-mamba-2.0.0/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/test_noderpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_callflags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11690 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_contractstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_nef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/contracts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_biginteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_cryptography.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/core/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/network/convenience/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_nodemanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_syncmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/convenience/test_various.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_ipfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61223 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10247 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/network/test_witnessrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:21:02.746176 neo-mamba-2.0.0/tests/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/rc2-wallet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-05 17:20:46.000000 neo-mamba-2.0.0/tests/wallet/test_wallet.py
```

### Comparing `neo-mamba-1.1.0/CHANGELOG.rst` & `neo-mamba-2.0.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/LICENSE.md` & `neo-mamba-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/Makefile` & `neo-mamba-2.0.0/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.PHONY: black build clean clean-test clean-pyc clean-build docs help test coverage version-major version-minor version-patch
+.PHONY: black build clean clean-test clean-pyc clean-build clean-docs docs docs-deploy help test coverage version-major version-minor version-patch
 .DEFAULT_GOAL := help
 define BROWSER_PYSCRIPT
 import os, webbrowser, sys
 try:
 	from urllib import pathname2url
 except:
 	from urllib.request import pathname2url
@@ -22,24 +22,27 @@
 endef
 export PRINT_HELP_PYSCRIPT
 BROWSER := python3 -c "$$BROWSER_PYSCRIPT"
 
 help:
 	@python3 -c "$$PRINT_HELP_PYSCRIPT" < $(MAKEFILE_LIST)
 
-clean: clean-build clean-pyc clean-test ## remove all build, test, coverage and Python artifacts
+clean: clean-build clean-pyc clean-test clean-docs ## remove all build, test, coverage and Python artifacts
 
 
 clean-build: ## remove build artifacts
 	rm -rf build/
 	rm -rf dist/
 	rm -rf .eggs/
 	find . -name '*.egg-info' -exec rm -fr {} +
 	find . -name '*.egg' -exec rm -f {} +
 
+clean-docs: ## clean the /docs/
+	rm -rf docs/site/
+
 clean-pyc: ## remove Python file artifacts
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 	find . -name '__pycache__' -exec rm -fr {} +
 
 clean-test: ## remove test and coverage artifacts
@@ -51,21 +54,21 @@
 
 coverage: ## check code coverage quickly with the default Python
 	coverage run -m unittest discover -v -s tests/
 	coverage report
 	coverage html
 	$(BROWSER) htmlcov/index.html
 
-clean-docs: ## clean the /docs/
-	cd docs && $(MAKE) clean
-
 docs: ## generate Sphinx HTML documentation, including API docs
-	rm -rf docs/build/
-	sphinx-build -b html docs/source/ docs/build/
-	$(BROWSER) docs/build/index.html
+	rm -rf docs/site/
+	mkdocs build -f docs/mkdocs.yml
+	$(BROWSER) docs/site/index.html
+
+docs-deploy: ## manually deploy the docs to github pages
+	aws s3 sync ./docs/site  s3://docs-coz/neo3/mamba --acl public-read
 
 type: ## perform static type checking using mypy
 	mypy neo3/
 
 black: ## apply black formatting
 	black neo3/ examples/ tests/
 
@@ -75,8 +78,8 @@
 version-major: ## bump the major version prior to release, auto commits and tag
 	bumpversion major
 
 version-minor: ## bump the minor version prior to release, auto commits and tag
 	bumpversion minor
 
 version-patch: ## bump the patch version prior to release, auto commits and tag
-	bumpversion patch
+	bumpversion patch
```

### Comparing `neo-mamba-1.1.0/PKG-INFO` & `neo-mamba-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: neo-mamba
-Version: 1.1.0
+Version: 2.0.0
 Summary: Python SDK for the NEO 3 blockchain
 Home-page: https://github.com/CityOfZion/neo-mamba
 Author: Erik van den Brink
 Author-email: erik@coz.io
 Maintainer: Erik van den Brink
 Maintainer-email: erik@coz.io
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ==3.10.*
+Requires-Python: <=3.12,>=3.10.0
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 .. image:: .github/resources/images/logo.png
     :width: 400 px
@@ -59,19 +59,26 @@
 
 Please report any issues on `Github <https://github.com/CityOfZion/neo-mamba/issues>`_ or submit ideas how to improve the SDK.
 
 Also check out our Python smart contract compiler `Boa <https://github.com/CityOfZion/neo3-boa>`_ !
 
 Installation and usage
 ----------------------
-Installation instructions, how to interact with smart contrats as well as API reference documentation can be found at
+Installation instructions, how to interact with smart contracts as well as API reference documentation can be found at
 https://mamba.coz.io/
 
 Developing or contributing
 --------------------------
 Install the requirements, modify the code and PR :-)
 ::
 
    pip install -e .[dev]
 
-The project uses `Black <https://github.com/psf/black>`_ for code formatting. You might want to
-`integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ this into your editor.
+For larger changes consider opening an issue first to discuss the change. Below are a few guidelines for contributing
+
+* The project uses `Black <https://github.com/psf/black>`_ for code formatting. PRs will fail if formatted incorrectly.
+  You might want to `integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ `black` into your
+  editor or run it manually with `make black`.
+* All public functions/classes must have docstrings.
+* All your code must be typed. Test your typing with `make type`. In rare cases it might be hard/impractical to add typing.
+  Point it out if that is the case and add a short description why we could do without.
+* Add tests that cover the newly added (or changed if applicable) code. Use `make test` and `make coverage`.
```

### Comparing `neo-mamba-1.1.0/README.rst` & `neo-mamba-2.0.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -38,19 +38,26 @@
 
 Please report any issues on `Github <https://github.com/CityOfZion/neo-mamba/issues>`_ or submit ideas how to improve the SDK.
 
 Also check out our Python smart contract compiler `Boa <https://github.com/CityOfZion/neo3-boa>`_ !
 
 Installation and usage
 ----------------------
-Installation instructions, how to interact with smart contrats as well as API reference documentation can be found at
+Installation instructions, how to interact with smart contracts as well as API reference documentation can be found at
 https://mamba.coz.io/
 
 Developing or contributing
 --------------------------
 Install the requirements, modify the code and PR :-)
 ::
 
    pip install -e .[dev]
 
-The project uses `Black <https://github.com/psf/black>`_ for code formatting. You might want to
-`integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ this into your editor.
+For larger changes consider opening an issue first to discuss the change. Below are a few guidelines for contributing
+
+* The project uses `Black <https://github.com/psf/black>`_ for code formatting. PRs will fail if formatted incorrectly.
+  You might want to `integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ `black` into your
+  editor or run it manually with `make black`.
+* All public functions/classes must have docstrings.
+* All your code must be typed. Test your typing with `make type`. In rare cases it might be hard/impractical to add typing.
+  Point it out if that is the case and add a short description why we could do without.
+* Add tests that cover the newly added (or changed if applicable) code. Use `make test` and `make coverage`.
```

### Comparing `neo-mamba-1.1.0/docs/source/faq.md` & `neo-mamba-2.0.0/docs/source/faq.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/docs/source/getting-started.md` & `neo-mamba-2.0.0/docs/source/getting-started.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,19 +9,14 @@
 Let's get setup and get a little taste of what using it looks like before diving into how it is structured and how to
 work with it to achieve your goals.
 
 ## Requirements
 * Python 3.10
 * Linux, OSX or Windows
 
-!!! note
-
-    ARM based platforms (e.g. Mac with M1 chip) are not supported due to native extensions
-    the project relies on. Not all of those have M1 supported binaries (yet). 
-
 ## Installation
 
 === "UNIX"
     ```linenums="0"
     pip install neo-mamba
     ```
 === "Windows"
```

### Comparing `neo-mamba-1.1.0/docs/source/home.html` & `neo-mamba-2.0.0/docs/source/home.html`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/docs/source/mamba-logo.png` & `neo-mamba-2.0.0/docs/source/mamba-logo.png`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/docs/source/smart-contracts.md` & `neo-mamba-2.0.0/docs/source/smart-contracts.md`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/docs/source/wrapper-hierarchy.png` & `neo-mamba-2.0.0/docs/source/wrapper-hierarchy.png`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/__init__.py` & `neo-mamba-2.0.0/examples/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/coz-wallet.json` & `neo-mamba-2.0.0/examples/shared/coz-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/default.neo-express` & `neo-mamba-2.0.0/examples/shared/default.neo-express`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json` & `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v1.py` & `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v1.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json` & `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/deploy-update-destroy/contract_v2.py` & `neo-mamba-2.0.0/examples/shared/deploy-update-destroy/contract_v2.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep11-token/nep11-token.manifest.json` & `neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep11-token/nep11-token.nef` & `neo-mamba-2.0.0/examples/shared/nep11-token/nep11-token.nef`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep11-token/nft.go` & `neo-mamba-2.0.0/examples/shared/nep11-token/nft.go`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep11-token/nft.yml` & `neo-mamba-2.0.0/examples/shared/nep11-token/nft.yml`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.manifest.json` & `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.manifest.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.nef` & `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.nef`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/nep17-token/nep17token.py` & `neo-mamba-2.0.0/examples/shared/nep17-token/nep17token.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/examples/shared/user-wallet.json` & `neo-mamba-2.0.0/examples/shared/user-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/api/helpers/signing.py` & `neo-mamba-2.0.0/neo3/api/helpers/signing.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,7 +59,30 @@
         tx: transaction.Transaction, details: SigningDetails
     ):
         # call some remote API to get the signature
         # and add a witness with the signature
         raise NotImplementedError
 
     return remote_server_signer
+
+
+def sign_insecure_with_multisig_account(
+    acc: account.Account, password: str
+) -> SigningFunction:
+    """
+    Sign and add a multi-signature witness.
+
+    This only works for a 1 out of n multi-signature account.
+
+    Args:
+        acc: a multi-signature account
+        password: the password of the account to sign with
+    """
+
+    async def insecure_account_signer(
+        tx: transaction.Transaction, details: SigningDetails
+    ):
+        ctx = account.MultiSigContext()
+        # this will automatically add a witness
+        acc.sign_multisig_tx(tx, password, ctx, details.network)
+
+    return insecure_account_signer
```

### Comparing `neo-mamba-1.1.0/neo3/api/helpers/txbuilder.py` & `neo-mamba-2.0.0/neo3/api/helpers/txbuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
             # adding a witness(es) so we can calculate the network fee
             for _ in range(len(self.tx.signers)):
                 self.tx.witnesses.append(TxBuilder._dummy_signing_witness())
             self.tx.network_fee = await self.client.calculate_network_fee(self.tx)
             # removing it here as it will be replaced by a proper one once we're signing
             self.tx.witnesses = []
         else:
+            if len(self.tx.signers) == 0:
+                raise ValueError("Cannot calculate network fee without signers")
             self.tx.network_fee = await self.client.calculate_network_fee(self.tx)
 
     @staticmethod
     def _dummy_signing_witness() -> verification.Witness:
         """single signature account witness"""
         acc = account.Account.create_new("abc")
         if acc.contract is None:
```

### Comparing `neo-mamba-1.1.0/neo3/api/helpers/unwrap.py` & `neo-mamba-2.0.0/neo3/api/helpers/unwrap.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,15 +140,16 @@
     """
     Convert the stack item at `idx` to a dictionary.
 
     Args:
         res: execution result.
         idx: idx: the index in the result stack to fetch the stack item from.
 
-    Returns:
+    Raises:
+        ValueError: if the index is out of range, or the value cannot be converted to a dict.
 
     """
     return item(res, idx).as_dict()
 
 
 def as_none(res: noderpc.ExecutionResult, idx: int = 0) -> None:
     """
@@ -160,14 +161,29 @@
 
     Raises:
         ValueError: if the index is out of range, or the value is not `None`.
     """
     return item(res, idx).as_none()
 
 
+def as_bytes(res: noderpc.ExecutionResult, idx: int = 0) -> bytes:
+    """
+    Convert the stack item at `idx` to `bytes`.
+
+    Args:
+        res: execution result.
+        idx: the index in the result stack to fetch the stack item from.
+
+    Raises:
+        ValueError: if the index is out of range, or the value cannot be converted to bytes.
+
+    """
+    return item(res, idx).as_bytes()
+
+
 def item(res: noderpc.ExecutionResult, idx: int = 0) -> noderpc.StackItem:
     """
     Fetch the stack item at `idx` from the result stack. Performs basic validation and bounds checking.
 
     Args:
         res: execution result.
         idx: the index in the result stack to fetch the stack item from.
```

### Comparing `neo-mamba-1.1.0/neo3/api/noderpc.py` & `neo-mamba-2.0.0/neo3/api/noderpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,27 @@
         """
         if self.type != StackItemType.BOOL:
             raise ValueError(
                 f"item is not of type '{StackItemType.BOOL}' but of type '{self.type}'"
             )
         return self.value
 
+    def as_bytes(self) -> bytes:
+        """
+        Unwrap as `bool`.
+
+        Raises:
+            ValueError: if internal item type does not match required.
+        """
+        if self.type != StackItemType.BYTE_STRING:
+            raise ValueError(
+                f"item is not of type '{StackItemType.BYTE_STRING}' but of type '{self.type}'"
+            )
+        return self.value
+
     def as_str(self) -> str:
         """
         Unwrap as `str`.
 
         Raises:
             ValueError: if internal item type does not match required.
         """
```

### Comparing `neo-mamba-1.1.0/neo3/api/wrappers.py` & `neo-mamba-2.0.0/neo3/api/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,15 +356,31 @@
             else:
                 await builder.calculate_system_fee()
                 builder.tx.system_fee += append_system_fee
 
             if network_fee > 0:
                 builder.tx.network_fee = network_fee
             else:
+                # calculate network fee has a chicken/egg problem for light wallet sdk's.
+                # in order to calculate the right network fees (especially multisig) the witnesses have to be constructed
+                # which is done in `build_and_sign()`.
+                # at the same time `network_fee` is part of the signed data.
+                # So here we call build_and_sign() just for creating the witnesses, then calculate the real fee (which will
+                # reset the witnesses) and then at the end of the function we build_and_sign() again to have a valid
+                # signature over the right network_fee
+
+                # if there were no witnesses prior to signging, then we should restore that after the tmp signing
+                reset_witnesses = len(builder.tx.witnesses) == 0
+                builder.tx.network_fee = 999
+                await builder.build_and_sign()
                 await builder.calculate_network_fee()
+
+                if reset_witnesses:
+                    builder.tx.witnesses = []
+
                 builder.tx.network_fee += append_network_fee
 
             tx = await builder.build_and_sign()
             return await client.send_transaction(tx)
 
     async def invoke_raw(
         self,
@@ -628,21 +644,21 @@
 
 
 class GenericContract:
     """
     Generic class to call arbitrary methods on a smart contract.
     """
 
-    def __init__(self, contract_hash):
+    def __init__(self, contract_hash: types.UInt160):
         self.hash = contract_hash
 
     def call_function(
         self,
         name,
-        args: Optional[Sequence] = None,
+        args: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[noderpc.ExecutionResult]:
         """
         Call a method on the contract.
 
         Args:
             name: the method name to call as defined in the manifest.
             args: optional list of arguments the function expects.
@@ -656,15 +672,15 @@
         return ContractMethodResult(script)
 
     def update(
         self,
         update_method: str = "update",
         nef: Optional[nef.NEF] = None,
         manifest: Optional[manifest.ContractManifest] = None,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[None]:
         """
         Update this contract on chain with a new manifest and/or contract (NEF).
 
         Assumes the update method on the contract uses the standard arguments; nef, manifest and (optional) data.
         If it uses custom arguments use `call_function` instead.
 
@@ -699,15 +715,15 @@
         sb = vm.ScriptBuilder().emit_contract_call(self.hash, destroy_method)
         return ContractMethodResult(sb.to_array(), unwrap.as_none)
 
     @staticmethod
     def deploy(
         nef: nef.NEF,
         manifest: manifest.ContractManifest,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[types.UInt160]:
         """
         Deploy a smart contract to the chain.
 
         Args:
             nef: compiled contract.
             manifest: contract manifest file.
@@ -814,15 +830,15 @@
         return ContractMethodResult(sb.to_array(), process)
 
     def transfer(
         self,
         source: types.UInt160 | NeoAddress,
         destination: types.UInt160 | NeoAddress,
         amount: int,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[bool]:
         """
         Transfer `amount` of tokens from `source` account to `destination` account.
         Forward `data` to `onNEP17Payment` handler if applicable.
 
         For this to pass while using `test_invoke()`, make sure to add a Signer with a script hash equal to the source
         account. i.e.
@@ -843,51 +859,51 @@
         destination = _check_address_and_convert(destination)
 
         sb = vm.ScriptBuilder().emit_contract_call_with_args(
             self.hash, "transfer", [source, destination, amount, data]
         )
         return ContractMethodResult(sb.to_array(), unwrap.as_bool)
 
-    def transfer_friendly(self, source, dest, amount):
+    def transfer_friendly(
+        self, source, dest, amount, data: Optional[noderpc.ContractParameter] = None
+    ):
         """
         Transfer `amount` of tokens from `source` account to `destination` account.
 
         Same as `transfer` but does not require manually convert amount if the token uses decimals.
 
         Returns:
             The return value after invoking with `invoke()` or `test_invoke()` is
                 `True` if the token transferred successful.
                 `False` otherwise.
         """
         sb = vm.ScriptBuilder()
-        sb.emit_push(None)  # data
+        sb.emit_push(data)
         sb.emit_push(10)  # multiplier base
         sb.emit_contract_call(self.hash, "decimals")
         sb.emit(vm.OpCode.POW)
         sb.emit_push(amount)
         sb.emit(vm.OpCode.MUL)
         sb.emit_push(dest)
         sb.emit_push(source)
         sb.emit_push(4)
         sb.emit(vm.OpCode.PACK)
         sb.emit_push(callflags.CallFlags.ALL)
         sb.emit_push("transfer")
         sb.emit_push(self.hash)
         sb.emit_syscall(vm.Syscalls.SYSTEM_CONTRACT_CALL)
 
-        for b in sb.to_array():
-            print(f"{hex(b)},", end="")
         return ContractMethodResult(sb.to_array(), unwrap.as_bool)
 
     def transfer_multi(
         self,
         source: types.UInt160 | NeoAddress,
         destinations: Sequence[types.UInt160 | NeoAddress],
         amount: int,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
         abort_on_failure: bool = False,
     ) -> ContractMethodResult[bool]:
         """
         Transfer `amount` of tokens from `source` to each account in `destinations`.
 
         Args:
             source: account to take funds from.
@@ -1177,28 +1193,32 @@
 
         def process(res: noderpc.ExecutionResult, _: int = 0) -> list[bytes]:
             raw_results: list[noderpc.StackItem] = unwrap.as_list(res)
             return [si.value for si in raw_results]
 
         return ContractMethodResult(sb.to_array(), process)
 
-    def tokens(self) -> ContractMethodResult[list[bytes]]:
+    def tokens(self, limit: int = 2000) -> ContractMethodResult[list[bytes]]:
         """
         Get all tokens minted by the contract.
 
+        limit: the maximum tokens to return. Note: there is a limit on the virtual machine (default: 2048) to avoid too
+        much compute being used. The limit is set slightly lower on purpose to allow other necessary items in the VM.
+        If the contract returns more items you'll have to resort to retrieving them using RPC Session Iterators.
+
         Note:
             This is an optional method and may not exist on the contract.
         """
 
         def process(res: noderpc.ExecutionResult, _: int = 0) -> list[bytes]:
             raw_results: list[noderpc.StackItem] = unwrap.as_list(res)
             return [si.value for si in raw_results]
 
         sb = vm.ScriptBuilder().emit_contract_call_and_unwrap_iterator(
-            self.hash, "tokens"
+            self.hash, "tokens", unwrap_limit=limit
         )
         return ContractMethodResult(sb.to_array(), process)
 
     def properties(self, token_id: bytes) -> ContractMethodResult[dict]:
         """
         Get all properties for the given NFT.
 
@@ -1220,15 +1240,15 @@
 
     def transfer(
         self,
         source: types.UInt160 | NeoAddress,
         destination: types.UInt160 | NeoAddress,
         amount: int,
         token_id: bytes,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[bool]:
         """
         Transfer `amount` of `token_id` from `source` account to `destination` account.
 
         For this to pass while using `test_invoke()`, make sure to add a Signer with a script hash equal to the source
         account. i.e.
 
@@ -1311,15 +1331,15 @@
 class NEP11NonDivisibleContract(_NEP11Contract):
     """Base class for non-divisible NFTs."""
 
     def transfer(
         self,
         destination: types.UInt160 | NeoAddress,
         token_id: bytes,
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
     ) -> ContractMethodResult[bool]:
         """
         Transfer `token_id` to `destination` account.
         The source account will be the account that pays for the fees (a.k.a. the transaction.sender).
 
         For this to pass while using `test_invoke()`, make sure to add a Signer with a script hash equal to the source
         account. i.e.
@@ -1341,15 +1361,15 @@
         )
         return ContractMethodResult(sb.to_array(), unwrap.as_bool)
 
     def transfer_multi(
         self,
         destinations: Sequence[types.UInt160 | NeoAddress],
         token_ids: list[bytes],
-        data: Optional[list] = None,
+        data: Optional[noderpc.ContractParameter] = None,
         abort_on_failure: bool = False,
     ) -> ContractMethodResult[bool]:
         """
         Transfer multiple token_ids to multiple destinations. Destination and token_ids are paired in order.
 
         Args:
             destinations: accounts to send tokens to.
```

### Comparing `neo-mamba-1.1.0/neo3/contracts/abi.py` & `neo-mamba-2.0.0/neo3/contracts/abi.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/contracts/callflags.py` & `neo-mamba-2.0.0/neo3/contracts/callflags.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/contracts/contract.py` & `neo-mamba-2.0.0/neo3/contracts/contract.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/contracts/manifest.py` & `neo-mamba-2.0.0/neo3/contracts/manifest.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/contracts/nef.py` & `neo-mamba-2.0.0/neo3/contracts/nef.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/contracts/utils.py` & `neo-mamba-2.0.0/neo3/contracts/utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/cryptography/__init__.py` & `neo-mamba-2.0.0/neo3/core/cryptography/__init__.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/cryptography/bloomfilter.py` & `neo-mamba-2.0.0/neo3/core/cryptography/bloomfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/cryptography/ecc.py` & `neo-mamba-2.0.0/neo3/core/cryptography/ecc.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/cryptography/merkletree.py` & `neo-mamba-2.0.0/neo3/core/cryptography/merkletree.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/serialization.py` & `neo-mamba-2.0.0/neo3/core/serialization.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/types/uint.py` & `neo-mamba-2.0.0/neo3/core/types/uint.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/core/utils.py` & `neo-mamba-2.0.0/neo3/core/utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/capabilities.py` & `neo-mamba-2.0.0/neo3/network/capabilities.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/convenience/flightinfo.py` & `neo-mamba-2.0.0/neo3/network/convenience/flightinfo.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/convenience/nodemanager.py` & `neo-mamba-2.0.0/neo3/network/convenience/nodemanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/convenience/nodeweight.py` & `neo-mamba-2.0.0/neo3/network/convenience/nodeweight.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/convenience/requestinfo.py` & `neo-mamba-2.0.0/neo3/network/convenience/requestinfo.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/convenience/syncmanager.py` & `neo-mamba-2.0.0/neo3/network/convenience/syncmanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/ipfilter.py` & `neo-mamba-2.0.0/neo3/network/ipfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/message.py` & `neo-mamba-2.0.0/neo3/network/message.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/node.py` & `neo-mamba-2.0.0/neo3/network/node.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/address.py` & `neo-mamba-2.0.0/neo3/network/payloads/address.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/block.py` & `neo-mamba-2.0.0/neo3/network/payloads/block.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/consensus.py` & `neo-mamba-2.0.0/neo3/network/payloads/consensus.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/extensible.py` & `neo-mamba-2.0.0/neo3/network/payloads/extensible.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/filter.py` & `neo-mamba-2.0.0/neo3/network/payloads/filter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/inventory.py` & `neo-mamba-2.0.0/neo3/network/payloads/inventory.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/ping.py` & `neo-mamba-2.0.0/neo3/network/payloads/ping.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/transaction.py` & `neo-mamba-2.0.0/neo3/network/payloads/transaction.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/verification.py` & `neo-mamba-2.0.0/neo3/network/payloads/verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,23 +416,34 @@
         return conditions
 
     @staticmethod
     def _deserialize_from(
         reader: serialization.BinaryReader, max_nesting_depth: int
     ) -> WitnessCondition:
         condition_type = reader.read_uint8()
-        for sub in WitnessCondition.__subclasses__():
-            child = sub._serializable_init()  # type: ignore
-            if child.type.value == condition_type:
-                child._deserialize_without_type(reader, max_nesting_depth)
-                return child
-        else:
+
+        def find_condition(condition) -> Optional[WitnessCondition]:
+            for sub in condition.__subclasses__():
+                child = sub._serializable_init()
+                if child.type.value == condition_type:
+                    child._deserialize_without_type(reader, max_nesting_depth)
+                    return child
+                if len(sub.__subclasses__()) > 0:
+                    condition = find_condition(sub)
+                    if condition is not None:
+                        return condition
+            return None
+
+        condition = find_condition(WitnessCondition)
+        if condition is None:
             raise ValueError(
-                f"Deserialization error - unknown witness condition. Type: {condition_type}"
+                f"Deserialization error - unknown witness condition. Type: {hex(condition_type)}"
             )
+        else:
+            return condition
 
     def to_json(self) -> dict:
         """Convert object into JSON representation."""
         return {"type": self.type.to_csharp_string()}
 
     @classmethod
     def from_json(cls, json: dict):
```

### Comparing `neo-mamba-1.1.0/neo3/network/payloads/version.py` & `neo-mamba-2.0.0/neo3/network/payloads/version.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/network/relaycache.py` & `neo-mamba-2.0.0/neo3/network/relaycache.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/settings.py` & `neo-mamba-2.0.0/neo3/settings.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/singleton.py` & `neo-mamba-2.0.0/neo3/singleton.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/vm.py` & `neo-mamba-2.0.0/neo3/vm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 NEO Virtual Machine classes.
 """
 from __future__ import annotations
 import hashlib
 from enum import IntEnum
 from neo3.contracts import callflags
-from neo3.core import types, serialization
-from typing import Optional, Iterator
+from neo3.core import types, serialization, cryptography
+from typing import Optional, Iterator, Union, Type, Protocol
 from collections.abc import Sequence
 
 
 def _syscall_name_to_int(name: str) -> int:
     return int.from_bytes(
         hashlib.sha256(name.encode()).digest()[:4], "little", signed=False
     )
@@ -246,14 +246,62 @@
             return other + self.value.to_bytes(1, "little")
         elif isinstance(other, OpCode):
             return other.to_bytes(1, "little") + self.value.to_bytes(1, "little")
         else:
             return super(OpCode, self).__radd__(other)
 
 
+ContractParameter = Union[
+    bool,
+    int,
+    str,
+    bytes,
+    bytearray,
+    types.BigInteger,
+    types.UInt160,
+    types.UInt256,
+    cryptography.ECPoint,
+    "ContractParameterArray",
+    "ContractParameterDict",
+    Type[serialization.ISerializable_T],
+]
+
+
+class ContractParameterArray(Protocol):
+    """"""
+
+    def insert(self, index: int, value: ContractParameter) -> None:
+        ...
+
+    def __getitem__(self, i: int) -> ContractParameter:
+        ...
+
+    def __setitem__(self, i: int, o: ContractParameter) -> None:
+        ...
+
+    def __delitem__(self, i: int) -> None:
+        ...
+
+
+class ContractParameterDict(Protocol):
+    """"""
+
+    def __setitem__(self, k: ContractParameter, v: ContractParameter) -> None:
+        ...
+
+    def __delitem__(self, v: ContractParameter) -> None:
+        ...
+
+    def __getitem__(self, k: ContractParameter) -> ContractParameter:
+        ...
+
+    def __iter__(self) -> Iterator[ContractParameter]:
+        ...
+
+
 class ScriptBuilder:
     """
     A utility class to create scripts (sequence of opcodes) that can be executed by the
     NEO Virtual Machine.
     """
 
     def __init__(self):
@@ -327,20 +375,33 @@
                 self.emit_raw(value)
             else:
                 self.emit(OpCode.PUSHDATA4)
                 self.emit_raw(len_value.to_bytes(4, "little"))
                 self.emit_raw(value)
             return self
         elif isinstance(value, Sequence):
-            self.emit(OpCode.NEWARRAY0)
-            for v in value:
-                self.emit(OpCode.DUP)
-                self.emit_push(v)
-                self.emit(OpCode.APPEND)
+            for item in reversed(value):
+                if isinstance(item, Sequence):
+                    self.emit_push(item)
+                    continue
+                self.emit_push(item)
+            self.emit_push(len(value))
+            self.emit(OpCode.PACK)
             return self
+        elif isinstance(value, dict):
+            for k, v in value.items():
+                # This restriction exists on the VM side where keys to a 'Map' may only be of 'PrimitiveType'
+                if not isinstance(k, (int, str, bool)):
+                    raise ValueError(
+                        f"Unsupported key type {type(k)}. Supported types by the VM are bool, int and str"
+                    )
+                self.emit_push(v)
+                self.emit_push(k)
+            self.emit_push(len(value))
+            return self.emit(OpCode.PACKMAP)
         else:
             raise ValueError(f"Unsupported value type {type(value)}")
 
     def emit_raw(self, data: bytes) -> ScriptBuilder:
         self.data.extend(data)
         return self
 
@@ -390,94 +451,117 @@
         self.emit_syscall(Syscalls.SYSTEM_CONTRACT_CALL)
         return self
 
     def emit_contract_call_with_args(
         self,
         script_hash: types.UInt160,
         operation: str,
-        args,
+        args: ContractParameter,
         call_flags: Optional[callflags.CallFlags] = None,
     ) -> ScriptBuilder:
         """
         Emit opcode sequence to call a smart contrat operation with arguments.
 
         Args:
             script_hash: contract script hash.
             operation: method to call on contract.
             args: parameters to pass to the `operation`.
             call_flags: call flags for the operation.
         """
-        for arg in reversed(args):
-            self.emit_push(arg)
-        self.emit_push(len(args))
-        self.emit(OpCode.PACK)
+        if isinstance(args, Sequence):
+            for arg in reversed(args):
+                self.emit_push(arg)
+            self.emit_push(len(args))
+            self.emit(OpCode.PACK)
+        else:
+            self.emit_push(args)
         self.emit_push(callflags.CallFlags.ALL if call_flags is None else call_flags)
         self.emit_push(operation)
         self.emit_push(script_hash)
         self.emit_syscall(Syscalls.SYSTEM_CONTRACT_CALL)
         return self
 
     def emit_contract_call_and_unwrap_iterator(
         self,
         script_hash,
         operation: str,
         call_flags: Optional[callflags.CallFlags] = None,
+        unwrap_limit: int = 2000,
     ) -> ScriptBuilder:
         return self._emit_contract_call_and_unwrap_iterator(
-            script_hash, operation, None, call_flags
+            script_hash, operation, None, call_flags, unwrap_limit
         )
 
     def emit_contract_call_with_args_and_unwrap_iterator(
         self,
         script_hash,
         operation: str,
-        args: list,
+        args: ContractParameter,
         call_flags: Optional[callflags.CallFlags] = None,
     ) -> ScriptBuilder:
         return self._emit_contract_call_and_unwrap_iterator(
             script_hash, operation, args, call_flags
         )
 
     def to_array(self) -> bytes:
         return bytes(self.data)
 
     def _emit_contract_call_and_unwrap_iterator(
         self,
         script_hash,
         operation: str,
-        args: Optional[list] = None,
+        args: Optional[ContractParameter] = None,
         call_flags: Optional[callflags.CallFlags] = None,
+        unwrap_limit: int = 2000,
     ) -> ScriptBuilder:
+        """
+
+        Args:
+            script_hash: contract hash to call
+            operation: method name to call
+            args: arguments passed to the method called
+            call_flags: call flags of the method called
+            unwrap_limit: maximum number of items to return. Can't be larger than the MaxStackSize limit configured for
+            the VM or it will throw an exception.
+            https://github.com/neo-project/neo-vm/blob/5b0a39811b34abacab1273f3ee5a9a9f7e52ac7b/src/Neo.VM/ExecutionEngineLimits.cs#L34C21-L34C33
+            The current default is slightly lower than the max, because that allows for a few other items to be on the
+            stack in other function frames.
+        """
         # jump to local variables initialization code
         self.emit_jump(OpCode.JMP, 4)
         # the following 2 instructions are for loading the result array and exiting the script
         # it is at the beginning because it make it easy to calculate the offset
         return_results = len(self.data)
         self.emit(OpCode.LDLOC0)
         self.emit(OpCode.RET)
         # reserve 2 local variables for the `iterator` and `results` list
         self.emit(OpCode.INITSLOT)
-        self.emit_raw(b"\x02")
+        self.emit_raw(b"\x03")
         self.emit_raw(b"\x00")
         # store results list in pos 0
         self.emit(OpCode.NEWARRAY0)
         self.emit(OpCode.STLOC0)
 
-        if args is None or len(args) == 0:
+        if args is None or (isinstance(args, Sequence) and len(args) == 0):
             self.emit_contract_call(script_hash, operation, call_flags)
         else:
             self.emit_contract_call_with_args(script_hash, operation, args, call_flags)
         # store iterator in pos 1
         self.emit(OpCode.STLOC1)
-
+        # store stack item counter in pos 2
+        self.emit_push(0)
+        self.emit(OpCode.STLOC2)
         """
         Next set of opcodes does the following
 
         while iterator.next()
           results.append(iterator.value)
+          ctr += 1
+          if ctr == stack_limit:
+            break
         return results
         """
         loop_start = len(self.data)
         # load iterator as argument for iterator.next
         self.emit(OpCode.LDLOC1)
         # test if the iterator has a value
         self.emit_syscall(Syscalls.SYSTEM_ITERATOR_NEXT)
@@ -488,14 +572,23 @@
         # get result
         self.emit_syscall(Syscalls.SYSTEM_ITERATOR_VALUE)
         # load array
         self.emit(OpCode.LDLOC0)
         # fix argument order for APPEND
         self.emit(OpCode.SWAP)
         self.emit(OpCode.APPEND)
+        # load stack item counter
+        self.emit(OpCode.LDLOC2)
+        self.emit(OpCode.INC)
+        self.emit(OpCode.DUP)
+        self.emit(OpCode.STLOC2)
+        # load stack item limit
+        self.emit_push(unwrap_limit)
+        self.emit(OpCode.NUMEQUAL)
+        self.emit_jump(OpCode.JMPIF, self._offset_to(return_results))
         # jump back to start of `while` loop
         self.emit_jump(OpCode.JMP, self._offset_to(loop_start))
         return self
 
     def _pad_right(self, data: bytearray, length: int, is_negative: bool):
         if len(data) >= length:
             return
```

### Comparing `neo-mamba-1.1.0/neo3/wallet/account.py` & `neo-mamba-2.0.0/neo3/wallet/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             },
         },
         "required": ["address", "label", "isDefault", "lock", "key", "extra"],
     }
 
     def __init__(
         self,
-        password: str,
+        password: Optional[str] = None,
         private_key: Optional[bytes] = None,
         watch_only: bool = False,
         address: Optional[NeoAddress] = None,
         label: Optional[str] = None,
         lock: bool = False,
         contract_: Optional[contract.Contract] = None,
         extra: Optional[dict[str, Any]] = None,
@@ -182,14 +182,19 @@
         if watch_only:
             if address is None:
                 raise ValueError("Creating a watch only account requires an address")
             else:
                 utils.validate_address(address)
 
         else:
+            if not watch_only and password is None:
+                raise ValueError(
+                    "Can't create an account without a password unless it is a watch only account. "
+                    "To create a watch only accont set `watch_only` to `True` and provide an address"
+                )
             key_pair: cryptography.KeyPair
 
             if private_key is None:
                 key_pair = cryptography.KeyPair.generate()
                 private_key = key_pair.private_key
             else:
                 key_pair = cryptography.KeyPair(private_key)
@@ -538,15 +543,15 @@
             "extra": self.extra if len(self.extra) > 0 else None,
         }
 
     @classmethod
     def from_json(
         cls,
         json: dict,
-        password: str,
+        password: Optional[str],
         scrypt_parameters: Optional[scrypt.ScryptParameters] = None,
     ) -> Account:
         """
         Parse object out of JSON data.
 
         Args:
             json: a dictionary.
@@ -554,27 +559,30 @@
             scrypt_parameters: the Scrypt parameters to use to encode the private key. Default conforms to NEP-2.
 
         Raises:
             KeyError: if the data supplied does not contain the necessary key.
         """
         validate(json, schema=cls._json_schema)
 
+        private_key = None
+        if json["key"] is not None and password is not None:
+            private_key = cls.private_key_from_nep2(
+                json["key"], password, scrypt_parameters
+            )
+
         return cls(
             password=password,
-            private_key=(
-                cls.private_key_from_nep2(json["key"], password, scrypt_parameters)
-                if json["key"] is not None
-                else json["key"]
-            ),
+            private_key=private_key,
             address=json["address"],
             label=json["label"],
             lock=json["lock"],
             contract_=AccountContract.from_json(json["contract"]),
             extra=json["extra"],
             scrypt_parameters=scrypt_parameters,
+            watch_only=True if private_key is None else False,
         )
 
     @staticmethod
     def private_key_from_nep2(
         nep2_key: str,
         passphrase: str,
         _scrypt_parameters: Optional[scrypt.ScryptParameters] = None,
```

### Comparing `neo-mamba-1.1.0/neo3/wallet/scrypt_parameters.py` & `neo-mamba-2.0.0/neo3/wallet/scrypt_parameters.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/neo3/wallet/utils.py` & `neo-mamba-2.0.0/neo3/wallet/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 NEO address utilities.
 """
 import base58
-from neo3.core import types
+from neo3.core import types, cryptography, utils as coreutils
 from neo3.wallet.types import NeoAddress
+from neo3.contracts import utils as contractutils
 
 
 def script_hash_to_address(
     script_hash: types.UInt160, address_version: int = 0x35
 ) -> NeoAddress:
     """
     Convert the specified script hash to an address.
@@ -33,14 +34,22 @@
         ValueError: if the account version is not valid.
     """
     validate_address(address)
     data = base58.b58decode_check(address)
     return types.UInt160(data[1:])
 
 
+def public_key_to_script_hash(public_key: cryptography.ECPoint) -> types.UInt160:
+    """
+    Convert the specified public key to a script hash.
+    """
+    contract_script = contractutils.create_signature_redeemscript(public_key)
+    return coreutils.to_script_hash(contract_script)
+
+
 def is_valid_address(address: NeoAddress) -> bool:
     """
     Test if the provided address is a valid address.
 
     Args:
         address: an address.
     """
```

### Comparing `neo-mamba-1.1.0/neo3/wallet/wallet.py` & `neo-mamba-2.0.0/neo3/wallet/wallet.py`

 * *Files 3% similar despite different names*

```diff
@@ -283,21 +283,21 @@
             and self._default_account.address == acc.address
         )
         json_account = acc.to_json()
         json_account["isDefault"] = is_default
         return json_account
 
     @classmethod
-    def from_json(cls, json: dict, password: Optional[str] = None):
+    def from_json(cls, json: dict, passwords: Optional[list[str]] = None):
         """
         Parse object out of JSON data.
 
         Args:
             json: a dictionary.
-            password: the password to decrypt the account data.
+            passwords: the password to decrypt the account data.
 
         Raises:
             KeyError: if the data supplied does not contain the necessary keys.
             ValueError: if the `version` property is under 1.0 or is not a valid string.
         """
         validate(json, schema=cls.json_schema)
         try:
@@ -305,50 +305,57 @@
                 raise ValueError("Format error - invalid 'version'")
         except ValueError:
             raise ValueError("Format error - invalid 'version'")
 
         accounts = []
         default_account = None
         scryptp = scrypt.ScryptParameters.from_json(json["scrypt"])
-        if len(json["accounts"]) > 0:
-            if password is None:
-                raise ValueError("Missing wallet password to decrypt account data")
+        if (len_accounts := len(json["accounts"])) > 0:
+            if passwords is None:
+                # mypy is being annoying about re-assigning to the same variable with a different type
+                # we just need a list with None's for zip() to work and to create a watch only account.
+                passwords = [None] * len(json["accounts"])  # type: ignore
             else:
-                for json_account in json["accounts"]:
-                    account_from_json = account.Account.from_json(
-                        json_account, password, scrypt_parameters=scryptp
+                len_pws = len(passwords)
+                if len_accounts != len_pws:
+                    raise ValueError(
+                        f"Incorrect number of passwords provided ({len_pws}) for number of accounts in wallet ({len_accounts})"
                     )
-                    accounts.append(account_from_json)
-                    if (
-                        default_account is None
-                        and hasattr(json, "isDefault")
-                        and json["isDefault"]
-                    ):
-                        default_account = account_from_json
+            for json_account, pw in zip(json["accounts"], passwords):
+                account_from_json = account.Account.from_json(
+                    json_account, pw, scrypt_parameters=scryptp
+                )
+                accounts.append(account_from_json)
+                if (
+                    default_account is None
+                    and hasattr(json, "isDefault")
+                    and json["isDefault"]
+                ):
+                    default_account = account_from_json
 
         return cls(
             name=json["name"],
             version=json["version"],
             scrypt_params=scryptp,
             accounts=accounts,
             default_account=default_account,
             extra=json["extra"],
         )
 
     @classmethod
-    def from_file(cls, path: str, password: Optional[str] = None):
+    def from_file(cls, path: str, passwords: Optional[list[str]] = None):
         """
         Load wallet from file.
 
         Args:
             path: path as passed to `open()`.
-            password: the password to decrypt the account data.
+            passwords: the password to decrypt the account data.
         """
         with open(path, "r") as f:
-            return cls.from_json(json.load(f), password)
+            return cls.from_json(json.load(f), passwords)
 
     def __enter__(self) -> Wallet:
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self.save()
 
@@ -425,20 +432,20 @@
             version=cls._wallet_version,
             scrypt_params=scrypt.ScryptParameters(),
             accounts=[],
             extra=None,
         )
 
     @classmethod
-    def from_json(cls, json: dict, password: Optional[str] = None):
-        w = Wallet.from_json(json, password)
+    def from_json(cls, json: dict, passwords: Optional[list[str]] = None):
+        w = Wallet.from_json(json, passwords)
         path = ""
         return cls(
             path, w.name, w.version, w.scrypt, w.accounts, w.account_default, w.extra
         )
 
     @classmethod
-    def from_file(cls, path: str, password: Optional[str] = None):
+    def from_file(cls, path: str, passwords: Optional[list[str]] = None):
         with open(path, "r") as f:
-            w = cls.from_json(json.load(f), password)
+            w = cls.from_json(json.load(f), passwords)
             w.path = path
             return w
```

### Comparing `neo-mamba-1.1.0/neo_mamba.egg-info/PKG-INFO` & `neo-mamba-2.0.0/neo_mamba.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: neo-mamba
-Version: 1.1.0
+Version: 2.0.0
 Summary: Python SDK for the NEO 3 blockchain
 Home-page: https://github.com/CityOfZion/neo-mamba
 Author: Erik van den Brink
 Author-email: erik@coz.io
 Maintainer: Erik van den Brink
 Maintainer-email: erik@coz.io
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ==3.10.*
+Requires-Python: <=3.12,>=3.10.0
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE.md
 
 .. image:: .github/resources/images/logo.png
     :width: 400 px
@@ -59,19 +59,26 @@
 
 Please report any issues on `Github <https://github.com/CityOfZion/neo-mamba/issues>`_ or submit ideas how to improve the SDK.
 
 Also check out our Python smart contract compiler `Boa <https://github.com/CityOfZion/neo3-boa>`_ !
 
 Installation and usage
 ----------------------
-Installation instructions, how to interact with smart contrats as well as API reference documentation can be found at
+Installation instructions, how to interact with smart contracts as well as API reference documentation can be found at
 https://mamba.coz.io/
 
 Developing or contributing
 --------------------------
 Install the requirements, modify the code and PR :-)
 ::
 
    pip install -e .[dev]
 
-The project uses `Black <https://github.com/psf/black>`_ for code formatting. You might want to
-`integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ this into your editor.
+For larger changes consider opening an issue first to discuss the change. Below are a few guidelines for contributing
+
+* The project uses `Black <https://github.com/psf/black>`_ for code formatting. PRs will fail if formatted incorrectly.
+  You might want to `integrate <https://black.readthedocs.io/en/stable/integrations/editors.html>`_ `black` into your
+  editor or run it manually with `make black`.
+* All public functions/classes must have docstrings.
+* All your code must be typed. Test your typing with `make type`. In rare cases it might be hard/impractical to add typing.
+  Point it out if that is the case and add a short description why we could do without.
+* Add tests that cover the newly added (or changed if applicable) code. Use `make test` and `make coverage`.
```

### Comparing `neo-mamba-1.1.0/neo_mamba.egg-info/SOURCES.txt` & `neo-mamba-2.0.0/neo_mamba.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 tests/core/test_cryptography.py
 tests/core/test_serialization.py
 tests/core/test_types.py
 tests/core/test_utils.py
 tests/network/__init__.py
 tests/network/test_capabilities.py
 tests/network/test_ipfilter.py
+tests/network/test_issues.py
 tests/network/test_message.py
 tests/network/test_node.py
 tests/network/test_payloads.py
 tests/network/test_witnessrules.py
 tests/network/convenience/__init__.py
 tests/network/convenience/test_nodemanager.py
 tests/network/convenience/test_syncmanager.py
```

### Comparing `neo-mamba-1.1.0/setup.cfg` & `neo-mamba-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.0
+current_version = 2.0.0
 commit = True
 tag = True
 
 [metadata]
 name = neo-mamba
 version = attr: neo3.__version__
 description = Python SDK for the NEO 3 blockchain
@@ -19,32 +19,32 @@
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3.10
 
 [options]
-python_requires = == 3.10.*
+python_requires = >= 3.10.0,<= 3.12
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	aiodns==3.0.0
 	aiohttp==3.7.4.post0
 	base58==2.1.0
 	bitarray==2.6.0
 	Events==0.4
 	jsonschema>=3.2.0
 	lz4==4.0.2
-	neo3crypto==0.3
+	neo3crypto==0.4
 	netaddr>=0.8.0
 	orjson>=3.8.2
 	pycryptodome==3.15.0
-	pybiginteger==1.2.7
-	pybiginteger-stubs==1.2.7
+	pybiginteger==1.3.0
+	pybiginteger-stubs==1.3.0
 
 [options.extras_require]
 dev = 
 	aioresponses==0.7.2
 	black==22.8.0
 	build==0.8.0
 	bump2version==1.0.1
```

### Comparing `neo-mamba-1.1.0/tests/api/test_noderpc.py` & `neo-mamba-2.0.0/tests/api/test_noderpc.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/api/test_wrappers.py` & `neo-mamba-2.0.0/tests/api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_abi.py` & `neo-mamba-2.0.0/tests/contracts/test_abi.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_callflags.py` & `neo-mamba-2.0.0/tests/contracts/test_callflags.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_contract.py` & `neo-mamba-2.0.0/tests/contracts/test_contract.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_contractstate.py` & `neo-mamba-2.0.0/tests/contracts/test_contractstate.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_manifest.py` & `neo-mamba-2.0.0/tests/contracts/test_manifest.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_nef.py` & `neo-mamba-2.0.0/tests/contracts/test_nef.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/contracts/test_utils.py` & `neo-mamba-2.0.0/tests/contracts/test_utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/core/test_biginteger.py` & `neo-mamba-2.0.0/tests/core/test_biginteger.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/core/test_cryptography.py` & `neo-mamba-2.0.0/tests/core/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/core/test_serialization.py` & `neo-mamba-2.0.0/tests/core/test_serialization.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/core/test_types.py` & `neo-mamba-2.0.0/tests/core/test_types.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/core/test_utils.py` & `neo-mamba-2.0.0/tests/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/convenience/test_nodemanager.py` & `neo-mamba-2.0.0/tests/network/convenience/test_nodemanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/convenience/test_syncmanager.py` & `neo-mamba-2.0.0/tests/network/convenience/test_syncmanager.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/convenience/test_various.py` & `neo-mamba-2.0.0/tests/network/convenience/test_various.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_capabilities.py` & `neo-mamba-2.0.0/tests/network/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_ipfilter.py` & `neo-mamba-2.0.0/tests/network/test_ipfilter.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_message.py` & `neo-mamba-2.0.0/tests/network/test_message.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_node.py` & `neo-mamba-2.0.0/tests/network/test_node.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_payloads.py` & `neo-mamba-2.0.0/tests/network/test_payloads.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/network/test_witnessrules.py` & `neo-mamba-2.0.0/tests/network/test_witnessrules.py`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/test_vm.py` & `neo-mamba-2.0.0/tests/test_vm.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,39 @@
         # too slow
         # data = b'\x01' * (0xFFFFFFFF + 1)
         # sb = vm.ScriptBuilder()
         # with self.assertRaises(ValueError) as context:
         #     sb.emit_push(data)
         # self.assertIn("Value is too long", str(context.exception))
 
+    def test_emit_push_dict(self):
+        data = {"a": 123, "b": 456}
+
+        sb = vm.ScriptBuilder()
+        sb.emit_push(data)
+        expected = "007b0c016101c8010c016212be"
+        self.assertEqual(expected, sb.to_array().hex())
+
+        # test invalid key type
+        sb = vm.ScriptBuilder()
+        with self.assertRaises(ValueError) as context:
+            sb.emit_push({1.0: "abc"})
+        self.assertEqual(
+            "Unsupported key type <class 'float'>. Supported types by the VM are bool, int and str",
+            str(context.exception),
+        )
+
+    def test_emit_push_list(self):
+        data = ["a", 123, "b", 456]
+
+        sb = vm.ScriptBuilder()
+        sb.emit_push(data)
+        expected = "01c8010c0162007b0c016114c0"
+        self.assertEqual(expected, sb.to_array().hex())
+
     def test_emit_push_unsupported(self):
         class Unsupported:
             pass
 
         sb = vm.ScriptBuilder()
         with self.assertRaises(ValueError) as context:
             sb.emit_push(Unsupported())
```

### Comparing `neo-mamba-1.1.0/tests/wallet/rc2-wallet.json` & `neo-mamba-2.0.0/tests/wallet/rc2-wallet.json`

 * *Files identical despite different names*

### Comparing `neo-mamba-1.1.0/tests/wallet/test_account.py` & `neo-mamba-2.0.0/tests/wallet/test_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,7 +117,15 @@
     def test_new_account_wrong_password(self):
         for testcase in account_list:
             with self.assertRaises(ValueError) as context:
                 account.Account.from_encrypted_key(
                     testcase["encrypted_key"], "wrong password"
                 )
             self.assertIn("Wrong passphrase", str(context.exception))
+
+    def test_new_account_no_password(self):
+        with self.assertRaises(ValueError) as context:
+            account.Account()
+        self.assertIn(
+            "Can't create an account without a password unless it is a watch only account",
+            str(context.exception),
+        )
```

### Comparing `neo-mamba-1.1.0/tests/wallet/test_wallet.py` & `neo-mamba-2.0.0/tests/wallet/test_wallet.py`

 * *Files 24% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         test_account = account.Account.create_new(
             password, scrypt_parameters=scrypt.ScryptParameters(2, 8, 8)
         )
         new_wallet.account_add(test_account, is_default=True)
 
         json_wallet = new_wallet.to_json()
 
-        test_wallet = wallet.Wallet.from_json(json_wallet, password="123")
+        test_wallet = wallet.Wallet.from_json(json_wallet, passwords=["123"])
         self.assertEqual(new_wallet.name, test_wallet.name)
         self.assertEqual("1.0", test_wallet.version)
         self.assertEqual(1, len(test_wallet.accounts))
         self.assertEqual(test_account, test_wallet.accounts[0])
         self.assertEqual(test_wallet._default_account, test_wallet.accounts[0])
 
     def test_wallet_account_new(self):
@@ -244,11 +244,52 @@
         self.assertEqual(account_3, test_wallet._default_account)
 
     def test_from_json_with_multisig_account(self):
         p = os.path.join(os.path.dirname(__file__), "rc2-wallet.json")
         with open(p) as f:
             data = json.load(f)
 
-        w = wallet.Wallet.from_json(data, "123")
+        w = wallet.Wallet.from_json(data, ["123", "123"])
         self.assertEqual(2, len(w.accounts))
         self.assertEqual("NY9qiu8YScTM9oAc3nnaeNjaX5fnraaRTA", w.accounts[0].address)
         self.assertEqual("NcmoFiYqThZJFiEYVF1BjYEk6YwF5vtkFA", w.accounts[1].address)
+
+    def test_from_json_with_multiple_accounts(self):
+        label_1 = "Account 1"
+        label_2 = "Account 2"
+
+        password1 = "123123"
+        password2 = "456456"
+        scryptp = scrypt.ScryptParameters(2, 8, 8)
+        account_1 = account.Account(
+            password=password1, label=label_1, scrypt_parameters=scryptp
+        )
+        account_2 = account.Account(
+            password=password2, label=label_2, scrypt_parameters=scryptp
+        )
+        w = wallet.Wallet(name="test wallet", scrypt_params=scryptp)
+        w.account_add(account_1)
+        w.account_add(account_2)
+        w_json = w.to_json()
+
+        # now test we can load it from_json
+        w2_with_passwords = wallet.Wallet.from_json(w_json, [password1, password2])
+        self.assertEqual(2, len(w2_with_passwords.accounts))
+        self.assertFalse(w2_with_passwords.accounts[0].is_watchonly)
+        self.assertFalse(w2_with_passwords.accounts[0].is_watchonly)
+
+        w2_as_watchonly = wallet.Wallet.from_json(w_json)
+        self.assertEqual(2, len(w2_with_passwords.accounts))
+        self.assertTrue(w2_as_watchonly.accounts[0].is_watchonly)
+        self.assertTrue(w2_as_watchonly.accounts[0].is_watchonly)
+
+    def test_insufficient_passwords_provided_from_json(self):
+        p = os.path.join(os.path.dirname(__file__), "rc2-wallet.json")
+        with open(p) as f:
+            data = json.load(f)
+
+        with self.assertRaises(ValueError) as context:
+            wallet.Wallet.from_json(data, ["123"])
+        self.assertIn(
+            "Incorrect number of passwords provided (1) for number of accounts in wallet (2)",
+            str(context.exception),
+        )
```

