# Comparing `tmp/kybra-0.4.0rc1.tar.gz` & `tmp/kybra-0.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kybra-0.4.0rc1.tar", last modified: Tue Jan 24 20:55:42 2023, max compression
+gzip compressed data, was "kybra-0.5.0rc0.tar", last modified: Wed Jul  5 21:21:07 2023, max compression
```

## Comparing `kybra-0.4.0rc1.tar` & `kybra-0.5.0rc0.tar`

### file list

```diff
@@ -1,216 +1,328 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    56891 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra/
--rw-r--r--   0 runner    (1001) docker     (123)    14804 2023-01-24 20:55:24.000000 kybra-0.4.0rc1/kybra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra/canisters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra/canisters/ledger/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/ledger/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/ledger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra/canisters/management/
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/management/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/management/bitcoin.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/canisters/management/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/cargotoml.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra/compiler/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/custom_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/custom_modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/custom_modules/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8059 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/custom_modules/principal.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/custom_modules/typing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2691 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/install_rust_dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/errors.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/async_result_handler.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.509866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.517866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/accept_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/arg_data_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/arg_data_raw_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/caller.rs
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/candid_decode.rs
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/candid_encode.rs
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/canister_balance.rs
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/canister_balance128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/clear_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/data_certificate.rs
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/id.rs
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/method_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_accept.rs
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_accept128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_available.rs
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_available128.rs
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_refunded.rs
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/msg_cycles_refunded128.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/notify_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/notify_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/notify_with_payment128_functions.rs
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/performance_counter.rs
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/print.rs
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/reject.rs
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/reject_code.rs
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/reject_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/reply.rs
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/reply_raw.rs
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/set_certified_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/set_timer.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/set_timer_interval.rs
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable64_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable64_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable64_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable64_write.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.517866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/contains_key.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/get.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/insert.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/is_empty.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/items.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/keys.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/len.rs
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/remove.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/values.rs
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_bytes.rs
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_grow.rs
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_read.rs
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_size.rs
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_write.rs
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/time.rs
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/trap.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/kybra_serde.rs
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/stable_b_tree_map.rs
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.517866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.517866 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/vec.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/basic.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/generic.rs
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/vec.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_ast/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_ast/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_ast/to_act.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_arguments/
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_arguments/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/array.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/generate_inline_name.rs
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/generator.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/get_dependencies.rs
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/hash.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/opt.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/to_act_data_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14536 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/to_hash_string.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/tuple.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_program/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_program/build_external_canisters.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_program/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_program/stable_b_tree_map_nodes.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/
--rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/canister_method.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.521867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/func/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/func/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/func/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/record_members/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/record_members/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/record_members/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/records/record_members/warnings.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/tuples/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/tuples/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/tuples/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/type_alias/
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/type_alias/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/variants_members/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/variants_members/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/variants_members/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/variants_members/warnings.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/external_canisters/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/external_canisters/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/get_dependencies.rs
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/get_source_info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/stable_b_tree_map_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/stable_b_tree_map_nodes/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/stable_b_tree_map_nodes/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/system_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/system_methods/errors.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/system_methods/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.525867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/type_alias/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/type_alias/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/heartbeat.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/init.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/inspect_message.rs
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/post_upgrade.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/system_methods/pre_upgrade.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/traits/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/traits/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/what_is_it/
--rw-r--r--   0 runner    (1001) docker     (123)    19325 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/what_is_it/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/source_map/
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/source_map/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/kybra/compiler/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/compiler/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/module_bundler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/timed.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/kybra/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:55:42.505865 kybra-0.4.0rc1/kybra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11855 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-24 20:55:42.000000 kybra-0.4.0rc1/kybra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 20:55:42.529867 kybra-0.4.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-01-24 20:52:50.000000 kybra-0.4.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra/
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-07-05 21:20:51.000000 kybra-0.5.0rc0/kybra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/build_wasm_binary_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/candid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra/canisters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/canisters/ledger/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/ledger/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/ledger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/canisters/management/
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/bitcoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/canisters/management/tecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80489 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/cargotoml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/custom_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/__pycache__/principal.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/custom_modules/typing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/install_rust_dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_deployer/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.038636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/async_result_handler.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/call_global_python_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/unwrap_rust_python_result.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/body/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/array.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_member.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_subscriptable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/invalid_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/none_cannot_be_a_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/not_exactly_one_target.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/errors/unsupported_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_call_takes_one_arg.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/func_formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/errors/return_type_mode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/func/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/opt.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/primitive.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/record/record_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.042636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/missing_decorator_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_must_have_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/service_with_non_function_defs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/too_many_decorators.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/errors/wrong_decorator.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/to_candid_type.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/tuple/tuple_members.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/type_ref.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/variants_members/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/default_value_ignored.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/warnings/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/guard_function_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/multiple_system_methods.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/errors/return_type_must_be_void.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/heartbeat_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/init_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/inspect_message_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/post_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.046636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/pre_upgrade_method/rust.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/query_or_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/query_or_update/update_method.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/canister_method/rust.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/constants.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)    33809 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/analyze.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/display_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/test_error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/what_is_it.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/collect_results.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/unreachable.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/exit_codes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_child_class_of.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/get_subscript_slice.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_param.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/guard_functions_return.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/guard_function.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/guard_function/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/ref_cells.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/traits.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/header/use_statements.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.050636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/accept_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/arg_data_raw_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/caller.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_decode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/candid_encode.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/canister_balance128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/clear_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/data_certificate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/method_name.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_accept128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_available128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/msg_cycles_refunded128.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/performance_counter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/print.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_code.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reject_message.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/reply_raw.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_certified_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/set_timer_interval.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable64_write.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/insert.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/keys.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/remove.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_bytes.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_grow.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_read.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_size.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_write.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/time.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/trap.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/keywords.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/kybra_modules_init/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/kybra_modules_init/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.058636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/dictionary_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/first_parameter_must_not_be_self.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/iterator_unpacking_operator_not_supported.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/param_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/return_type_annotation_required.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/errors/too_many_params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/params.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/method_utils/returns.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/errors.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/get_stmt_kinds.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/py_ast.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/py_ast/to_act.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/
+-rw-r--r--   0 runner    (1001) docker     (123)    22031 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/
+-rw-r--r--   0 runner    (1001) docker     (123)    28330 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/source_map/token_length/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/invalid_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_key_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_size_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/max_value_size_missing.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_an_integer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_integer_constant.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_must_be_non_negative.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/memory_id_too_big.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/missing_memory_id.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/errors/stable_b_tree_map_node_format.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10126 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/bounded_storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/ref_cell_ident.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/storable_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/try_into_vm_value_impl.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/stable_b_tree_map_nodes/rust/wrapper_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/tuple.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.062636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_modules_init/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/dfx.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/install_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/main.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/permissions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_app_canister.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_chunk.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_post_install/src/upload_python_stdlib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/shared_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/shared_utils/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/shared_utils/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/shared_utils/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.066636 kybra-0.5.0rc0/kybra/compiler/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/compiler/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/module_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/run_kybra_generate_or_exit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/timed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/kybra/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 21:21:07.034636 kybra-0.5.0rc0/kybra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-07-05 21:21:07.000000 kybra-0.5.0rc0/kybra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-05 21:21:06.000000 kybra-0.5.0rc0/kybra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 21:21:07.070636 kybra-0.5.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-05 21:18:30.000000 kybra-0.5.0rc0/setup.py
```

### Comparing `kybra-0.4.0rc1/LICENSE` & `kybra-0.5.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/NOTICE` & `kybra-0.5.0rc0/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/kybra/__main__.py` & `kybra-0.5.0rc0/kybra/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 import os
 from pathlib import Path
 import re
 import shutil
 import subprocess
 import sys
 import time
+import site
 from typing import Any, Callable
 
 import kybra
+from kybra.build_wasm_binary_or_exit import build_wasm_binary_or_exit
+from kybra.cargotoml import generate_cargo_toml, generate_cargo_lock
 from kybra.colors import red, yellow, green, dim
+from kybra.run_kybra_generate_or_exit import run_kybra_generate_or_exit
 from kybra.timed import timed, timed_inline
 from kybra.types import Args, Paths
-from kybra.cargotoml import generate_cargo_toml
 
 
 @timed
 def main():
     args = parse_args_or_exit(sys.argv)
     paths = create_paths(args)
     is_verbose = args["flags"]["verbose"]
@@ -45,58 +48,95 @@
         )
 
     # Copy all of the Rust project structure from the pip package to an area designed for Rust compiling
     if os.path.exists(paths["canister"]):
         shutil.rmtree(paths["canister"])
     shutil.copytree(paths["compiler"], paths["canister"], dirs_exist_ok=True)
     create_file(f"{paths['canister']}/Cargo.toml", generate_cargo_toml(canister_name))
+    create_file(f"{paths['canister']}/Cargo.lock", generate_cargo_lock())
+    create_file(
+        f"{paths['canister']}/post_install.sh",
+        generate_post_install_script(canister_name, kybra.__rust_version__, is_verbose),
+    )
+    os.system(f"chmod +x {paths['canister']}/post_install.sh")
 
     # Add CARGO_TARGET_DIR to env for all cargo commands
     cargo_env = {
         **os.environ.copy(),
         "CARGO_TARGET_DIR": paths["global_kybra_target_dir"],
-        "CARGO_HOME": paths["global_kybra_config_dir"],
-        "RUSTUP_HOME": paths["global_kybra_config_dir"],
+        "CARGO_HOME": paths["global_kybra_rust_dir"],
+        "RUSTUP_HOME": paths["global_kybra_rust_dir"],
     }
 
+    if not os.path.exists(paths["global_kybra_bin_dir"]):
+        os.makedirs(paths["global_kybra_bin_dir"])
+
     compile_python_or_exit(
         paths, cargo_env, verbose=is_verbose, label="[1/3] 🔨 Compiling Python..."
     )
 
