# Comparing `tmp/curvesim-0.4.0a2.tar.gz` & `tmp/curvesim-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvesim-0.4.0a2.tar", last modified: Fri May 19 22:24:41 2023, max compression
+gzip compressed data, was "curvesim-0.4.5.tar", last modified: Wed Jul  5 20:32:59 2023, max compression
```

## Comparing `curvesim-0.4.0a2.tar` & `curvesim-0.4.5.tar`

### file list

```diff
@@ -1,127 +1,142 @@
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.995117 curvesim-0.4.0a2/
--rw-r--r--   0 suh        (501) staff       (20)     1071 2022-11-09 15:51:57.000000 curvesim-0.4.0a2/LICENSE.md
--rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 22:24:41.995473 curvesim-0.4.0a2/PKG-INFO
--rw-r--r--   0 suh        (501) staff       (20)     8738 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/README.md
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.807599 curvesim-0.4.0a2/curvesim/
--rw-r--r--   0 suh        (501) staff       (20)      281 2023-03-06 16:00:39.000000 curvesim-0.4.0a2/curvesim/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)      427 2023-04-07 15:09:59.000000 curvesim-0.4.0a2/curvesim/__main__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.811215 curvesim-0.4.0a2/curvesim/_bonding_curve/
--rw-r--r--   0 suh        (501) staff       (20)     2391 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/_bonding_curve/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.812066 curvesim-0.4.0a2/curvesim/_order_book/
--rw-r--r--   0 suh        (501) staff       (20)     3600 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/_order_book/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.814781 curvesim-0.4.0a2/curvesim/exceptions/
--rw-r--r--   0 suh        (501) staff       (20)     1466 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/exceptions/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.817026 curvesim-0.4.0a2/curvesim/iterators/
--rw-r--r--   0 suh        (501) staff       (20)      408 2022-11-12 00:31:20.000000 curvesim-0.4.0a2/curvesim/iterators/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.821111 curvesim-0.4.0a2/curvesim/iterators/param_samplers/
--rw-r--r--   0 suh        (501) staff       (20)      116 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/iterators/param_samplers/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     3358 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/iterators/param_samplers/grid.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.826278 curvesim-0.4.0a2/curvesim/iterators/price_samplers/
--rw-r--r--   0 suh        (501) staff       (20)      153 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/iterators/price_samplers/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2620 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/iterators/price_samplers/price_volume.py
--rw-r--r--   0 suh        (501) staff       (20)     3394 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/logging.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.832631 curvesim-0.4.0a2/curvesim/metrics/
--rw-r--r--   0 suh        (501) staff       (20)     1542 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/metrics/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    13007 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/base.py
--rw-r--r--   0 suh        (501) staff       (20)    16984 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/metrics.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.839191 curvesim-0.4.0a2/curvesim/metrics/results/
--rw-r--r--   0 suh        (501) staff       (20)      215 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1469 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/make_results.py
--rw-r--r--   0 suh        (501) staff       (20)     3805 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/results/sim_results.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.848754 curvesim-0.4.0a2/curvesim/metrics/state_log/
--rw-r--r--   0 suh        (501) staff       (20)      186 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1861 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/log.py
--rw-r--r--   0 suh        (501) staff       (20)     1268 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/pool_parameters.py
--rw-r--r--   0 suh        (501) staff       (20)     1034 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/metrics/state_log/pool_state.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.864543 curvesim-0.4.0a2/curvesim/network/
--rw-r--r--   0 suh        (501) staff       (20)      459 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/network/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     6157 2022-11-12 00:31:19.000000 curvesim-0.4.0a2/curvesim/network/coingecko.py
--rw-r--r--   0 suh        (501) staff       (20)     1704 2023-04-26 15:33:34.000000 curvesim-0.4.0a2/curvesim/network/http.py
--rw-r--r--   0 suh        (501) staff       (20)     2680 2022-11-13 23:49:59.000000 curvesim-0.4.0a2/curvesim/network/llamaAPI.py
--rw-r--r--   0 suh        (501) staff       (20)    14800 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/curvesim/network/nomics.py
--rw-r--r--   0 suh        (501) staff       (20)    13108 2023-05-19 19:57:52.000000 curvesim-0.4.0a2/curvesim/network/subgraph.py
--rw-r--r--   0 suh        (501) staff       (20)     1921 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/network/utils.py
--rw-r--r--   0 suh        (501) staff       (20)     4302 2023-04-25 20:54:10.000000 curvesim-0.4.0a2/curvesim/network/web3.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.866428 curvesim-0.4.0a2/curvesim/overrides/
--rw-r--r--   0 suh        (501) staff       (20)     1024 2022-11-12 00:31:19.000000 curvesim-0.4.0a2/curvesim/overrides/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.873692 curvesim-0.4.0a2/curvesim/pipelines/
--rw-r--r--   0 suh        (501) staff       (20)      501 2022-11-09 14:28:48.000000 curvesim-0.4.0a2/curvesim/pipelines/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    14384 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pipelines/arbitrage.py
--rw-r--r--   0 suh        (501) staff       (20)     5277 2023-05-18 18:36:37.000000 curvesim-0.4.0a2/curvesim/pipelines/templates.py
--rw-r--r--   0 suh        (501) staff       (20)     2646 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pipelines/utils.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.881693 curvesim-0.4.0a2/curvesim/plot/
--rw-r--r--   0 suh        (501) staff       (20)      122 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/__init__.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.907373 curvesim-0.4.0a2/curvesim/plot/altair/
--rw-r--r--   0 suh        (501) staff       (20)      169 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/altair/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1749 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/chart_properties.py
--rw-r--r--   0 suh        (501) staff       (20)     1474 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/make_chart.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.920390 curvesim-0.4.0a2/curvesim/plot/altair/results/
--rw-r--r--   0 suh        (501) staff       (20)        0 2023-05-19 22:22:27.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     3083 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/make_page.py
--rw-r--r--   0 suh        (501) staff       (20)     1558 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/preprocessing.py
--rw-r--r--   0 suh        (501) staff       (20)     1618 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/result_plotter.py
--rw-r--r--   0 suh        (501) staff       (20)     2597 2023-05-19 21:47:18.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/result_selectors.py
--rw-r--r--   0 suh        (501) staff       (20)      436 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/results/tooltip.py
--rw-r--r--   0 suh        (501) staff       (20)     1948 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/selectors.py
--rw-r--r--   0 suh        (501) staff       (20)     1001 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/curvesim/plot/altair/styles.py
--rw-r--r--   0 suh        (501) staff       (20)     2132 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/plot/result_plotter.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.926321 curvesim-0.4.0a2/curvesim/pool/
--rw-r--r--   0 suh        (501) staff       (20)     6772 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/pool/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2552 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/base.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.930644 curvesim-0.4.0a2/curvesim/pool/cryptoswap/
--rw-r--r--   0 suh        (501) staff       (20)      112 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/curvesim/pool/cryptoswap/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    36552 2023-05-18 17:46:09.000000 curvesim-0.4.0a2/curvesim/pool/cryptoswap/pool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.943349 curvesim-0.4.0a2/curvesim/pool/sim_interface/
--rw-r--r--   0 suh        (501) staff       (20)      174 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     5327 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/metapool.py
--rw-r--r--   0 suh        (501) staff       (20)     2967 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/pool.py
--rw-r--r--   0 suh        (501) staff       (20)     1098 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/raipool.py
--rw-r--r--   0 suh        (501) staff       (20)     1787 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/sim_interface/simpool.py
--rw-r--r--   0 suh        (501) staff       (20)     4154 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/snapshot.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.954135 curvesim-0.4.0a2/curvesim/pool/stableswap/
--rw-r--r--   0 suh        (501) staff       (20)      267 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    24771 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/metapool.py
--rw-r--r--   0 suh        (501) staff       (20)    17204 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/pool.py
--rw-r--r--   0 suh        (501) staff       (20)     1502 2023-01-20 15:19:10.000000 curvesim-0.4.0a2/curvesim/pool/stableswap/raipool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.959305 curvesim-0.4.0a2/curvesim/pool_data/
--rw-r--r--   0 suh        (501) staff       (20)     1574 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     4790 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/cache.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.968252 curvesim-0.4.0a2/curvesim/pool_data/metadata/
--rw-r--r--   0 suh        (501) staff       (20)     2376 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     2618 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/base.py
--rw-r--r--   0 suh        (501) staff       (20)     2007 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/cryptoswap.py
--rw-r--r--   0 suh        (501) staff       (20)     2515 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/curvesim/pool_data/metadata/stableswap.py
--rw-r--r--   0 suh        (501) staff       (20)     1287 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/pool_data/queries.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.972477 curvesim-0.4.0a2/curvesim/price_data/
--rw-r--r--   0 suh        (501) staff       (20)     1382 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/price_data/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1586 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/curvesim/price_data/sources.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.974202 curvesim-0.4.0a2/curvesim/sim/
--rw-r--r--   0 suh        (501) staff       (20)     6025 2023-05-19 21:10:12.000000 curvesim-0.4.0a2/curvesim/sim/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     3676 2023-05-19 14:49:10.000000 curvesim-0.4.0a2/curvesim/utils.py
--rw-r--r--   0 suh        (501) staff       (20)      361 2023-05-19 22:23:56.000000 curvesim-0.4.0a2/curvesim/version.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.810710 curvesim-0.4.0a2/curvesim.egg-info/
--rw-r--r--   0 suh        (501) staff       (20)     9758 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/PKG-INFO
--rw-r--r--   0 suh        (501) staff       (20)     3029 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/SOURCES.txt
--rw-r--r--   0 suh        (501) staff       (20)        1 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/dependency_links.txt
--rw-r--r--   0 suh        (501) staff       (20)      155 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/requires.txt
--rw-r--r--   0 suh        (501) staff       (20)       14 2023-05-19 22:24:41.000000 curvesim-0.4.0a2/curvesim.egg-info/top_level.txt
--rw-r--r--   0 suh        (501) staff       (20)      170 2022-11-08 18:43:56.000000 curvesim-0.4.0a2/pyproject.toml
--rw-r--r--   0 suh        (501) staff       (20)     1960 2023-05-19 22:24:41.996864 curvesim-0.4.0a2/setup.cfg
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.786510 curvesim-0.4.0a2/test/
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.976685 curvesim-0.4.0a2/test/fixtures/
--rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a2/test/fixtures/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     5506 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/test/fixtures/pool.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.978964 curvesim-0.4.0a2/test/integration/
--rw-r--r--   0 suh        (501) staff       (20)        0 2023-04-27 21:23:34.000000 curvesim-0.4.0a2/test/integration/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     1581 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/integration/test_subgraph.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.981117 curvesim-0.4.0a2/test/scripts/
--rw-r--r--   0 suh        (501) staff       (20)        0 2023-01-20 15:19:11.000000 curvesim-0.4.0a2/test/scripts/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)     4078 2023-05-17 22:06:08.000000 curvesim-0.4.0a2/test/scripts/make_test_data.py
-drwxr-xr-x   0 suh        (501) staff       (20)        0 2023-05-19 22:24:41.993640 curvesim-0.4.0a2/test/unit/
--rw-r--r--   0 suh        (501) staff       (20)        0 2022-10-14 18:34:20.000000 curvesim-0.4.0a2/test/unit/__init__.py
--rw-r--r--   0 suh        (501) staff       (20)    22383 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/unit/test_cryptopool.py
--rw-r--r--   0 suh        (501) staff       (20)    13246 2023-02-13 20:22:55.000000 curvesim-0.4.0a2/test/unit/test_metapool.py
--rw-r--r--   0 suh        (501) staff       (20)     8717 2023-03-02 16:07:35.000000 curvesim-0.4.0a2/test/unit/test_pool.py
--rw-r--r--   0 suh        (501) staff       (20)    11214 2023-05-17 21:31:12.000000 curvesim-0.4.0a2/test/unit/test_pool_metadata.py
--rw-r--r--   0 suh        (501) staff       (20)     4168 2023-05-17 18:59:58.000000 curvesim-0.4.0a2/test/unit/test_sim_stableswap.py
--rw-r--r--   0 suh        (501) staff       (20)     3531 2023-01-20 15:19:11.000000 curvesim-0.4.0a2/test/unit/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 20:32:49.000000 curvesim-0.4.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-05 20:32:59.009940 curvesim-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-05 20:32:49.000000 curvesim-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.981939 curvesim-0.4.5/curvesim/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/_bonding_curve/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/_bonding_curve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/_order_book/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/_order_book/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/iterators/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/iterators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/iterators/param_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/iterators/param_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/iterators/param_samplers/grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/iterators/price_samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/iterators/price_samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/iterators/price_samplers/price_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.985939 curvesim-0.4.5/curvesim/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.989939 curvesim-0.4.5/curvesim/metrics/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/results/make_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/results/sim_results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.989939 curvesim-0.4.5/curvesim/metrics/state_log/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/state_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/state_log/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/state_log/pool_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/metrics/state_log/pool_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/coingecko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/llamaAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/nomics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/network/web3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/overrides/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/pipelines/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/simple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/simple/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/simple/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/pipelines/vol_limited_arb/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/vol_limited_arb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/vol_limited_arb/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pipelines/vol_limited_arb/trader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.993939 curvesim-0.4.5/curvesim/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.997939 curvesim-0.4.5/curvesim/plot/altair/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/chart_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/make_chart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.997939 curvesim-0.4.5/curvesim/plot/altair/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/make_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/result_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/result_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/results/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/altair/styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/plot/result_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.001940 curvesim-0.4.5/curvesim/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.001940 curvesim-0.4.5/curvesim/pool/cryptoswap/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/cryptoswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36552 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/cryptoswap/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.001940 curvesim-0.4.5/curvesim/pool/sim_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/sim_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/sim_interface/asset_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/sim_interface/metapool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/sim_interface/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/sim_interface/raipool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.001940 curvesim-0.4.5/curvesim/pool/stableswap/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/stableswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/stableswap/metapool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/stableswap/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool/stableswap/raipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.005940 curvesim-0.4.5/curvesim/pool_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.005940 curvesim-0.4.5/curvesim/pool_data/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/metadata/cryptoswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/metadata/stableswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/pool_data/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.005940 curvesim-0.4.5/curvesim/price_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/price_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/price_data/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.005940 curvesim-0.4.5/curvesim/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/sim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/curvesim/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/sim_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/sim_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/templates/trader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 20:32:49.000000 curvesim-0.4.5/curvesim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.981939 curvesim-0.4.5/curvesim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-07-05 20:32:58.000000 curvesim-0.4.5/curvesim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-05 20:32:58.000000 curvesim-0.4.5/curvesim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:32:58.000000 curvesim-0.4.5/curvesim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 20:32:58.000000 curvesim-0.4.5/curvesim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-05 20:32:58.000000 curvesim-0.4.5/curvesim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 20:32:49.000000 curvesim-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-05 20:32:59.009940 curvesim-0.4.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:58.977939 curvesim-0.4.5/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/fixtures/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/integration/test_pool_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/integration/test_subgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/test/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/scripts/make_test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:59.009940 curvesim-0.4.5/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_coin_indices_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22383 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_cryptopool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_metapool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_pool_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 20:32:49.000000 curvesim-0.4.5/test/unit/test_snapshot.py
```

### Comparing `curvesim-0.4.0a2/LICENSE.md` & `curvesim-0.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/PKG-INFO` & `curvesim-0.4.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,40 @@
-Metadata-Version: 2.1
-Name: curvesim
-Version: 0.4.0a2
-Summary: Simulate Curve pools
-Home-page: https://github.com/curveresearch/curvesim
-Author: Curve Research
-Author-email: help@curveresearch.org
-License: MIT
-Project-URL: Documentation, https://curvesim.readthedocs.io
-Project-URL: Source, https://github.com/curveresearch/curvesim
-Project-URL: Tracker, https://github.com/curveresearch/curvesim/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 [![image](https://img.shields.io/pypi/v/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/l/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![image](https://img.shields.io/pypi/pyversions/curvesim.svg)](https://pypi.org/project/curvesim/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml/badge.svg)](https://github.com/curveresearch/curvesim/actions/workflows/CI.yml)
 [![Docs](https://readthedocs.org/projects/curvesim/badge/?version=latest)](https://curvesim.readthedocs.io/en/latest)
 ![badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/chanhosuh/3da3c072e081f4509ebdd09c63e6ede5/raw/curvesim_coverage_badge.json)
 
 
 # Curvesim
-Curvesim simulates Curve finance pools with optimal arbitrageurs trading against them. It's primary use is to determine optimal amplitude (A) and fee parameters given historical price and volume feeds.
+Curvesim simulates Curve pools with optimal arbitrageurs trading against them to determine reasonable risk and reward parameters, such as amplitude (A) and fee, given historical price and volume feeds.
+
+Users can re-use simulation components to simulate custom strategies and generate custom metrics.  Pool objects enable simpler integration with Curve pools for both manual and automated analytics usage.
+
 
 #### Dependencies:
-The maintainers use Python 3.8 or above, but 3.11 is not yet supported.  The code is likely fine for 3.6 and 3.7 but not officially supported.
+Python versions 3.8 - 3.11 are supported.
 
 Primary package dependencies: scipy, numpy, pandas, altair, matplotlib, requests, web3, gmpy2
 
 When working on the codebase, to avoid dependency issues it is recommended to use the included `requirements.txt` file in a Python virtual environment (`venv`).  Python 3.10 is required for this.
 
 
 ## Documentation
-Check out the full documentation at https://curvesim.readthedocs.io/
+Check out the full documentation at https://curvesim.readthedocs.io/.  We recommend starting with the "Quickstart" guide.
 
 ## Licensing
 Portions of the codebase are authorized derivatives of code owned by Curve.fi (Swiss Stake GmbH).  These are the vyper snippets used for testing (`test/fixtures/curve`) and the python code derived from them (`curvesim/pool/stableswap` and `curvesim/pool/cryptoswap`); there are copyright notices placed appropriately.  The rest of the codebase has an MIT license.
 
 ## Basic Use: Autosim
 The autosim() function simulates existing Curve pools with a range of A and/or fee parameters. The function fetches pool properties (e.g., current pool size) and 2 months of price/volume data, runs multiple simulations in parallel, and returns a results object that can be introspected or generate charts.
 
-Curve pools from any chain supported by the [Convex Community Subgraphs](https://thegraph.com/hosted-service/subgraph/convex-community/volume-mainnet) can be simulated directly by inputting the pool's address or symbol. For factory pools, the pool and LP token use the same symbol. For earlier pools, we use the LP token symbol.
+Curve pools from any chain supported by the [Convex Community Subgraphs](https://thegraph.com/hosted-service/subgraph/convex-community/volume-mainnet) can be simulated directly by inputting the pool's address.
 
 ### Example:
 To simulate 3pool with the default configuration:
 
 ```python
 import curvesim
 res = curvesim.autosim("0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7")
@@ -68,26 +45,71 @@
 ```python
 import curvesim
 # run sim on Arbitrum 2Crv
 res = curvesim.autosim("0x7f90122BF0700F9E7e1F688fe926940E8839F353", chain="arbitrum")
 ```
 
 
-### Results:
-Plots of the results will be saved to the "results/poolname" (e.g., pools/3crv) directory. The output dictionary, "res", contains pandas dataframes for all of the data plotted in the figures:
+## Simulation Results
+The simulation returns a SimResults object that can plot simulation metrics or return them as DataFrames.
+
+### Plotting results:
+```python
+#Plot results using Altair
+res.plot() 
+
+#Save plot results as results.html
+res.plot(save_as="results.html")
+
+```
+
+### Example output:
+![Alt text](/docs/images/plot_summary_screenshot.png?raw=true "Summary statistics")
+
+![Alt text](/docs/images/plot_timeseries_screenshot.png?raw=true "Timeseries data")
+
+
+
+### Summary statistics:
+```python
+>>> res.summary()
+metric pool_value_virtual         pool_value  ...   pool_volume price_error
+stat   annualized_returns annualized_returns  ...           sum      median
+0                0.003580           0.005156  ...  2.286297e+09    0.000669
+1                0.006158           0.007741  ...  1.966299e+09    0.000600
+2                0.007760           0.009348  ...  1.652965e+09    0.000775
+3                0.008611           0.010200  ...  1.377299e+09    0.000956
+4                0.003760           0.005439  ...  2.400174e+09    0.000777
+..                    ...                ...  ...           ...         ...
+59               0.009523           0.012018  ...  1.521524e+09    0.001155
+60               0.003742           0.006247  ...  2.388746e+09    0.001063
+61               0.006533           0.009082  ...  2.084530e+09    0.000915
+62               0.008344           0.010894  ...  1.775963e+09    0.000974
+63               0.009402           0.011974  ...  1.502494e+09    0.001133
+```
+
+### Timeseries data:
+```python
+>>> res.data()
+       run                 timestamp  ...      pool_volume  price_error
+0        0 2023-03-21 23:30:00+00:00  ...  15206414.533633     0.005310
+1        0 2023-03-22 00:30:00+00:00  ...    7278720.40969     0.002029
+2        0 2023-03-22 01:30:00+00:00  ...   6125207.553072     0.000100
+3        0 2023-03-22 02:30:00+00:00  ...    7066251.03295     0.000100
+4        0 2023-03-22 03:30:00+00:00  ...   3512782.000945     0.000299
+...    ...                       ...  ...              ...          ...
+93755   63 2023-05-21 19:30:00+00:00  ...    879436.331564     0.000893
+93756   63 2023-05-21 20:30:00+00:00  ...              0.0     0.001091
+93757   63 2023-05-21 21:30:00+00:00  ...    720837.826971     0.000800
+93758   63 2023-05-21 22:30:00+00:00  ...    445967.506177     0.001414
+93759   63 2023-05-21 23:30:00+00:00  ...    391060.986022     0.000906
+```
+
+
 
-* **ar**: annualized returns
-* **bal**: balance parameter over time, bal=1 when in perfect balance, and bal=0 when all holdings are in 1 coin
-* **pool_value**: time series of pool's value (based on virtual price)
-* **depth**: time series of price depth, averaged across pool's coins
-* **volume**: time series of pool volume
-* **log_returns**: log returns over time
-* **err**: time series of absolute price errors, (dy-fee)/dx - p, summed accros coin pairs
-* **x**: time series of pool holdings
-* **p**: time series of pool precisions (incl. basepool virtual price and/or RAI redemption price)
 
 ## Customizing Simulation Parameters
 By default, pools are simulated using:
 * on-chain or Curve Subgraph data about the pool
 * a broad range of A (16 values, 64 to 11,585) and fee (5 values, 0.02 to 0.06%) values
 * CoinGecko price/volume data
 * all detected CPU cores
@@ -116,15 +138,15 @@
 ```
 
 
 ### Overriding Simulation Parameters
 The following parameters are automatically specified by autosim(), but can be overridden with keyword arguments:
 * **D**: total deposit size; default: fetched from on-chain data
 * **vol_mult**: multiplied by market volume to produce trade size limits; default: computed from Curve Subraph data (see Volume Limits for details)
-* **feemul**: fee multiplier used in dynamic fee pools; default: specified in poolDF_\*.csv
+* **feemul**: fee multiplier used in dynamic fee pools
 
 ```python
 import curvesim
 
 #Simulate 3pool assuming total deposit of $10B, fee = 0.03%
 res = curvesim.autosim('0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7', D=10000000000, fee=3000000)
 
@@ -148,15 +170,15 @@
 * **vol_mode = 1**: limits trade volumes proportionally to market volume for each pair (default)
 * **vol_mode = 2**: limits trade volumes equally across pairs
 * **vol_mode = 3**: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
 We reccomend using the default vol_mode 1 in most cases. However, if that returns noisy/uninterpretable results, it may be worth trying mode 2 (for normal pools) or mode 3 (for meta-pools).
 
 ### Data Sources
-The "src" argument can be used to choose between 3 different data sources:
+The "src" argument can be used to choose between two different data sources:
 * **src = "coingecko"**: CoinGecko API (free); default
 * **src = "local"**: local data stored in the "data" folder
 
 Note that Nomics data is no longer supported since they went out of service.
 
 #### Note on CoinGecko Data
 Coingecko price/volume data is computed using all trading pairs for each coin, with volume summed across all pairs. Therefore, market volume taken from CoinGecko can be much higher than that of any specific trading pair used in a simulation. This issue is largely ameloriated by our volume limiting approach, with CoinGecko results typically mirroring results from pairwise data, but it should be noted that CoinGecko data may be less reliable than more granular data for certain simulations.
```

### Comparing `curvesim-0.4.0a2/curvesim/_bonding_curve/__init__.py` & `curvesim-0.4.5/curvesim/_bonding_curve/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/_order_book/__init__.py` & `curvesim-0.4.5/curvesim/_order_book/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/exceptions/__init__.py` & `curvesim-0.4.5/curvesim/exceptions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,7 +53,11 @@
 
 class PlotError(CurvesimException):
     """Error in plotting."""
 
 
 class NetworkError(CurvesimException):
     """Error for network subpackage."""
+
+
+class SimPoolError(CurvesimException):
+    """Error in a SimPool operation."""
```

### Comparing `curvesim-0.4.0a2/curvesim/iterators/param_samplers/grid.py` & `curvesim-0.4.5/curvesim/iterators/param_samplers/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,34 +31,30 @@
             Pool parameters set before all simulations.
             keys: pool parameters, values: ints
 
         """
         self.pool_template = pool
         self.set_attributes(self.pool_template, fixed_params)
         self.param_grid = self.param_product(variable_params)
-        self.param_generator = iter(self.param_grid)
 
     def __iter__(self):
-        return self
-
-    def __next__(self):
         """
-        Returns
+        Yields
         -------
         pool : pool object
             A pool object with the current variable parameters set.
 
         params : dict
             A dictionary of the pool parameters set on this iteration.
 
         """
-        params = next(self.param_generator)
-        pool = deepcopy(self.pool_template)
-        self.set_attributes(pool, params)
-        return pool, params
+        for params in self.param_grid:
+            pool = deepcopy(self.pool_template)
+            self.set_attributes(pool, params)
+            yield pool, params
 
     @staticmethod
     def param_product(p_dict):
         p_dict = p_dict.copy()
         basepool = p_dict.pop("basepool", None)
 
         keys = p_dict.keys()
```

### Comparing `curvesim-0.4.0a2/curvesim/logging.py` & `curvesim-0.4.5/curvesim/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             "level": "DEBUG",
             "propagate": False,
         },
     },
 }
 
 # 3rd party loggers that we want to largely ignore
-silenced_loggers = ["matplotlib", "asyncio", "rlp", "parso"]
+silenced_loggers = ["matplotlib", "asyncio", "rlp", "parso", "web3"]
 configured_loggers = CUSTOM_LOGGING_CONFIG["loggers"]
 for name in silenced_loggers:
     configured_loggers[name] = {
         "handlers": HANDLERS,
         "level": "INFO",
         "propagate": False,
     }
```

### Comparing `curvesim-0.4.0a2/curvesim/metrics/__init__.py` & `curvesim-0.4.5/curvesim/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/metrics/base.py` & `curvesim-0.4.5/curvesim/metrics/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
     "PoolPricingMetric",
 ]
 
 
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 
-from pandas import DataFrame, MultiIndex
+from pandas import DataFrame, Series, MultiIndex
 
 from curvesim.exceptions import MetricError
-from curvesim.utils import cache, get_pairs, override
+from curvesim.utils import cache, override
 
 
 class MetricBase(ABC):
     """
     Metric base class with required properties for any metric object in Curvesim.
 
     Typically, the :func:`compute_metric` method is defined in generalized sub-classes
@@ -51,23 +51,24 @@
                 A pandas DataFrame of the computed metrics.
 
             summary_data : DataFrame or None
                 A pandas Dataframe of the summary data computed using
                 :func:`summary_functions`. If :func:`summary_functions` is not
                 specified, returns None.
         """
-        data = self.metric_function(**state_log)
+        timestamps = state_log["price_sample"].timestamp
+        data = self.metric_function(**state_log).set_index(timestamps)
         return data, summarize_data(data, self.summary_functions)
 
     @property
     @abstractmethod
     def config(self):
         """
         A dict specifying how to compute, summarize, and/or plot the recorded data.
-        See `Metric Configuration`_ for formatting details.
+        See :ref:`metric-configuration` for formatting details.
 
         Raises :python:`NotImplementedError` if property is not defined.
         """
         raise NotImplementedError
 
     @property
     @abstractmethod
@@ -95,28 +96,28 @@
         """
         Configuration for plotting the metric and/or summary statistics. (Optional)
 
         Returns
         -------
             dict or None
                 Plot specification for each sub-metric and/or summary statistic.
-                See `Metric Configuration`_ for format details. Returns None if
+                See :ref:`metric-configuration` for format details. Returns None if
                 :python:`self.config["plot"]` is not present.
         """
 
     @property
     def summary_functions(self):
         """
         Specifies functions for computing summary statistics. (Optional)
 
         Returns
         -------
         dict or None
             A dict specifying the functions used to summarize each sub-metric.
-            See `Metric Configuration`_ for format details. Returns None if
+            See :ref:`metric-configuration` for format details. Returns None if
             :python:`self.config["functions"]["summary"]` not present.
         """
 
 
 class Metric(MetricBase):
     """
     Metric computed using a single function defined in the `config` property.
@@ -154,15 +155,15 @@
         """
         Configuration for plotting the metric and/or summary statistics. (Optional)
 
         Returns
         -------
         config["plot"] : dict or None
             Plot specification for each sub-metric and/or summary statistic.
-            See `Metric Configuration`_ for format details. Returns None if
+            See :ref:`metric-configuration` for format details. Returns None if
             :python:`self.config["plot"]` is not present.
         """
         try:
             return self.config["plot"]
         except KeyError:
             return None
 
@@ -172,15 +173,15 @@
         """
         Specifies functions for computing summary statistics. (Optional)
 
         Returns
         -------
         config["functions"]["summary"] : dict or None
             A dict specifying the functions used to summarize each sub-metric.
-            See `Metric Configuration`_ for format details. Returns None if
+            See :ref:`metric-configuration` for format details. Returns None if
             :python:`self.config["functions"]["summary"]` not present.
         """
         try:
             return self.config["functions"]["summary"]
         except KeyError:
             return None
 
@@ -255,15 +256,15 @@
         super().__init__(**kwargs)  # kwargs are ignored
 
     @property
     @abstractmethod
     def pool_config(self):
         """
         A dict mapping pool types to dicts in the format of :func:`MetricBase.config`.
-        See `Metric Configuration`_ for format details.
+        See :ref:`metric-configuration` for format details.
 
         Raises :python:`NotImplementedError` if property is not defined.
         """
         raise NotImplementedError
 
     def set_pool(self, pool):
         self._pool = pool
@@ -299,107 +300,101 @@
     """
     Mixin to incorporate current simulation prices into computations.
 
     Also provides :code:`numeraire` and :code:`numeraire_idx` attributes for computing
     prices or values with a preferred numeraire.
     """
 
-    def __init__(self, coin_names, n_coins=None, **kwargs):
+    def __init__(self, coin_names, **kwargs):
         """
         Parameters
         ----------
         coin_names : iterable of str
             Symbols for the coins used in a simulation. A numeraire is selected from
             the specified coins.
+        """
 
-        n_coins : int, optional
-            Number of coins used in the simulation. Defaults to length of "coin_names".
-            Used to map pools' coin indices to columns of the price feed.
-        """
-        n_coins = n_coins or len(coin_names)
-        idx_pairs = get_pairs(n_coins)
-        self._idx_map = {pair: i for i, pair in enumerate(idx_pairs)}
-        self.numeraire, self.numeraire_idx = get_numeraire(coin_names)
+        self.coin_names = coin_names
+        self.numeraire = get_numeraire(coin_names)
         super().__init__(**kwargs)
 
-    def get_market_price(self, i, j, prices):
+    def get_market_price(self, base, quote, prices):
         """
         Returns exchange rate for two coins identified by their pool indicies.
 
         Parameters
         ----------
-        i : int
-            Index of "in" coin; the "base" currency
-        j : int
-            Index of "out" coin; the "quote" currency
-        prices : list-like
-            Market prices for each pair, ordered as in
-            :python:`itertools.combinations(range(n_coins), 2)`. In the simulator
-            context, this is provided on each iteration of the :mod:`price_sampler`.
+        base : str
+            Symbol for the "in" coin; the "base" currency
+        quote : str
+            Symbol for the "out" coin; the "quote" currency
+        prices : pandas.DataFrame or pandas.Series
+            Market prices for each pair. In the simulator context, this is provided on
+            each iteration of the :mod:`price_sampler`.
 
         Returns
         -------
         float
-            The price of coin i, quoted in coin j.
+            The price of the "base" coin, quoted in the "quote" coin.
 
         """
-        if i == j:
+        try:
+            coin_pairs = getattr(prices, pandas_coin_pair_attr[type(prices)])
+        except KeyError as e:
+            raise MetricError(
+                f"Argument 'price' must be DataFrame or Series, not {type(prices)}"
+            ) from e
+
+        if base == quote:
             return 1
-        if i > j:
-            j, i = i, j
-            reciprocal = True
-        else:
-            reciprocal = False
-
-        idx = self._idx_map[(i, j)]
-        price = prices[idx]
-        if reciprocal:
-            return 1 / price
 
-        return price
+        if (base, quote) not in coin_pairs:
+            return 1 / prices[(quote, base)]
+
+        return prices[(base, quote)]
+
+
+pandas_coin_pair_attr = {DataFrame: "columns", Series: "index"}
 
 
 def get_numeraire(coins):
     """
-    Returns a preferred numeraire and its index based on the provided list of coins.
+    Returns a preferred numeraire from the provided list of coins.
     """
     numeraire = coins[0]
     preferred = ["USDC", "USDT", "ETH", "WETH", "CRV"]
 
     # Heuristic: base coin in pool of derivatives
     base = min(coins, key=len).upper()
     if all(base in c.upper() for c in coins):
         preferred.append(base)
 
     for coin in coins:
         if coin.upper() in preferred:
             numeraire = coin
             break
 
-    return numeraire, coins.index(numeraire)
+    return numeraire
 
 
 class PricingMetric(PricingMixin, Metric):
     """
     :class:`Metric` with :class:`PricingMixin` functionality.
     """
 
-    def __init__(self, coin_names, n_coins=None, **kwargs):
+    def __init__(self, coin_names, **kwargs):
         """
         Parameters
         ----------
         coin_names : iterable of str
             Symbols for the coins used in a simulation. A numeraire is selected from
             the specified coins.
 
-        n_coins : int, optional
-            Number of coins used in the simulation. Defaults to length of "coin_names".
-            Used to map pools' coin indices to columns of the price feed.
         """
-        super().__init__(coin_names, n_coins)
+        super().__init__(coin_names)
 
 
 class PoolPricingMetric(PricingMixin, PoolMetric):
     """
     :class:`PoolMetric` with :class:`PricingMixin` functionality.
     """
 
@@ -408,9 +403,8 @@
         Parameters
         ----------
         pool : SimPool object
             A pool simulation interface. Used to select the pool's configuration from
             :func:`pool_config` and stored as :python:`self._pool` for access during
             metric computations. Number and names of coins derived from pool metadata.
         """
-        coin_names = list(pool.coin_indices)
-        super().__init__(coin_names, pool.n_total, pool=pool)
+        super().__init__(pool.assets.symbols, pool=pool)
```

### Comparing `curvesim-0.4.0a2/curvesim/metrics/metrics.py` & `curvesim-0.4.5/curvesim/metrics/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,40 +7,40 @@
     "ArbMetrics",
     "PoolBalance",
     "PoolValue",
     "PriceDepth",
     "Timestamp",
 ]
 
-from functools import partial
+from copy import deepcopy
 
 from altair import Axis, Scale
-from numpy import array, exp, log
+from numpy import array, exp, log, timedelta64
 from pandas import DataFrame, concat
 
 from curvesim.pool.sim_interface import SimCurveMetaPool, SimCurvePool, SimCurveRaiPool
-from curvesim.utils import cache, get_pairs
-from .base import Metric, PoolMetric, PricingMetric, PoolPricingMetric
+from curvesim.utils import get_pairs
+
+from .base import Metric, PoolMetric, PoolPricingMetric, PricingMetric
 
 
 class ArbMetrics(PricingMetric):
     """
     Computes metrics characterizing arbitrage trades: arbitrageur profits, pool fees,
-    trade volume, and post-trade price error between target and pool price.
+    and post-trade price error between target and pool price.
     """
 
     @property
     def config(self):
         return {
             "functions": {
                 "metrics": self.compute_arb_metrics,
                 "summary": {
                     "arb_profit": "sum",
                     "pool_fees": "sum",
-                    "pool_volume": "sum",
                     "price_error": "median",
                 },
             },
             "plot": {
                 "metrics": {
                     "arb_profit": {
                         "title": f"Daily Arbitrageur Profit (in {self.numeraire})",
@@ -48,19 +48,14 @@
                         "resample": "sum",
                     },
                     "pool_fees": {
                         "title": f"Daily Pool Fees (in {self.numeraire})",
                         "style": "time_series",
                         "resample": "sum",
                     },
-                    "pool_volume": {
-                        "title": "Daily Volume",
-                        "style": "time_series",
-                        "resample": "sum",
-                    },
                     "price_error": {
                         "title": "Price Error",
                         "style": "histogram",
                         "encoding": {
                             "x": {
                                 "title": "Price Error (binned)",
                                 "shorthand": "price_error",
@@ -74,67 +69,151 @@
                         "title": f"Total Arbitrageur Profit (in {self.numeraire})",
                         "style": "point_line",
                     },
                     "pool_fees": {
                         "title": f"Total Pool Fees (in {self.numeraire})",
                         "style": "point_line",
                     },
-                    "pool_volume": {
-                        "title": "Total Volume",
-                        "style": "point_line",
-                    },
                     "price_error": {
                         "title": "Price Error (median)",
                         "style": "point_line",
                     },
                 },
             },
         }
 
     def __init__(self, pool, **kwargs):
-        coin_names = list(pool.coin_indices.keys())
-        super().__init__(coin_names, pool.n_total)
+        super().__init__(pool.assets.symbols)
 
     def compute_arb_metrics(self, price_sample, trade_data, **kwargs):
         """Computes all metrics for each timestamp in an individual run."""
 
-        data = concat([price_sample.prices, trade_data], axis=1)
+        prices = DataFrame(price_sample.prices.to_list(), index=price_sample.index)
 
-        profits = data.apply(self._compute_profits, axis=1, result_type="expand")
-        volume = data.volume / 10**18
-        price_error = data.price_errors.abs().apply(sum)
+        profits = self._compute_profits(prices, trade_data.trades)
+        price_error = trade_data.price_errors.apply(
+            lambda errors: sum(abs(e) for e in errors)
+        )
 
-        results = concat([profits, volume, price_error], axis=1)
+        results = concat([profits, price_error], axis=1)
         results.columns = list(self.config["plot"]["metrics"])
+
         return results
 
-    def _compute_profits(self, data_row):
+    def _compute_profits(self, price_df, trade_df):
         """
         Computes arbitrageur profits and pool fees for a single row of data (i.e.,
         a single timestamp) in units of the chosen numeraire, `self.numeraire`.
         """
         get_price = self.get_market_price
-        num_idx = self.numeraire_idx
-        prices = data_row.prices
+        numeraire = self.numeraire
+
+        profit = []
+        for price_row, trade_row in zip(price_df.iterrows(), trade_df):
+
+            timestamp, prices = price_row
+            arb_profit = 0
+            pool_profit = 0
+
+            for trade in trade_row:
+                market_price = get_price(trade.coin_in, trade.coin_out, prices)
+                arb = trade.amount_out - trade.amount_in * market_price
+                fee = trade.fee
+
+                if trade.coin_out != numeraire:
+                    price = get_price(trade.coin_out, numeraire, prices)
+                    arb = arb * price
+                    fee = fee * price
+
+                arb_profit += arb
+                pool_profit += fee
+
+            profit.append(
+                {
+                    "timestamp": timestamp,
+                    "arb_profit": arb_profit / 10**18,
+                    "pool_profit": pool_profit / 10**18,
+                }
+            )
+
+        return DataFrame(profit).set_index("timestamp")
+
+
+class PoolVolume(PoolMetric):
+    """
+    Records total trade volume for each timestamp.
+    """
+
+    @property
+    def pool_config(self):
+        base = {
+            "functions": {"summary": {"pool_volume": "sum"}},
+            "plot": {
+                "metrics": {
+                    "pool_volume": {
+                        "title": "Daily Volume",
+                        "style": "time_series",
+                        "resample": "sum",
+                    },
+                },
+                "summary": {
+                    "pool_volume": {
+                        "title": "Total Volume",
+                        "style": "point_line",
+                    },
+                },
+            },
+        }
+
+        functions = {
+            SimCurvePool: self.get_stableswap_pool_volume,
+            SimCurveMetaPool: self.get_stableswap_metapool_volume,
+            SimCurveRaiPool: self.get_stableswap_metapool_volume,
+        }
+
+        config = {}
+        for pool, fn in functions.items():
+            config[pool] = deepcopy(base)
+            config[pool]["functions"]["metrics"] = fn
 
-        arb_profit = 0
-        pool_profit = 0
-        for trade in data_row.trades:
-            i, j, dx, dy, fee = trade
-            arb = dy - dx * get_price(i, j, prices)
-
-            if j != num_idx:
-                price = get_price(j, num_idx, prices)
-                arb = arb * price
-                fee = fee * price
+        return config
+
+    def get_stableswap_pool_volume(self, trade_data, **kwargs):
+        """
+        Records trade volume for stableswap non-meta-pools.
+        """
+
+        def per_timestamp_function(trades):
+            return sum([trade.amount_in for trade in trades]) / 10**18
+
+        return self._get_volume(trade_data, per_timestamp_function)
+
+    def get_stableswap_metapool_volume(self, trade_data, **kwargs):
+        """
+        Records trade volume for stableswap meta-pools. Only includes trades involving
+        the meta-asset (basepool-only trades are ignored).
+        """
 
-            arb_profit += arb / 10**18
-            pool_profit += fee / 10**18
+        meta_asset = self._pool.assets.symbols[0]
 
-        return arb_profit, pool_profit
+        def per_timestamp_function(trades):
+            volume = 0
+            for trade in trades:
+                if meta_asset in (trade.coin_in, trade.coin_out):
+                    volume += trade.amount_in
+            return volume / 10**18
+
+        return self._get_volume(trade_data, per_timestamp_function)
+
+    def _get_volume(self, trade_data, per_timestamp_function):
+        trades = trade_data.trades
+        volume = trades.apply(per_timestamp_function)
+        results = DataFrame(volume)
+        results.columns = ["pool_volume"]
+        return results
 
 
 class PoolBalance(PoolMetric):
     """
     Computes the pool balance metric, which ranges from 0 (completely imbalanced) to 1
     (completely balanced).
     """
@@ -201,16 +280,14 @@
 
 class PoolValue(PoolPricingMetric):
     """
     Computes pool's value over time in virtual units and the chosen
     numeraire, `self.numeraire`. Each are summarized as annualized returns.
     """
 
-    __slots__ = ["_freq"]
-
     @property
     def pool_config(self):
         ss_plot = {
             "metrics": {
                 "pool_value_virtual": {
                     "title": "Pool Value (Virtual)",
                     "style": "time_series",
@@ -263,25 +340,26 @@
                     "metrics": self.get_stableswap_metapool_value,
                     "summary": ss_summary_fns,
                 },
                 "plot": ss_plot,
             },
         }
 
-    def __init__(self, pool, freq, **kwargs):
-        self._freq = freq
-        super().__init__(pool)
-
     def get_stableswap_pool_value(self, pool_state, price_sample, **kwargs):
         """
         Computes all metrics for each timestamp in an individual run.
         Used for non-meta stableswap pools.
         """
-        reserves = DataFrame(pool_state.balances.to_list())
-        prices = DataFrame(price_sample.prices.to_list())
+        reserves = DataFrame(
+            pool_state.balances.to_list(),
+            index=pool_state.index,
+            columns=self._pool.coin_names,
+        )
+
+        prices = DataFrame(price_sample.prices.to_list(), index=price_sample.index)
 
         pool_value = self._get_value_from_prices(reserves / 10**18, prices)
         pool_value_virtual = pool_state.apply(
             self._get_stableswap_virtual_value, axis=1
         )
 
         results = concat([pool_value_virtual, pool_value], axis=1)
@@ -289,23 +367,34 @@
         return results.astype("float64")
 
     def get_stableswap_metapool_value(self, pool_state, price_sample, **kwargs):
         """
         Computes all metrics for each timestamp in an individual run.
         Used for stableswap metapools.
         """
-        meta_reserves = DataFrame(pool_state.balances.to_list())
-        base_reserves = DataFrame(pool_state.balances_base.to_list())
-        prices = DataFrame(price_sample.prices.to_list())
         max_coin = self._pool.max_coin
+        pool = self._pool
+
+        meta_reserves = DataFrame(
+            pool_state.balances.to_list(),
+            index=pool_state.index,
+            columns=pool.coin_names,
+        )
+
+        base_reserves = DataFrame(
+            pool_state.balances_base.to_list(),
+            index=pool_state.index,
+            columns=pool.basepool.coin_names,
+        )
+
+        prices = DataFrame(price_sample.prices.to_list(), index=price_sample.index)
 
-        LP_token_proportion = meta_reserves[max_coin] / pool_state.tokens_base
+        LP_token_proportion = meta_reserves.iloc[:, max_coin] / pool_state.tokens_base
         base_reserves = base_reserves.mul(LP_token_proportion, axis=0)
         reserves = concat([meta_reserves.iloc[:, :max_coin], base_reserves], axis=1)
-        reserves.columns = range(len(reserves.columns))
 
         pool_value = self._get_value_from_prices(reserves / 10**18, prices)
         pool_value_virtual = pool_state.apply(
             self._get_stableswap_virtual_value, axis=1
         )
 
         results = concat([pool_value_virtual, pool_value], axis=1)
@@ -314,174 +403,137 @@
 
     def _get_value_from_prices(self, reserves, prices):
         """
         Computes pool value in the chosen numeraire, `self.numeraire`.
         Can be used for any pool type.
         """
         get_price = self.get_market_price
-        num_idx = self.numeraire_idx
+        numeraire = self.numeraire
 
         value = 0
-        for i in reserves.columns:  # columns are ordered range of ints
-            value += reserves[i] * get_price(i, num_idx, prices)
-
+        for coin_name in reserves.columns:
+            value += reserves[coin_name] * get_price(coin_name, numeraire, prices)
         return value
 
     def _get_stableswap_virtual_value(self, pool_state_row):
         """
         Computes virtual pool value for a single row of data (i.e., a single timestamp).
         Used for any stableswap pool.
         """
         self.set_pool_state(pool_state_row)
         return self._pool.D() / 10**18
 
     def compute_annualized_returns(self, data):
         """Computes annualized returns from a series of pool values."""
+        year_multipliers = timedelta64(1, "Y") / data.index.to_series().diff()
         log_returns = log(data).diff()  # pylint: disable=no-member
-        year_mult = 60 / self._freq * 24 * 365
-        return exp(log_returns.mean() * year_mult) - 1
+
+        return exp((log_returns * year_multipliers).mean()) - 1
 
 
 class PriceDepth(PoolMetric):
     """
     Computes metrics indicating a pool's price (liquidity) depth. Generally, uses
     liquidity density, % change in reserves per % change in price.
     """
 
     __slots__ = ["_factor"]
 
     @property
     def pool_config(self):
-        ss_plot = {
-            "metrics": {
-                "liquidity_density": {
-                    "title": "Liquidity Density",
-                    "style": "time_series",
-                    "resample": "median",
-                    "encoding": {"y": {"title": "Liquidity Density (Daily Median)"}},
-                }
-            },
-            "summary": {
-                "liquidity_density": {
-                    "title": "Liquidity Density",
-                    "style": "point_line",
-                }
-            },
-        }
-
-        ss_summary_fns = {"liquidity_density": ["median", "min"]}
-
-        return {
-            SimCurvePool: {
-                "functions": {
-                    "metrics": self.get_curve_pool_LD,
-                    "summary": ss_summary_fns,
-                },
-                "plot": ss_plot,
+        ss_config = {
+            "functions": {
+                "metrics": self.get_curve_LD,
+                "summary": {"liquidity_density": ["median", "min"]},
             },
-            SimCurveMetaPool: {
-                "functions": {
-                    "metrics": self.get_curve_metapool_LD,
-                    "summary": ss_summary_fns,
+            "plot": {
+                "metrics": {
+                    "liquidity_density": {
+                        "title": "Liquidity Density (Daily Median)",
+                        "style": "time_series",
+                        "resample": "median",
+                        "encoding": {
+                            "y": {"title": "Liquidity Density (Daily Median)"}
+                        },
+                    }
                 },
-                "plot": ss_plot,
-            },
-            SimCurveRaiPool: {
-                "functions": {
-                    "metrics": self.get_curve_metapool_LD,
-                    "summary": ss_summary_fns,
+                "summary": {
+                    "liquidity_density": {
+                        "title": "Liquidity Density",
+                        "style": "point_line",
+                    }
                 },
-                "plot": ss_plot,
             },
         }
 
+        return dict.fromkeys(
+            [SimCurveMetaPool, SimCurvePool, SimCurveRaiPool], ss_config
+        )
+
     def __init__(self, pool, factor=10**8, **kwargs):
         self._factor = factor
         super().__init__(pool)
 
-    def get_curve_pool_LD(self, pool_state, **kwargs):
-        """
-        Computes liquidity density for each timestamp in an individual run, averaging
-        across all coin pairs. Used for non-meta stableswap pools.
-        """
-        index_combos = self._curve_pool_index_combos
-        return self._get_curve_LD(index_combos, pool_state)
-
-    def get_curve_metapool_LD(self, pool_state, **kwargs):
-        """
-        Computes liquidity density for each timestamp in an individual run, using only
-        top-level coin pairs in a metapool. Used for Curve metapools.
-        """
-        index_combos = self._curve_metapool_index_combos
-        return self._get_curve_LD(index_combos, pool_state)
-
-    def _get_curve_LD(self, index_combos, pool_state):
+    def get_curve_LD(self, pool_state, **kwargs):
         """
         Computes liquidity density for each timestamp in an individual run.
         Used for all Curve pools.
         """
-        get_LD = partial(self._get_curve_LD_by_row, index_combos=index_combos)
-        LD = pool_state.apply(get_LD, axis=1)
+        coin_pairs = get_pairs(
+            self._pool.coin_names
+        )  # for metapool, uses only meta assets
+        LD = pool_state.apply(self._get_curve_LD_by_row, axis=1, coin_pairs=coin_pairs)
         return DataFrame(LD, columns=["liquidity_density"])
 
-    def _get_curve_LD_by_row(self, pool_state_row, index_combos):
+    def _get_curve_LD_by_row(self, pool_state_row, coin_pairs):
         """
         Computes liquidity density for a single row of data (i.e., a single timestamp).
         Used for all Curve pools.
         """
         self.set_pool_state(pool_state_row)
+
         LD = []
-        for i, j in index_combos:
-            ld = self._compute_liquidity_density(i, j)
+        for pair in coin_pairs:
+            ld = self._compute_liquidity_density(*pair)
             LD.append(ld)
         return sum(LD) / len(LD)
 
-    @property
-    @cache
-    def _curve_pool_index_combos(self):
-        """Returns all pairwise combinations of coin indices."""
-        return get_pairs(self._pool.n)
-
-    @property
-    @cache
-    def _curve_metapool_index_combos(self):
-        """
-        Returns pairwise combinations of coin indices in the top level of a metapool.
-
-        Our convention for the basepool LP token index is to use
-        the total number of stablecoins (including basepool).
-        This removes ambiguity as it is one "off the end" and thus
-        either doesn't exist or is the basepool LP token.
-        """
-        pool = self._pool
-        base_idx = list(range(pool.n))
-        base_idx[pool.max_coin] = pool.n_total
-        return get_pairs(base_idx)
-
     def _compute_liquidity_density(self, coin_in, coin_out):
         """
         Computes liquidity density for a single pair of coins.
-
-        Only for top-level liquidity density.  Cannot compare between
-        coins in basepool and primary stablecoin in metapool.
         """
         factor = self._factor
         pool = self._pool
+        post_trade_price = self._post_trade_price
 
         price_pre = pool.price(coin_in, coin_out, use_fee=False)
-        price_post = pool.test_trade(coin_in, coin_out, factor, use_fee=False)
+        price_post = post_trade_price(pool, coin_in, coin_out, factor)
         LD1 = price_pre / ((price_pre - price_post) * factor)
 
         price_pre = pool.price(coin_out, coin_in, use_fee=False)
         # pylint: disable-next=arguments-out-of-order
-        price_post = pool.test_trade(coin_out, coin_in, factor, use_fee=False)
+        price_post = post_trade_price(pool, coin_out, coin_in, factor)
         LD2 = price_pre / ((price_pre - price_post) * factor)
 
         return (LD1 + LD2) / 2
 
+    @staticmethod
+    def _post_trade_price(pool, coin_in, coin_out, factor, use_fee=False):
+        """
+        Computes price after executing a trade of size coin_in balances / factor.
+        """
+
+        size = pool.asset_balances[coin_in] // factor
+
+        with pool.use_snapshot_context():
+            pool.trade(coin_in, coin_out, size)
+            price = pool.price(coin_in, coin_out, use_fee=use_fee)
+
+        return price
+
 
 class Timestamp(Metric):
     """Simple pass-through metric to record timestamps."""
 
     @property
     def config(self):
         return {"functions": {"metrics": self._get_timestamp}}
```

### Comparing `curvesim-0.4.0a2/curvesim/metrics/results/make_results.py` & `curvesim-0.4.5/curvesim/metrics/results/make_results.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/metrics/results/sim_results.py` & `curvesim-0.4.5/curvesim/metrics/results/sim_results.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/metrics/state_log/log.py` & `curvesim-0.4.5/curvesim/metrics/state_log/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,26 +29,32 @@
 
         self.state_per_trade.append({"pool_state": get_pool_state(self.pool), **kwargs})
 
     def get_logs(self):
         """Returns the accumulated log data."""
 
         df = DataFrame(self.state_per_trade)
-        state_per_trade = {col: DataFrame(df[col].to_list()) for col in df}
-        return {**self.state_per_run, **state_per_trade}
+
+        times = [state["price_sample"].timestamp for state in self.state_per_trade]
+        state_per_trade = {col: DataFrame(df[col].to_list(), index=times) for col in df}
+
+        return {
+            "pool_parameters": DataFrame(self.state_per_run, index=[0]),
+            **state_per_trade,
+        }
 
     def compute_metrics(self):
         """Computes metrics from the accumulated log data."""
 
         state_logs = self.get_logs()
         metric_data = [metric.compute(state_logs) for metric in self.metrics]
         data_per_trade, summary_data = tuple(zip(*metric_data))  # transpose tuple list
 
         return (
-            DataFrame(self.state_per_run, index=[0]),
+            state_logs["pool_parameters"],
             concat(data_per_trade, axis=1),
             concat(summary_data, axis=1),
         )
 
 
 def prepare_metrics(metrics, pool):
     """
```

### Comparing `curvesim-0.4.0a2/curvesim/metrics/state_log/pool_parameters.py` & `curvesim-0.4.5/curvesim/metrics/state_log/pool_parameters.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/metrics/state_log/pool_state.py` & `curvesim-0.4.5/curvesim/metrics/state_log/pool_state.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/network/http.py` & `curvesim-0.4.5/curvesim/network/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 General utility for http requests.
 """
 import aiohttp
 from aiohttp import ClientResponseError
-from tenacity import retry, stop_after_attempt, wait_random_exponential
+from tenacity import retry, stop_after_attempt, wait_exponential
 
 from curvesim.exceptions import HttpClientError
 
-stop_rule = stop_after_attempt(10)
-wait_rule = wait_random_exponential(multiplier=1, min=2, max=20)
+stop_rule = stop_after_attempt(8)
+wait_rule = wait_exponential(multiplier=1.5, min=2, max=60)
 
 
 class HTTP:
     @staticmethod
     @retry(stop=stop_rule, wait=wait_rule)
     async def get(url, params=None):
```

### Comparing `curvesim-0.4.0a2/curvesim/network/llamaAPI.py` & `curvesim-0.4.5/curvesim/network/llamaAPI.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/network/nomics.py` & `curvesim-0.4.5/curvesim/network/nomics.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/network/subgraph.py` & `curvesim-0.4.5/curvesim/network/subgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Network connector for subgraphs
 """
 
 from asyncio import gather
 from datetime import datetime, timedelta, timezone
+from decimal import Decimal
 
 import pandas as pd
 from eth_utils import to_checksum_address
 
 from curvesim.logging import get_logger
 
 from ..exceptions import SubgraphResultError
@@ -222,25 +223,29 @@
         for _r in r:
             _vol = [float(e["volume"]) for e in _r]
             vol.append(_vol)
 
     return vol
 
 
-async def _pool_snapshot(address, chain):
-    q = (
-        """
+async def _pool_snapshot(address, chain, end_ts=None):
+    if not end_ts:
+        end_date = datetime.now(timezone.utc)
+        end_ts = int(end_date.timestamp())
+
+    q = """
         {
           dailyPoolSnapshots(
             orderBy: timestamp,
             orderDirection: desc,
             first: 1,
             where:
               {
                 pool: "%s"
+                timestamp_lte: %d
               }
           )
           {
             pool {
               name
               address
               symbol
@@ -273,30 +278,31 @@
             priceOracle
             lastPrices
             lastPricesTimestamp
             xcpProfit
             xcpProfitA
           }
         }
-    """
-        % address.lower()
+    """ % (
+        address.lower(),
+        end_ts,
     )
 
     r = await convex(chain, q)
     try:
         r = r["dailyPoolSnapshots"][0]
     except IndexError:
         raise SubgraphResultError(
             f"No daily snapshot for this pool: {address}, {chain}"
         )
 
     return r
 
 
-async def pool_snapshot(address, chain):
+async def pool_snapshot(address, chain, end_ts=None):
     """
     Async function to pull pool state and metadata from daily snapshots.
 
     Parameters
     ----------
     address : str
         The pool address.
@@ -306,15 +312,16 @@
 
     Returns
     -------
     dict
         A formatted dict of pool state/metadata information.
 
     """
-    r = await _pool_snapshot(address, chain)
+    r = await _pool_snapshot(address, chain, end_ts)
+    logger.debug(f"Pool snapshot: {r}")
 
     # Flatten
     pool = r.pop("pool")
     r.update(pool)
 
     # D
     D = compute_D(r["normalizedReserves"], r["A"])
@@ -340,32 +347,32 @@
 
     # Reserves
     normalized_reserves = [int(r) for r in r["normalizedReserves"]]
     unnormalized_reserves = [int(r) for r in r["reserves"]]
 
     # Basepool
     if r["metapool"]:
-        basepool = await pool_snapshot(r["basePool"], chain)
+        basepool = await pool_snapshot(r["basePool"], chain, end_ts)
     else:
         basepool = None
 
     # Output
     if version == 1:
         data = {
             "name": r["name"],
             "address": to_checksum_address(r["address"]),
             "chain": chain,
             "symbol": r["symbol"].strip(),
             "version": version,
             "pool_type": r["poolType"],
             "params": {
                 "A": int(r["A"]),
-                "fee": int(float(r["fee"]) * 10**10),
+                "fee": int(Decimal(r["fee"]) * 10**10),
                 "fee_mul": fee_mul,
-                "admin_fee": int(r["adminFee"]),
+                "admin_fee": int(Decimal(r["adminFee"]) * 10**10),
             },
             "coins": coins,
             "reserves": {
                 "D": D,
                 "by_coin": normalized_reserves,
                 "unnormalized_by_coin": unnormalized_reserves,
                 "virtual_price": int(r["virtualPrice"]),
@@ -391,15 +398,15 @@
                 "allowed_extra_profit": int(r["allowedExtraProfit"]),
                 "adjustment_step": int(r["adjustmentStep"]),
                 "ma_half_time": int(r["adjustmentStep"]),
                 "price_scale": int(r["priceScale"]),
                 "price_oracle": int(r["priceOracle"]),
                 "last_prices": int(r["lastPrices"]),
                 "last_prices_timestamp": int(r["lastPricesTimestamp"]),
-                "admin_fee": int(r["adminFee"]),
+                "admin_fee": int(Decimal(r["adminFee"]) * 10**10),
                 "xcp_profit": int(r["xcpProfit"]),
                 "xcp_profit_a": int(r["xcpProfitA"]),
             },
             "coins": coins,
             "reserves": {
                 "D": D,
                 "by_coin": normalized_reserves,
```

### Comparing `curvesim-0.4.0a2/curvesim/network/utils.py` & `curvesim-0.4.5/curvesim/network/utils.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/network/web3.py` & `curvesim-0.4.5/curvesim/network/web3.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     """
     abi = abi or await ABI(address)
     w3 = _load_web3()
     c = w3.eth.contract(address=address, abi=abi)
     return c
 
 
-async def _underlying_coin_address(address):
+async def _underlying_coin_info(address):
     c = await contract(address)
 
     fns = ["upgradeToAndCall", "underlying", "token"]
     n_fns = len(fns) - 1
 
     for i, fn in enumerate(fns):
         if fn in dir(c.functions):
@@ -145,20 +145,22 @@
 
     # Handle Aave proxy
     if fn == "upgradeToAndCall":
         abi = await ABI("0x1C050bCa8BAbe53Ef769d0d2e411f556e1a27E7B")
         c = await contract(address, abi)
         fn = "UNDERLYING_ASSET_ADDRESS"
 
-    address = await c.functions[fn]().call()
+    address, decimals = await gather(
+        c.functions[fn]().call(), c.functions.decimals().call()
+    )
 
-    return address
+    return address, decimals
 
 
-async def underlying_coin_addresses(addresses):
+async def underlying_coin_info(addresses):
     """
     Async function to get the underlying coin addresses for lending tokens
     (aTokens, cTokens, and yTokens).
 
     Parameters
     ----------
     addresses : iterable of str
@@ -167,24 +169,25 @@
     Returns
     -------
     addresses : list of str
         The addresses of the underlying tokens.
 
     """
     if isinstance(addresses, str):
-        addrs = await _underlying_coin_address(addresses)
+        addrs, decimals = await _underlying_coin_info(addresses)
 
     else:
         tasks = []
         for address in addresses:
-            tasks.append(_underlying_coin_address(address))
+            tasks.append(_underlying_coin_info(address))
 
-        addrs = await gather(*tasks)
+        response = await gather(*tasks)
+        addrs, decimals = map(list, zip(*response))
 
-    return addrs
+    return addrs, decimals
 
 
 # Sync
 explorer_sync = sync(explorer)
 ABI_sync = sync(ABI)
 contract_sync = sync(contract)
-underlying_coin_addresses_sync = sync(underlying_coin_addresses)
+underlying_coin_info_sync = sync(underlying_coin_info)
```

### Comparing `curvesim-0.4.0a2/curvesim/overrides/__init__.py` & `curvesim-0.4.5/curvesim/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pipelines/utils.py` & `curvesim-0.4.5/curvesim/pipelines/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Miscellaneous utility functions."""
 from math import factorial
 
-from numpy import append
+from numpy import append, array
 
 from curvesim.logging import get_logger
 from curvesim.pool import CurveMetaPool, CurvePool
 
 logger = get_logger(__name__)
 
 
 def compute_volume_multipliers(pool_vol, market_vol, n, pool_type, mode=1):
     """
     Computes volume multipliers (vol_mult) used for volume limiting.
 
     Parameters
     ----------
-    pool_vol : numpy.ndarray
+    pool_vol : float, int, or list
         Total volume for the pool over the simulation period.
 
-    market_vol : numpy.ndarray
+    market_vol : dict
         Total market volume for each token pair over the simulation period.
 
     n : int
         The number of token-types in the pool (e.g., DAI, USDC, USDT = 3)
 
     pool_type : str
         "CurvePool" or "CurveMetaPool"
@@ -33,37 +33,45 @@
         1: limits trade volumes proportionally to market volume for each pair
 
         2: limits trade volumes equally across pairs
 
         3: mode 2 for trades with meta-pool asset, mode 1 for basepool-only trades
 
     """
-    if pool_type is CurvePool:
-        vol_mult = pool_vol_mult(pool_vol, market_vol, n, mode)
+    pairs, market_vol = zip(*market_vol.items())
+    pool_vol_array = array(pool_vol)
+    market_vol_array = array(market_vol)
+
+    try:
+        get_vol_mult = _pool_functions[pool_type]
+    except KeyError as e:
+        raise TypeError(
+            f"Pool type {pool_type} not supported by volume limiter."
+        ) from e
 
-    elif pool_type is CurveMetaPool:
-        vol_mult = metapool_vol_mult(pool_vol, market_vol, n, mode)
+    vol_mult = get_vol_mult(pool_vol_array, market_vol_array, n, mode)
+    vol_mult_dict = dict(zip(pairs, vol_mult))
 
-    else:
-        raise TypeError(f"Pool type {pool_type} not supported by this pipeline")
-
-    logger.info(f"Volume Multipliers: {vol_mult}")
-    return vol_mult
+    logger.info(f"Volume Multipliers: {format_info_str(vol_mult_dict)}")
+    return vol_mult_dict
 
 
 def pool_vol_mult(pool_vol, market_vol, n, mode):
     if mode == 1:
-        vol_mult = pool_vol / market_vol.sum()
+        vol_mult = [pool_vol / market_vol.sum()] * n
 
-    if mode == 2:
+    elif mode == 2:
         vol_mult = pool_vol.repeat(n) / n / market_vol
 
-    if mode == 3:
+    elif mode == 3:
         logger.info("Vol_mode=3 only available for meta-pools. Reverting to vol_mode=1")
-        vol_mult = pool_vol / market_vol.sum()
+        vol_mult = [pool_vol / market_vol.sum()] * n
+
+    else:
+        raise ValueError(f"Mode must be integer 1, 2, or 3, not {mode}.")
 
     return vol_mult
 
 
 def metapool_vol_mult(pool_vol, market_vol, n, mode):
     pool_vol_meta = pool_vol[0]
     pool_vol_base = pool_vol[1]
@@ -86,8 +94,20 @@
 
     elif mode == 3:
         vol_mult = append(
             pool_vol_meta.repeat(n[1]) / n[1] / mkt_vol_meta,
             pool_vol_base / mkt_vol_base.sum().repeat(n_base_pairs),
         )
 
+    else:
+        raise ValueError(f"Mode must be integer 1, 2, or 3, not {mode}.")
+
     return vol_mult
+
+
+def format_info_str(vol_mult_dict):
+    info = [f"{base}/{quote}: {mult}" for (base, quote), mult in vol_mult_dict.items()]
+    new_line = "\n    "
+    return new_line + new_line.join(info)
+
+
+_pool_functions = {CurvePool: pool_vol_mult, CurveMetaPool: metapool_vol_mult}
```

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/chart_properties.py` & `curvesim-0.4.5/curvesim/plot/altair/chart_properties.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/make_chart.py` & `curvesim-0.4.5/curvesim/plot/altair/make_chart.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/results/make_page.py` & `curvesim-0.4.5/curvesim/plot/altair/results/make_page.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/results/preprocessing.py` & `curvesim-0.4.5/curvesim/plot/altair/results/preprocessing.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/results/result_plotter.py` & `curvesim-0.4.5/curvesim/plot/altair/results/result_plotter.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/results/result_selectors.py` & `curvesim-0.4.5/curvesim/plot/altair/results/result_selectors.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/selectors.py` & `curvesim-0.4.5/curvesim/plot/altair/selectors.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/altair/styles.py` & `curvesim-0.4.5/curvesim/plot/altair/styles.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/plot/result_plotter.py` & `curvesim-0.4.5/curvesim/plot/result_plotter.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/__init__.py` & `curvesim-0.4.5/curvesim/pool/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -201,26 +201,35 @@
 def get_sim_pool(
     pool_metadata,
     chain="mainnet",
     balanced=True,
     balanced_base=True,
     custom_kwargs=None,
     pool_data_cache=None,
+    end_ts=None,
 ):
     """
     Effectively the same as the `get_pool` function but returns
     an object in the `SimPool` hierarchy.
     """
     custom_kwargs = custom_kwargs or {}
 
     if isinstance(pool_metadata, str):
-        pool_metadata = get_metadata(pool_metadata, chain=chain)
+        pool_metadata = get_metadata(pool_metadata, chain=chain, end_ts=end_ts)
     elif isinstance(pool_metadata, dict):
+        if end_ts:
+            raise CurvesimValueError(
+                "`end_ts` has no effect unless pool address is used."
+            )
         pool_metadata = PoolMetaData(pool_metadata)
     elif isinstance(pool_metadata, PoolMetaDataInterface):
+        if end_ts:
+            raise CurvesimValueError(
+                "`end_ts` has no effect unless pool address is used."
+            )
         pass
     else:
         raise CurvesimValueError(
             "`pool_metadata` must be of type `str`, `dict`, or `PoolMetaDataInterface`."
         )
 
     init_kwargs = pool_metadata.init_kwargs(balanced, balanced_base, normalize=True)
```

### Comparing `curvesim-0.4.0a2/curvesim/pool/base.py` & `curvesim-0.4.5/curvesim/pool/base.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/cryptoswap/pool.py` & `curvesim-0.4.5/curvesim/pool/cryptoswap/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/sim_interface/raipool.py` & `curvesim-0.4.5/curvesim/pool/sim_interface/raipool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/snapshot.py` & `curvesim-0.4.5/curvesim/pool/snapshot.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/stableswap/metapool.py` & `curvesim-0.4.5/curvesim/pool/stableswap/metapool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/stableswap/pool.py` & `curvesim-0.4.5/curvesim/pool/stableswap/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool/stableswap/raipool.py` & `curvesim-0.4.5/curvesim/pool/stableswap/raipool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/__init__.py` & `curvesim-0.4.5/curvesim/pool_data/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,21 +34,21 @@
 
     Returns
     -------
     :class:`PoolDataCache`
 
     """
     # TODO: validate function arguments
-    metadata_dict = from_address(address, chain)
+    metadata_dict = from_address(address, chain, end_ts=end)
     pool_data = PoolDataCache(metadata_dict, days=days, end=end)
 
     return pool_data
 
 
-def get_metadata(address, chain="mainnet"):
+def get_metadata(address, chain="mainnet", end_ts=None):
     """
     Pulls pool state and metadata from daily snapshot.
 
     Parameters
     ----------
     address : str
         Pool address prefixed with “0x”.
@@ -58,11 +58,11 @@
 
     Returns
     -------
     :class:`~curvesim.pool_data.metadata.PoolMetaDataInterface`
 
     """
     # TODO: validate function arguments
-    metadata_dict = from_address(address, chain)
+    metadata_dict = from_address(address, chain, end_ts=end_ts)
     metadata = PoolMetaData(metadata_dict)
 
     return metadata
```

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/cache.py` & `curvesim-0.4.5/curvesim/pool_data/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from numpy import array
-
 from curvesim.exceptions import CurvesimValueError
 from curvesim.logging import get_logger
 from curvesim.network.subgraph import redemption_prices_sync as _redemption_prices
 from curvesim.network.subgraph import volume_sync as _volume
 from curvesim.pool.stableswap.metapool import CurveMetaPool
 from curvesim.pool_data.metadata.base import PoolMetaDataInterface
 
@@ -106,18 +104,18 @@
         end = self.end
 
         if issubclass(self.metadata.pool_type, CurveMetaPool):
             # pylint: disable-next=protected-access
             basepool_address = self.metadata._dict["basepool"]["address"]
             addresses = [addresses, basepool_address]
             vol = _volume(addresses, chain, days=days, end=end)
-            summed_vol = array([sum(v) for v in vol])
+            summed_vol = [sum(v) for v in vol]
         else:
             vol = _volume(addresses, chain, days=days, end=end)
-            summed_vol = array(sum(vol))
+            summed_vol = sum(vol)
 
         return summed_vol
 
     @property
     def redemption_prices(self):
         """
         Fetches the pool's redemption price over the specified number of days.
```

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/metadata/__init__.py` & `curvesim-0.4.5/curvesim/pool_data/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/metadata/base.py` & `curvesim-0.4.5/curvesim/pool_data/metadata/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from abc import abstractmethod, abstractproperty
+from abc import ABC, abstractmethod, abstractproperty
 
 
-class PoolMetaDataInterface:
+class PoolMetaDataInterface(ABC):
     @abstractmethod
     def init_kwargs(self, balanced=True, balanced_base=True, normalize=True):
         raise NotImplementedError
 
     @abstractproperty
     def address(self):
         raise NotImplementedError
@@ -90,15 +90,15 @@
 
             N_metapool includes the basepool LP token.
 
         """
         raise NotImplementedError
 
 
-class PoolMetaDataBase(PoolMetaDataInterface):
+class PoolMetaDataBase(PoolMetaDataInterface, ABC):
     def __init__(self, metadata_dict, pool_type, sim_pool_type):
         self._dict = metadata_dict
         self._pool_type = pool_type
         self._sim_pool_type = sim_pool_type
 
     @property
     def address(self):
```

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/metadata/cryptoswap.py` & `curvesim-0.4.5/curvesim/pool_data/metadata/cryptoswap.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/metadata/stableswap.py` & `curvesim-0.4.5/curvesim/pool_data/metadata/stableswap.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/curvesim/pool_data/queries.py` & `curvesim-0.4.5/curvesim/pool_data/queries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 
-from ..network.coingecko import crosschain_coin_addresses_sync
 from ..network.subgraph import pool_snapshot_sync, symbol_address_sync
-from ..network.web3 import underlying_coin_addresses_sync
+from ..network.web3 import underlying_coin_info_sync
 
 
-def from_address(address, chain):
+def from_address(address, chain, end_ts=None):
     """
     Returns
 
     Parameters
     ----------
     address: str
         Address prefixed with '0x'
@@ -18,31 +17,31 @@
 
     Returns
     -------
     Pool snapshot dictionary in the format returned by
     :func:`curvesim.network.subgraph.pool_snapshot`.
     """
     loop = asyncio.get_event_loop()
-    data = pool_snapshot_sync(address, chain, event_loop=loop)
-
-    # Get mainnet addresses for coins
-    m_addrs = crosschain_coin_addresses_sync(
-        data["coins"]["addresses"], chain, "mainnet", event_loop=loop
-    )
-
-    data["coins"]["addresses"] = m_addrs
+    data = pool_snapshot_sync(address, chain, end_ts=end_ts, event_loop=loop)
 
     # Get underlying token addresses
     if data["pool_type"] == "LENDING":
-        u_addrs = underlying_coin_addresses_sync(m_addrs, event_loop=loop)
+        u_addrs, u_decimals = underlying_coin_info_sync(
+            data["coins"]["addresses"], event_loop=loop
+        )
 
         m = data.pop("coins")
         names = [n[1:] for n in m["names"]]
 
-        data["coins"] = {"names": names, "addresses": u_addrs, "wrapper": m}
+        data["coins"] = {
+            "names": names,
+            "addresses": u_addrs,
+            "decimals": u_decimals,
+            "wrapper": m,
+        }
 
     return data
 
 
 def from_symbol(symbol, chain):
     address = symbol_address_sync(symbol, chain)
```

### Comparing `curvesim-0.4.0a2/curvesim/price_data/__init__.py` & `curvesim-0.4.5/curvesim/price_data/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 Tools for retrieving price data.
-Currently supports Coingecko, Nomics, and locally stored data.
-
-To use nomics, set the OS environment variable NOMICS_API_KEY.
+Currently supports Coingecko and locally stored data.
 
+Note
+-----
+Nomics data is deprecated.
 """
 
 from curvesim.exceptions import NetworkError
 
 from .sources import coingecko, local
 
 
-def get(coins, days=60, data_dir="data", src="coingecko", end=None):
+def get(coins, chain="mainnet", days=60, data_dir="data", src="coingecko", end=None):
     """
     Pull price and volume data for given coins.
 
     Data is returned for all pairwise combinations of the input coins.
 
     Parameters
     ----------
@@ -41,15 +42,15 @@
         Timestamped volumes for each pair of coins.
 
     pzero : int or pandas.Series
         Proportion of timestamps with zero volume.
 
     """
     if src == "coingecko":
-        prices, volumes, pzero = coingecko(coins, days=days)
+        prices, volumes, pzero = coingecko(coins, chain=chain, days=days, end=end)
 
     elif src == "nomics":
         raise NetworkError("Nomics data is no longer supported.")
 
     elif src == "local":
         prices, volumes, pzero = local(coins, data_dir=data_dir, end=end)
```

### Comparing `curvesim-0.4.0a2/curvesim/price_data/sources.py` & `curvesim-0.4.5/curvesim/price_data/sources.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,19 @@
-from datetime import datetime, timedelta, timezone
+from datetime import datetime, timezone
 
 from curvesim.logging import get_logger
 from curvesim.network import coingecko as _coingecko
 from curvesim.network import nomics as _nomics
 
 logger = get_logger(__name__)
 
 
-def nomics(coins, days=60, data_dir="data", end=None):
-    if end is None:
-        t_end = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
-        custom_suffix = ""
-    else:
-        t_end = datetime.fromtimestamp(end, tz=timezone.utc)
-        custom_suffix = "-" + str(end)
-    t_start = t_end - timedelta(days=days)
-
-    logger.info("Fetching Nomics price data...")
-    logger.info("Timerange: %s to %s" % (str(t_start), str(t_end)))
-
-    _nomics.update(
-        coins, None, t_start, t_end, data_dir=data_dir, custom_suffix=custom_suffix
-    )
-    prices, volumes, pzero = _nomics.pool_prices(
-        coins, data_dir=data_dir, custom_suffix=custom_suffix
-    )
-
-    return prices, volumes, pzero
-
-
-def coingecko(coins, days=60):
+def coingecko(coins, chain="mainnet", days=60, end=None):
     logger.info("Fetching CoinGecko price data...")
-    prices, volumes = _coingecko.pool_prices(coins, "usd", days)
+    prices, volumes = _coingecko.pool_prices(coins, "usd", days, chain=chain, end=end)
     pzero = 0
 
     return prices, volumes, pzero
 
 
 def local(coins, data_dir="data", end=None):
     logger.info("Using local data...")
```

### Comparing `curvesim-0.4.0a2/curvesim/sim/__init__.py` & `curvesim-0.4.5/curvesim/sim/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 """
-A simulation runs trades against Curve pools, possibly a variety of
-informed and noisy trades, although currently only "optimal" arbitrages
-are supported.
+A simulation runs trades against Curve pools, using a strategy that may
+utilize different types of informed or noise trades.
 
-The primary use-case is to determine optimal amplitude (A) and
-fee parameters given historical price and volume feeds.
+The :mod:`simulation pipeline framework <curvesim.pipelines>` allows the
+user to build custom strategies for simulation.
+
+Most users will want to use the `autosim` function, which supports
+"optimal" arbitrages via the
+:func:`volume-limited arbitrage pipeline <curvesim.pipelines.vol_limited_arb.pipeline>`.
+The primary use-case is to determine optimal amplitude (A) and fee
+parameters given historical price and volume feeds.
 """
 from curvesim.logging import get_logger
-from curvesim.pipelines.arbitrage import DEFAULT_PARAMS, volume_limited_arbitrage
+from curvesim.pipelines.vol_limited_arb import DEFAULT_PARAMS
+from curvesim.pipelines.vol_limited_arb import pipeline as volume_limited_arbitrage
 from curvesim.pool_data import get_metadata
 
 logger = get_logger(__name__)
 
 
 def autosim(
     pool=None, chain="mainnet", pool_metadata=None, pool_data_cache=None, **kwargs
```

### Comparing `curvesim-0.4.0a2/curvesim/utils.py` & `curvesim-0.4.5/curvesim/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 """Utlity functions for general usage in Curvesim."""
 import functools
 import inspect
 import os
 import re
+import sys
+from dataclasses import dataclass as _dataclass
 from itertools import combinations
 
 from dotenv import load_dotenv
 
 from curvesim.exceptions import CurvesimException, MissingEnvVarError
 
 load_dotenv()
 
+is_py310 = sys.version_info.minor >= 10 or sys.version_info.major > 3
+"""
+Some utils require knowing the python version.  Right now it's only important to
+distinguish between 3.10 and earlier versions.
+"""
 
-# Dummy value for optional default arg
-# so that any value, including `None`,
-# can be set as a default.
 _NOT_VALUE = object()
+"""
+Dummy value for optional default arg
+so that any value, including `None`,
+can be set as a default.
+"""
 
 
 def get_env_var(var_name, default=_NOT_VALUE):
     """
     Retrieve environment variable.
 
     Parameters
@@ -127,7 +136,23 @@
     list
         Sorted pairwise combinations of the input.
     """
     if isinstance(arg, int):
         arg = range(arg)
 
     return list(combinations(arg, 2))
+
+
+def dataclass(*args, **kwargs):
+    """
+    Slightly modified version of the standard library's `dataclass`.
+
+    The modification is to allow the setting of slots on versions of
+    python before 3.10.
+
+    Right now, we just remove the `slots` kwarg if it exists, but in the
+    future we can implement our own custom slots for old versions.
+    """
+    if "slots" in kwargs and not is_py310:
+        del kwargs["slots"]
+
+    return _dataclass(*args, **kwargs)
```

### Comparing `curvesim-0.4.0a2/curvesim.egg-info/SOURCES.txt` & `curvesim-0.4.5/curvesim.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -36,17 +36,22 @@
 curvesim/network/llamaAPI.py
 curvesim/network/nomics.py
 curvesim/network/subgraph.py
 curvesim/network/utils.py
 curvesim/network/web3.py
 curvesim/overrides/__init__.py
 curvesim/pipelines/__init__.py
-curvesim/pipelines/arbitrage.py
-curvesim/pipelines/templates.py
 curvesim/pipelines/utils.py
+curvesim/pipelines/simple/__init__.py
+curvesim/pipelines/simple/__main__.py
+curvesim/pipelines/simple/strategy.py
+curvesim/pipelines/simple/trader.py
+curvesim/pipelines/vol_limited_arb/__init__.py
+curvesim/pipelines/vol_limited_arb/strategy.py
+curvesim/pipelines/vol_limited_arb/trader.py
 curvesim/plot/__init__.py
 curvesim/plot/result_plotter.py
 curvesim/plot/altair/__init__.py
 curvesim/plot/altair/chart_properties.py
 curvesim/plot/altair/make_chart.py
 curvesim/plot/altair/selectors.py
 curvesim/plot/altair/styles.py
@@ -58,38 +63,45 @@
 curvesim/plot/altair/results/tooltip.py
 curvesim/pool/__init__.py
 curvesim/pool/base.py
 curvesim/pool/snapshot.py
 curvesim/pool/cryptoswap/__init__.py
 curvesim/pool/cryptoswap/pool.py
 curvesim/pool/sim_interface/__init__.py
+curvesim/pool/sim_interface/asset_indices.py
 curvesim/pool/sim_interface/metapool.py
 curvesim/pool/sim_interface/pool.py
 curvesim/pool/sim_interface/raipool.py
-curvesim/pool/sim_interface/simpool.py
 curvesim/pool/stableswap/__init__.py
 curvesim/pool/stableswap/metapool.py
 curvesim/pool/stableswap/pool.py
 curvesim/pool/stableswap/raipool.py
 curvesim/pool_data/__init__.py
 curvesim/pool_data/cache.py
 curvesim/pool_data/queries.py
 curvesim/pool_data/metadata/__init__.py
 curvesim/pool_data/metadata/base.py
 curvesim/pool_data/metadata/cryptoswap.py
 curvesim/pool_data/metadata/stableswap.py
 curvesim/price_data/__init__.py
 curvesim/price_data/sources.py
 curvesim/sim/__init__.py
+curvesim/templates/__init__.py
+curvesim/templates/samplers.py
+curvesim/templates/sim_assets.py
+curvesim/templates/sim_pool.py
+curvesim/templates/strategy.py
+curvesim/templates/trader.py
 test/fixtures/__init__.py
 test/fixtures/pool.py
 test/integration/__init__.py
+test/integration/test_pool_metadata.py
 test/integration/test_subgraph.py
 test/scripts/__init__.py
 test/scripts/make_test_data.py
 test/unit/__init__.py
+test/unit/test_coin_indices_mixin.py
 test/unit/test_cryptopool.py
 test/unit/test_metapool.py
 test/unit/test_pool.py
 test/unit/test_pool_metadata.py
-test/unit/test_sim_stableswap.py
 test/unit/test_snapshot.py
```

### Comparing `curvesim-0.4.0a2/setup.cfg` & `curvesim-0.4.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0.a2
+current_version = 0.4.5
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>.*)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{build}
 	{major}.{minor}.{patch}
 commit = True
 tag = True
 
@@ -59,14 +59,15 @@
 	Intended Audience :: Financial and Insurance Industry
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 project_urls = 
 	Documentation = https://curvesim.readthedocs.io
 	Source = https://github.com/curveresearch/curvesim
 	Tracker = https://github.com/curveresearch/curvesim/issues
 
 [options]
 packages = find:
```

### Comparing `curvesim-0.4.0a2/test/fixtures/pool.py` & `curvesim-0.4.5/test/fixtures/pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/test/integration/test_subgraph.py` & `curvesim-0.4.5/test/integration/test_subgraph.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,48 +9,54 @@
 
 def test_convex_subgraph_volume_query():
     """Test the volume query."""
 
     chain = "mainnet"
     address = "0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7"
     _volume_sync = sync(_volume)
-    volumes = _volume_sync(address, chain, days=2)
+    volumes = _volume_sync(address, chain, days=2, end=1686700800)
     assert len(volumes) == 2
 
-    volumes = _volume_sync(ZERO_ADDRESS, chain, days=2)
+    volumes = _volume_sync(ZERO_ADDRESS, chain, days=2, end=1686700800)
     assert len(volumes) == 0
 
 
 def test_convex_subgraph_stableswap_snapshot_query():
     """Test the pool snapshot query for stableswap."""
 
     chain = "mainnet"
     address = "0xbEbc44782C7dB0a1A60Cb6fe97d0b483032FF1C7"
+    end_ts = 1687305600
     _snapshot_sync = sync(pool_snapshot)
-    snapshot = _snapshot_sync(address, chain)
+    snapshot = _snapshot_sync(address, chain, end_ts=end_ts)
     assert snapshot["address"] == address
     assert snapshot["chain"] == chain
 
+    assert snapshot["timestamp"] <= end_ts
+
     assert snapshot["version"] == 1
 
     params = snapshot["params"]
     assert params["A"] > 0
 
     with pytest.raises(SubgraphError):
         _snapshot_sync(ZERO_ADDRESS, chain)
 
 
 def test_convex_subgraph_cryptoswap_snapshot_query():
     """Test the pool snapshot query for cryptoswap."""
 
     chain = "mainnet"
     address = "0x3211C6cBeF1429da3D0d58494938299C92Ad5860"
+    end_ts = 1687305600
     _snapshot_sync = sync(pool_snapshot)
-    snapshot = _snapshot_sync(address, chain)
+    snapshot = _snapshot_sync(address, chain, end_ts=end_ts)
     assert snapshot["address"] == address
     assert snapshot["chain"] == chain
 
+    assert snapshot["timestamp"] <= end_ts
+
     assert snapshot["version"] == 2
 
     params = snapshot["params"]
     assert params["A"] > 0
     assert params["gamma"] > 0
```

### Comparing `curvesim-0.4.0a2/test/scripts/make_test_data.py` & `curvesim-0.4.5/test/scripts/make_test_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pickle
 import sys
 
 import curvesim
 
 # from curvesim.network.nomics import coin_ids_from_addresses_sync
-from curvesim.pipelines.arbitrage import volume_limited_arbitrage as pipeline
+from curvesim.pipelines.vol_limited_arb import pipeline
 
 # import shutil
 # from itertools import combinations
 
 
 def main(fetch_data=False):
     """
```

### Comparing `curvesim-0.4.0a2/test/unit/test_cryptopool.py` & `curvesim-0.4.5/test/unit/test_cryptopool.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
 
     # profit increased but not enough to adjust the price scale
     assert pool.virtual_price > old_virtual_price
     assert pool.price_scale == old_scale
 
     old_virtual_price = pool.virtual_price
 
-    xp[0] = xp[0] * 105 // 100
+    xp[0] = xp[0] * 115 // 100
 
     # omitting price will calculate the spot price in `tweak_price`
     pool._tweak_price(A, gamma, xp, 0, 0)
     vyper_cryptopool.eval(f"self.tweak_price({A_gamma}, {xp}, 0, 0)")
 
     assert pool.price_scale == vyper_cryptopool.price_scale()
     assert pool._price_oracle == vyper_cryptopool.eval("self._price_oracle")
```

### Comparing `curvesim-0.4.0a2/test/unit/test_metapool.py` & `curvesim-0.4.5/test/unit/test_metapool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/test/unit/test_pool.py` & `curvesim-0.4.5/test/unit/test_pool.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/test/unit/test_pool_metadata.py` & `curvesim-0.4.5/test/unit/test_pool_metadata.py`

 * *Files identical despite different names*

### Comparing `curvesim-0.4.0a2/test/unit/test_snapshot.py` & `curvesim-0.4.5/test/unit/test_snapshot.py`

 * *Files identical despite different names*