-    generate_candid_file_or_exit(
+    build_wasm_binary_or_exit(
         paths,
+        canister_name,
         cargo_env,
         verbose=is_verbose,
-        label=f"[2/3] 📝 Generating Candid file...{encourage_patience(is_initial_compile)}",
+        label=f"[2/3] 🚧 Building Wasm binary...{show_empathy(is_initial_compile)}",
     )
 
-    build_wasm_binary_or_exit(
+    optimize_wasm_binary_or_exit(
         paths,
         canister_name,
         cargo_env,
         verbose=is_verbose,
-        label=f"[3/3] 🚧 Building Wasm binary...{show_empathy(is_initial_compile)}",
+        label=f"[3/3] 🚀 Optimizing Wasm binary...{show_empathy(is_initial_compile)}",
     )
 
-    print(f"\n🎉 Built canister {green(canister_name)} at {dim(paths['gzipped_wasm'])}")
+    print(f"\n🎉 Built canister {green(canister_name)} at {dim(paths['wasm'])}")
+
+
+def generate_post_install_script(
+    canister_name: str, rust_version: str, is_verbose: bool
+) -> str:
+    main_command = f"KYBRA_VERSION={kybra.__version__} cargo run --manifest-path=.kybra/{canister_name}/kybra_post_install/Cargo.toml {canister_name}"
+    main_command_not_verbose = f'exec 3>&1; output=$({main_command} 2>&1 1>&3 3>&-); exit_code=$?; exec 3>&-; if [ $exit_code -ne 0 ]; then echo "$output"; exit $exit_code; fi'
+
+    return f"""#!/bin/bash
+
+rust_version="{rust_version}"
+
+global_kybra_config_dir=~/.config/kybra
+global_kybra_rust_dir="$global_kybra_config_dir"/rust/"$rust_version"
+global_kybra_rust_bin_dir="$global_kybra_rust_dir"/bin
+global_kybra_logs_dir="$global_kybra_rust_dir"/logs
+global_kybra_cargo_bin="$global_kybra_rust_bin_dir"/cargo
+global_kybra_rustup_bin="$global_kybra_rust_bin_dir"/rustup
+
+export CARGO_TARGET_DIR="$global_kybra_config_dir"/rust/target
+export CARGO_HOME="$global_kybra_rust_dir"
+export RUSTUP_HOME="$global_kybra_rust_dir"
+
+echo "\nPreparing canister binaries for upload...\n"
+
+{main_command if is_verbose else main_command_not_verbose}
+    """
 
 
 def parse_args_or_exit(args: list[str]) -> Args:
     args = args[1:]  # Discard the path to kybra
 
     flags = [arg for arg in args if (arg.startswith("-") or arg.startswith("--"))]
     args = [arg for arg in args if not (arg.startswith("-") or arg.startswith("--"))]
 
     if len(args) == 0:
         print(f"\nkybra {kybra.__version__}")
         print("\nUsage: kybra [-v|--verbose] <canister_name> <entry_point> <did_path>")
         sys.exit(0)
 
     if len(args) != 3:
-        print(red("\n💣 wrong number of arguments\n"))
+        print(red("\n💣 Kybra error: wrong number of arguments\n"))
         print("Usage: kybra [-v|--verbose] <canister_name> <entry_point> <did_path>")
         print("\n💀 Build failed!")
         sys.exit(1)
 
     return {
         "empty": False,
         "flags": {"verbose": "--verbose" in flags or "-v" in flags},
@@ -119,15 +159,15 @@
     canister_path = f".kybra/{canister_name}"
 
     # We want to bundle/gather all Python files into the python_source directory for RustPython freezing
     # The location that Kybra will look to when running py_freeze!
     # py_freeze! will compile all of the Python code in the directory recursively (modules must have an __init__.py to be included)
     python_source_path = f"{canister_path}/python_source"
 
-    py_file_names_file_path = f"{canister_path}/file_names.txt"
+    py_file_names_file_path = f"{canister_path}/py_file_names.csv"
 
     # This is the path to the developer's Candid file passed into python -m kybra from the dfx.json build command
     did_path = args["did_path"]
 
     # This is the path to the Kybra compiler Rust code delivered with the Python package
     compiler_path = os.path.dirname(kybra.__file__) + "/compiler"
 
@@ -136,41 +176,41 @@
 
     # This is the location of the Candid file generated from the final generated Rust file
     generated_did_path = f"{canister_path}/index.did"
 
     # This is the unzipped generated Wasm that is the canister
     wasm_path = f"{canister_path}/{canister_name}.wasm"
 
-    # This is the final zipped generated Wasm that will actually run on the Internet Computer
-    gzipped_wasm_path = f"{wasm_path}.gz"
-
     # This is where we store custom Python modules, such as stripped-down versions of stdlib modules
     custom_modules_path = f"{compiler_path}/custom_modules"
 
     home_dir = os.path.expanduser("~")
-    global_kybra_config_dir = f"{home_dir}/.config/kybra/{kybra.__version__}"
-    global_kybra_bin_dir = f"{global_kybra_config_dir}/bin"
-    global_kybra_target_dir = f"{global_kybra_config_dir}/target"
+    global_kybra_config_dir = f"{home_dir}/.config/kybra"
+    global_kybra_rust_dir = f"{global_kybra_config_dir}/rust/{kybra.__rust_version__}"
+    global_kybra_rust_bin_dir = f"{global_kybra_rust_dir}/bin"
+    global_kybra_target_dir = f"{global_kybra_config_dir}/rust/target"
+    global_kybra_bin_dir = f"{global_kybra_config_dir}/{kybra.__version__}/bin"
 
     return {
         "py_entry_file": py_entry_file_path,
         "py_entry_module_name": py_entry_module_name,
         "canister": canister_path,
         "python_source": python_source_path,
         "py_file_names_file": py_file_names_file_path,
         "did": did_path,
         "compiler": compiler_path,
         "lib": lib_path,
         "generated_did": generated_did_path,
         "wasm": wasm_path,
-        "gzipped_wasm": gzipped_wasm_path,
         "custom_modules": custom_modules_path,
         "global_kybra_config_dir": global_kybra_config_dir,
-        "global_kybra_bin_dir": global_kybra_bin_dir,
+        "global_kybra_rust_dir": global_kybra_rust_dir,
+        "global_kybra_rust_bin_dir": global_kybra_rust_bin_dir,
         "global_kybra_target_dir": global_kybra_target_dir,
+        "global_kybra_bin_dir": global_kybra_bin_dir,
     }
 
 
 def detect_initial_compile(global_kybra_target_dir: str) -> bool:
     return not os.path.exists(global_kybra_target_dir)
 
 
@@ -185,17 +225,21 @@
 
 def encourage_patience(is_initial_compile: bool) -> str:
     return " (be patient, this will take a while)" if is_initial_compile else ""
 
 
 def bundle_python_code(paths: Paths):
     # Begin module bundling/gathering process
-    path = list(filter(lambda x: x.startswith(os.getcwd()), sys.path)) + [
-        os.path.dirname(paths["py_entry_file"])
-    ]
+    path = (
+        list(filter(lambda x: x.startswith(os.getcwd()), sys.path))
+        + [
+            os.path.dirname(paths["py_entry_file"]),
+        ]
+        + site.getsitepackages()
+    )
 
     graph = modulegraph.modulegraph.ModuleGraph(path)  # type: ignore
     entry_point = graph.run_script(paths["py_entry_file"])  # type: ignore
 
     python_source_path = paths["python_source"]
 
     if os.path.exists(python_source_path):
@@ -220,67 +264,47 @@
             )
 
         if type(node) == modulegraph.modulegraph.Package:  # type: ignore
             shutil.copytree(
                 node.packagepath[0],  # type: ignore
                 f"{python_source_path}/{node.identifier}",  # type: ignore
                 dirs_exist_ok=True,
+                ignore=ignore_specific_dir,
             )
 
         if type(node) == modulegraph.modulegraph.NamespacePackage:  # type: ignore
             shutil.copytree(
                 node.packagepath[0],  # type: ignore
                 f"{python_source_path}/{node.identifier}",  # type: ignore
                 dirs_exist_ok=True,
+                ignore=ignore_specific_dir,
             )
 
     py_file_names = list(  # type: ignore
         filter(
-            lambda filename: filename is not None,  # type: ignore
+            lambda filename: filename is not None and filename.endswith(".py"),  # type: ignore
             map(
                 lambda node: node.filename,  # type: ignore
                 filter(
                     lambda node: node.filename  # type: ignore
                     is not "-",  # This filters out namespace packages
                     flattened_graph,  # type: ignore
                 ),  # type: ignore
             ),  # type: ignore
         )  # type: ignore
     )
 
     create_file(paths["py_file_names_file"], ",".join(py_file_names))  # type: ignore
 
 
-def run_kybra_generate_or_exit(paths: Paths, cargo_env: dict[str, str], verbose: bool):
-    # Generate the Rust code
-    kybra_generate_result = subprocess.run(
-        [
-            f"{paths['global_kybra_bin_dir']}/cargo",
-            "run",
-            f"--manifest-path={paths['canister']}/kybra_generate/Cargo.toml",
-            paths["py_file_names_file"],
-            paths["py_entry_module_name"],
-            paths["lib"],
-        ],
-        capture_output=not verbose,
-        env=cargo_env,
-    )
-
-    if kybra_generate_result.returncode != 0:
-        print(
-            red("\n💣 Something about your Python code violates Kybra's requirements\n")
-        )
-        print(parse_kybra_generate_error(kybra_generate_result.stderr))
-        print(
-            "\nIf you are unable to decipher the error above, reach out in the #typescript"
-        )
-        print("channel of the DFINITY DEV OFFICIAL discord:")
-        print("\nhttps://discord.com/channels/748416164832608337/1019372359775440988\n")
-        print("💀 Build failed")
-        sys.exit(1)
+def ignore_specific_dir(dirname: str, filenames: list[str]) -> list[str]:
+    if "kybra_post_install/src/Lib" in dirname:
+        return filenames
+    else:
+        return []
 
 
 def parse_kybra_generate_error(stdout: bytes) -> str:
     err = stdout.decode("utf-8")
     std_err_lines = err.splitlines()
     try:
         line_where_error_message_starts = next(
@@ -288,182 +312,131 @@
             for i, v in enumerate(std_err_lines)
             if v.startswith("thread 'main' panicked at '")
         )
         line_where_error_message_ends = next(
             i for i, v in enumerate(std_err_lines) if "', src/" in v
         )
     except:
-        return (
-            "The underlying cause is likely at the bottom of the following output:\n\n"
-            + err
-        )
+        return err
 
     err_lines = std_err_lines[
         line_where_error_message_starts : line_where_error_message_ends + 1
     ]
     err_lines[0] = err_lines[0].replace("thread 'main' panicked at '", "")
     err_lines[-1] = re.sub("', src/.*", "", err_lines[-1])
 
     return red("\n".join(err_lines))
 
 
 def run_rustfmt_or_exit(paths: Paths, cargo_env: dict[str, str], verbose: bool = False):
     rustfmt_result = subprocess.run(
-        [f"{paths['global_kybra_bin_dir']}/rustfmt", "--edition=2018", paths["lib"]],
+        [
+            f"{paths['global_kybra_rust_bin_dir']}/rustfmt",
+            "--edition=2018",
+            paths["lib"],
+        ],
         capture_output=not verbose,
         env=cargo_env,
     )
 
     if rustfmt_result.returncode != 0:
-        print(
-            red(
-                "\n💣 Kybra has experienced an internal error while trying to\n   format your generated rust canister"
-            )
-        )
+        print(red("\n💣 Kybra error: internal Rust formatting"))
         print(
             f'\nPlease open an issue at https://github.com/demergent-labs/kybra/issues/new\nincluding this message and the following error:\n\n {red(rustfmt_result.stderr.decode("utf-8"))}'
         )
         print("💀 Build failed")
         sys.exit(1)
 
 
+# TODO working on optimization
 @timed_inline
-def build_wasm_binary_or_exit(
+def optimize_wasm_binary_or_exit(
     paths: Paths, canister_name: str, cargo_env: dict[str, str], verbose: bool = False
 ):
-    # Compile the generated Rust code
-    cargo_build_result = subprocess.run(
-        [
-            f"{paths['global_kybra_bin_dir']}/cargo",
-            "build",
-            f"--manifest-path={paths['canister']}/Cargo.toml",
-            "--target=wasm32-unknown-unknown",
-            f"--package={canister_name}",
-            "--release",
-        ],
-        capture_output=not verbose,
-        env=cargo_env,
-    )
-
-    if cargo_build_result.returncode != 0:
-        print(red("\n💣 Error building Wasm binary:"))
-        print(cargo_build_result.stderr.decode("utf-8"))
-        print("💀 Build failed")
-        sys.exit(1)
-
-    # Optimize the Wasm binary
-    # TODO this should eventually be replaced with ic-wasm once this is resolved: https://forum.dfinity.org/t/wasm-module-contains-a-function-that-is-too-complex/15407/43?u=lastmjs
     optimization_result = subprocess.run(
         [
-            f"{paths['global_kybra_bin_dir']}/ic-cdk-optimizer",
-            f"{paths['global_kybra_target_dir']}/wasm32-unknown-unknown/release/{canister_name}.wasm",
-            f"-o={paths['wasm']}",
+            f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
+            f"{paths['canister']}/{canister_name}_app.wasm",
+            "-o",
+            f"{paths['canister']}/{canister_name}_app.wasm",
+            "shrink",
+            # "--optimize",
+            # "Oz",
         ],
         capture_output=not verbose,
     )
-    # optimization_result = subprocess.run(
-    #     [
-    #         f"{cargo_bin_root}/bin/ic-wasm",
-    #         f"{paths['target']}/wasm32-unknown-unknown/release/{canister_name}.wasm",
-    #         f"-o={paths['wasm']}",
-    #         "shrink",
-    #     ],
-    #     capture_output=not verbose,
-    # )
 
     if optimization_result.returncode != 0:
-        print(red("\n💣 Error optimizing generated Wasm:"))
+        print(red("\n💣 Kybra error: optimizing generated Wasm"))
         print(optimization_result.stderr.decode("utf-8"))
         print("💀 Build failed")
         sys.exit(1)
 
-    add_metadata_to_wasm_or_exit(paths, verbose=verbose)
+    # TODO we should be able to get rid of this now
+    add_metadata_to_wasm_or_exit(paths, canister_name, verbose=verbose)
 
-    # gzip the Wasm binary
-    os.system(f"gzip -f -k {paths['wasm']}")
+    os.system(f"gzip -9 -f -k {paths['canister']}/{canister_name}_app.wasm")
 
 
-def add_metadata_to_wasm_or_exit(paths: Paths, verbose: bool = False):
+def add_metadata_to_wasm_or_exit(
+    paths: Paths, canister_name: str, verbose: bool = False
+):
     add_candid_to_wasm_result = subprocess.run(
         [
-            f"{paths['global_kybra_bin_dir']}/ic-wasm",
-            paths["wasm"],
+            f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
+            f"{paths['canister']}/{canister_name}_app.wasm",
             "-o",
-            paths["wasm"],
+            f"{paths['canister']}/{canister_name}_app.wasm",
             "metadata",
             "candid:service",
             "-f",
             paths["did"],
             "-v",
             "public",
         ],
         capture_output=not verbose,
     )
 
     if add_candid_to_wasm_result.returncode != 0:
-        print(red("\n💣 Error adding candid to Wasm:"))
+        print(red("\n💣 Kybra error: adding candid to Wasm"))
         print(add_candid_to_wasm_result.stderr.decode("utf-8"))
         print("💀 Build failed")
         sys.exit(1)
 
     add_cdk_info_to_wasm_result = subprocess.run(
         [
-            f"{paths['global_kybra_bin_dir']}/ic-wasm",
-            paths["wasm"],
+            f"{paths['global_kybra_rust_bin_dir']}/ic-wasm",
+            f"{paths['canister']}/{canister_name}_app.wasm",
             "-o",
-            paths["wasm"],
+            f"{paths['canister']}/{canister_name}_app.wasm",
             "metadata",
             "cdk",
             "-d",
             f"kybra {kybra.__version__}",
             "-v",
             "public",
         ],
         capture_output=not verbose,
     )
 
     if add_cdk_info_to_wasm_result.returncode != 0:
-        print(red("\n💣 Error adding cdk name/version to Wasm:"))
+        print(red("\n💣 Kybra error: adding cdk name/version to Wasm"))
         print(add_cdk_info_to_wasm_result.stderr.decode("utf-8"))
         print("💀 Build failed")
         sys.exit(1)
 
 
 def show_empathy(is_initial_compile: bool) -> str:
     return (
         " (❤ hang in there, this will be faster next time)"
         if is_initial_compile
         else ""
     )
 
 
-@timed_inline
-def generate_candid_file_or_exit(
-    paths: Paths, cargo_env: dict[str, str], verbose: bool = False
-):
-    generate_candid_result = subprocess.run(
-        [
-            f"{paths['global_kybra_bin_dir']}/cargo",
-            "test",
-            f"--manifest-path={paths['canister']}/Cargo.toml",
-        ],
-        capture_output=not verbose,
-        env=cargo_env,
-    )
-
-    if generate_candid_result.returncode != 0:
-        print(red("\n💣 Error generating candid:"))
-        print(generate_candid_result.stderr.decode("utf-8"))
-        print("💀 Build failed")
-        sys.exit(1)
-
-    # Copy the generated Candid file to the developer's source directory
-    os.system(f"cp {paths['generated_did']} {paths['did']}")
-
-
 def create_file(file_path: str, contents: str):
     file = open(file_path, "w")
     file.write(contents)
     file.close()
 
 
 def inline_timed(
```

### Comparing `kybra-0.4.0rc1/kybra/canisters/ledger/NOTICE` & `kybra-0.5.0rc0/kybra/canisters/ledger/NOTICE`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/kybra/canisters/ledger/__init__.py` & `kybra-0.5.0rc0/kybra/canisters/ledger/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,268 +1,339 @@
-from kybra import blob, Canister, Func, method, nat32, nat64, opt, Principal, Query, Record, Variant
-from typing import TypeAlias
+from kybra import (
+    Alias,
+    blob,
+    Func,
+    nat32,
+    nat64,
+    null,
+    Opt,
+    Principal,
+    Query,
+    Record,
+    Service,
+    service_query,
+    service_update,
+    Variant,
+    Vec,
+)
 
 # Amount of tokens, measured in 10^-8 of a token.
+
+
 class Tokens(Record):
     e8s: nat64
 
+
 # Number of nanoseconds from the UNIX epoch in UTC timezone.
+
+
 class TimeStamp(Record):
     timestamp_nanos: nat64
 
+
 # AccountIdentifier is a 32-byte array.
 # The first 4 bytes is big-endian encoding of a CRC32 checksum of the last 28 bytes.
-AccountIdentifier = blob
+AccountIdentifier = Alias[blob]
 
 # Subaccount is an arbitrary 32-byte byte array.
 # Ledger uses subaccounts to compute the source address, which enables one
 # principal to control multiple ledger accounts.
-SubAccount = blob
+SubAccount = Alias[blob]
 
 # Sequence number of a block produced by the ledger.
-BlockIndex = nat64
+BlockIndex = Alias[nat64]
 
 # An arbitrary number associated with a transaction.
 # The caller can set it in a `transfer` call as a correlation identifier.
-Memo = nat64
+Memo = Alias[nat64]
 
 # Arguments for the `transfer` call.
+
+
 class TransferArgs(Record):
     # Transaction memo.
     # See comments for the `Memo` type.
     memo: Memo
     # The amount that the caller wants to transfer to the destination address.
     amount: Tokens
     # The amount that the caller pays for the transaction.
     # Must be 10000 e8s.
     fee: Tokens
     # The subaccount from which the caller wants to transfer funds.
     # If null, the ledger uses the default (all zeros) subaccount to compute the source address.
     # See comments for the `SubAccount` type.
-    from_subaccount: opt[SubAccount]
+    from_subaccount: Opt[SubAccount]
     # The destination account.
     # If the transfer is successful, the balance of this address increases by `amount`.
     to: AccountIdentifier
     # The point in time when the caller created this request.
     # If null, the ledger uses current IC time as the timestamp.
-    created_at_time: opt[TimeStamp]
+    created_at_time: Opt[TimeStamp]
+
 
 class TransferError_BadFee(Record):
     expected_fee: Tokens
 
+
 class TransferError_InsufficientFunds(Record):
     balance: Tokens
 
+
 class TransferError_TxTooOld(Record):
     allowed_window_nanos: nat64
 
+
 class TransferError_TxDuplicate(Record):
     duplicate_of: BlockIndex
 
+
 class TransferError(Variant, total=False):
     # The fee that the caller specified in the transfer request was not the one that ledger expects.
     # The caller can change the transfer fee to the `expected_fee` and retry the request.
     BadFee: TransferError_BadFee
     # The account specified by the caller doesn't have enough funds.
     InsufficientFunds: TransferError_InsufficientFunds
     # The request is too old.
     # The ledger only accepts requests created within 24 hours window.
     # This is a non-recoverable error.
     TxTooOld: TransferError_TxTooOld
     # The caller specified `created_at_time` that is too far in future.
     # The caller can retry the request later.
-    TxCreatedInFuture: None
+    TxCreatedInFuture: null
     # The ledger has already executed the request.
     # `duplicate_of` field is equal to the index of the block containing the original transaction.
     TxDuplicate: TransferError_TxDuplicate
 
+
 class TransferResult(Variant, total=False):
     Ok: nat64
     Err: TransferError
 
+
 # Arguments for the `account_balance` call.
+
+
 class AccountBalanceArgs(Record):
     account: AccountIdentifier
 
-class TransferFeeArg(Record): ...
+
+class TransferFeeArg(Record):
+    ...
+
 
 class TransferFee(Record):
     # The fee to pay to perform a transfer
     transfer_fee: Tokens
 
+
 class GetBlocksArgs(Record):
     # The index of the first block to fetch.
     start: BlockIndex
     # Max number of blocks to fetch.
     length: nat64
 
+
 class Operation_Mint(Record):
     to: AccountIdentifier
     amount: Tokens
 
+
 class Operation_Burn(Record):
     from_: AccountIdentifier
     amount: Tokens
 
+
 class Operation_Transfer(Record):
     from_: AccountIdentifier
     to: AccountIdentifier
     amount: Tokens
     fee: Tokens
 
+
 class Operation(Variant, total=False):
     Mint: Operation_Mint
     Burn: Operation_Burn
     Transfer: Operation_Transfer
 
+
 class Transaction(Record):
     memo: Memo
-    operation: opt[Operation]
+    operation: Opt[Operation]
     created_at_time: TimeStamp
 
+
 class Block(Record):
-    parent_hash: opt[blob]
+    parent_hash: Opt[blob]
     transaction: Transaction
     timestamp: TimeStamp
 
+
 # A prefix of the block range specified in the [GetBlocksArgs] request.
+
+
 class BlockRange(Record):
     # A prefix of the requested block range.
     # The index of the first block is equal to [GetBlocksArgs.from].
     #
     # Note that the number of blocks might be less than the requested
     # [GetBlocksArgs.len] for various reasons, for example:
     #
     # 1. The query might have hit the replica with an outdated state
     #    that doesn't have the full block range yet.
     # 2. The requested range is too large to fit into a single reply.
     #
     # NOTE: the list of blocks can be empty if:
     # 1. [GetBlocksArgs.len] was zero.
     # 2. [GetBlocksArgs.from] was larger than the last block known to the canister.
-    blocks: list[Block]
+    blocks: Vec[Block]
+
 
 class QueryArchiveError_BadFirstBlockIndex(Record):
     requested_index: BlockIndex
     first_valid_index: BlockIndex
 
+
 class QueryArchiveError_Other(Record):
     error_code: nat64
     error_message: str
 
+
 # An error indicating that the arguments passed to [QueryArchiveFn] were invalid.
+
+
 class QueryArchiveError(Variant, total=False):
     # [GetBlocksArgs.from] argument was smaller than the first block
     # served by the canister that received the request.
     BadFirstBlockIndex: QueryArchiveError_BadFirstBlockIndex
     # Reserved for future use.
     Other: QueryArchiveError_Other
 
+
 class QueryArchiveResult(Variant, total=False):
     # Successfully fetched zero or more blocks.
     Ok: BlockRange
     # The [GetBlocksArgs] request was invalid.
     Err: QueryArchiveError
 
+
 # A function that is used for fetching archived ledger blocks.
-QueryArchiveFn: TypeAlias = Func(Query[[GetBlocksArgs], QueryArchiveResult])
+QueryArchiveFn = Func(Query[[GetBlocksArgs], QueryArchiveResult])
+
 
 class QueryBlocksResponse_archived_blocks(Record):
     # The index of the first archived block that can be fetched using the callback.
     start: BlockIndex
 
     # The number of blocks that can be fetch using the callback.
     length: nat64
 
     # The function that should be called to fetch the archived blocks.
     # The range of the blocks accessible using this function is given by [from]
     # and [len] fields above.
     callback: QueryArchiveFn
 
+
 # The result of a "query_blocks" call.
 #
 # The structure of the result is somewhat complicated because the main ledger canister might
 # not have all the blocks that the caller requested: One or more "archive" canisters might
 # store some of the requested blocks.
 #
 # Note: as of Q4 2021 when this interface is authored, the IC doesn't support making nested
 # query calls within a query call.
+
+
 class QueryBlocksResponse(Record):
     # The total number of blocks in the chain.
     # If the chain length is positive, the index of the last block is `chain_len - 1`.
     chain_length: nat64
 
     # System certificate for the hash of the latest block in the chain.
     # Only present if `query_blocks` is called in a non-replicated query context.
-    certificate: opt[blob]
+    certificate: Opt[blob]
 
     # List of blocks that were available in the ledger when it processed the call.
     #
     # The blocks form a contiguous range, with the first block having index
     # [first_block_index] (see below), and the last block having index
     # [first_block_index] + len(blocks) - 1.
     #
     # The block range can be an arbitrary sub-range of the originally requested range.
-    blocks: list[Block]
+    blocks: Vec[Block]
 
     # The index of the first block in "blocks".
     # If the blocks vector is empty, the exact value of this field is not specified.
     first_block_index: BlockIndex
 
     # Encoding of instructions for fetching archived blocks whose indices fall into the
     # requested range.
     #
     # For each entry `e` in [archived_blocks], `[e.from, e.from + len)` is a sub-range
     # of the originally requested block range.
-    archived_blocks: list[QueryBlocksResponse_archived_blocks]
+    archived_blocks: Vec[QueryBlocksResponse_archived_blocks]
+
 
 class Archive(Record):
     canister_id: Principal
 
+
 class Archives(Record):
-    archives: list[Archive]
+    archives: Vec[Archive]
+
 
 class SymbolResult(Record):
     symbol: str
 
+
 class NameResult(Record):
     name: str
 
+
 class DecimalsResult(Record):
     decimals: nat32
 
-Address = str
 
-class Ledger(Canister):
+Address = Alias[str]
+
+
+class Ledger(Service):
     # Transfers tokens from a subaccount of the caller to the destination address.
     # The source address is computed from the principal of the caller and the specified subaccount.
     # When successful, returns the index of the block containing the transaction.
-    @method
-    def transfer(self, transfer_args: TransferArgs) -> TransferResult: ...
+    @service_update
+    def transfer(self, transfer_args: TransferArgs) -> TransferResult:
+        ...
 
     # Returns the amount of Tokens on the specified account.
-    @method
-    def account_balance(self, account_balance_args: AccountBalanceArgs) -> Tokens: ...
+    @service_query
+    def account_balance(self, account_balance_args: AccountBalanceArgs) -> Tokens:
+        ...
 
     # Returns the current transfer_fee.
-    @method
-    def transfer_fee(self, transfer_fee_arg: TransferFeeArg) -> TransferFee: ...
+    @service_query
+    def transfer_fee(self, transfer_fee_arg: TransferFeeArg) -> TransferFee:
+        ...
 
     # Queries blocks in the specified range.
-    @method
-    def query_blocks(self, get_blocks_args: GetBlocksArgs) -> QueryBlocksResponse: ...
+    @service_query
+    def query_blocks(self, get_blocks_args: GetBlocksArgs) -> QueryBlocksResponse:
+        ...
 
     # Returns token symbol.
-    @method
-    def symbol(self) -> SymbolResult: ...
+    @service_query
+    def symbol(self) -> SymbolResult:
+        ...
 
     # Returns token name.
-    @method
-    def name(self) -> NameResult: ...
+    @service_query
+    def name(self) -> NameResult:
+        ...
 
     # Returns token decimals.
-    @method
-    def decimals(self) -> DecimalsResult: ...
+    @service_query
+    def decimals(self) -> DecimalsResult:
+        ...
 
     # Returns the existing archive canisters information.
-    @method
-    def archives(self) -> Archives: ...
+    @service_query
+    def archives(self) -> Archives:
+        ...
```

### Comparing `kybra-0.4.0rc1/kybra/canisters/management/basic.py` & `kybra-0.5.0rc0/kybra/canisters/management/basic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,98 @@
-from kybra import blob, nat, opt, Principal, Record, Variant
+from kybra import blob, nat, null, Opt, Principal, Record, Variant, Vec
 
 # TODO type aliases do not work yet
 # TODO many canister_id fields need to be changed to use this alias
 # CanisterId = Principal
 # WasmModule = blob
 
+
 class CreateCanisterArgs(Record):
-    settings: opt["CanisterSettings"]
+    settings: Opt["CanisterSettings"]
+
 
 class CanisterSettings(Record):
-    controllers: opt[list[Principal]]
-    compute_allocation: opt[nat]
-    memory_allocation: opt[nat]
-    freezing_threshold: opt[nat]
+    controllers: Opt[Vec[Principal]]
+    compute_allocation: Opt[nat]
+    memory_allocation: Opt[nat]
+    freezing_threshold: Opt[nat]
+
 
 class DefiniteCanisterSettings(Record):
-    controllers: list[Principal]
+    controllers: Vec[Principal]
     compute_allocation: nat
     memory_allocation: nat
     freezing_threshold: nat
 
+
 class CreateCanisterResult(Record):
     canister_id: Principal
 
+
 class UpdateSettingsArgs(Record):
     canister_id: Principal
     settings: CanisterSettings
 
-# TODO this should be below InstallCodeArgs once double quote type syntax is allowed
-class InstallCodeMode(Variant, total=False):
-    install: None
-    reinstall: None
-    upgrade: None
 
 class InstallCodeArgs(Record):
-    mode: InstallCodeMode
+    mode: "InstallCodeMode"
     canister_id: Principal
     wasm_module: blob
     arg: blob
 
+
+class InstallCodeMode(Variant, total=False):
+    install: null
+    reinstall: null
+    upgrade: null
+
+
 class UninstallCodeArgs(Record):
     canister_id: Principal
 
+
 class StartCanisterArgs(Record):
     canister_id: Principal
 
+
 class StopCanisterArgs(Record):
     canister_id: Principal
 
+
 class CanisterStatusArgs(Record):
     canister_id: Principal
 
-# TODO this should be below CanisterStatusResult once double quote type syntax is allowed
-class CanisterStatus(Variant):
-    running: None
-    stopping: None
-    stopped: None
 
 class CanisterStatusResult(Record):
-    status: CanisterStatus
+    status: "CanisterStatus"
     settings: DefiniteCanisterSettings
-    module_hash: opt[blob]
+    module_hash: Opt[blob]
     memory_size: nat
     cycles: nat
 
+
+class CanisterStatus(Variant):
+    running: null
+    stopping: null
+    stopped: null
+
+
 class DeleteCanisterArgs(Record):
     canister_id: Principal
 
+
 class DepositCyclesArgs(Record):
     canister_id: Principal
 
+
 class ProvisionalCreateCanisterWithCyclesArgs(Record):
-    amount: opt[nat]
-    settings: opt[CanisterSettings]
+    amount: Opt[nat]
+    settings: Opt[CanisterSettings]
+
 
 class ProvisionalCreateCanisterWithCyclesResult(Record):
     canister_id: Principal
 
+
 class ProvisionalTopUpCanisterArgs(Record):
     canister_id: Principal
     amount: nat
```

### Comparing `kybra-0.4.0rc1/kybra/canisters/management/bitcoin.py` & `kybra-0.5.0rc0/kybra/canisters/management/bitcoin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from kybra import blob, nat32, nat64, opt, Record, Variant
+from kybra import Alias, blob, nat32, nat64, null, Opt, Record, Variant, Vec
 
-BitcoinAddress = str
-BlockHash = blob
+BitcoinAddress = Alias[str]
+BlockHash = Alias[blob]
 
 
 class BitcoinNetwork(Variant, total=False):
-    Mainnet: None
-    Regtest: None
-    Testnet: None
+    Mainnet: null
+    Regtest: null
+    Testnet: null
 
 
 class GetBalanceArgs(Record):
     address: BitcoinAddress
-    min_confirmations: opt[nat32]
+    min_confirmations: Opt[nat32]
     network: BitcoinNetwork
 
 
 class GetCurrentFeePercentilesArgs(Record):
     network: BitcoinNetwork
 
 
-Page = blob
+Page = Alias[blob]
 
 
 class UtxosFilter(Variant, total=False):
     MinConfirmations: nat32
     Page: Page
 
 
 class GetUtxosArgs(Record):
     address: BitcoinAddress
-    filter: opt[UtxosFilter]
+    filter: Opt[UtxosFilter]
     network: BitcoinNetwork
 
 
 class Outpoint(Record):
     txid: blob
     vout: nat32
 
 
-Satoshi = nat64
+Satoshi = Alias[nat64]
 
 
 class Utxo(Record):
     height: nat32
     outpoint: Outpoint
     value: Satoshi
 
 
 class GetUtxosResult(Record):
-    next_page: opt[Page]
+    next_page: Opt[Page]
     tip_block_hash: BlockHash
     tip_height: nat32
-    utxos: list[Utxo]
+    utxos: Vec[Utxo]
 
 
-MillisatoshiPerByte = nat64
+MillisatoshiPerByte = Alias[nat64]
 
 
 class SendTransactionArgs(Record):
     transaction: blob
     network: BitcoinNetwork
 
 
 class SendTransactionError(Variant, total=False):
-    MalformedTransaction: None
-    QueueFull: None
+    MalformedTransaction: null
+    QueueFull: null
```

### Comparing `kybra-0.4.0rc1/kybra/canisters/management/http.py` & `kybra-0.5.0rc0/kybra/canisters/management/http.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-from kybra import blob, Func, nat, nat64, opt, Query, Record, Variant
-from typing import TypeAlias
+from kybra import blob, Func, nat, nat64, null, Opt, Query, Record, Variant, Vec
 
 
 class HttpMethod(Variant, total=False):
-    get: None
-    head: None
-    post: None
+    get: null
+    head: null
+    post: null
 
 
 class HttpHeader(Record):
     name: str
     value: str
 
 
 class HttpResponse(Record):
     status: nat
-    headers: list[HttpHeader]
+    headers: Vec[HttpHeader]
     body: blob
 
 
 class HttpTransformArgs(Record):
     response: HttpResponse
     context: blob
 
 
-HttpTransformFunc: TypeAlias = Func(Query[[HttpTransformArgs], HttpResponse])
+HttpTransformFunc = Func(Query[[HttpTransformArgs], HttpResponse])
 
 
 class HttpTransform(Record):
     function: HttpTransformFunc
     context: blob
 
 
 class HttpRequestArgs(Record):
     url: str
-    max_response_bytes: opt[nat64]
+    max_response_bytes: Opt[nat64]
     method: HttpMethod
-    headers: list[HttpHeader]
-    body: opt[blob]
-    transform: opt[HttpTransform]
+    headers: Vec[HttpHeader]
+    body: Opt[blob]
+    transform: Opt[HttpTransform]
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/custom_modules/typing.py` & `kybra-0.5.0rc0/kybra/compiler/custom_modules/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 # This file has been modified from the RustPython code, which was most likely created mostly from the CPython code
 # The license to CPython can be found here: kybra/licenses/CPYTHON_LICENSE
 # The license to RustPython can be found here: kybra/licenses/RUST_PYTHON_LICENSE
 
 import sys
 
+class Annotated():
+    def __class_getitem__(cls, x):
+        return cls
+
 class Optional():
     def __class_getitem__(cls, x):
         return cls
 
 class Callable():
     def __class_getitem__(cls, x):
         return True
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/install_rust_dependencies.sh` & `kybra-0.5.0rc0/kybra/compiler/install_rust_dependencies.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 #!/bin/bash
 
 # TODO If we want to save a little bit of time we might be able to instruct rustup to not install some components initially, like clippy and docs
-# TODO we might want to implement all of this in Node.js in the future for platform-independence etc
-# TODO once ic-cdk-optimizer and ic-wasm are no longer required, we can probably just check for the wasm32-unknown-unknown target being installed: $global_kybra_rustup_bin target list | grep -q "wasm32-unknown-unknown (installed)"
+# TODO we might want to implement all of this in Python/Rust in the future for platform-independence etc
+# TODO once ic-wasm is no longer required, we can probably just check for the wasm32-wasi target being installed: $global_kybra_rustup_bin target list | grep -q "wasm32-wasi (installed)"
 
 kybra_version="$1"
 rust_version="$2"
 
-global_kybra_config_dir=~/.config/kybra/"$kybra_version"
-global_kybra_bin_dir="$global_kybra_config_dir"/bin
-global_kybra_cargo_bin="$global_kybra_bin_dir"/cargo
-global_kybra_logs_dir="$global_kybra_config_dir"/logs
-global_kybra_rustup_bin="$global_kybra_bin_dir"/rustup
-
-export CARGO_HOME="$global_kybra_config_dir"
-export RUSTUP_HOME="$global_kybra_config_dir"
+global_kybra_config_dir=~/.config/kybra
+global_kybra_rust_dir="$global_kybra_config_dir"/rust/"$rust_version"
+global_kybra_rust_bin_dir="$global_kybra_rust_dir"/bin
+global_kybra_logs_dir="$global_kybra_rust_dir"/logs
+global_kybra_cargo_bin="$global_kybra_rust_bin_dir"/cargo
+global_kybra_rustup_bin="$global_kybra_rust_bin_dir"/rustup
+
+export CARGO_TARGET_DIR="$global_kybra_config_dir"/rust/target
+export CARGO_HOME="$global_kybra_rust_dir"
+export RUSTUP_HOME="$global_kybra_rust_dir"
 
 function run() {
-    ic_wasm_already_installed=$(test -e "$global_kybra_bin_dir"/ic-wasm; echo $?)
-    ic_cdk_optimizer_already_installed=$(test -e "$global_kybra_bin_dir"/ic-cdk-optimizer; echo $?)
+    ic_wasm_already_installed=$(test -e "$global_kybra_rust_bin_dir"/ic-wasm; echo $?)
 
-    if [ "$ic_wasm_already_installed" -eq 1 ] || [ "$ic_cdk_optimizer_already_installed" -eq 1 ]; then
+    if [ "$ic_wasm_already_installed" -eq 1 ]; then
         echo -e "\nKybra "$kybra_version" prerequisite installation (this may take a few minutes)\n"
 
-        mkdir -p "$global_kybra_config_dir"
+        mkdir -p "$global_kybra_rust_dir"
         mkdir -p "$global_kybra_logs_dir"
 
         install_rustup
-        install_wasm32_unknown_unknown
+        install_wasm32
+        install_wasi2ic
         install_ic_wasm "$ic_wasm_already_installed"
-        install_ic_cdk_optimizer "$ic_cdk_optimizer_already_installed"
-        echo -e "\n"
     else
         update_rustup
     fi
 }
 
 function install_rustup() {
     echo -e "1/4) Installing Rust"
 
-    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- --no-modify-path -y --default-toolchain="$rust_version" &> "$global_kybra_logs_dir"/step_1_rust
+    curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- --no-modify-path -y --default-toolchain="$rust_version" &> "$global_kybra_logs_dir"/install_rustup
 }
 
 function update_rustup() {
     "$global_kybra_rustup_bin" update "$rust_version" &> "$global_kybra_logs_dir"/rustup_update
 }
 
-function install_wasm32_unknown_unknown() {
-    echo -e "2/4) Installing wasm32-unknown-unknown"
+function install_wasm32() {
+    echo -e "2/4) Installing wasm32"
 
-    "$global_kybra_rustup_bin" target add wasm32-unknown-unknown &> "$global_kybra_logs_dir"/step_2_wasm32_unknown_unknown
+    "$global_kybra_rustup_bin" target add wasm32-wasi &> "$global_kybra_logs_dir"/install_wasm32_wasi
+    "$global_kybra_rustup_bin" target add wasm32-unknown-unknown &> "$global_kybra_logs_dir"/install_wasm32_unknown_unknown
 }
 
-function install_ic_wasm() {
-    echo -e "3/4) Installing ic-wasm"
+function install_wasi2ic() {
+    echo -e "3/4) Installing wasi2ic"
 
-    if [ "$1" -eq 1 ]; then
-        "$global_kybra_cargo_bin" install ic-wasm --version 0.3.0 &> "$global_kybra_logs_dir"/step_3_ic_wasm
-    fi
+    "$global_kybra_cargo_bin" install --git https://github.com/wasm-forge/wasi2ic --rev 7418e0bd1a7810c8e9c55cc0155c921503a793b8 &> "$global_kybra_logs_dir"/install_wasi2ic
 }
 
-function install_ic_cdk_optimizer() {
-    echo -e "4/4) Installing ic-cdk-optimizer"
+function install_ic_wasm() {
+    echo -e "4/4) Installing ic-wasm"
 
     if [ "$1" -eq 1 ]; then
-        "$global_kybra_cargo_bin" install ic-cdk-optimizer --version 0.3.4  &> "$global_kybra_logs_dir"/step_4_ic_cdk_optimizer
+        "$global_kybra_cargo_bin" install ic-wasm --version 0.3.6 &> "$global_kybra_logs_dir"/install_ic_wasm
     fi
 }
 
 run
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/errors.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/errors/compiler_output.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,85 @@
 use annotate_snippets::{
     display_list::{DisplayList, FormatOptions},
     snippet::{Annotation, AnnotationType, Slice, Snippet, SourceAnnotation},
 };
-use std::fmt;
 
+use crate::source_map::GetSourceInfo;
+
+#[derive(Clone, Debug)]
 pub struct Suggestion {
     pub title: String,
-    pub source: String,
-    pub range: (usize, usize),
+    pub source: Option<String>,
+    pub range: Option<(usize, usize)>,
     pub annotation: Option<String>,
     pub import_suggestion: Option<String>,
 }
 
-pub struct Message {
+#[derive(Clone, Debug)]
+pub struct CompilerOutput {
     pub title: String,
-    pub origin: String,
-    pub line_number: usize,
-    pub source: String,
-    pub range: (usize, usize),
+    pub location: Location,
     pub annotation: String,
     pub suggestion: Option<Suggestion>,
 }
 
-pub struct WarningMessage {
-    pub message: Message,
-}
-
-pub struct ErrorMessage {
-    pub message: Message,
-}
-
-impl ErrorMessage {
-    fn to_string(&self) -> String {
-        self.message.to_string(AnnotationType::Error)
-    }
+#[derive(Clone, Debug)]
+pub struct Location {
+    pub origin: String,
+    pub line_number: usize,
+    pub source: String,
+    pub range: (usize, usize),
 }
 
-impl WarningMessage {
-    fn to_string(&self) -> String {
-        self.message.to_string(AnnotationType::Warning)
-    }
+pub trait CreateLocation {
+    fn create_location(&self) -> Location;
 }
 
-impl Message {
-    fn to_string(&self, annotation_type: AnnotationType) -> String {
+impl CompilerOutput {
+    pub fn to_string(&self, annotation_type: AnnotationType) -> String {
         let error_snippet = Snippet {
             title: Some(Annotation {
                 label: Some(&self.title),
                 id: None,
                 annotation_type,
             }),
             footer: vec![],
             slices: vec![Slice {
-                source: &self.source,
-                line_start: self.line_number,
-                origin: Some(&self.origin),
+                source: &self.location.source,
+                line_start: self.location.line_number,
+                origin: Some(&self.location.origin),
                 fold: true,
                 annotations: vec![SourceAnnotation {
                     label: &self.annotation,
                     annotation_type,
-                    range: self.range,
+                    range: self.location.range,
                 }],
             }],
             opt: FormatOptions {
                 color: true,
                 ..Default::default()
             },
         };
 
         match &self.suggestion {
             None => format!("{}", DisplayList::from(error_snippet)),
             Some(suggestion) => {
+                let suggestion_source = suggestion.source.clone().unwrap_or(Default::default());
                 let suggestion_slice = Slice {
-                    source: &suggestion.source,
-                    line_start: self.line_number,
+                    source: suggestion_source.as_str(),
+                    line_start: self.location.line_number,
                     origin: None,
                     fold: false,
                     annotations: vec![SourceAnnotation {
                         label: match &suggestion.annotation {
                             Some(annotation) => &annotation,
                             None => "",
                         },
                         annotation_type: AnnotationType::Help,
-                        range: suggestion.range,
+                        range: suggestion.range.unwrap_or(Default::default()),
                     }],
                 };
                 let slices = match &suggestion.import_suggestion {
                     Some(import) => vec![
                         Slice {
                             source: &import,
                             line_start: 1,
@@ -119,18 +112,20 @@
                     DisplayList::from(suggestion_snippet)
                 )
             }
         }
     }
 }
 
-impl fmt::Display for ErrorMessage {
-    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "{}", self.to_string())
-    }
-}
-
-impl fmt::Display for WarningMessage {
-    fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "{}", self.to_string())
+impl<T> CreateLocation for T
+where
+    T: GetSourceInfo,
+{
+    fn create_location(&self) -> Location {
+        return Location {
+            origin: self.get_origin(),
+            line_number: self.get_line_number(),
+            source: "".to_string(),
+            range: (0, 0),
+        };
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/mod.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/notify_functions.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_functions.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,90 @@
 use cdk_framework::{
-    nodes::{ActExternalCanister, ActExternalCanisterMethod},
-    ToTokenStream,
+    act::node::{
+        candid::{service::Method, Service},
+        Context,
+    },
+    traits::ToTypeAnnotation,
 };
 use proc_macro2::TokenStream;
 use quote::{format_ident, quote};
 
-use crate::generators::tuple;
+use crate::{keywords, tuple};
 
-pub fn generate_notify_functions(
-    external_canisters: &Vec<ActExternalCanister>,
-) -> Vec<TokenStream> {
-    external_canisters.iter().map(|canister| {
-        canister.methods.iter().map(|method| {
-            let function_name_string = format!("_kybra_notify_{}_{}", canister.name, method.name);
-            let real_function_name = format_ident!("{}", function_name_string);
-            let wrapper_fn_name = format_ident!("{}_wrapper", function_name_string);
-            let param_variable_definitions = generate_param_variables(method);
-            let param_names = method.params.iter().map(|param| {
-                let name = format_ident!("{}", param.prefixed_name());
-                quote!{#name}
-            }).collect();
-            let params = tuple::generate_tuple(&param_names);
-
-            quote!{
-                #[pymethod]
-                fn #wrapper_fn_name(&self, args_py_object_refs: Vec<PyObjectRef>, vm: &VirtualMachine) -> PyObjectRef {
-                    let canister_id_principal: ic_cdk::export::Principal = args_py_object_refs[0].clone().try_from_vm_value(vm).unwrap();
-
-                    #(#param_variable_definitions)*
-
-                    let notify_result = #real_function_name(
-                        canister_id_principal,
-                        #params
-                    );
-
-                    notify_result.try_into_vm_value(vm).unwrap()
-                }
-            }
-        }).collect()
-    }).collect::<Vec<Vec<TokenStream>>>().concat()
+pub fn generate(services: &Vec<Service>) -> Vec<TokenStream> {
+    services
+        .iter()
+        .map(|canister| {
+            canister
+                .methods
+                .iter()
+                .map(|method| {
+                    let function_name_string = format!("notify_{}_{}", canister.name, method.name);
+                    let real_function_name = format_ident!("{}", function_name_string);
+                    let wrapper_fn_name = format_ident!("{}_wrapper", function_name_string);
+                    let param_variable_definitions =
+                        generate_param_variables(method, &canister.name);
+                    let param_names = method
+                        .params
+                        .iter()
+                        .map(|param| {
+                            let name = format_ident!("{}", param.get_prefixed_name());
+                            quote! {#name}
+                        })
+                        .collect();
+                    let params = tuple::generate_tuple(&param_names);
+
+                    quote! {
+                        #[pymethod]
+                        fn #wrapper_fn_name(
+                            &self,
+                            args_py_object_refs: Vec<rustpython_vm::PyObjectRef>,
+                            vm: &rustpython_vm::VirtualMachine
+                        ) -> rustpython_vm::PyResult {
+                            let canister_id_principal: ic_cdk::export::Principal = args_py_object_refs[0]
+                                .clone()
+                                .try_from_vm_value(vm)
+                                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+
+                            #(#param_variable_definitions)*
+
+                            let notify_result = #real_function_name(
+                                canister_id_principal,
+                                #params
+                            );
+
+                            notify_result
+                                .try_into_vm_value(vm)
+                                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
+                        }
+                    }
+                })
+                .collect()
+        })
+        .collect::<Vec<Vec<TokenStream>>>()
+        .concat()
 }
 
-fn generate_param_variables(method: &ActExternalCanisterMethod) -> Vec<TokenStream> {
-    method.params.iter().enumerate().map(|(index, act_fn_param)| {
-        let variable_name = format_ident!("{}", act_fn_param.prefixed_name());
-        let variable_type = act_fn_param.data_type.to_token_stream(&crate::get_python_keywords());
-        let actual_index = index + 2;
-
-        quote! {
-            let #variable_name: #variable_type = args_py_object_refs[#actual_index].clone().try_from_vm_value(vm).unwrap();
-        }
-    }).collect()
+fn generate_param_variables(method: &Method, canister_name: &String) -> Vec<TokenStream> {
+    method
+        .params
+        .iter()
+        .enumerate()
+        .map(|(index, param)| {
+            let variable_name = format_ident!("{}", param.get_prefixed_name());
+            let context = Context {
+                keyword_list: keywords::get_python_keywords(),
+                cdk_name: "kybra".to_string(),
+            };
+            let variable_type =
+                param.to_type_annotation(&context, method.create_qualified_name(canister_name));
+            let actual_index = index + 2;
+
+            quote! {
+                let #variable_name: #variable_type = args_py_object_refs[#actual_index]
+                    .clone()
+                    .try_from_vm_value(vm)
+                    .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+            }
+        })
+        .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/contains_key.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/contains_key.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,61 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_contains_key(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_contains_key(&self, memory_id_py_object_ref: PyObjectRef, key_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_contains_key(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            key_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
                 #(#match_arms)*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident = stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
-            let (key_wrapper_type_name, _) = stable_b_tree_map::generate_wrapper_type(&stable_b_tree_map_node.key_type, memory_id, "Key");
+            let (key_wrapper_type_name, _) =
+                rust::wrapper_type::generate(&stable_b_tree_map_node.key_type, memory_id, "Key");
 
             quote! {
                 #memory_id => {
-                    #map_name_ident.with(|p| p.borrow().contains_key(&#key_wrapper_type_name(key_py_object_ref.try_from_vm_value(vm).unwrap()))).try_into_vm_value(vm).unwrap()
+                    let key = #key_wrapper_type_name(
+                        key_py_object_ref
+                            .try_from_vm_value(vm)
+                            .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?,
+                    );
+
+                    #stable_b_tree_map_ref_cell
+                        .with(|map_ref_cell| map_ref_cell.borrow().contains_key(&key))
+                        .try_into_vm_value(vm)
+                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
                 }
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/get.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/get.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,63 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_get(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_get(&self, memory_id_py_object_ref: PyObjectRef, key_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_get(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            key_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
                 #(#match_arms)*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident = stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
-            let (key_wrapper_type_name, _) = stable_b_tree_map::generate_wrapper_type(&stable_b_tree_map_node.key_type, memory_id, "Key");
+            let (key_wrapper_type_name, _) =
+                rust::wrapper_type::generate(&stable_b_tree_map_node.key_type, memory_id, "Key");
 
             quote! {
                 #memory_id => {
-                    match #map_name_ident.with(|p| p.borrow().get(&#key_wrapper_type_name(key_py_object_ref.try_from_vm_value(vm).unwrap()))) {
-                        Some(value) => value.0.try_into_vm_value(vm).unwrap(),
-                        None => vm.ctx.none()
-                    }
+                    let key = #key_wrapper_type_name(
+                        key_py_object_ref
+                            .try_from_vm_value(vm)
+                            .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?
+                    );
+
+                    // TODO: Once we have a more complex opt type we will need
+                    // to update this, the Python side, the tests, and the documentation.
+                    #stable_b_tree_map_ref_cell
+                        .with(|map_ref_cell| map_ref_cell.borrow().get(&key))
+                        .try_into_vm_value(vm)
+                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
                 }
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/insert.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/items.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,80 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_insert(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_insert(&self, memory_id_py_object_ref: PyObjectRef, key_py_object_ref: PyObjectRef, value_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_items(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
-                #(#match_arms),*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                #(#match_arms)*
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let stable_b_tree_map_ref_cell = stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
-            let (key_wrapper_type_name, _) = stable_b_tree_map::generate_wrapper_type(&stable_b_tree_map_node.key_type, memory_id, "Key");
-            let (value_wrapper_type_name, _) = stable_b_tree_map::generate_wrapper_type(&stable_b_tree_map_node.value_type, memory_id, "Value");
-
-            // TODO the return value here might need a little work like in get
             quote! {
                 #memory_id => {
-                    let key = #key_wrapper_type_name(key_py_object_ref.try_from_vm_value(vm).unwrap());
-                    let value = #value_wrapper_type_name(value_py_object_ref.try_from_vm_value(vm).unwrap());
-
-                    let result = #stable_b_tree_map_ref_cell.with(|stable_b_tree_map_ref_cell| {
-                        stable_b_tree_map_ref_cell
-                            .borrow_mut()
-                            .insert(key, value)
-                    });
-
-                    let insert_result_class = _kybra_unwrap_rust_python_result(vm.run_block_expr(
-                    vm.new_scope_with_builtins(),
-                        r#"
-from kybra import InsertResult
-
-InsertResult
-                        "#
-                    ), vm);
-
-                    match result {
-                        Ok(ok) => {
-                            let method_result = vm.invoke(&insert_result_class, (ok.try_into_vm_value(vm).unwrap(), vm.ctx.none()));
-
-                            _kybra_unwrap_rust_python_result(method_result, vm)
-
-                            // TODO Consider using dict once we are on Python 3.11: https://github.com/python/cpython/issues/89026
-                            // let dict = vm.ctx.new_dict();
-
-                            // dict.set_item("ok", ok.try_into_vm_value(vm).unwrap(), vm);
-
-                            // dict
-                        },
-                        Err(err) => {
-                            let method_result = vm.invoke(&insert_result_class, (vm.ctx.none(), err.try_into_vm_value(vm).unwrap()));
-                            _kybra_unwrap_rust_python_result(method_result, vm)
-
-                            // TODO Consider using dict once we are on Python 3.11: https://github.com/python/cpython/issues/89026
-                            // let dict = vm.ctx.new_dict();
-
-                            // dict.set_item("err", err_string.try_into_vm_value(vm).unwrap(), vm);
+                    #stable_b_tree_map_ref_cell
+                        .with(|map_ref_cell| {
+                            let (key_value_pairs, type_errors) = map_ref_cell
+                                .borrow()
+                                .iter()
+                                .map(|(key_wrapper_type, value_wrapper_type)| -> Result<
+                                    rustpython_vm::PyObjectRef,
+                                    rustpython_vm::builtins::PyBaseExceptionRef
+                                > {
+                                    let key = key_wrapper_type.0
+                                        .try_into_vm_value(vm)
+                                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+
+                                    let value = value_wrapper_type.0
+                                        .try_into_vm_value(vm)
+                                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+
+                                    Ok(vm.ctx.new_tuple(vec![key, value]).into())
+                                })
+                                .fold((vec![], vec![]), |mut acc, result| {
+                                    match result {
+                                        Ok(key_value_pair) => acc.0.push(key_value_pair),
+                                        Err(type_error) => acc.1.push(type_error),
+                                    }
+                                    acc
+                                });
+
+                            if type_errors.is_empty() {
+                                return Ok(vm.ctx.new_list(key_value_pairs).into());
+                            }
 
-                            // dict
-                        }
-                    }
+                            Err(type_errors[0].clone())
+                        })
                 }
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/is_empty.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/is_empty.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,51 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_is_empty(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_is_empty(&self, memory_id_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_is_empty(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
                 #(#match_arms)*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident =
-                stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
             quote! {
                 #memory_id => {
-                    #map_name_ident.with(|p| p.borrow().is_empty()).try_into_vm_value(vm).unwrap()
+                    #stable_b_tree_map_ref_cell
+                        .with(|map_ref_cell| map_ref_cell.borrow().is_empty())
+                        .try_into_vm_value(vm)
+                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
                 }
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/keys.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/mod.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-use quote::quote;
+use proc_macro2::TokenStream;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::StableBTreeMapNode;
 
-pub fn generate_stable_b_tree_map_keys(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
-    let match_arms = generate_match_arms(stable_b_tree_map_nodes);
-
-    quote! {
-        #[pymethod]
-        fn _kybra_stable_b_tree_map_keys(&self, memory_id_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> Vec<PyObjectRef> {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
-
-            match memory_id {
-                #(#match_arms)*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
-            }
-        }
+pub mod contains_key;
+pub mod get;
+pub mod insert;
+pub mod is_empty;
+pub mod items;
+pub mod keys;
+pub mod len;
+pub mod remove;
+pub mod values;
+
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
+    let contains_key = contains_key::generate(stable_b_tree_map_nodes);
+    let get = get::generate(stable_b_tree_map_nodes);
+    let insert = insert::generate(stable_b_tree_map_nodes);
+    let is_empty = is_empty::generate(stable_b_tree_map_nodes);
+    let items = items::generate(stable_b_tree_map_nodes);
+    let keys = keys::generate(stable_b_tree_map_nodes);
+    let len = len::generate(stable_b_tree_map_nodes);
+    let remove = remove::generate(stable_b_tree_map_nodes);
+    let values = values::generate(stable_b_tree_map_nodes);
+
+    quote::quote! {
+        #contains_key
+        #get
+        #insert
+        #is_empty
+        #items
+        #keys
+        #len
+        #remove
+        #values
     }
 }
-
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
-    stable_b_tree_map_nodes
-        .iter()
-        .map(|stable_b_tree_map_node| {
-            let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident = stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
-
-            quote! {
-                #memory_id => {
-                    #map_name_ident.with(|p| p.borrow().iter().map(|(key_wrapper_type, _)| key_wrapper_type.0.try_into_vm_value(vm).unwrap()).collect())
-                }
-            }
-        })
-        .collect()
-}
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/len.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/len.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,49 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_len(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_len(&self, memory_id_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_len(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
                 #(#match_arms)*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident =
-                stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
             quote! {
-                #memory_id => {
-                    #map_name_ident.with(|p| p.borrow().len()).try_into_vm_value(vm).unwrap()
-                }
+                #memory_id => #stable_b_tree_map_ref_cell
+                    .with(|map_ref_cell| map_ref_cell.borrow().len())
+                    .try_into_vm_value(vm)
+                    .map_err(|vmc_err| vm.new_type_error(vmc_err.0)),
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/ic_object/functions/stable_b_tree_map/remove.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/stable_b_tree_map/values.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,71 @@
+use proc_macro2::TokenStream;
 use quote::quote;
 
-use crate::{generators::stable_b_tree_map, py_ast::kybra_types::StableBTreeMapNode};
+use crate::{stable_b_tree_map_nodes::rust, StableBTreeMapNode};
 
-pub fn generate_stable_b_tree_map_remove(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> proc_macro2::TokenStream {
+pub fn generate(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> TokenStream {
     let match_arms = generate_match_arms(stable_b_tree_map_nodes);
 
     quote! {
         #[pymethod]
-        fn _kybra_stable_b_tree_map_remove(&self, memory_id_py_object_ref: PyObjectRef, key_py_object_ref: PyObjectRef, vm: &VirtualMachine) -> PyObjectRef {
-            let memory_id: u8 = memory_id_py_object_ref.try_from_vm_value(vm).unwrap();
+        fn stable_b_tree_map_values(
+            &self,
+            memory_id_py_object_ref: rustpython_vm::PyObjectRef,
+            vm: &rustpython_vm::VirtualMachine
+        ) -> rustpython_vm::PyResult {
+            let memory_id: u8 = memory_id_py_object_ref
+                .try_from_vm_value(vm)
+                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
 
             match memory_id {
-                #(#match_arms),*
-                _ => panic!("memory_id {} does not have an associated StableBTreeMap", memory_id)
+                #(#match_arms)*
+                // TODO: Consider creating a custom error or using
+                // IndexError, KeyError, or ValueError
+                _ => Err(vm.new_lookup_error(format!(
+                    "memory_id {} does not have an associated StableBTreeMap",
+                    memory_id
+                )))
             }
         }
     }
 }
 
-fn generate_match_arms(
-    stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>,
-) -> Vec<proc_macro2::TokenStream> {
+fn generate_match_arms(stable_b_tree_map_nodes: &Vec<StableBTreeMapNode>) -> Vec<TokenStream> {
     stable_b_tree_map_nodes
         .iter()
         .map(|stable_b_tree_map_node| {
             let memory_id = stable_b_tree_map_node.memory_id;
-            let map_name_ident = stable_b_tree_map::ref_cell_ident(stable_b_tree_map_node.memory_id);
-
-            let (key_wrapper_type_name, _) = stable_b_tree_map::generate_wrapper_type(&stable_b_tree_map_node.key_type, memory_id, "Key");
+            let stable_b_tree_map_ref_cell =
+                rust::ref_cell_ident::generate(stable_b_tree_map_node.memory_id);
 
             quote! {
                 #memory_id => {
-                    match #map_name_ident.with(|p| p.borrow_mut().remove(&#key_wrapper_type_name(key_py_object_ref.try_from_vm_value(vm).unwrap()))) {
-                        Some(value) => value.0.try_into_vm_value(vm).unwrap(),
-                        None => vm.ctx.none()
-                    }
+                    #stable_b_tree_map_ref_cell
+                        .with(|map_ref_cell| {
+                            let (values, type_errors) = map_ref_cell
+                                .borrow()
+                                .iter()
+                                .map(|(_, value_wrapper_type)| {
+                                    value_wrapper_type.0
+                                        .try_into_vm_value(vm)
+                                        .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
+                                })
+                                .fold((vec![], vec![]), |mut acc, result| {
+                                    match result {
+                                        Ok(value) => acc.0.push(value),
+                                        Err(type_error) => acc.1.push(type_error),
+                                    }
+                                    acc
+                                });
+
+                                if type_errors.is_empty() {
+                                    return Ok(vm.ctx.new_list(values).into());
+                                }
+
+                                Err(type_errors[0].clone())
+                        })
                 }
             }
         })
         .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/basic.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/generic.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,46 @@
-pub fn generate_basic_impls() -> proc_macro2::TokenStream {
-    quote::quote! {
-        impl CdkActTryFromVmValue<(), &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<(), CdkActTryFromVmValueError> {
-                Ok(())
-            }
-        }
+use proc_macro2::TokenStream;
 
-        impl CdkActTryFromVmValue<bool, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<bool, CdkActTryFromVmValueError> {
-                match self.try_into_value(vm) {
-                    Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to bool".to_string())) // TODO consider using the try_into_value err
+pub fn generate() -> TokenStream {
+    quote::quote! {
+        impl<T> CdkActTryFromVmValue<(T,), &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        where
+            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+        {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<(T,), CdkActTryFromVmValueError> {
+                match self.try_from_vm_value(vm) {
+                    Ok(value) => Ok((value,)),
+                    Err(_) => Err(CdkActTryFromVmValueError("TypeError: Could not convert value to tuple".to_string()))
                 }
             }
         }
 
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Empty, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Empty, CdkActTryFromVmValueError> {
-                panic!("PyObjectRef cannot be converted into Empty");
-            }
-        }
-
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Func, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Func, CdkActTryFromVmValueError> {
-                let tuple_self: PyTupleRef = _kybra_unwrap_rust_python_result(self.try_into_value(vm), vm);
-                let principal = tuple_self.get(0).unwrap();
-                let method = tuple_self.get(1).unwrap();
-
-                Ok(ic_cdk::export::candid::Func {
-                    principal: principal.clone().try_from_vm_value(vm).unwrap(),
-                    method: method.clone().try_from_vm_value(vm).unwrap()
-                })
-            }
-        }
-
-        impl CdkActTryFromVmValue<ic_cdk::export::Principal, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::Principal, CdkActTryFromVmValueError> {
-                let to_str = _kybra_unwrap_rust_python_result(self.get_attr("to_str", vm), vm);
-                let result = _kybra_unwrap_rust_python_result(vm.invoke(&to_str, ()), vm);
-                let result_string: String = _kybra_unwrap_rust_python_result(result.try_into_value(vm), vm);
-                Ok(ic_cdk::export::Principal::from_text(result_string).unwrap())
-            }
-        }
-
-        impl CdkActTryFromVmValue<ic_cdk::export::candid::Reserved, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Reserved, CdkActTryFromVmValueError> {
-                Ok(ic_cdk::export::candid::Reserved)
-            }
-        }
-
-        impl CdkActTryFromVmValue<ic_cdk::timer::TimerId, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::timer::TimerId, CdkActTryFromVmValueError> {
-                let vm_value_as_u64: u64 = _kybra_unwrap_rust_python_result(self.try_into_value(vm), vm);
-                Ok(ic_cdk::timer::TimerId::from(slotmap::KeyData::from_ffi(vm_value_as_u64)))
+        impl<T> CdkActTryFromVmValue<Box<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        where
+            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+        {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Box<T>, CdkActTryFromVmValueError> {
+                match self.try_from_vm_value(vm) {
+                    Ok(value) => Ok(Box::new(value)),
+                    Err(err) => Err(err)
+                }
             }
         }
 
-        impl CdkActTryFromVmValue<String, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<String, CdkActTryFromVmValueError> {
-                match self.try_into_value(vm) {
-                    Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to String".to_string())) // TODO consider using the try_into_value err
+        impl<T> CdkActTryFromVmValue<Option<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        where
+            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+        {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Option<T>, CdkActTryFromVmValueError> {
+                if self.is(&vm.ctx.none()) {
+                    Ok(None)
+                }
+                else {
+                    match self.try_from_vm_value(vm) {
+                        Ok(value) => Ok(Some(value)),
+                        Err(err) => Err(err)
+                    }
                 }
             }
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/generic.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/generic.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-pub fn generate_generic_impls() -> proc_macro2::TokenStream {
+use proc_macro2::TokenStream;
+
+pub fn generate() -> TokenStream {
     quote::quote! {
-        impl<T> CdkActTryFromVmValue<(T,), &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        impl<T> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for (T,)
         where
-            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+            T : for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>,
         {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<(T,), CdkActTryFromVmValueError> {
-                Ok((self.try_from_vm_value(vm).unwrap(),))
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                self.0.try_into_vm_value(vm)
             }
         }
 
-        impl<T> CdkActTryFromVmValue<Box<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        impl<T> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Box<T>
         where
-            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+            T : for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>,
         {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Box<T>, CdkActTryFromVmValueError> {
-                match self.try_from_vm_value(vm) {
-                    Ok(value) => Ok(Box::new(value)),
-                    Err(err) => Err(err)
-                }
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                (*self).try_into_vm_value(vm)
             }
         }
 
-        impl<T> CdkActTryFromVmValue<Option<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
+        impl<T> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Option<T>
         where
-            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
+            T: for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
         {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Option<T>, CdkActTryFromVmValueError> {
-                if self.is(&vm.ctx.none()) {
-                    Ok(None)
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                match self {
+                    Some(value) => value.try_into_vm_value(vm),
+                    None => Ok(().to_pyobject(vm))
                 }
-                else {
-                    match self.try_from_vm_value(vm) {
-                        Ok(value) => Ok(Some(value)),
-                        Err(err) => Err(err)
+            }
+        }
+
+        impl<T, K> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Result<T, K>
+        where
+            T: for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>,
+            K: for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
+        {
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                match self {
+                    Ok(ok) => {
+                        let dict = vm.ctx.new_dict();
+
+                        dict.set_item("Ok", ok.try_into_vm_value(vm)?, vm);
+
+                        Ok(dict.into())
+                    },
+                    Err(err) => {
+                        let dict = vm.ctx.new_dict();
+
+                        dict.set_item("Err", err.try_into_vm_value(vm)?, vm);
+
+                        Ok(dict.into())
                     }
                 }
             }
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/numeric.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/numeric.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,142 +1,165 @@
-pub fn generate_numeric_impls() -> proc_macro2::TokenStream {
+use proc_macro2::TokenStream;
+
+pub fn generate() -> TokenStream {
     quote::quote! {
         impl CdkActTryFromVmValue<f64, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<f64, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to f64".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to f64".to_string()))
+                }
+            }
+        }
+
+        impl CdkActTryFromVmValue<_CdkFloat64, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<_CdkFloat64, CdkActTryFromVmValueError> {
+                match self.try_into_value(vm) {
+                    Ok(value) => Ok(_CdkFloat64(value)),
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to _CdkFloat64".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<f32, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<f32, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to f32".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to f32".to_string()))
+                }
+            }
+        }
+
+        impl CdkActTryFromVmValue<_CdkFloat32, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<_CdkFloat32, CdkActTryFromVmValueError> {
+                match self.try_into_value(vm) {
+                    Ok(value) => Ok(_CdkFloat32(value)),
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to _CdkFloat32".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<ic_cdk::export::candid::Int, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Int, CdkActTryFromVmValueError> {
-                let int_result: Result<PyIntRef, _> = self.try_into_value(vm);
+                let int_result: Result<rustpython_vm::builtins::PyIntRef, _> = self.try_into_value(vm);
 
                 match int_result {
                     Ok(int) => Ok(ic_cdk::export::candid::Int(int.as_bigint().clone())),
-                    Err(_) => Err(CdkActTryFromVmValueError("PyObjectRef is not a PyIntRef".to_string()))
+                    Err(_) => Err(CdkActTryFromVmValueError("TypeError: PyObjectRef is not a PyIntRef".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i128, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<i128, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to i128".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to i128".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i64, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<i64, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to i64".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to i64".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i32, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<i32, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to i32".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to i32".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i16, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<i16, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to i16".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to i16".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<i8, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<i8, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to i8".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to i8".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<ic_cdk::export::candid::Nat, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Nat, CdkActTryFromVmValueError> {
-                let int_result: Result<PyIntRef, _> = self.try_into_value(vm);
+                let int_result: Result<rustpython_vm::builtins::PyIntRef, _> = self.try_into_value(vm);
 
                 match int_result {
-                    Ok(int) => Ok(ic_cdk::export::candid::Nat::from_str(&int.as_bigint().to_string()).unwrap()), // TODO probably not the best conversion
+                    Ok(int) => match ic_cdk::export::candid::Nat::from_str(&int.as_bigint().to_string()) { // TODO probably not the best conversion
+                        Ok(nat) => Ok(nat),
+                        Err(_) => Err(CdkActTryFromVmValueError("TypeError: Could not convert value to nat".to_string()))
+                    },
                     Err(_) => Err(CdkActTryFromVmValueError("PyObjectRef is not a PyIntRef".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<u128, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<u128, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to u128".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to u128".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<u64, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<u64, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to u64".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to u64".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<usize, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<usize, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to usize".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to usize".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<u32, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<u32, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to u32".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to u32".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<u16, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<u16, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to u16".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to u16".to_string()))
                 }
             }
         }
 
         impl CdkActTryFromVmValue<u8, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<u8, CdkActTryFromVmValueError> {
                 match self.try_into_value(vm) {
                     Ok(value) => Ok(value),
-                    Err(err) => Err(CdkActTryFromVmValueError("Could not convert PyObjectRef to u8".to_string()))
+                    Err(err) => Err(CdkActTryFromVmValueError("TypeError: Could not convert PyObjectRef to u8".to_string()))
                 }
             }
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_from_vm_value/vec.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_from_vm_value_impls/basic.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,131 +1,115 @@
-pub fn generate_vec_impls() -> proc_macro2::TokenStream {
-    quote::quote! {
-        impl CdkActTryFromVmValue<Vec<bool>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<bool>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+use proc_macro2::TokenStream;
 
-        impl CdkActTryFromVmValue<Vec<String>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<String>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+pub fn generate() -> TokenStream {
+    quote::quote! {
+        impl CdkActTryFromVmValue<(), &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<(), CdkActTryFromVmValueError> {
+                if self.is(&vm.ctx.none()) {
+                    Ok(())
+                } else {
+                    let type_name = self.to_pyobject(vm).class().name().to_string();
 
-        impl CdkActTryFromVmValue<Vec<f64>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<f64>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+                    Err(CdkActTryFromVmValueError(format!("TypeError: expected NoneType but received {type_name}")))
+                }
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<f32>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<f32>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+        impl CdkActTryFromVmValue<bool, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<bool, CdkActTryFromVmValueError> {
+                let type_name = self.class().name().to_string();
 
-        impl CdkActTryFromVmValue<Vec<i128>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<i128>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+                match self.try_into_value(vm) {
+                    Ok(value) => Ok(value),
+                    Err(err) => Err(CdkActTryFromVmValueError(format!("TypeError: expected bool but received {type_name}"))) // TODO consider using the try_into_value err
+                }
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<i64>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<i64>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+        impl CdkActTryFromVmValue<ic_cdk::export::candid::Empty, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Empty, CdkActTryFromVmValueError> {
+                Err(CdkActTryFromVmValueError("TypeError: PyObjectRef cannot be converted into Empty".to_string()))
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<i32>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<i32>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+        impl CdkActTryFromVmValue<ic_cdk::export::candid::Func, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Func, CdkActTryFromVmValueError> {
+                let tuple_self: rustpython_vm::builtins::PyTupleRef = self
+                    .try_into_value(vm)
+                    .map_err(|err| err.to_cdk_act_try_from_vm_value_error(vm))?;
+                let principal = match tuple_self.get(0) {
+                    Some(principal) => principal,
+                    None => return Err(CdkActTryFromVmValueError("TypeError: could not convert value to Func, missing Principal".to_string()))
+                };
+                let method = match tuple_self.get(1) {
+                    Some(method) => method,
+                    None => return Err(CdkActTryFromVmValueError("TypeError: could not convert value to Func, missing method".to_string()))
+                };
 
-        impl CdkActTryFromVmValue<Vec<i16>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<i16>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+                Ok(ic_cdk::export::candid::Func {
+                    principal: principal.clone().try_from_vm_value(vm)?,
+                    method: method.clone().try_from_vm_value(vm)?
+                })
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<i8>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<i8>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+        impl CdkActTryFromVmValue<ic_cdk::export::Principal, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::Principal, CdkActTryFromVmValueError> {
+                let to_str = self.get_attr("to_str", vm)
+                    .map_err(|err| err.to_cdk_act_try_from_vm_value_error(vm))?;
+                let result = to_str.call((), vm)
+                    .map_err(|err| err.to_cdk_act_try_from_vm_value_error(vm))?;
+                let result_string: String = result.try_into_value(vm)
+                    .map_err(|err| err.to_cdk_act_try_from_vm_value_error(vm))?;
+                match ic_cdk::export::Principal::from_text(result_string) {
+                    Ok(principal) => Ok(principal),
+                    Err(err) => Err(CdkActTryFromVmValueError(format!("TypeError: could not convert value to Principal: {}", err.to_string()))),
+                }
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<u128>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<u128>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+        impl CdkActTryFromVmValue<ic_cdk::export::candid::Reserved, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk::export::candid::Reserved, CdkActTryFromVmValueError> {
+                Ok(ic_cdk::export::candid::Reserved)
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<u64>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<u64>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+        impl CdkActTryFromVmValue<ic_cdk_timers::TimerId, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<ic_cdk_timers::TimerId, CdkActTryFromVmValueError> {
+                let vm_value_as_u64: u64 = self.try_into_value(vm)
+                    .map_err(|err| err.to_cdk_act_try_from_vm_value_error(vm))?;
+                Ok(ic_cdk_timers::TimerId::from(slotmap::KeyData::from_ffi(vm_value_as_u64)))
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<u32>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<u32>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+        impl CdkActTryFromVmValue<String, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<String, CdkActTryFromVmValueError> {
+                let type_name = self.class().name().to_string();
 
-        impl CdkActTryFromVmValue<Vec<u16>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<u16>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
+                match self.try_into_value(vm) {
+                    Ok(value) => Ok(value),
+                    Err(err) => {
+                        Err(CdkActTryFromVmValueError(format!("TypeError: expected str but received {type_name}"))) // TODO consider using the try_into_value err
+                    }
+                }
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<u8>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<u8>, CdkActTryFromVmValueError> {
-                Ok(_kybra_unwrap_rust_python_result(self.try_into_value(vm), vm))
-            }
-        }
+        impl CdkActTryFromVmValue<Result<(), String>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
+            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Result<(), String>, CdkActTryFromVmValueError> {
+                let err = self.get_item("Err", vm);
+                if let Ok(error_message) = err {
+                    return Ok(Err(error_message.try_from_vm_value(vm)?));
+                }
 
-        trait KybraTryFromVec {}
+                let ok = self.get_item("Ok", vm);
+                if let Ok(value) = ok {
+                    let result: () = value.try_from_vm_value(vm)?;
+                    return Ok(Ok(()))
+                }
 
-        impl<T> KybraTryFromVec for Vec<T> {}
-
-        impl KybraTryFromVec for () {}
-
-        impl<T> KybraTryFromVec for Option<T> {}
-
-        impl KybraTryFromVec for ic_cdk::export::candid::Empty {}
-
-        impl KybraTryFromVec for ic_cdk::export::candid::Reserved {}
-
-        impl KybraTryFromVec for ic_cdk::export::candid::Func {}
-
-        impl KybraTryFromVec for ic_cdk::export::Principal {}
-
-        impl KybraTryFromVec for ic_cdk::timer::TimerId {}
-
-        impl KybraTryFromVec for ic_cdk::export::candid::Int {}
-
-        impl KybraTryFromVec for ic_cdk::export::candid::Nat {}
-
-        impl<T> CdkActTryFromVmValue<Vec<T>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef
-        where
-            T: KybraTryFromVec,
-            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
-        {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<T>, CdkActTryFromVmValueError> {
-                try_from_vm_value_generic_array(self, vm)
+                let type_name = self.to_pyobject(vm).class().name().to_string();
+                Err(CdkActTryFromVmValueError(format!("TypeError: expected Result but received {type_name}")))
             }
         }
-
-        fn try_from_vm_value_generic_array<T>(py_object_ref: rustpython::vm::PyObjectRef, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<T>, CdkActTryFromVmValueError>
-        where
-            rustpython::vm::PyObjectRef: for<'a> CdkActTryFromVmValue<T, &'a rustpython::vm::VirtualMachine>
-        {
-            let py_list: PyListRef = _kybra_unwrap_rust_python_result(py_object_ref.try_into_value(vm), vm);
-            let vec = py_list.borrow_vec();
-
-            Ok(vec.iter().map(|item| {
-                item.clone().try_from_vm_value(vm).unwrap()
-            }).collect())
-        }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/basic.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/basic.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-pub fn generate_basic_impls() -> proc_macro2::TokenStream {
+use proc_macro2::TokenStream;
+
+pub fn generate() -> TokenStream {
     quote::quote! {
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for () {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.none())
             }
         }
 
@@ -10,128 +12,87 @@
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Empty {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
-                panic!("Empty cannot be converted into PyObjectRef");
+                Err(CdkActTryIntoVmValueError("type \"empty\" cannot be represented in python".to_string()))
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Func {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
-                Ok(vm.ctx.new_tuple(vec![self.principal.try_into_vm_value(vm).unwrap(), self.method.try_into_vm_value(vm).unwrap()]).into())
+                let principal = self.principal.try_into_vm_value(vm)?;
+                let method = self.method.try_into_vm_value(vm)?;
+                Ok(vm.ctx.new_tuple(vec![principal, method]).into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::Principal {
+            // TODO: In the future CdkActTryIntoVmValue needs to return rustpython_vm::object::PyResult
+            // When it does all these map_err calls will be unnecessary and should be replaced with
+            // question mark syntax.
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
-                let principal_class = _kybra_unwrap_rust_python_result(vm.run_block_expr(
+                let principal_class = vm.run_block_expr(
                     vm.new_scope_with_builtins(),
-                    r#"
-from kybra import Principal
-
-Principal
-                    "#
-                ), vm);
+                    "from kybra import Principal; Principal"
+                ).map_err(|err| err.to_cdk_act_try_into_vm_value_error(vm))?;
 
-                let from_str = _kybra_unwrap_rust_python_result(principal_class.get_attr("from_str", vm), vm);
-                let principal_instance = _kybra_unwrap_rust_python_result(vm.invoke(&from_str, (self.to_text(),)), vm);
+                let from_str = principal_class
+                    .get_attr("from_str", vm)
+                    .map_err(|err| err.to_cdk_act_try_into_vm_value_error(vm))?;
+                let principal_instance = from_str
+                    .call((self.to_text(),), vm)
+                    .map_err(|err| err.to_cdk_act_try_into_vm_value_error(vm))?;
 
                 Ok(principal_instance)
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::api::call::RejectionCode {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
-                match self {
-                    ic_cdk::api::call::RejectionCode::NoError => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("NoError", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::SysFatal => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("SysFatal", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::SysTransient => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("SysTransient", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::DestinationInvalid => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("DestinationInvalid", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::CanisterReject => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("CanisterReject", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::CanisterError => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("CanisterError", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::call::RejectionCode::Unknown => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("Unknown", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                }
+                let attribute = match self {
+                    ic_cdk::api::call::RejectionCode::NoError => "NoError",
+                    ic_cdk::api::call::RejectionCode::SysFatal => "SysFatal",
+                    ic_cdk::api::call::RejectionCode::SysTransient => "SysTransient",
+                    ic_cdk::api::call::RejectionCode::DestinationInvalid => "DestinationInvalid",
+                    ic_cdk::api::call::RejectionCode::CanisterReject => "CanisterReject",
+                    ic_cdk::api::call::RejectionCode::CanisterError => "CanisterError",
+                    ic_cdk::api::call::RejectionCode::Unknown => "Unknown",
+                };
+
+                let dict = vm.ctx.new_dict();
+                dict.set_item(attribute, vm.ctx.none(), vm);
+                Ok(dict.into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Reserved {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.none())
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::timer::TimerId {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk_timers::TimerId {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.data().as_ffi().to_pyobject(vm))
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::api::stable::StableMemoryError {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
-                match self {
-                    ic_cdk::api::stable::StableMemoryError::OutOfMemory => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("OutOfMemory", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                    ic_cdk::api::stable::StableMemoryError::OutOfBounds => {
-                        let dict = vm.ctx.new_dict();
-
-                        dict.set_item("OutOfBounds", vm.ctx.none(), vm);
-
-                        Ok(dict.into())
-                    }
-                }
+                let attribute = match self {
+                    ic_cdk::api::stable::StableMemoryError::OutOfMemory => "OutOfMemory",
+                    ic_cdk::api::stable::StableMemoryError::OutOfBounds => "OutOfBounds",
+                };
+
+                let dict = vm.ctx.new_dict();
+                dict.set_item(attribute, vm.ctx.none(), vm);
+                Ok(dict.into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for String {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
@@ -140,27 +101,27 @@
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_stable_structures::btreemap::InsertError {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 match self {
                     ic_stable_structures::btreemap::InsertError::KeyTooLarge {given, max} => {
                         let dict = vm.ctx.new_dict();
 
                         let key_too_large_dict = vm.ctx.new_dict();
-                        key_too_large_dict.set_item("given", given.try_into_vm_value(vm).unwrap(), vm);
-                        key_too_large_dict.set_item("max", max.try_into_vm_value(vm).unwrap(), vm);
+                        key_too_large_dict.set_item("given", given.try_into_vm_value(vm)?, vm);
+                        key_too_large_dict.set_item("max", max.try_into_vm_value(vm)?, vm);
 
                         dict.set_item("KeyTooLarge", key_too_large_dict.into(), vm);
 
                         Ok(dict.into())
                     },
                     ic_stable_structures::btreemap::InsertError::ValueTooLarge {given, max} => {
                         let dict = vm.ctx.new_dict();
 
                         let value_too_large_dict = vm.ctx.new_dict();
-                        value_too_large_dict.set_item("given", given.try_into_vm_value(vm).unwrap(), vm);
-                        value_too_large_dict.set_item("max", max.try_into_vm_value(vm).unwrap(), vm);
+                        value_too_large_dict.set_item("given", given.try_into_vm_value(vm)?, vm);
+                        value_too_large_dict.set_item("max", max.try_into_vm_value(vm)?, vm);
 
                         dict.set_item("ValueTooLarge", value_too_large_dict.into(), vm);
 
                         Ok(dict.into())
                     }
                 }
             }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/numeric.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/numeric.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,35 @@
-pub fn generate_numeric_impls() -> proc_macro2::TokenStream {
+use proc_macro2::TokenStream;
+
+pub fn generate() -> TokenStream {
     quote::quote! {
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for f64 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
         }
 
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for _CdkFloat64 {
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                Ok(self.0.to_pyobject(vm))
+            }
+        }
+
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for f32 {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(self.to_pyobject(vm))
             }
         }
 
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for _CdkFloat32 {
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                Ok(self.0.to_pyobject(vm))
+            }
+        }
+
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for ic_cdk::export::candid::Int {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.new_int(self.0).into())
             }
         }
 
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for i128 {
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/generators/vm_value_conversion/try_into_vm_value/vec.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/vm_value_conversion/try_into_vm_value_impls/vec.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-pub fn generate_vec_impls() -> proc_macro2::TokenStream {
+use proc_macro2::TokenStream;
+
+pub fn generate() -> TokenStream {
     quote::quote! {
         trait KybraTryIntoVec {}
 
         impl KybraTryIntoVec for () {}
 
         impl KybraTryIntoVec for bool {}
 
@@ -12,22 +14,26 @@
 
         impl KybraTryIntoVec for ic_cdk::export::candid::Reserved {}
 
         impl KybraTryIntoVec for ic_cdk::export::candid::Func {}
 
         impl KybraTryIntoVec for ic_cdk::export::Principal {}
 
-        impl KybraTryIntoVec for ic_cdk::timer::TimerId {}
+        impl KybraTryIntoVec for ic_cdk_timers::TimerId {}
 
         impl KybraTryIntoVec for ic_cdk::api::call::RejectionCode {}
 
         impl KybraTryIntoVec for f64 {}
 
         impl KybraTryIntoVec for f32 {}
 
+        impl KybraTryIntoVec for _CdkFloat64 {}
+
+        impl KybraTryIntoVec for _CdkFloat32 {}
+
         impl KybraTryIntoVec for ic_cdk::export::candid::Int {}
 
         impl KybraTryIntoVec for i128 {}
 
         impl KybraTryIntoVec for i64 {}
 
         impl KybraTryIntoVec for i32 {}
@@ -46,35 +52,59 @@
 
         impl KybraTryIntoVec for u32 {}
 
         impl KybraTryIntoVec for u16 {}
 
         impl<T> KybraTryIntoVec for Option<T> {}
 
+        impl<T> KybraTryIntoVec for Box<T> {}
+
         impl<T> KybraTryIntoVec for Vec<T> {}
 
-        impl<T> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Vec<T>
+        impl<T> CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
+            for Vec<T>
         where
             T: KybraTryIntoVec,
-            T: for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
+            T: for<'a> CdkActTryIntoVmValue<
+                &'a rustpython::vm::VirtualMachine,
+                rustpython::vm::PyObjectRef,
+            >,
         {
-            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+            fn try_into_vm_value(
+                self,
+                vm: &rustpython::vm::VirtualMachine,
+            ) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 try_into_vm_value_generic_array(self, vm)
             }
         }
 
-        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Vec<u8> {
-            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
+            for Vec<u8>
+        {
+            fn try_into_vm_value(
+                self,
+                vm: &rustpython::vm::VirtualMachine,
+            ) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 Ok(vm.ctx.new_bytes(self).into())
             }
         }
 
-        fn try_into_vm_value_generic_array<T>(generic_array: Vec<T>, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError>
+
+        fn try_into_vm_value_generic_array<T>(
+            generic_array: Vec<T>,
+            vm: &rustpython::vm::VirtualMachine,
+        ) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError>
         where
-            T:  for<'a> CdkActTryIntoVmValue<&'a rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef>
+            T: for<'a> CdkActTryIntoVmValue<
+                &'a rustpython::vm::VirtualMachine,
+                rustpython::vm::PyObjectRef,
+            >,
         {
-            let py_object_refs = generic_array.into_iter().map(|item| item.try_into_vm_value(vm).unwrap()).collect::<Vec<PyObjectRef>>();
+            let py_object_refs_result: Result<Vec<rustpython_vm::PyObjectRef>, CdkActTryIntoVmValueError> = generic_array
+                .into_iter()
+                .map(|item| item.try_into_vm_value(vm))
+                .collect();
 
-            Ok(vm.ctx.new_list(py_object_refs).into())
+            Ok(vm.ctx.new_list(py_object_refs_result?).into())
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_expr/to_hash_string.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/debug/to_hash_string.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-use super::KybraExpr;
+use std::ops::Deref;
+
 use rustpython_parser::ast::{
     ArgData, Arguments, Boolop, Cmpop, Comprehension, Constant, ExprContext, ExprKind, KeywordData,
     Located, Operator, Unaryop,
 };
 
+use crate::source_map::SourceMapped;
+
 pub trait ToHashString {
     fn to_hashable_string(&self) -> String;
 }
 
-impl ToHashString for KybraExpr<'_> {
+impl ToHashString for SourceMapped<Located<ExprKind>> {
     fn to_hashable_string(&self) -> String {
         format!(
-            "Kybra Expression: {} from {}",
-            self.located_expr.to_hashable_string(),
-            "main.py"
-        ) // TODO Add the source file for an even better hash
+            "SourceMapped: {} from {}",
+            self.deref().to_hashable_string(),
+            self.source_map.file_name
+        )
     }
 }
 
 impl<T> ToHashString for Vec<T>
 where
     T: ToHashString,
 {
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/data_types/variants/mod.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/variant/mod.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,41 @@
-use rustpython_parser::ast::{ExprKind, StmtKind};
+use rustpython_parser::ast::{Located, StmtKind};
 
-use crate::py_ast::kybra_types::KybraStmt;
-use cdk_framework::{
-    nodes::data_type_nodes::{
-        act_variants::{Variant, VariantTypeAlias},
-        ActVariant, ActVariantMember, LiteralOrTypeAlias,
-    },
-    ActDataType,
-};
+use crate::{errors::CollectResults, py_ast::PyAst, source_map::SourceMapped, Error};
+use cdk_framework::act::node::candid;
 
-mod errors;
 mod variants_members;
 
-impl KybraStmt<'_> {
-    pub fn as_variant(&self) -> ActDataType {
-        match &self.stmt_kind.node {
-            StmtKind::ClassDef { name, body, .. } => {
-                let members: Vec<ActVariantMember> = body
+impl PyAst {
+    pub fn build_variants(&self) -> Result<Vec<candid::Variant>, Vec<Error>> {
+        Ok(self
+            .get_stmt_kinds()
+            .iter()
+            .map(|source_mapped_stmt_kind| source_mapped_stmt_kind.as_variant())
+            .collect_results()?
+            .drain(..)
+            .filter_map(|x| x)
+            .collect())
+    }
+}
+
+impl SourceMapped<&Located<StmtKind>> {
+    fn as_variant(&self) -> Result<Option<candid::Variant>, Vec<Error>> {
+        match self.get_child_class_of("Variant") {
+            Some(variant) => {
+                let members = variant
+                    .body
                     .iter()
                     .map(|stmt| {
-                        KybraStmt {
-                            stmt_kind: stmt,
-                            source_map: self.source_map,
-                        }
-                        .as_variant_member()
+                        SourceMapped::new(stmt, self.source_map.clone()).to_variant_member()
                     })
-                    .collect();
-                ActDataType::Variant(ActVariant {
-                    act_type: LiteralOrTypeAlias::TypeAlias(VariantTypeAlias {
-                        variant: Variant {
-                            name: name.clone(),
-                            members,
-                        },
-                    }),
-                })
+                    .collect_results()?;
+                Ok(Some(candid::Variant {
+                    name: Some(variant.name.clone()),
+                    members,
+                    type_params: vec![].into(),
+                }))
             }
-            _ => panic!("{}", self.not_a_variant_error()),
-        }
-    }
-
-    pub fn is_variant(&self) -> bool {
-        match &self.stmt_kind.node {
-            StmtKind::ClassDef { bases, .. } => bases.iter().fold(false, |acc, base| {
-                let is_variant = match &base.node {
-                    ExprKind::Name { id, .. } => id == "Variant",
-                    _ => false,
-                };
-                acc || is_variant
-            }),
-            _ => false,
+            None => Ok(None),
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/external_canisters/mod.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/candid_type/service/mod.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,109 +1,141 @@
+pub mod errors;
+mod rust;
+
 use cdk_framework::{
-    nodes::{ActExternalCanister, ActExternalCanisterMethod},
-    ToActDataType,
+    act::node::{
+        candid::{self, service::Method},
+        node_parts::mode::Mode,
+        ReturnType,
+    },
+    traits::CollectResults,
 };
 use rustpython_parser::ast::{ExprKind, Located, StmtKind};
 
-use super::KybraStmt;
-use crate::py_ast::kybra_types::{KybraArguments, KybraExpr};
+use crate::{
+    constants::{SERVICE, SERVICE_QUERY, SERVICE_UPDATE},
+    errors::CollectResults as OtherCollectResults,
+    get_name::HasName,
+    method_utils::params::InternalOrExternal,
+    py_ast::PyAst,
+    source_map::SourceMapped,
+    Error,
+};
+
+use self::errors::{
+    MissingDecorator, ServiceMustHaveMethods, ServiceWithNonFunctionDefs, TooManyDecorators,
+    WrongDecorator,
+};
+
+impl PyAst {
+    pub fn build_services(&self) -> Result<Vec<candid::Service>, Vec<Error>> {
+        Ok(self
+            .get_stmt_kinds()
+            .iter()
+            .map(|source_mapped_stmt_kind| source_mapped_stmt_kind.as_service())
+            .collect_results()?
+            .drain(..)
+            .filter_map(|x| x)
+            .collect())
+    }
+}
+
+impl SourceMapped<&Located<StmtKind>> {
+    fn to_service_method(&self, canister_name: &String) -> Result<Method, Vec<Error>> {
+        match &self.node {
+            StmtKind::FunctionDef {
+                name,
+                decorator_list,
+                ..
+            } => {
+                let (params, return_type) = (
+                    self.build_params(InternalOrExternal::External),
+                    self.build_return_type(),
+                )
+                    .collect_results()?;
+                Ok(Method {
+                    name: name.clone(),
+                    params,
+                    return_type: ReturnType::new(return_type),
+                    mode: match build_mode(self, decorator_list, &canister_name, name) {
+                        Ok(mode) => mode,
+                        Err(err) => return Err(err.into()),
+                    },
+                })
+            }
+            _ => Err(ServiceWithNonFunctionDefs::err_from_stmt(self, &canister_name).into()),
+        }
+    }
+}
 
-impl KybraStmt<'_> {
-    pub fn to_act_external_canister(&self) -> ActExternalCanister {
-        match &self.stmt_kind.node {
-            StmtKind::ClassDef { name, body, .. } => {
-                let canister_name = name.clone();
-                let methods: Vec<ActExternalCanisterMethod> = body
+impl SourceMapped<&Located<StmtKind>> {
+    fn as_service(&self) -> Result<Option<candid::Service>, Vec<Error>> {
+        match self.get_child_class_of(SERVICE) {
+            Some(service) => {
+                let method_results: Vec<_> = service
+                    .body
                     .iter()
-                    .map(|located_statement| -> ActExternalCanisterMethod {
-                        match &located_statement.node {
-                            StmtKind::FunctionDef { name, args, body: _, decorator_list, returns, type_comment: _ } => {
-                                ensure_decorated_as_method_or_panic(decorator_list, &canister_name, name);
-
-                                let params = KybraArguments {
-                                    arguments: args.as_ref(),
-                                    source_map: self.source_map
-                                }.to_act_fn_params()
-                                 .unwrap_or_else(|e| panic!("{}.{} violates Kybra requirements: {}", canister_name, name, e) );
-
-                                let expr_kind = returns.as_ref().expect(&format!("{}.{} is missing a return type", canister_name, &name));
-
-                                let return_type = KybraExpr {
-                                    located_expr: expr_kind,
-                                    source_map: self.source_map,
-                                }.to_act_data_type(&None);
-
-                                ActExternalCanisterMethod {
-                                    name: name.clone(),
-                                    params,
-                                    return_type,
-                                }
-                            },
-                            _ => panic!("class \"{}\" should only contain function definitions. Please remove everything else.", name)
-                        }
+                    .map(|located_statement| {
+                        SourceMapped::new(located_statement, self.source_map.clone())
+                            .to_service_method(&service.name)
                     })
                     .collect();
 
+                let methods = method_results.into_iter().collect_results()?;
+
                 if methods.len() == 0 {
-                    panic!("class \"{}\" doesn't have any methods. External canisters are required to expose at least one method.", name)
+                    return Err(ServiceMustHaveMethods::err_from_stmt(self, service.name).into());
                 }
 
-                ActExternalCanister {
-                    name: canister_name,
+                Ok(Some(candid::Service {
+                    name: service.name.clone(),
                     methods,
-                }
+                    to_vm_value: rust::to_vm_value,
+                    list_to_vm_value: rust::list_to_vm_value,
+                    from_vm_value: rust::from_vm_value,
+                    list_from_vm_value: rust::list_from_vm_value,
+                }))
             }
-            // We filter out any non classDefs in KybraProgram.get_external_canister_declarations
-            _ => panic!("Oops! Looks like we introduced a bug while refactoring. Please open a ticket at https://github.com/demergent-labs/kybra/issues/new"),
-        }
-    }
-
-    pub fn is_external_canister(&self) -> bool {
-        match &self.stmt_kind.node {
-            StmtKind::ClassDef { bases, .. } => bases.iter().fold(false, |acc, base| {
-                let is_external_canister = match &base.node {
-                    ExprKind::Name { id, .. } => id == "Canister",
-                    _ => false,
-                };
-                acc || is_external_canister
-            }),
-            _ => false,
+            None => Ok(None),
         }
     }
 }
 
-fn ensure_decorated_as_method_or_panic(
+fn build_mode(
+    method_stmt: &SourceMapped<&Located<StmtKind>>,
     decorator_list: &Vec<Located<ExprKind>>,
     canister_name: &String,
     method_name: &String,
-) {
-    let decorator_name = "@method";
-
+) -> Result<Mode, Error> {
     if decorator_list.len() == 0 {
-        panic!(
-            "{}.{} is missing a \"{}\" decorator. Please add it above the method",
-            canister_name, method_name, decorator_name
-        );
+        return Err(MissingDecorator::err_from_stmt(
+            method_stmt,
+            canister_name,
+            method_name,
+        ));
     }
 
     if decorator_list.len() > 1 {
-        panic!(
-            "{}.{} has too many decorators. Please remove all but \"{}\"",
-            canister_name, method_name, decorator_name
-        )
+        return Err(TooManyDecorators::err_from_stmt(
+            method_stmt,
+            canister_name,
+            method_name,
+        ));
     }
 
-    match &decorator_list[0].node {
-        ExprKind::Name { id, ctx: _ } => {
-            if id != "method" {
-                panic!(
-                    "{}.{} has the wrong decorator: expected \"{}\", got \"@{}\"",
-                    canister_name, method_name, decorator_name, id
-                )
-            }
-        }
-        _ => panic!(
-            "{}.{} has an invalid decorator. Change it to \"{}\"",
-            canister_name, method_name, decorator_name
-        ),
+    match decorator_list[0].get_name() {
+        Some(SERVICE_QUERY) => Ok(Mode::Query),
+        Some(SERVICE_UPDATE) => Ok(Mode::Update),
+        Some(decorator_name) => Err(WrongDecorator::err_from_stmt(
+            method_stmt,
+            canister_name,
+            method_name,
+            Some(decorator_name),
+        )),
+        None => Err(WrongDecorator::err_from_stmt(
+            method_stmt,
+            canister_name,
+            method_name,
+            None,
+        )),
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_generate/src/py_ast/kybra_types/kybra_stmt/system_methods/mod.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_generate/src/ic_object/functions/notify_with_payment128_functions.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,97 @@
+use cdk_framework::{
+    act::node::{
+        candid::{service::Method, Service},
+        Context,
+    },
+    traits::ToTypeAnnotation,
+};
 use proc_macro2::TokenStream;
 use quote::{format_ident, quote};
 
-use super::KybraStmt;
-use crate::{generators::tuple, py_ast::kybra_types::KybraExpr};
-use cdk_framework::{nodes::ActFnParam, ToActDataType};
-
-mod errors;
-
-impl KybraStmt<'_> {
-    pub fn build_params(&self) -> Vec<ActFnParam> {
-        match &self.stmt_kind.node {
-            rustpython_parser::ast::StmtKind::FunctionDef { args, .. } => args
-                .args
+use crate::{keywords, tuple};
+
+pub fn generate(services: &Vec<Service>) -> Vec<TokenStream> {
+    services
+        .iter()
+        .map(|canister| {
+            canister
+                .methods
                 .iter()
-                .map(|arg| {
-                    let data_type = match &arg.node.annotation {
-                        Some(annotation) => KybraExpr {
-                            located_expr: &annotation,
-                            source_map: self.source_map,
+                .map(|method| {
+                    let function_name_string =
+                        format!("notify_with_payment128_{}_{}", canister.name, method.name);
+                    let real_function_name = format_ident!("{}", function_name_string);
+                    let wrapper_fn_name = format_ident!("{}_wrapper", function_name_string);
+                    let param_variable_definitions =
+                        generate_param_variables(method, &canister.name);
+                    let param_names = method
+                        .params
+                        .iter()
+                        .map(|param| {
+                            let name = format_ident!("{}", param.get_prefixed_name());
+                            quote! { #name }
+                        })
+                        .collect();
+                    let params = tuple::generate_tuple(&param_names);
+
+                    quote! {
+                        #[pymethod]
+                        fn #wrapper_fn_name(
+                            &self,
+                            args_py_object_refs: Vec<rustpython_vm::PyObjectRef>,
+                            vm: &rustpython_vm::VirtualMachine
+                        ) -> rustpython_vm::PyResult {
+                            let canister_id_principal: ic_cdk::export::Principal = args_py_object_refs[0]
+                                .clone()
+                                .try_from_vm_value(vm)
+                                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+
+                            #(#param_variable_definitions)*
+
+                            let cycles: u128 = args_py_object_refs[args_py_object_refs.len() - 1]
+                                .clone()
+                                .try_from_vm_value(vm)
+                                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
+
+                            let notify_result = #real_function_name(
+                                canister_id_principal,
+                                #params,
+                                cycles
+                            );
+
+                            notify_result
+                                .try_into_vm_value(vm)
+                                .map_err(|vmc_err| vm.new_type_error(vmc_err.0))
                         }
-                        .to_act_data_type(&None),
-                        None => panic!("{}", self.missing_type_annotation_error()),
-                    };
-                    ActFnParam {
-                        name: arg.node.arg.clone(),
-                        data_type,
                     }
                 })
-                .collect(),
-            _ => panic!("{}", self.not_a_function_def_error()),
-        }
-    }
-
-    pub fn get_function_name(&self) -> String {
-        match &self.stmt_kind.node {
-            rustpython_parser::ast::StmtKind::FunctionDef { name, .. } => name.clone(),
-            _ => panic!("{}", self.not_a_function_def_error()),
-        }
-    }
-
-    pub fn generate_call_to_py_function(&self) -> TokenStream {
-        match &self.stmt_kind.node {
-            rustpython_parser::ast::StmtKind::FunctionDef { .. } => {
-                let function_name = self.get_function_name();
-                let act_params = self.build_params();
-
-                let param_conversions = act_params
-                    .iter()
-                    .map(|act_fn_param| {
-                        let name = format_ident!("{}", act_fn_param.prefixed_name());
-                        quote! {
-                            #name.try_into_vm_value(vm).unwrap()
-                        }
-                    })
-                    .collect();
-                let params = tuple::generate_tuple(&param_conversions);
-
-                quote! {
-                    let _kybra_interpreter = _KYBRA_INTERPRETER_OPTION.as_mut().unwrap();
-                    let _kybra_scope = _KYBRA_SCOPE_OPTION.as_mut().unwrap();
-
-                    _kybra_interpreter.enter(|vm| {
-                        let method_py_object_ref = _kybra_unwrap_rust_python_result(_kybra_scope.globals.get_item(#function_name, vm), vm);
-
-                        let result_py_object_ref = vm.invoke(&method_py_object_ref, #params);
-
-                        match result_py_object_ref {
-                            Ok(py_object_ref) => py_object_ref.try_from_vm_value(vm).unwrap(),
-                            Err(err) => {
-                                let err_string: String = err.to_pyobject(vm).repr(vm).unwrap().to_string();
+                .collect()
+        })
+        .collect::<Vec<Vec<TokenStream>>>()
+        .concat()
+}
 
-                                panic!("{}", err_string);
-                            }
-                        }
-                    });
-                }
+fn generate_param_variables(method: &Method, canister_name: &String) -> Vec<TokenStream> {
+    method
+        .params
+        .iter()
+        .enumerate()
+        .map(|(index, param)| {
+            let variable_name = format_ident!("{}", param.get_prefixed_name());
+            let context = Context {
+                keyword_list: keywords::get_python_keywords(),
+                cdk_name: "kybra".to_string(),
+            };
+            let variable_type =
+                param.to_type_annotation(&context, method.create_qualified_name(canister_name));
+            let actual_index = index + 2;
+
+            quote! {
+                let #variable_name: #variable_type = args_py_object_refs[#actual_index]
+                    .clone()
+                    .try_from_vm_value(vm)
+                    .map_err(|vmc_err| vm.new_type_error(vmc_err.0))?;
             }
-            _ => panic!("{}", self.not_a_function_def_error()),
-        }
-    }
+        })
+        .collect()
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_enum.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-use cdk_framework::nodes::data_type_nodes::ToIdent;
+use cdk_framework::traits::ToIdent;
 use proc_macro2::Ident;
+use proc_macro2::TokenStream;
 use quote::quote;
 use syn::{DataEnum, Fields};
 
-pub fn derive_try_from_vm_value_enum(
-    enum_name: &Ident,
-    data_enum: &DataEnum,
-) -> proc_macro2::TokenStream {
+pub fn derive_try_from_vm_value_enum(enum_name: &Ident, data_enum: &DataEnum) -> TokenStream {
     let item_initializers = derive_item_initializers(enum_name, data_enum);
 
     quote! {
         impl CdkActTryFromVmValue<#enum_name, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<#enum_name, CdkActTryFromVmValueError> {
                 #(#item_initializers)*
 
@@ -22,18 +20,15 @@
             fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<#enum_name>, CdkActTryFromVmValueError> {
                 try_from_vm_value_generic_array(self, vm)
             }
         }
     }
 }
 
-fn derive_item_initializers(
-    enum_name: &Ident,
-    data_enum: &DataEnum,
-) -> Vec<proc_macro2::TokenStream> {
+fn derive_item_initializers(enum_name: &Ident, data_enum: &DataEnum) -> Vec<TokenStream> {
     data_enum
         .variants
         .iter()
         .map(|variant| {
             let variant_name = &variant.ident;
 
             match &variant.fields {
@@ -46,38 +41,35 @@
         })
         .collect()
 }
 
 fn derive_item_initializers_for_unnamed_fields(
     enum_name: &Ident,
     variant_name: &Ident,
-) -> proc_macro2::TokenStream {
+) -> TokenStream {
     let restored_variant_name = cdk_framework::keyword::restore_for_vm(
         &variant_name.to_string(),
         &crate::get_python_keywords(),
     )
-    .to_identifier();
+    .to_ident();
     quote! {
         let get_item_result = self.get_item(stringify!(#restored_variant_name), vm);
 
         if let Ok(item) = get_item_result {
-            return Ok(#enum_name::#variant_name(item.try_from_vm_value(vm).unwrap()));
+            return Ok(#enum_name::#variant_name(item.try_from_vm_value(vm)?));
         }
     }
 }
 
-fn derive_item_initializers_for_unit(
-    enum_name: &Ident,
-    variant_name: &Ident,
-) -> proc_macro2::TokenStream {
+fn derive_item_initializers_for_unit(enum_name: &Ident, variant_name: &Ident) -> TokenStream {
     let restored_variant_name = cdk_framework::keyword::restore_for_vm(
         &variant_name.to_string(),
         &crate::get_python_keywords(),
     )
-    .to_identifier();
+    .to_ident();
     quote! {
         let get_item_result = self.get_item(stringify!(#restored_variant_name), vm);
 
         if let Ok(_) = get_item_result {
             return Ok(#enum_name::#variant_name);
         }
     }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_from_vm_value/derive_try_from_vm_value_struct.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_struct.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,114 @@
-use cdk_framework::nodes::data_type_nodes::ToIdent;
-use proc_macro2::Ident;
+use cdk_framework::traits::ToIdent;
+use proc_macro2::{Ident, TokenStream};
 use quote::{format_ident, quote};
 use syn::{DataStruct, Fields, Index};
 
-pub fn derive_try_from_vm_value_struct(
+pub fn derive_try_into_vm_value_struct(
     struct_name: &Ident,
     data_struct: &DataStruct,
-) -> proc_macro2::TokenStream {
-    let field_variable_definitions = generate_field_variable_definitions(data_struct);
-    let field_variable_names = generate_field_initializers(data_struct);
+) -> TokenStream {
+    let data_structure_definition = derive_data_structure_definition(data_struct);
+    let variable_definitions = derive_struct_fields_variable_definitions(data_struct);
+    let property_definitions = derive_struct_fields_property_definitions(data_struct);
 
     quote! {
-        impl CdkActTryFromVmValue<#struct_name, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<#struct_name, CdkActTryFromVmValueError> {
-                #(#field_variable_definitions)*
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for #struct_name {
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                #(#variable_definitions)*
 
-                Ok(#struct_name {
-                    #(#field_variable_names),*
-                })
+                #data_structure_definition
+
+                #(#property_definitions)*
+
+                Ok(py_data_structure.into())
             }
         }
 
-        impl CdkActTryFromVmValue<Vec<#struct_name>, &rustpython::vm::VirtualMachine> for rustpython::vm::PyObjectRef {
-            fn try_from_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<Vec<#struct_name>, CdkActTryFromVmValueError> {
-                try_from_vm_value_generic_array(self, vm)
+        impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for Vec<#struct_name> {
+            fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
+                try_into_vm_value_generic_array(self, vm)
             }
         }
     }
 }
 
-fn generate_field_variable_definitions(data_struct: &DataStruct) -> Vec<proc_macro2::TokenStream> {
+fn derive_data_structure_definition(data_struct: &DataStruct) -> TokenStream {
+    match &data_struct.fields {
+        Fields::Named(_) => quote!(let py_data_structure = vm.ctx.new_dict();),
+        Fields::Unnamed(fields_unnamed) => {
+            let field_names: Vec<TokenStream> = fields_unnamed
+                .unnamed
+                .iter()
+                .enumerate()
+                .map(|(index, _)| {
+                    let field_name = format_ident!("field_{}_js_value", index);
+
+                    quote!(#field_name)
+                })
+                .collect();
+
+            quote!(let py_data_structure = vm.ctx.new_tuple(vec![#(#field_names),*]);)
+        }
+        _ => panic!("Only named and unnamed fields supported for Structs"),
+    }
+}
+
+fn derive_struct_fields_variable_definitions(data_struct: &DataStruct) -> Vec<TokenStream> {
     match &data_struct.fields {
         Fields::Named(fields_named) => fields_named
             .named
             .iter()
             .map(|field| {
-                let field_name = &field.ident;
-
-                let restored_field_name = match field_name {
-                    Some(field_name) => Some(cdk_framework::keyword::restore_for_vm(&field_name.to_string(), &crate::get_python_keywords()).to_identifier()),
-                    None => field_name.clone(),
-                };
+                let field_name = field.ident.as_ref().expect("Named field must have a name");
+                let variable_name = format_ident!("{}_js_value", field_name);
 
                 quote! {
-                    let #field_name = _kybra_unwrap_rust_python_result(self.get_item(stringify!(#restored_field_name), vm), vm);
+                    let #variable_name = self.#field_name.try_into_vm_value(vm)?;
                 }
             })
             .collect(),
         Fields::Unnamed(fields_unnamed) => fields_unnamed
             .unnamed
             .iter()
             .enumerate()
             .map(|(index, _)| {
-                let field_name = format_ident!("field_{}", index);
+                let variable_name = format_ident!("field_{}_js_value", index);
                 let syn_index = Index::from(index);
 
                 quote! {
-                    // TODO tuple_self is being repeated more times than necessary
-                    let tuple_self: PyTupleRef = _kybra_unwrap_rust_python_result(self.clone().try_into_value(vm), vm);
-                    let #field_name = tuple_self.get(#syn_index).unwrap();
+                    let #variable_name = self.#syn_index.try_into_vm_value(vm)?;
                 }
             })
             .collect(),
         _ => panic!("Only named and unnamed fields supported for Structs"),
     }
 }
 
-fn generate_field_initializers(data_struct: &DataStruct) -> Vec<proc_macro2::TokenStream> {
+fn derive_struct_fields_property_definitions(data_struct: &DataStruct) -> Vec<TokenStream> {
     match &data_struct.fields {
         Fields::Named(fields_named) => fields_named
             .named
             .iter()
             .map(|field| {
-                let field_name = &field.ident;
+                let field_name = field.ident.as_ref().expect("Named field must have a name");
+                let variable_name = format_ident!("{}_js_value", field_name);
 
-                quote! {
-                    #field_name: #field_name.try_from_vm_value(vm).unwrap()
-                }
-            })
-            .collect(),
-        Fields::Unnamed(fields_unnamed) => fields_unnamed
-            .unnamed
-            .iter()
-            .enumerate()
-            .map(|(index, _)| {
-                let field_name = format_ident!("field_{}", index);
-                let syn_index = Index::from(index);
+                let restored_field_name = cdk_framework::keyword::restore_for_vm(
+                    &field_name.to_string(),
+                    &crate::get_python_keywords(),
+                )
+                .to_ident();
 
                 quote! {
-                    #syn_index: #field_name.clone().try_from_vm_value(vm).unwrap()
+                    py_data_structure.set_item(
+                        stringify!(#restored_field_name),
+                        #variable_name,
+                        vm
+                    );
                 }
             })
             .collect(),
+        Fields::Unnamed(_) => vec![],
         _ => panic!("Only named and unnamed fields supported for Structs"),
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/derive_try_into_vm_value/derive_try_into_vm_value_enum.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-use cdk_framework::nodes::data_type_nodes::ToIdent;
+use cdk_framework::traits::ToIdent;
 use proc_macro2::Ident;
+use proc_macro2::TokenStream;
 use quote::quote;
 use syn::{DataEnum, Field, Fields};
 
-pub fn derive_try_into_vm_value_enum(
-    enum_name: &Ident,
-    data_enum: &DataEnum,
-) -> proc_macro2::TokenStream {
+pub fn derive_try_into_vm_value_enum(enum_name: &Ident, data_enum: &DataEnum) -> TokenStream {
     let variant_branches = derive_variant_branches(&enum_name, &data_enum);
 
     quote! {
         impl CdkActTryIntoVmValue<&rustpython::vm::VirtualMachine, rustpython::vm::PyObjectRef> for #enum_name {
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 match self {
                     #(#variant_branches),*
@@ -22,18 +20,15 @@
             fn try_into_vm_value(self, vm: &rustpython::vm::VirtualMachine) -> Result<rustpython::vm::PyObjectRef, CdkActTryIntoVmValueError> {
                 try_into_vm_value_generic_array(self, vm)
             }
         }
     }
 }
 
-fn derive_variant_branches(
-    enum_name: &Ident,
-    data_enum: &DataEnum,
-) -> Vec<proc_macro2::TokenStream> {
+fn derive_variant_branches(enum_name: &Ident, data_enum: &DataEnum) -> Vec<TokenStream> {
     data_enum
         .variants
         .iter()
         .map(|variant| {
             let variant_name = &variant.ident;
 
             match &variant.fields {
@@ -51,20 +46,20 @@
         .collect()
 }
 
 fn derive_variant_branches_unnamed_fields(
     enum_name: &Ident,
     variant_name: &Ident,
     unnamed_fields: Vec<&Field>,
-) -> proc_macro2::TokenStream {
+) -> TokenStream {
     let restored_variant_name = cdk_framework::keyword::restore_for_vm(
         &variant_name.to_string(),
         &crate::get_python_keywords(),
     )
-    .to_identifier();
+    .to_ident();
     if unnamed_fields.len() == 0 {
         quote! {
             #enum_name::#variant_name => {
                 let dict = vm.ctx.new_dict();
 
                 dict.set_item(stringify!(#restored_variant_name), vm.ctx.none(), vm);
 
@@ -72,14 +67,14 @@
             }
         }
     } else {
         quote! {
             #enum_name::#variant_name(value) => {
                 let dict = vm.ctx.new_dict();
 
-                dict.set_item(stringify!(#restored_variant_name), value.try_into_vm_value(vm).unwrap(), vm);
+                dict.set_item(stringify!(#restored_variant_name), value.try_into_vm_value(vm)?, vm);
 
                 Ok(dict.into())
             }
         }
     }
 }
```

### Comparing `kybra-0.4.0rc1/kybra/compiler/kybra_vm_value_derive/src/lib.rs` & `kybra-0.5.0rc0/kybra/compiler/kybra_vm_value_derive/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/kybra/module_bundler.py` & `kybra-0.5.0rc0/kybra/module_bundler.py`

 * *Files identical despite different names*

### Comparing `kybra-0.4.0rc1/kybra/timed.py` & `kybra-0.5.0rc0/kybra/timed.py`

 * *Files identical despite different names*

