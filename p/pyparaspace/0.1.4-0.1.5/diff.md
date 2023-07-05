# Comparing `tmp/pyparaspace-0.1.4.tar.gz` & `tmp/pyparaspace-0.1.5.tar.gz`

## Comparing `pyparaspace-0.1.4.tar` & `pyparaspace-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/local_dependencies/paraspace/Cargo.toml
--rw-r--r--   0        0        0     1106 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/LICENSE
--rw-r--r--   0        0        0      165 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/README.md
--rw-r--r--   0        0        0     1097 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt
--rw-r--r--   0        0        0     1315 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt
--rw-r--r--   0        0        0     2640 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt
--rw-r--r--   0        0        0        0 2023-06-17 17:54:52.000000 pyparaspace-0.1.4/local_dependencies/paraspace/examples/.emptydir
--rw-r--r--   0        0        0      130 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/scripts/mkbenchmarks.sh
--rw-r--r--   0        0        0     3795 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/scripts/plot_timeline.py
--rw-r--r--   0        0        0     1626 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/cores.rs
--rw-r--r--   0        0        0     2128 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/carbonaraproblem.py
--rw-r--r--   0        0        0     2079 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/ceramicproblem.py
--rw-r--r--   0        0        0     2422 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/goacproblem.py
--rw-r--r--   0        0        0     4776 2023-06-17 17:54:53.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/timelinedsl.py
--rw-r--r--   0        0        0      886 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/lib.rs
--rw-r--r--   0        0        0     3853 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/main.rs
--rw-r--r--   0        0        0     2373 2023-06-23 12:37:36.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/problem.rs
--rw-r--r--   0        0        0    69611 2023-06-23 12:37:36.000000 pyparaspace-0.1.4/local_dependencies/paraspace/src/transitionsolver.rs
--rw-r--r--   0        0        0     3565 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_1.rs
--rw-r--r--   0        0        0     2385 2023-06-21 14:17:33.000000 pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_2.rs
--rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/Cargo.toml
--rw-r--r--   0        0        0      756 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/.gitignore
--rw-r--r--   0        0        0      102 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/.gitmodules
--rw-r--r--   0        0        0      869 2023-06-21 15:00:11.000000 pyparaspace-0.1.4/Dockerfile
--rw-r--r--   0        0        0     1923 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/README.md
--rw-r--r--   0        0        0      390 2023-06-17 17:54:48.000000 pyparaspace-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    15373 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/src/lib.rs
--rw-r--r--   0        0        0     1932 2023-06-23 12:37:18.000000 pyparaspace-0.1.4/testPyParaspace.py
--rw-r--r--   0        0        0    20342 2023-06-23 12:37:22.000000 pyparaspace-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 pyparaspace-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 pyparaspace-0.1.5/local_dependencies/paraspace/Cargo.toml
+-rw-rw-r--   0     1000     1000     1085 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/LICENSE
+-rw-rw-r--   0     1000     1000      163 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/README.md
+-rw-rw-r--   0     1000     1000     1061 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt
+-rw-rw-r--   0     1000     1000     1272 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt
+-rw-rw-r--   0     1000     1000     2554 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt
+-rw-rw-r--   0     1000     1000        0 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/examples/.emptydir
+-rwxrwxr-x   0     1000     1000      126 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/scripts/mkbenchmarks.sh
+-rw-rw-r--   0     1000     1000     3697 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/scripts/plot_timeline.py
+-rw-rw-r--   0     1000     1000     1583 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/cores.rs
+-rw-rw-r--   0     1000     1000     2083 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/carbonaraproblem.py
+-rw-rw-r--   0     1000     1000     2031 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/ceramicproblem.py
+-rw-rw-r--   0     1000     1000     2352 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/goacproblem.py
+-rw-rw-r--   0     1000     1000     4648 2023-06-12 05:25:52.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/timelinedsl.py
+-rw-rw-r--   0     1000     1000      847 2023-06-21 11:55:19.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/lib.rs
+-rw-rw-r--   0     1000     1000     4307 2023-07-05 11:18:23.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/main.rs
+-rw-rw-r--   0     1000     1000     2277 2023-06-23 12:33:25.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/problem.rs
+-rw-rw-r--   0     1000     1000    67533 2023-07-05 11:18:23.000000 pyparaspace-0.1.5/local_dependencies/paraspace/src/transitionsolver.rs
+-rw-rw-r--   0     1000     1000     3465 2023-06-19 05:48:08.000000 pyparaspace-0.1.5/local_dependencies/paraspace/tests/transitions_1.rs
+-rw-rw-r--   0     1000     1000     2322 2023-06-19 05:48:08.000000 pyparaspace-0.1.5/local_dependencies/paraspace/tests/transitions_2.rs
+-rw-r--r--   0        0        0      386 1970-01-01 00:00:00.000000 pyparaspace-0.1.5/Cargo.toml
+-rw-rw-r--   0     1000     1000      685 2023-06-12 05:25:51.000000 pyparaspace-0.1.5/.gitignore
+-rw-rw-r--   0     1000     1000       99 2023-06-12 05:25:51.000000 pyparaspace-0.1.5/.gitmodules
+-rw-rw-r--   0     1000     1000        0 2023-06-21 11:17:26.000000 pyparaspace-0.1.5/.z3-trace
+-rw-rw-r--   0     1000     1000      843 2023-06-21 14:57:20.000000 pyparaspace-0.1.5/Dockerfile
+-rw-rw-r--   0     1000     1000     1861 2023-06-21 15:05:22.000000 pyparaspace-0.1.5/README.md
+-rw-rw-r--   0     1000     1000      374 2023-06-12 05:25:51.000000 pyparaspace-0.1.5/pyproject.toml
+-rw-rw-r--   0     1000     1000    14787 2023-06-23 12:35:31.000000 pyparaspace-0.1.5/src/lib.rs
+-rw-rw-r--   0     1000     1000     1873 2023-06-22 09:56:41.000000 pyparaspace-0.1.5/testPyParaspace.py
+-rw-rw-r--   0     1000     1000    20342 2023-07-05 12:23:47.000000 pyparaspace-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 pyparaspace-0.1.5/PKG-INFO
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/LICENSE` & `pyparaspace-0.1.5/local_dependencies/paraspace/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Bjørnar Steinnes Luteberget
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Bjørnar Steinnes Luteberget
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt` & `pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-10-26-7d48297e5fc95b983ab0350936022f3a3f758ca0.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-carbonara_1p_1c took 15.06ms
-carbonara_1p_2c took 12.04ms
-carbonara_1p_3c took 13.12ms
-carbonara_1p_4c took 14.40ms
-carbonara_1p_5c took 13.76ms
-carbonara_1p_6c took 17.38ms
-carbonara_1p_7c took 15.42ms
-carbonara_1p_8c took 20.34ms
-carbonara_1p_9c took 20.15ms
-carbonara_1p_10c took 20.50ms
-carbonara_1p_15c took 32.54ms
-carbonara_1p_20c took 43.02ms
-carbonara_1p_25c took 60.64ms
-carbonara_1p_30c took 83.56ms
-carbonara_1p_40c took 147.33ms
-carbonara_1p_50c took 230.48ms
-carbonara_1p_75c took 668.92ms
-carbonara_1p_100c took 1.35s
-carbonara_2p_1c took 12.71ms
-carbonara_2p_2c took 9.90ms
-carbonara_2p_3c took 11.22ms
-carbonara_2p_4c took 12.18ms
-carbonara_2p_5c took 19.49ms
-carbonara_2p_6c took 17.63ms
-carbonara_2p_7c took 17.85ms
-carbonara_2p_8c took 17.49ms
-carbonara_2p_9c took 22.41ms
-carbonara_2p_10c took 23.41ms
-carbonara_2p_15c took 28.48ms
-carbonara_2p_20c took 37.80ms
-carbonara_2p_25c took 77.41ms
-carbonara_2p_30c took 179.41ms
-carbonara_2p_40c took 235.39ms
-carbonara_2p_50c took 1.28s
-carbonara_2p_75c took 3.94s
-carbonara_2p_100c took 17.28s
+carbonara_1p_1c took 15.06ms
+carbonara_1p_2c took 12.04ms
+carbonara_1p_3c took 13.12ms
+carbonara_1p_4c took 14.40ms
+carbonara_1p_5c took 13.76ms
+carbonara_1p_6c took 17.38ms
+carbonara_1p_7c took 15.42ms
+carbonara_1p_8c took 20.34ms
+carbonara_1p_9c took 20.15ms
+carbonara_1p_10c took 20.50ms
+carbonara_1p_15c took 32.54ms
+carbonara_1p_20c took 43.02ms
+carbonara_1p_25c took 60.64ms
+carbonara_1p_30c took 83.56ms
+carbonara_1p_40c took 147.33ms
+carbonara_1p_50c took 230.48ms
+carbonara_1p_75c took 668.92ms
+carbonara_1p_100c took 1.35s
+carbonara_2p_1c took 12.71ms
+carbonara_2p_2c took 9.90ms
+carbonara_2p_3c took 11.22ms
+carbonara_2p_4c took 12.18ms
+carbonara_2p_5c took 19.49ms
+carbonara_2p_6c took 17.63ms
+carbonara_2p_7c took 17.85ms
+carbonara_2p_8c took 17.49ms
+carbonara_2p_9c took 22.41ms
+carbonara_2p_10c took 23.41ms
+carbonara_2p_15c took 28.48ms
+carbonara_2p_20c took 37.80ms
+carbonara_2p_25c took 77.41ms
+carbonara_2p_30c took 179.41ms
+carbonara_2p_40c took 235.39ms
+carbonara_2p_50c took 1.28s
+carbonara_2p_75c took 3.94s
+carbonara_2p_100c took 17.28s
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt` & `pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-10-27-b8d2e9b7590fb942387728e9d8089e336b111037.txt`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-Opt { input: None, output: None, perftest: true }
-carbonara_1p_1c took 16.24ms
-carbonara_1p_2c took 12.72ms
-carbonara_1p_3c took 13.57ms
-carbonara_1p_4c took 15.12ms
-carbonara_1p_5c took 17.45ms
-carbonara_1p_6c took 17.83ms
-carbonara_1p_7c took 17.92ms
-carbonara_1p_8c took 22.14ms
-carbonara_1p_9c took 24.05ms
-carbonara_1p_10c took 30.49ms
-carbonara_1p_15c took 40.81ms
-carbonara_1p_20c took 48.29ms
-carbonara_1p_25c took 67.83ms
-carbonara_1p_30c took 84.32ms
-carbonara_1p_40c took 137.88ms
-carbonara_1p_50c took 226.12ms
-carbonara_1p_75c took 654.66ms
-carbonara_1p_100c took 1.40s
-carbonara_2p_1c took 14.16ms
-carbonara_2p_2c took 13.60ms
-carbonara_2p_3c took 12.05ms
-carbonara_2p_4c took 16.32ms
-carbonara_2p_5c took 17.32ms
-carbonara_2p_6c took 18.57ms
-carbonara_2p_7c took 18.60ms
-carbonara_2p_8c took 20.83ms
-carbonara_2p_9c took 23.91ms
-carbonara_2p_10c took 27.12ms
-carbonara_2p_15c took 44.33ms
-carbonara_2p_20c took 61.43ms
-carbonara_2p_25c took 91.36ms
-carbonara_2p_30c took 120.81ms
-carbonara_2p_40c took 249.23ms
-carbonara_2p_50c took 698.14ms
-carbonara_2p_75c took 2.59s
-carbonara_2p_100c took 7.13s
-ceramic_1m_2j took 9.32ms
-ceramic_2m_4j took 28.85ms
-ceramic_2m_6j took 129.39ms
-ceramic_4m_6j took 1.79s
-ceramic_5m_10j took 102.67s
-No problem files given.
+Opt { input: None, output: None, perftest: true }
+carbonara_1p_1c took 16.24ms
+carbonara_1p_2c took 12.72ms
+carbonara_1p_3c took 13.57ms
+carbonara_1p_4c took 15.12ms
+carbonara_1p_5c took 17.45ms
+carbonara_1p_6c took 17.83ms
+carbonara_1p_7c took 17.92ms
+carbonara_1p_8c took 22.14ms
+carbonara_1p_9c took 24.05ms
+carbonara_1p_10c took 30.49ms
+carbonara_1p_15c took 40.81ms
+carbonara_1p_20c took 48.29ms
+carbonara_1p_25c took 67.83ms
+carbonara_1p_30c took 84.32ms
+carbonara_1p_40c took 137.88ms
+carbonara_1p_50c took 226.12ms
+carbonara_1p_75c took 654.66ms
+carbonara_1p_100c took 1.40s
+carbonara_2p_1c took 14.16ms
+carbonara_2p_2c took 13.60ms
+carbonara_2p_3c took 12.05ms
+carbonara_2p_4c took 16.32ms
+carbonara_2p_5c took 17.32ms
+carbonara_2p_6c took 18.57ms
+carbonara_2p_7c took 18.60ms
+carbonara_2p_8c took 20.83ms
+carbonara_2p_9c took 23.91ms
+carbonara_2p_10c took 27.12ms
+carbonara_2p_15c took 44.33ms
+carbonara_2p_20c took 61.43ms
+carbonara_2p_25c took 91.36ms
+carbonara_2p_30c took 120.81ms
+carbonara_2p_40c took 249.23ms
+carbonara_2p_50c took 698.14ms
+carbonara_2p_75c took 2.59s
+carbonara_2p_100c took 7.13s
+ceramic_1m_2j took 9.32ms
+ceramic_2m_4j took 28.85ms
+ceramic_2m_6j took 129.39ms
+ceramic_4m_6j took 1.79s
+ceramic_5m_10j took 102.67s
+No problem files given.
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt` & `pyparaspace-0.1.5/local_dependencies/paraspace/docs/perfhistory/2021-11-02-a3ef5ee9280eb1002f194bb80cca6a8103430112.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-carbonara_1p_1c took 16.54ms
-carbonara_1p_2c took 22.07ms
-carbonara_1p_3c took 18.78ms
-carbonara_1p_4c took 18.86ms
-carbonara_1p_5c took 19.10ms
-carbonara_1p_6c took 19.84ms
-carbonara_1p_7c took 20.26ms
-carbonara_1p_8c took 24.41ms
-carbonara_1p_9c took 28.88ms
-carbonara_1p_10c took 31.05ms
-carbonara_1p_15c took 37.99ms
-carbonara_1p_20c took 52.98ms
-carbonara_1p_25c took 77.25ms
-carbonara_1p_30c took 107.60ms
-carbonara_1p_40c took 207.75ms
-carbonara_1p_50c took 382.87ms
-carbonara_1p_75c took 1.36s
-carbonara_1p_100c took 3.27s
-carbonara_2p_1c took 22.45ms
-carbonara_2p_2c took 23.52ms
-carbonara_2p_3c took 23.59ms
-carbonara_2p_4c took 25.22ms
-carbonara_2p_5c took 27.32ms
-carbonara_2p_6c took 27.42ms
-carbonara_2p_7c took 27.97ms
-carbonara_2p_8c took 29.16ms
-carbonara_2p_9c took 30.64ms
-carbonara_2p_10c took 32.46ms
-carbonara_2p_15c took 35.63ms
-carbonara_2p_20c took 49.38ms
-carbonara_2p_25c took 95.02ms
-carbonara_2p_30c took 154.26ms
-carbonara_2p_40c took 290.61ms
-carbonara_2p_50c took 462.90ms
-carbonara_2p_75c took 2.17s
-carbonara_2p_100c took 3.91s
-ceramic_1m_2j took 17.34ms
-ceramic_2m_4j took 22.58ms
-ceramic_2m_6j took 26.02ms
-ceramic_4m_6j took 25.69ms
-ceramic_5m_10j took 203.31ms
-goac_1pics_1wind took 13.21ms
-goac_1pics_2wind took 14.23ms
-goac_1pics_3wind took 14.15ms
-goac_1pics_4wind took 14.19ms
-goac_1pics_5wind took 14.28ms
-goac_2pics_1wind took 15.71ms
-goac_2pics_2wind took 15.74ms
-goac_2pics_3wind took 15.80ms
-goac_2pics_4wind took 15.87ms
-goac_2pics_5wind took 16.14ms
-goac_3pics_1wind took 20.06ms
-goac_3pics_2wind took 19.75ms
-goac_3pics_3wind took 20.20ms
-goac_3pics_4wind took 19.33ms
-goac_3pics_5wind took 19.78ms
-goac_4pics_1wind took 24.99ms
-goac_4pics_2wind took 23.99ms
-goac_4pics_3wind took 23.92ms
-goac_4pics_4wind took 24.25ms
-goac_4pics_5wind took 23.80ms
-goac_5pics_1wind took 28.64ms
-goac_5pics_2wind took 29.27ms
-goac_5pics_3wind took 28.59ms
-goac_5pics_4wind took 31.11ms
-goac_5pics_5wind took 29.43ms
-goac_6pics_1wind took 34.50ms
-goac_6pics_2wind took 43.89ms
-goac_6pics_3wind took 37.13ms
-goac_6pics_4wind took 35.12ms
-goac_6pics_5wind took 35.80ms
-goac_7pics_1wind took 45.90ms
-goac_7pics_2wind took 49.28ms
-goac_7pics_3wind took 41.39ms
-goac_7pics_4wind took 39.36ms
-goac_7pics_5wind took 41.46ms
-goac_8pics_1wind took 78.49ms
-goac_8pics_2wind took 68.84ms
-goac_8pics_3wind took 77.93ms
-goac_8pics_4wind took 72.46ms
-goac_8pics_5wind took 72.97ms
-goac_9pics_1wind took 165.31ms
-goac_9pics_2wind took 138.30ms
-goac_9pics_3wind took 188.80ms
-goac_9pics_4wind took 150.25ms
-goac_9pics_5wind took 164.71ms
+carbonara_1p_1c took 16.54ms
+carbonara_1p_2c took 22.07ms
+carbonara_1p_3c took 18.78ms
+carbonara_1p_4c took 18.86ms
+carbonara_1p_5c took 19.10ms
+carbonara_1p_6c took 19.84ms
+carbonara_1p_7c took 20.26ms
+carbonara_1p_8c took 24.41ms
+carbonara_1p_9c took 28.88ms
+carbonara_1p_10c took 31.05ms
+carbonara_1p_15c took 37.99ms
+carbonara_1p_20c took 52.98ms
+carbonara_1p_25c took 77.25ms
+carbonara_1p_30c took 107.60ms
+carbonara_1p_40c took 207.75ms
+carbonara_1p_50c took 382.87ms
+carbonara_1p_75c took 1.36s
+carbonara_1p_100c took 3.27s
+carbonara_2p_1c took 22.45ms
+carbonara_2p_2c took 23.52ms
+carbonara_2p_3c took 23.59ms
+carbonara_2p_4c took 25.22ms
+carbonara_2p_5c took 27.32ms
+carbonara_2p_6c took 27.42ms
+carbonara_2p_7c took 27.97ms
+carbonara_2p_8c took 29.16ms
+carbonara_2p_9c took 30.64ms
+carbonara_2p_10c took 32.46ms
+carbonara_2p_15c took 35.63ms
+carbonara_2p_20c took 49.38ms
+carbonara_2p_25c took 95.02ms
+carbonara_2p_30c took 154.26ms
+carbonara_2p_40c took 290.61ms
+carbonara_2p_50c took 462.90ms
+carbonara_2p_75c took 2.17s
+carbonara_2p_100c took 3.91s
+ceramic_1m_2j took 17.34ms
+ceramic_2m_4j took 22.58ms
+ceramic_2m_6j took 26.02ms
+ceramic_4m_6j took 25.69ms
+ceramic_5m_10j took 203.31ms
+goac_1pics_1wind took 13.21ms
+goac_1pics_2wind took 14.23ms
+goac_1pics_3wind took 14.15ms
+goac_1pics_4wind took 14.19ms
+goac_1pics_5wind took 14.28ms
+goac_2pics_1wind took 15.71ms
+goac_2pics_2wind took 15.74ms
+goac_2pics_3wind took 15.80ms
+goac_2pics_4wind took 15.87ms
+goac_2pics_5wind took 16.14ms
+goac_3pics_1wind took 20.06ms
+goac_3pics_2wind took 19.75ms
+goac_3pics_3wind took 20.20ms
+goac_3pics_4wind took 19.33ms
+goac_3pics_5wind took 19.78ms
+goac_4pics_1wind took 24.99ms
+goac_4pics_2wind took 23.99ms
+goac_4pics_3wind took 23.92ms
+goac_4pics_4wind took 24.25ms
+goac_4pics_5wind took 23.80ms
+goac_5pics_1wind took 28.64ms
+goac_5pics_2wind took 29.27ms
+goac_5pics_3wind took 28.59ms
+goac_5pics_4wind took 31.11ms
+goac_5pics_5wind took 29.43ms
+goac_6pics_1wind took 34.50ms
+goac_6pics_2wind took 43.89ms
+goac_6pics_3wind took 37.13ms
+goac_6pics_4wind took 35.12ms
+goac_6pics_5wind took 35.80ms
+goac_7pics_1wind took 45.90ms
+goac_7pics_2wind took 49.28ms
+goac_7pics_3wind took 41.39ms
+goac_7pics_4wind took 39.36ms
+goac_7pics_5wind took 41.46ms
+goac_8pics_1wind took 78.49ms
+goac_8pics_2wind took 68.84ms
+goac_8pics_3wind took 77.93ms
+goac_8pics_4wind took 72.46ms
+goac_8pics_5wind took 72.97ms
+goac_9pics_1wind took 165.31ms
+goac_9pics_2wind took 138.30ms
+goac_9pics_3wind took 188.80ms
+goac_9pics_4wind took 150.25ms
+goac_9pics_5wind took 164.71ms
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/scripts/plot_timeline.py` & `pyparaspace-0.1.5/local_dependencies/paraspace/scripts/plot_timeline.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-import sys, json
-import matplotlib
-import matplotlib.pyplot as plt
-from collections import defaultdict
-
-colors = ["red","green","blue","purple","orange","black","gray"]
-
-filename = sys.argv[1]
-print(f"Reading file {filename}")
-
-with open(filename, "r") as f:
-    model = json.load(f)
-
-print(f"got model {model}")
-
-fig, ax = plt.subplots(figsize=(10,6),dpi=120)
-
-def rat(x):
-    return float(x[0]) / float(x[1])
-
-y_stack = []
-y_names = {}
-
-timelines = defaultdict(list)
-for token in model["tokens"]:
-    timelines[token["object_name"]].append(token)
-
-for (timeline_name,tokens) in timelines.items():
-    y_names[timeline_name] = len(y_stack)
-    intervals = []
-    for token in tokens:
-        start = token["start_time"] if token["start_time"] is not None else  token["end_time"] - 1
-        end = token["end_time"] if token["end_time"] is not None else  token["start_time"] + 1
-        intervals.append((start, end, colors[hash(token["value"]) % len(colors)], token["value"]))
-    y_stack.append( { "name": timeline_name, "intervals" : intervals })
-
-#y_names["visibility"] = len(y_stack)
-#y_stack.append({ "name": "visibility", "intervals": [(rat(x[0]),rat(x[1]),"red") for x in model["problem"]["visibility_time_windows"]] })
-#
-#for (l_idx, location) in enumerate(model["locations"]):
-#    name = f"loc{l_idx}_@{location[0]}"
-#    y_names[name] = len(y_stack)
-#    y_stack.append({"name": name, "intervals": [(location[1][0], location[1][1], "blue")]})
-#
-#for (_idx, take_picture) in enumerate(model["take_picture"]):
-#    name = f"take_@{take_picture[0]}"
-#    y_names[name] = len(y_stack)
-#    y_stack.append({"name": name, "intervals": [(take_picture[1][0], take_picture[1][1], "green")]})
-#
-#for (_idx, download) in enumerate(model["download"]):
-#    name = f"dl_{download[0]}"
-#    y_names[name] = len(y_stack)
-#    y_stack.append({"name": name, "intervals": [(download[1][0], download[1][1], "orange")]})
-
-#for (idx,water) in enumerate(model["problem"]["visibility_time_windows"]):
-#    name = f"water{idx}"
-#for (idx,oil) in enumerate(model["oil_heat"]):
-#    name = f"oil{idx}"
-#    y_names[name] = len(y_stack)
-#    y_stack.append({ "name": name, "intervals": [(oil[1],oil[2],"red")] })
-#
-#for (idx,carbonara) in enumerate(model["carbonaras"]):
-#    name = f"carbonara{idx}"
-#    y_names[name] = len(y_stack)
-#    y_stack.append({ "name": name, "intervals": [
-#        (carbonara["spaghetti_start"],carbonara["spaghetti_end"],"red"),
-#        (carbonara["lardon_start"],carbonara["lardon_end"],"green"),
-#        (carbonara["eggs_start"],carbonara["eggs_end"],"blue"),
-#        (carbonara["cook_start"],carbonara["cook_end"],"orange"),
-#        (carbonara["eat_start"],carbonara["eat_end"],"purple"),
-#    ]})
-
-
-ax.set_ylim([-0.5, len(y_stack)-1 +0.5])
-ax.set_yticks(list(range(len(y_stack))))
-ax.set_yticklabels([x["name"] for x in y_stack])
-fig.subplots_adjust(left=0.3)
-
-for item in y_stack:
-    y = y_names[item["name"]]
-    print(f"item {item}")
-    for i,x in enumerate(item["intervals"]):
-        ax.broken_barh([(x[0],x[1]-x[0])], 
-                       (y-0.4+0.1*i,0.1),
-                       facecolor=[x[2]])
-        ax.text(x[0], y-0.4+0.1*i+0.05, x[3])
-
-# ARROWS
-#for (structure_idx,structure) in enumerate(model["problem"]["structures"]):
-#    for p_idx in [structure["piece_1"], structure["piece_2"]]:
-#        p_x = model["pieces"][p_idx]["treated"]
-#        p_y = y_names[f"piece{p_idx}"]
-#        s_x = model["structures"][structure_idx]["assemble"]
-#        s_y = y_names[f"structure{structure_idx}"]
-#        ax.arrow(p_x, p_y, s_x - p_x, s_y - p_y, color="blue", head_width=0.1, head_length=0.15, length_includes_head=True)
-
-
-plt.savefig(f"{filename}.plot.png")
+import sys, json
+import matplotlib
+import matplotlib.pyplot as plt
+from collections import defaultdict
+
+colors = ["red","green","blue","purple","orange","black","gray"]
+
+filename = sys.argv[1]
+print(f"Reading file {filename}")
+
+with open(filename, "r") as f:
+    model = json.load(f)
+
+print(f"got model {model}")
+
+fig, ax = plt.subplots(figsize=(10,6),dpi=120)
+
+def rat(x):
+    return float(x[0]) / float(x[1])
+
+y_stack = []
+y_names = {}
+
+timelines = defaultdict(list)
+for token in model["tokens"]:
+    timelines[token["object_name"]].append(token)
+
+for (timeline_name,tokens) in timelines.items():
+    y_names[timeline_name] = len(y_stack)
+    intervals = []
+    for token in tokens:
+        start = token["start_time"] if token["start_time"] is not None else  token["end_time"] - 1
+        end = token["end_time"] if token["end_time"] is not None else  token["start_time"] + 1
+        intervals.append((start, end, colors[hash(token["value"]) % len(colors)], token["value"]))
+    y_stack.append( { "name": timeline_name, "intervals" : intervals })
+
+#y_names["visibility"] = len(y_stack)
+#y_stack.append({ "name": "visibility", "intervals": [(rat(x[0]),rat(x[1]),"red") for x in model["problem"]["visibility_time_windows"]] })
+#
+#for (l_idx, location) in enumerate(model["locations"]):
+#    name = f"loc{l_idx}_@{location[0]}"
+#    y_names[name] = len(y_stack)
+#    y_stack.append({"name": name, "intervals": [(location[1][0], location[1][1], "blue")]})
+#
+#for (_idx, take_picture) in enumerate(model["take_picture"]):
+#    name = f"take_@{take_picture[0]}"
+#    y_names[name] = len(y_stack)
+#    y_stack.append({"name": name, "intervals": [(take_picture[1][0], take_picture[1][1], "green")]})
+#
+#for (_idx, download) in enumerate(model["download"]):
+#    name = f"dl_{download[0]}"
+#    y_names[name] = len(y_stack)
+#    y_stack.append({"name": name, "intervals": [(download[1][0], download[1][1], "orange")]})
+
+#for (idx,water) in enumerate(model["problem"]["visibility_time_windows"]):
+#    name = f"water{idx}"
+#for (idx,oil) in enumerate(model["oil_heat"]):
+#    name = f"oil{idx}"
+#    y_names[name] = len(y_stack)
+#    y_stack.append({ "name": name, "intervals": [(oil[1],oil[2],"red")] })
+#
+#for (idx,carbonara) in enumerate(model["carbonaras"]):
+#    name = f"carbonara{idx}"
+#    y_names[name] = len(y_stack)
+#    y_stack.append({ "name": name, "intervals": [
+#        (carbonara["spaghetti_start"],carbonara["spaghetti_end"],"red"),
+#        (carbonara["lardon_start"],carbonara["lardon_end"],"green"),
+#        (carbonara["eggs_start"],carbonara["eggs_end"],"blue"),
+#        (carbonara["cook_start"],carbonara["cook_end"],"orange"),
+#        (carbonara["eat_start"],carbonara["eat_end"],"purple"),
+#    ]})
+
+
+ax.set_ylim([-0.5, len(y_stack)-1 +0.5])
+ax.set_yticks(list(range(len(y_stack))))
+ax.set_yticklabels([x["name"] for x in y_stack])
+fig.subplots_adjust(left=0.3)
+
+for item in y_stack:
+    y = y_names[item["name"]]
+    print(f"item {item}")
+    for i,x in enumerate(item["intervals"]):
+        ax.broken_barh([(x[0],x[1]-x[0])], 
+                       (y-0.4+0.1*i,0.1),
+                       facecolor=[x[2]])
+        ax.text(x[0], y-0.4+0.1*i+0.05, x[3])
+
+# ARROWS
+#for (structure_idx,structure) in enumerate(model["problem"]["structures"]):
+#    for p_idx in [structure["piece_1"], structure["piece_2"]]:
+#        p_x = model["pieces"][p_idx]["treated"]
+#        p_y = y_names[f"piece{p_idx}"]
+#        s_x = model["structures"][structure_idx]["assemble"]
+#        s_y = y_names[f"structure{structure_idx}"]
+#        ax.arrow(p_x, p_y, s_x - p_x, s_y - p_y, color="blue", head_width=0.1, head_length=0.15, length_includes_head=True)
+
+
+plt.savefig(f"{filename}.plot.png")
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/cores.rs` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/cores.rs`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-
-pub fn minimize_core<'ctx>(core: &mut Vec<z3::ast::Bool<'ctx>>, solver: &z3::Solver<'ctx>, print :impl Fn(&str)) {
-    print("Starting core minimization.");
-    let mut i = 0;
-    'minimize_loop: loop {
-        for _ in 0..core.len() {
-            let last_core_size = core.len();
-            let mut assumptions = core.clone();
-            let remove_idx = i % assumptions.len();
-            assumptions.remove(remove_idx);
-            print(&format!(
-                "Solving core #{}->{} removed {}",
-                core.len(),
-                assumptions.len(),
-                remove_idx
-            ));
-            let result = solver.check_assumptions(&assumptions);
-            if matches!(result, z3::SatResult::Unsat) {
-                *core = solver.get_unsat_core();
-                print(&format!("Minimized {}->{}", last_core_size, core.len()));
-                continue 'minimize_loop;
-            }
-            i += 1;
-        }
-        print(&"Finished core minimization.".to_string());
-        break;
-    }
-}
-
-pub fn trim_core<'ctx>(core: &mut Vec<z3::ast::Bool<'ctx>>, solver: &z3::Solver<'ctx>, print :impl Fn(&str)) {
-    print("Starting core trim.");
-    loop {
-        let last_core_size = core.len();
-        // Try to trim the core.
-        let result = solver.check_assumptions(&*core);
-        assert!(matches!(result, z3::SatResult::Unsat));
-        *core = solver.get_unsat_core();
-        if core.len() == last_core_size {
-            break;
-        } else {
-            print(&format!("Trimmed {}->{}", last_core_size, core.len()));
-        }
-    }
+
+pub fn minimize_core<'ctx>(core: &mut Vec<z3::ast::Bool<'ctx>>, solver: &z3::Solver<'ctx>, print :impl Fn(&str)) {
+    print("Starting core minimization.");
+    let mut i = 0;
+    'minimize_loop: loop {
+        for _ in 0..core.len() {
+            let last_core_size = core.len();
+            let mut assumptions = core.clone();
+            let remove_idx = i % assumptions.len();
+            assumptions.remove(remove_idx);
+            print(&format!(
+                "Solving core #{}->{} removed {}",
+                core.len(),
+                assumptions.len(),
+                remove_idx
+            ));
+            let result = solver.check_assumptions(&assumptions);
+            if matches!(result, z3::SatResult::Unsat) {
+                *core = solver.get_unsat_core();
+                print(&format!("Minimized {}->{}", last_core_size, core.len()));
+                continue 'minimize_loop;
+            }
+            i += 1;
+        }
+        print(&"Finished core minimization.".to_string());
+        break;
+    }
+}
+
+pub fn trim_core<'ctx>(core: &mut Vec<z3::ast::Bool<'ctx>>, solver: &z3::Solver<'ctx>, print :impl Fn(&str)) {
+    print("Starting core trim.");
+    loop {
+        let last_core_size = core.len();
+        // Try to trim the core.
+        let result = solver.check_assumptions(&*core);
+        assert!(matches!(result, z3::SatResult::Unsat));
+        *core = solver.get_unsat_core();
+        if core.len() == last_core_size {
+            break;
+        } else {
+            print(&format!("Trimmed {}->{}", last_core_size, core.len()));
+        }
+    }
 }
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/carbonaraproblem.py` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/carbonaraproblem.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from timelinedsl import *
-
-for plates in [1,2]:
-    for n_carbonaras in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 15, 20, 25, 30, 40, 50, 75, 100]:
-
-        p = Problem()
-
-        for _ in range(plates):
-            p.resource("Plate", capacity=1)
-
-        water1 = p.timeline("Water")
-        water1.state("Heating", dur=(10, 10), conditions=[UseResource(Any("Plate"), 1)])
-        water1.state("HotWater", conditions=[TransitionFrom("Heating")])
-
-        oil1 = p.timeline("Oil")
-        oil1.state("Heating", dur=(10, 10), conditions=[UseResource(Any("Plate"), 1)])
-        oil1.state("HotOil", conditions=[TransitionFrom("Heating")])
-
-        for i in range(n_carbonaras):
-            spaghetti = p.timeline(classname="Spaghetti", name=f"spaghetti_{i}")
-            spaghetti.state("Cooking", dur=(5, 5), conditions=[During(Any("Water"), "HotWater")])
-            spaghetti.state("Cooked", conditions=[TransitionFrom("Cooking")])
-
-            lardon = p.timeline(classname="Lardon", name=f"lardon_{i}")
-            lardon.state("Cooking", dur=(5, 5), conditions=[During(Any("Oil"), "HotOil")])
-            lardon.state("Cooked", conditions=[TransitionFrom("Cooking")])
-
-            eggs = p.timeline(classname="Eggs", name=f"eggs_{i}")
-            eggs.state("Beating", dur=(5, 5))
-            eggs.state("Beaten", conditions=[TransitionFrom("Beating")])
-
-            carbonara = p.timeline(classname="Carbonara", name=f"carbonara_{i}")
-            carbonara.state("Cooking", dur=(3, 3), conditions=[
-                StartsAfter(f"spaghetti_{i}", "Cooked"),
-                StartsAfter(f"lardon_{i}", "Cooked"),
-                StartsAfter(f"eggs_{i}", "Beaten"),
-                UseResource(Any("Plate"), 1)
-            ])
-            carbonara.state("Cooked", conditions=[TransitionFrom("Cooking")])
-            carbonara.state("Eating", dur=(5, 5), conditions=[TransitionFrom("Cooked")])
-            carbonara.state("Eaten", conditions=[TransitionFrom("Eating")])
-
-            p.goal(f"carbonara_{i}", "Eaten")
-
-        p.save_json(f"examples/carbonara_{plates}p_{n_carbonaras}c.json")
+from timelinedsl import *
+
+for plates in [1,2]:
+    for n_carbonaras in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 15, 20, 25, 30, 40, 50, 75, 100]:
+
+        p = Problem()
+
+        for _ in range(plates):
+            p.resource("Plate", capacity=1)
+
+        water1 = p.timeline("Water")
+        water1.state("Heating", dur=(10, 10), conditions=[UseResource(Any("Plate"), 1)])
+        water1.state("HotWater", conditions=[TransitionFrom("Heating")])
+
+        oil1 = p.timeline("Oil")
+        oil1.state("Heating", dur=(10, 10), conditions=[UseResource(Any("Plate"), 1)])
+        oil1.state("HotOil", conditions=[TransitionFrom("Heating")])
+
+        for i in range(n_carbonaras):
+            spaghetti = p.timeline(classname="Spaghetti", name=f"spaghetti_{i}")
+            spaghetti.state("Cooking", dur=(5, 5), conditions=[During(Any("Water"), "HotWater")])
+            spaghetti.state("Cooked", conditions=[TransitionFrom("Cooking")])
+
+            lardon = p.timeline(classname="Lardon", name=f"lardon_{i}")
+            lardon.state("Cooking", dur=(5, 5), conditions=[During(Any("Oil"), "HotOil")])
+            lardon.state("Cooked", conditions=[TransitionFrom("Cooking")])
+
+            eggs = p.timeline(classname="Eggs", name=f"eggs_{i}")
+            eggs.state("Beating", dur=(5, 5))
+            eggs.state("Beaten", conditions=[TransitionFrom("Beating")])
+
+            carbonara = p.timeline(classname="Carbonara", name=f"carbonara_{i}")
+            carbonara.state("Cooking", dur=(3, 3), conditions=[
+                StartsAfter(f"spaghetti_{i}", "Cooked"),
+                StartsAfter(f"lardon_{i}", "Cooked"),
+                StartsAfter(f"eggs_{i}", "Beaten"),
+                UseResource(Any("Plate"), 1)
+            ])
+            carbonara.state("Cooked", conditions=[TransitionFrom("Cooking")])
+            carbonara.state("Eating", dur=(5, 5), conditions=[TransitionFrom("Cooked")])
+            carbonara.state("Eaten", conditions=[TransitionFrom("Eating")])
+
+            p.goal(f"carbonara_{i}", "Eaten")
+
+        p.save_json(f"examples/carbonara_{plates}p_{n_carbonaras}c.json")
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/ceramicproblem.py` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/ceramicproblem.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from timelinedsl import *
-
-for (n_kilns,n_pieces) in [(1,2),(2,4),(2,6),(4,6),(5,10),(1,10)]:
-
-    p = Problem()
-    p.resource("Electricity", capacity=1)
-
-    for kiln_idx in range(n_kilns):
-        kiln = p.timeline("Kiln", f"kiln_{kiln_idx}")
-        kiln.state("Ready", dur=(5,None), conditions=[TransitionFrom("Fire")])
-        kiln.state("Fire", dur=(20,20), capacity=2, conditions=[
-            TransitionFrom("Ready"), 
-            UseResource(Any("Electricity"), 1)])
-        p.fact(f"kiln_{kiln_idx}", "Ready")
-
-    piece_param_types = [(5,2),(8,3),(11,1)]
-    pieces = []
-    while len(pieces) < n_pieces:
-        pieces.append(piece_param_types[len(pieces) % len(piece_param_types)])
-
-    for (piece_idx,(bake_time,treat_time)) in enumerate(pieces):
-        piece = p.timeline("Piece", f"piece_{piece_idx}")
-        piece.state("Baking", dur=(bake_time,bake_time), conditions=[
-            During(Any("Kiln"), "Fire", 1),
-        ])
-        piece.state("Baked", conditions=[TransitionFrom("Baking")])
-        piece.state("Treating", dur=(treat_time, treat_time), 
-            conditions=[TransitionFrom("Baked")])
-        piece.state("Treated", conditions=[TransitionFrom("Treating")])
-
-        if piece_idx >= 2*(n_pieces//2):
-            p.goal(f"piece_{piece_idx}", "Baked")
-
-    for structure_idx in range(n_pieces // 2):
-        structure = p.timeline("Structure", f"structure_{structure_idx}")
-        structure.state("Assembling", dur=(1,1), conditions=[
-            During(f"piece_{2*structure_idx}", "Treated"),
-            During(f"piece_{2*structure_idx +1}", "Treated")
-        ])
-        structure.state("Assembled", conditions=[TransitionFrom("Assembling")])
-        structure.state("Baking", dur=(3,3), conditions=[
-            During(Any("Kiln"), "Fire", 1),
-            TransitionFrom("Assembled"),
-        ])
-        structure.state("Baked", conditions=[TransitionFrom("Baking")])
-        p.goal(f"structure_{structure_idx}", "Baked")
-
-    p.save_json(f"examples/ceramic_{n_kilns}m_{n_pieces}j.json")
+from timelinedsl import *
+
+for (n_kilns,n_pieces) in [(1,2),(2,4),(2,6),(4,6),(5,10),(1,10)]:
+
+    p = Problem()
+    p.resource("Electricity", capacity=1)
+
+    for kiln_idx in range(n_kilns):
+        kiln = p.timeline("Kiln", f"kiln_{kiln_idx}")
+        kiln.state("Ready", dur=(5,None), conditions=[TransitionFrom("Fire")])
+        kiln.state("Fire", dur=(20,20), capacity=2, conditions=[
+            TransitionFrom("Ready"), 
+            UseResource(Any("Electricity"), 1)])
+        p.fact(f"kiln_{kiln_idx}", "Ready")
+
+    piece_param_types = [(5,2),(8,3),(11,1)]
+    pieces = []
+    while len(pieces) < n_pieces:
+        pieces.append(piece_param_types[len(pieces) % len(piece_param_types)])
+
+    for (piece_idx,(bake_time,treat_time)) in enumerate(pieces):
+        piece = p.timeline("Piece", f"piece_{piece_idx}")
+        piece.state("Baking", dur=(bake_time,bake_time), conditions=[
+            During(Any("Kiln"), "Fire", 1),
+        ])
+        piece.state("Baked", conditions=[TransitionFrom("Baking")])
+        piece.state("Treating", dur=(treat_time, treat_time), 
+            conditions=[TransitionFrom("Baked")])
+        piece.state("Treated", conditions=[TransitionFrom("Treating")])
+
+        if piece_idx >= 2*(n_pieces//2):
+            p.goal(f"piece_{piece_idx}", "Baked")
+
+    for structure_idx in range(n_pieces // 2):
+        structure = p.timeline("Structure", f"structure_{structure_idx}")
+        structure.state("Assembling", dur=(1,1), conditions=[
+            During(f"piece_{2*structure_idx}", "Treated"),
+            During(f"piece_{2*structure_idx +1}", "Treated")
+        ])
+        structure.state("Assembled", conditions=[TransitionFrom("Assembling")])
+        structure.state("Baking", dur=(3,3), conditions=[
+            During(Any("Kiln"), "Fire", 1),
+            TransitionFrom("Assembled"),
+        ])
+        structure.state("Baked", conditions=[TransitionFrom("Baking")])
+        p.goal(f"structure_{structure_idx}", "Baked")
+
+    p.save_json(f"examples/ceramic_{n_kilns}m_{n_pieces}j.json")
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/frontend/goacproblem.py` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/frontend/goacproblem.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from timelinedsl import *
-
-time_windows = [(280,4000), (8000,15000), (20000,25000), (30000,35000), (40000,45000)]
-locations = [0, 1,2,3,4,5,6,7,8,9]
-speed = 1
-download_time = 6*40
-take_pic_time = 50
-edges = [
-        (0, 1, 100),
-        (0, 2, 200),
-        (0, 4, 100),
-        (0, 5, 200),
-        (0, 9, 300),
-        (1, 2, 100),
-        (1, 6, 200),
-        (2, 3, 100),
-        (2, 7, 200),
-        (2, 8, 300),
-        (3, 4, 200),
-        (3, 7, 100),
-        (3, 8, 200),
-        (4, 5, 100),
-        (4, 9, 200),
-        (5, 6, 100),
-        (5, 7, 200),
-        (5, 9, 100),
-        (6, 7, 100),
-        (7, 8, 100),
-        (8, 9, 200),
-]
-
-edges = edges + [(b,a,l) for a,b,l in edges]
-
-
-for n_pics in [1,2,3,4,5,6,7,8,9]:
-    for n_windows in [1,2,3,4,5]:
-
-        p = Problem()
-        p.resource("Antenna", name="Antenna", capacity=1)
-        for (start,end) in time_windows[:n_windows]:
-            p.fact("Visibility", "Available", start=start, end=end)
-        
-        loc_timeline = p.timeline("Location", name="loc")
-        p.fact("loc", "At(0)",start=0) # Start at location 0
-
-        for loc in locations:
-            loc_timeline.state(f"At({loc})")
-        for a,b,l in edges:
-            loc_timeline.state(f"Going({locations[a]},{locations[b]})", dur=(l,l), conditions=[
-                TransitionFrom(f"At({locations[a]})"), 
-                TransitionTo(f"At({locations[b]})")])
-        
-        for loc_idx in range(n_pics):
-
-            # Take the picture
-            pic_timeline = p.timeline("HavePicture", name=f"HavePicture{loc_idx}")
-            pic_timeline.state("Taking", dur=(take_pic_time, take_pic_time),conditions=[During("loc", f"At({loc_idx})")])
-            pic_timeline.state("Done", conditions=[TransitionFrom("Taking")])
-
-            # Download the picture
-            dl_timeline = p.timeline("Download", name=f"Download{loc_idx}")
-            dl_timeline.state("Downloading", dur=(download_time, download_time), conditions=[
-                During(f"HavePicture{loc_idx}", "Done"), 
-                During(f"Visibility", "Available"),
-                During(f"Antenna", "Available", amount=1)])
-            dl_timeline.state("Done", conditions=[TransitionFrom("Downloading")])
-
-            p.goal(f"Download{loc_idx}", "Done")
-
-        p.save_json(f"examples/goac_{n_pics}pics_{n_windows}wind.json")
+from timelinedsl import *
+
+time_windows = [(280,4000), (8000,15000), (20000,25000), (30000,35000), (40000,45000)]
+locations = [0, 1,2,3,4,5,6,7,8,9]
+speed = 1
+download_time = 6*40
+take_pic_time = 50
+edges = [
+        (0, 1, 100),
+        (0, 2, 200),
+        (0, 4, 100),
+        (0, 5, 200),
+        (0, 9, 300),
+        (1, 2, 100),
+        (1, 6, 200),
+        (2, 3, 100),
+        (2, 7, 200),
+        (2, 8, 300),
+        (3, 4, 200),
+        (3, 7, 100),
+        (3, 8, 200),
+        (4, 5, 100),
+        (4, 9, 200),
+        (5, 6, 100),
+        (5, 7, 200),
+        (5, 9, 100),
+        (6, 7, 100),
+        (7, 8, 100),
+        (8, 9, 200),
+]
+
+edges = edges + [(b,a,l) for a,b,l in edges]
+
+
+for n_pics in [1,2,3,4,5,6,7,8,9]:
+    for n_windows in [1,2,3,4,5]:
+
+        p = Problem()
+        p.resource("Antenna", name="Antenna", capacity=1)
+        for (start,end) in time_windows[:n_windows]:
+            p.fact("Visibility", "Available", start=start, end=end)
+        
+        loc_timeline = p.timeline("Location", name="loc")
+        p.fact("loc", "At(0)",start=0) # Start at location 0
+
+        for loc in locations:
+            loc_timeline.state(f"At({loc})")
+        for a,b,l in edges:
+            loc_timeline.state(f"Going({locations[a]},{locations[b]})", dur=(l,l), conditions=[
+                TransitionFrom(f"At({locations[a]})"), 
+                TransitionTo(f"At({locations[b]})")])
+        
+        for loc_idx in range(n_pics):
+
+            # Take the picture
+            pic_timeline = p.timeline("HavePicture", name=f"HavePicture{loc_idx}")
+            pic_timeline.state("Taking", dur=(take_pic_time, take_pic_time),conditions=[During("loc", f"At({loc_idx})")])
+            pic_timeline.state("Done", conditions=[TransitionFrom("Taking")])
+
+            # Download the picture
+            dl_timeline = p.timeline("Download", name=f"Download{loc_idx}")
+            dl_timeline.state("Downloading", dur=(download_time, download_time), conditions=[
+                During(f"HavePicture{loc_idx}", "Done"), 
+                During(f"Visibility", "Available"),
+                During(f"Antenna", "Available", amount=1)])
+            dl_timeline.state("Done", conditions=[TransitionFrom("Downloading")])
+
+            p.goal(f"Download{loc_idx}", "Done")
+
+        p.save_json(f"examples/goac_{n_pics}pics_{n_windows}wind.json")
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/lib.rs` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/lib.rs`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-pub mod problem;
-pub mod transitionsolver;
-pub mod cores;
-
-pub fn solve_json(input :String) -> String {
-    let problem = serde_json::de::from_str::<problem::Problem>(&input).unwrap();
-    println!("{:#?}", problem);
-    "".to_string()
-}
-
-pub fn to_json(input :&problem::Problem) -> String {
-    serde_json::to_string_pretty(input).unwrap()
-}
-
-pub fn print_calc_time<T>(name: &str, f: impl FnOnce() -> T) -> T{
-    use std::time::Instant;
-    let now = Instant::now();
-
-    let result = {
-        f()
-    };
-
-    let elapsed = now.elapsed();
-    println!("{} took {:.2?}", name, elapsed);
-    result
-}
-
-#[derive(Clone, Debug)]
-pub enum SolverError {
-    NoSolution,
-    GoalValueDurationLimit,
-    GoalStateMissing,
-}
-
-
-pub fn z3real_value(real: &z3::ast::Real) -> f32 {
-    let (num, den) = real.as_real().unwrap();
-    num as f32 / den as f32
-}
+pub mod problem;
+pub mod transitionsolver;
+pub mod cores;
+
+pub fn solve_json(input :String) -> String {
+    let problem = serde_json::de::from_str::<problem::Problem>(&input).unwrap();
+    println!("{:#?}", problem);
+    "".to_string()
+}
+
+pub fn to_json(input :&problem::Problem) -> String {
+    serde_json::to_string_pretty(input).unwrap()
+}
+
+pub fn print_calc_time<T>(name: &str, f: impl FnOnce() -> T) -> T{
+    use std::time::Instant;
+    let now = Instant::now();
+
+    let result = {
+        f()
+    };
+
+    let elapsed = now.elapsed();
+    println!("{} took {:.2?}", name, elapsed);
+    result
+}
+
+#[derive(Clone, Debug)]
+pub enum SolverError {
+    NoSolution,
+    GoalValueDurationLimit,
+    GoalStateMissing,
+}
+
+
+pub fn z3real_value(real: &z3::ast::Real) -> f32 {
+    let (num, den) = real.as_real().unwrap();
+    num as f32 / den as f32
+}
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/src/main.rs` & `pyparaspace-0.1.5/local_dependencies/paraspace/src/main.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,131 @@
-use paraspace::{print_calc_time, problem, transitionsolver};
-use std::path::PathBuf;
-use structopt::StructOpt;
-
-#[derive(Debug, StructOpt)]
-#[structopt(name = "timelinemodel", about = "Timelines SMT-based solver.")]
-struct Opt {
-    /// Input file
-    #[structopt(parse(from_os_str))]
-    input: Option<PathBuf>,
-
-    /// Output file, stdout if not present
-    #[structopt(parse(from_os_str))]
-    output: Option<PathBuf>,
-
-    #[structopt(long = "benchmark")]
-    perftest: bool,
-
-    #[structopt(long = "minimizecores")]
-    minimizecores: bool,
-}
-
-fn main() {
-    let opt = Opt::from_args();
-    println!("{:?}", opt);
-
-    if opt.perftest {
-        perftest();
-    }
-
-    let solver_func = transitionsolver::solve;
-
-    if let Some(filename) = opt.input {
-        let problem = {
-            let _p = hprof::enter("load_problem");
-            let contents = std::fs::read_to_string(&filename).unwrap();
-            serde_json::de::from_str::<problem::Problem>(&contents).unwrap()
-        };
-
-        let minimizecores = opt.minimizecores;
-        let result = print_calc_time(filename.to_str().unwrap(), || {
-            solver_func(&problem, &Default::default())
-        });
-        match result {
-            Ok(solution) => {
-                println!("Solved.");
-
-                if let Some(output) = opt.output {
-                    std::fs::write(&output, serde_json::to_string_pretty(&solution).unwrap())
-                        .unwrap();
-
-                    println!("Wrote to file '{}'", output.to_str().unwrap());
-                }
-            }
-            Err(err) => {
-                println!("Error: {:#?}", err);
-            }
-        }
-    } else {
-        println!("No problem files given.");
-    }
-
-    hprof::profiler().print_timing();
-}
-
-fn perftest() {
-    let mut problem_names = Vec::new();
-    for plates in [1, 2] {
-        for n_carbonaras in [
-            1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 15, 20, 25, 30, 40, 50, 75, 100,
-        ] {
-            let problem_name = format!("carbonara_{}p_{}c", plates, n_carbonaras);
-            problem_names.push(problem_name);
-        }
-    }
-
-    for (n_kilns, n_pieces) in [(1, 2), (2, 4), (2, 6), (4, 6), (5, 10)] {
-        let problem_name = format!("ceramic_{}m_{}j", n_kilns, n_pieces);
-        problem_names.push(problem_name);
-    }
-
-    for n_pics in 1..=9 {
-        for n_windows in 1..=5 {
-            let problem_name = format!("goac_{}pics_{}wind", n_pics, n_windows);
-            problem_names.push(problem_name);
-        }
-    }
-
-    for problem_name in problem_names {
-        let contents = std::fs::read_to_string(&format!("examples/{}.json", problem_name)).unwrap();
-        let problem = serde_json::de::from_str::<problem::Problem>(&contents).unwrap();
-
-        // println!("Problem:\n{:#?}", problem);
-        // println!("Solving...");
-        let result = print_calc_time(&problem_name, || transitionsolver::solve(&problem, &Default::default()));
-        match result {
-            Ok(solution) => {
-                // println!("Success!");
-                std::fs::write(
-                    &format!("examples/{}.out.json", problem_name),
-                    serde_json::to_string_pretty(&solution).unwrap(),
-                )
-                .unwrap();
-            }
-            Err(err) => {
-                println!("Error: {:#?}", err);
-            }
-        }
-    }
-}
-
-// Compilation idea:
-//  Detect when two resources can be joined together into one
-//  For example, in carbonara domain, boiling/cooking needs to select a plate,
-//   and then use it exclusively, but if there are several plates they behave
-//   just like if there was a resource with higher capacity. Symmetry reduction
-//   effect by treating them as interchangable.
+use paraspace::{print_calc_time, problem, transitionsolver};
+use std::path::PathBuf;
+use structopt::StructOpt;
+
+#[derive(Debug, StructOpt)]
+#[structopt(name = "timelinemodel", about = "Timelines SMT-based solver.")]
+struct Opt {
+    /// Input file
+    #[structopt(parse(from_os_str))]
+    input: Option<PathBuf>,
+
+    /// Output file, stdout if not present
+    #[structopt(parse(from_os_str))]
+    output: Option<PathBuf>,
+
+    #[structopt(long = "benchmark")]
+    perftest: bool,
+
+    #[structopt(long = "minimizecores")]
+    minimizecores: bool,
+}
+
+fn main() {
+    let opt = Opt::from_args();
+    println!("{:?}", opt);
+
+    if opt.perftest {
+        perftest();
+    }
+
+    let solver_func = transitionsolver::solve;
+
+    if let Some(filename) = opt.input {
+        let problem = {
+            let _p = hprof::enter("load_problem");
+            let contents = std::fs::read_to_string(&filename).unwrap();
+            serde_json::de::from_str::<problem::Problem>(&contents).unwrap()
+        };
+
+        let minimizecores = opt.minimizecores;
+        let result = print_calc_time(filename.to_str().unwrap(), || {
+            solver_func(&problem, &Default::default())
+        });
+        match result {
+            Ok(solution) => {
+                println!("Solved.  (end of time = {})", solution.end_of_time);
+                for timeline in solution.timelines.iter() {
+                    println!(
+                        "Timeline \"{}\": {}",
+                        timeline.name,
+                        timeline
+                            .tokens
+                            .iter()
+                            .map(|t| format!("({},{},{})", t.value, t.start_time, t.end_time))
+                            .collect::<Vec<_>>()
+                            .join(", ")
+                    )
+                }
+
+                if let Some(output) = opt.output {
+                    std::fs::write(&output, serde_json::to_string_pretty(&solution).unwrap())
+                        .unwrap();
+
+                    println!("Wrote to file '{}'", output.to_str().unwrap());
+                }
+            }
+            Err(err) => {
+                println!("Error: {:#?}", err);
+            }
+        }
+    } else {
+        println!("No problem files given.");
+    }
+
+    hprof::profiler().print_timing();
+}
+
+fn perftest() {
+    let mut problem_names = Vec::new();
+    for plates in [1, 2] {
+        for n_carbonaras in [
+            1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 15, 20, 25, 30, 40, 50, 75, 100,
+        ] {
+            let problem_name = format!("carbonara_{}p_{}c", plates, n_carbonaras);
+            problem_names.push(problem_name);
+        }
+    }
+
+    for (n_kilns, n_pieces) in [(1, 2), (2, 4), (2, 6), (4, 6), (5, 10)] {
+        let problem_name = format!("ceramic_{}m_{}j", n_kilns, n_pieces);
+        problem_names.push(problem_name);
+    }
+
+    for n_pics in 1..=9 {
+        for n_windows in 1..=5 {
+            let problem_name = format!("goac_{}pics_{}wind", n_pics, n_windows);
+            problem_names.push(problem_name);
+        }
+    }
+
+    for problem_name in problem_names {
+        let contents = std::fs::read_to_string(&format!("examples/{}.json", problem_name)).unwrap();
+        let problem = serde_json::de::from_str::<problem::Problem>(&contents).unwrap();
+
+        // println!("Problem:\n{:#?}", problem);
+        // println!("Solving...");
+        let result = print_calc_time(&problem_name, || {
+            transitionsolver::solve(&problem, &Default::default())
+        });
+        match result {
+            Ok(solution) => {
+                // println!("Success!");
+                std::fs::write(
+                    &format!("examples/{}.out.json", problem_name),
+                    serde_json::to_string_pretty(&solution).unwrap(),
+                )
+                .unwrap();
+            }
+            Err(err) => {
+                println!("Error: {:#?}", err);
+            }
+        }
+    }
+}
+
+// Compilation idea:
+//  Detect when two resources can be joined together into one
+//  For example, in carbonara domain, boiling/cooking needs to select a plate,
+//   and then use it exclusively, but if there are several plates they behave
+//   just like if there was a resource with higher capacity. Symmetry reduction
+//   effect by treating them as interchangable.
```

### Comparing `pyparaspace-0.1.4/local_dependencies/paraspace/tests/transitions_2.rs` & `pyparaspace-0.1.5/local_dependencies/paraspace/tests/transitions_2.rs`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-use paraspace::{problem::*, transitionsolver::solve};
-
-#[test]
-pub fn transitions_2() {
-    let problem = Problem {
-        timelines: vec![Timeline {
-            name: "obj".to_string(),
-            token_types: vec![
-                TokenType {
-                    value: "s1".to_string(),
-                    conditions: Vec::new(),
-                    duration_limits: (5, Some(6)),
-                    capacity: 0,
-                },
-                TokenType {
-                    value: "s2".to_string(),
-                    conditions: vec![vec![Condition {
-                        temporal_relationship: TemporalRelationship::MetBy,
-                        amount: 0,
-                        timeline_ref: "obj".to_string(),
-                        value: "s1".to_string(),
-                    }]],
-                    duration_limits: (1, None),
-                    capacity: 0,
-                },
-                TokenType {
-                    value: "s3".to_string(),
-                    conditions: vec![vec![Condition {
-                        temporal_relationship: TemporalRelationship::MetBy,
-                        amount: 0,
-                        timeline_ref: "obj".to_string(),
-                        value: "s2".to_string(),
-                    }]],
-                    duration_limits: (1, None),
-                    capacity: 0,
-                },
-            ],
-            static_tokens: vec![Token {
-                value: "s3".to_string(),
-                const_time: TokenTime::Goal,
-                capacity: 0,
-                conditions: vec![],
-            }],
-        }],
-    };
-
-    let solution = solve(&problem, &Default::default()).unwrap();
-    println!("SOLUTION {:#?}", solution);
-
-    assert!(solution.timelines.len() == 1);
-
-    let token0 = &solution.timelines[0].tokens[0];
-    let token1 = &solution.timelines[0].tokens[1];
-    let token2 = &solution.timelines[0].tokens[2];   
-
-    assert!(token0.value == "s1");
-    assert!(token1.value == "s2");
-    assert!(token2.value == "s3");
-    assert!(token0.end_time - token0.start_time >= 5. && token0.end_time - token0.start_time <= 6.);
-    assert!((token1.end_time - token2.start_time).abs() < 1e-5);
-    assert!((token0.end_time - token1.start_time).abs() < 1e-5);
-    assert!(token2.end_time == solution.end_of_time);
-}
+use paraspace::{problem::*, transitionsolver::solve};
+
+#[test]
+pub fn transitions_2() {
+    let problem = Problem {
+        timelines: vec![Timeline {
+            name: "obj".to_string(),
+            token_types: vec![
+                TokenType {
+                    value: "s1".to_string(),
+                    conditions: Vec::new(),
+                    duration_limits: (5, Some(6)),
+                    capacity: 0,
+                },
+                TokenType {
+                    value: "s2".to_string(),
+                    conditions: vec![vec![Condition {
+                        temporal_relationship: TemporalRelationship::MetBy,
+                        amount: 0,
+                        timeline_ref: "obj".to_string(),
+                        value: "s1".to_string(),
+                    }]],
+                    duration_limits: (1, None),
+                    capacity: 0,
+                },
+                TokenType {
+                    value: "s3".to_string(),
+                    conditions: vec![vec![Condition {
+                        temporal_relationship: TemporalRelationship::MetBy,
+                        amount: 0,
+                        timeline_ref: "obj".to_string(),
+                        value: "s2".to_string(),
+                    }]],
+                    duration_limits: (1, None),
+                    capacity: 0,
+                },
+            ],
+            static_tokens: vec![Token {
+                value: "s3".to_string(),
+                const_time: TokenTime::Goal,
+                capacity: 0,
+                conditions: vec![],
+            }],
+        }],
+    };
+
+    let solution = solve(&problem, &Default::default()).unwrap();
+    println!("SOLUTION {:#?}", solution);
+
+    assert!(solution.timelines.len() == 1);
+
+    let token0 = &solution.timelines[0].tokens[0];
+    let token1 = &solution.timelines[0].tokens[1];
+    let token2 = &solution.timelines[0].tokens[2];   
+
+    assert!(token0.value == "s1");
+    assert!(token1.value == "s2");
+    assert!(token2.value == "s3");
+    assert!(token0.end_time - token0.start_time >= 5. && token0.end_time - token0.start_time <= 6.);
+    assert!((token1.end_time - token2.start_time).abs() < 1e-5);
+    assert!((token0.end_time - token1.start_time).abs() < 1e-5);
+    assert!(token2.end_time == solution.end_of_time);
+}
```

### Comparing `pyparaspace-0.1.4/Dockerfile` & `pyparaspace-0.1.5/Dockerfile`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-FROM quay.io/pypa/manylinux2014_x86_64:latest	
-
-#ENV PATH /opt/python/cp35-cp35m/bin/:/opt/python/cp36-cp36m/bin/:/opt/python/cp37-cp37m/bin/:/opt/python/cp310-cp310m/:$PATH
-
-ENV PATH /root/.cargo/bin:$PATH
-RUN curl https://sh.rustup.rs -sSf | sh -s -- -y \
-    && rustup update
-
-RUN yum update -y
-RUN yum install -y  centos-release-scl llvm-toolset-7
-
-RUN which python3.10
-RUN python3.10 -m pip install maturin
-RUN python3.10 -m pip show maturin
-RUN python3.10 -m site
-RUN python3.10 -m sysconfig
-
-RUN mkdir /io
-WORKDIR /io
-RUN echo "#!/bin/bash" > ~/entry.sh
-RUN echo "echo GOT ARGUMENTS \"\$@\"" >> /root/entry.sh
-RUN echo "source scl_source enable llvm-toolset-7" >> /root/entry.sh
-RUN echo "/opt/_internal/cpython-3.10.12/bin/maturin \$@" >> /root/entry.sh
-RUN cat /root/entry.sh
-RUN chmod +x /root/entry.sh
-ENTRYPOINT ["/root/entry.sh"]
+FROM quay.io/pypa/manylinux2014_x86_64:latest	
+
+#ENV PATH /opt/python/cp35-cp35m/bin/:/opt/python/cp36-cp36m/bin/:/opt/python/cp37-cp37m/bin/:/opt/python/cp310-cp310m/:$PATH
+
+ENV PATH /root/.cargo/bin:$PATH
+RUN curl https://sh.rustup.rs -sSf | sh -s -- -y \
+    && rustup update
+
+RUN yum update -y
+RUN yum install -y  centos-release-scl llvm-toolset-7
+
+RUN which python3.10
+RUN python3.10 -m pip install maturin
+RUN python3.10 -m pip show maturin
+RUN python3.10 -m site
+RUN python3.10 -m sysconfig
+
+RUN mkdir /io
+WORKDIR /io
+RUN echo "#!/bin/bash" > ~/entry.sh
+RUN echo "echo GOT ARGUMENTS \"\$@\"" >> /root/entry.sh
+RUN echo "source scl_source enable llvm-toolset-7" >> /root/entry.sh
+RUN echo "/opt/_internal/cpython-3.10.12/bin/maturin \$@" >> /root/entry.sh
+RUN cat /root/entry.sh
+RUN chmod +x /root/entry.sh
+ENTRYPOINT ["/root/entry.sh"]
```

### Comparing `pyparaspace-0.1.4/README.md` & `pyparaspace-0.1.5/README.md`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-`pyparaspace`: a Python wrapper for the [ParaSpace timelines planner](https://github.com/luteberget/paraspace) -- a simple, flexible and extensible solver for timeline-based planning problems using the [Z3 Theorem Prover](https://github.com/Z3Prover/z3).
-
-# Installing
-
-Install using Pip. 
-
-```
-pip install pyparaspace
-```
-
-See the file `testPyParaspace.py` for example usage.
-
-# Building locally
-
-Requirements: Rust, Cargo, Clang/LLVM/LibClang, CMake.
-
- * Create a virtual environment
-```
-python3 -m venv env
-source env/bin/activate
-```
-
- * Install maturin
-```
-pip install maturin
-```
-
- * Build package
-```
-maturin develop
-```
-
-# Building and releasing
-
-This section is intended for package maintainers. The `pyparaspace`  package is
-released on PyPi with Python wheel packages that make it convenient to use
-`paraspace` without needing to set up Rust and C++ compilers and tools.
-Through the `z3-sys` package's static link option, we get the whole planner,
-including the Z3 solver, statically linked. This greatly increases the
-convenience for users of the library.
-
-Windows and Manylinux platforms are currently supported.
-
-
-## Windows
-
-If building and installing the local package works, then using `maturin build --release` 
-should also correctly build a wheel package, which can be uploaded to PyPi using `maturin publish`.
-
-## Manylinux
-
-`paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
-which makes it requires a bit of setup to correcly build the manylinux wheel. 
-There is a Dockerfile available that can be used to build a Docker image with 
-an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
-
-The builds should work using the following commands.
-```
-docker build -t mybuild .
-docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
-```
-
+`pyparaspace`: a Python wrapper for the [ParaSpace timelines planner](https://github.com/luteberget/paraspace) -- a simple, flexible and extensible solver for timeline-based planning problems using the [Z3 Theorem Prover](https://github.com/Z3Prover/z3).
+
+# Installing
+
+Install using Pip. 
+
+```
+pip install pyparaspace
+```
+
+See the file `testPyParaspace.py` for example usage.
+
+# Building locally
+
+Requirements: Rust, Cargo, Clang/LLVM/LibClang, CMake.
+
+ * Create a virtual environment
+```
+python3 -m venv env
+source env/bin/activate
+```
+
+ * Install maturin
+```
+pip install maturin
+```
+
+ * Build package
+```
+maturin develop
+```
+
+# Building and releasing
+
+This section is intended for package maintainers. The `pyparaspace`  package is
+released on PyPi with Python wheel packages that make it convenient to use
+`paraspace` without needing to set up Rust and C++ compilers and tools.
+Through the `z3-sys` package's static link option, we get the whole planner,
+including the Z3 solver, statically linked. This greatly increases the
+convenience for users of the library.
+
+Windows and Manylinux platforms are currently supported.
+
+
+## Windows
+
+If building and installing the local package works, then using `maturin build --release` 
+should also correctly build a wheel package, which can be uploaded to PyPi using `maturin publish`.
+
+## Manylinux
+
+`paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
+which makes it requires a bit of setup to correcly build the manylinux wheel. 
+There is a Dockerfile available that can be used to build a Docker image with 
+an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
+
+The builds should work using the following commands.
+```
+docker build -t mybuild .
+docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
+```
+
```

### Comparing `pyparaspace-0.1.4/testPyParaspace.py` & `pyparaspace-0.1.5/testPyParaspace.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import math
-import unittest
-import pyparaspace
-
-
-def test_pyparaspace():
-    problem = pyparaspace.Problem(
-        timelines=[
-            pyparaspace.Timeline(
-                name="obj",
-                token_types=[
-                    pyparaspace.TokenType(
-                        value="s1", conditions=[], duration_limits=(5, 6), capacity=0
-                    ),
-                    pyparaspace.TokenType(
-                        value="s2",
-                        conditions=[
-                            pyparaspace.TemporalCond(
-                                temporal_relation=pyparaspace.TemporalRelation.MetBy,
-                                amount=0,
-                                timeline="obj",
-                                value="s1",
-                            )
-                        ],
-                        duration_limits=(1, None),
-                        capacity=0,
-                    ),
-                ],
-                static_tokens=[
-                    pyparaspace.StaticToken(
-                        value="s2",
-                        const_time=pyparaspace.goal(),
-                        capacity=0,
-                        conditions=[],
-                    )
-                ],
-            )
-        ],
-    )
-
-    solution = pyparaspace.solve(problem)
-    print(f"Solution: {solution}")
-    timeline = solution.timelines[0]
-    assert len(timeline.tokens) == 2, "Number of tokens should be 2"
-
-    token1 = timeline.tokens[0]
-    token2 = timeline.tokens[1]
-    assert token1.value == "s1", "Token value 1 should be s1"
-    assert token2.value == "s2", "Token value 2 should be s2"
-
-    assert (
-        token1.end_time - token1.start_time >= 5.0
-        and token1.end_time - token1.start_time <= 6.0
-    )
-    assert abs(token1.end_time - token2.start_time) < 1e-5
-
-
-if __name__ == "__main__":
-    test_pyparaspace()
+import math
+import unittest
+import pyparaspace
+
+
+def test_pyparaspace():
+    problem = pyparaspace.Problem(
+        timelines=[
+            pyparaspace.Timeline(
+                name="obj",
+                token_types=[
+                    pyparaspace.TokenType(
+                        value="s1", conditions=[], duration_limits=(5, 6), capacity=0
+                    ),
+                    pyparaspace.TokenType(
+                        value="s2",
+                        conditions=[
+                            pyparaspace.TemporalCond(
+                                temporal_relation=pyparaspace.TemporalRelation.MetBy,
+                                amount=0,
+                                timeline="obj",
+                                value="s1",
+                            )
+                        ],
+                        duration_limits=(1, None),
+                        capacity=0,
+                    ),
+                ],
+                static_tokens=[
+                    pyparaspace.StaticToken(
+                        value="s2",
+                        const_time=pyparaspace.goal(),
+                        capacity=0,
+                        conditions=[],
+                    )
+                ],
+            )
+        ],
+    )
+
+    solution = pyparaspace.solve(problem)
+    print(f"Solution: {solution}")
+    timeline = solution.timelines[0]
+    assert len(timeline.tokens) == 2, "Number of tokens should be 2"
+
+    token1 = timeline.tokens[0]
+    token2 = timeline.tokens[1]
+    assert token1.value == "s1", "Token value 1 should be s1"
+    assert token2.value == "s2", "Token value 2 should be s2"
+
+    assert (
+        token1.end_time - token1.start_time >= 5.0
+        and token1.end_time - token1.start_time <= 6.0
+    )
+    assert abs(token1.end_time - token2.start_time) < 1e-5
+
+
+if __name__ == "__main__":
+    test_pyparaspace()
```

### Comparing `pyparaspace-0.1.4/Cargo.lock` & `pyparaspace-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyparaspace"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "indexmap",
  "paraspace",
  "pyo3",
 ]
 
 [[package]]
@@ -526,17 +526,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.97"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
```

### Comparing `pyparaspace-0.1.4/PKG-INFO` & `pyparaspace-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 Metadata-Version: 2.1
 Name: pyparaspace
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
-`pyparaspace`: a Python wrapper for the [ParaSpace timelines planner](https://github.com/luteberget/paraspace) -- a simple, flexible and extensible solver for timeline-based planning problems using the [Z3 Theorem Prover](https://github.com/Z3Prover/z3).
-
-# Installing
-
-Install using Pip. 
-
-```
-pip install pyparaspace
-```
-
-See the file `testPyParaspace.py` for example usage.
-
-# Building locally
-
-Requirements: Rust, Cargo, Clang/LLVM/LibClang, CMake.
-
- * Create a virtual environment
-```
-python3 -m venv env
-source env/bin/activate
-```
-
- * Install maturin
-```
-pip install maturin
-```
-
- * Build package
-```
-maturin develop
-```
-
-# Building and releasing
-
-This section is intended for package maintainers. The `pyparaspace`  package is
-released on PyPi with Python wheel packages that make it convenient to use
-`paraspace` without needing to set up Rust and C++ compilers and tools.
-Through the `z3-sys` package's static link option, we get the whole planner,
-including the Z3 solver, statically linked. This greatly increases the
-convenience for users of the library.
-
-Windows and Manylinux platforms are currently supported.
-
-
-## Windows
-
-If building and installing the local package works, then using `maturin build --release` 
-should also correctly build a wheel package, which can be uploaded to PyPi using `maturin publish`.
-
-## Manylinux
-
-`paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
-which makes it requires a bit of setup to correcly build the manylinux wheel. 
-There is a Dockerfile available that can be used to build a Docker image with 
-an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
-
-The builds should work using the following commands.
-```
-docker build -t mybuild .
-docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
-```
-
+`pyparaspace`: a Python wrapper for the [ParaSpace timelines planner](https://github.com/luteberget/paraspace) -- a simple, flexible and extensible solver for timeline-based planning problems using the [Z3 Theorem Prover](https://github.com/Z3Prover/z3).
+
+# Installing
+
+Install using Pip. 
+
+```
+pip install pyparaspace
+```
+
+See the file `testPyParaspace.py` for example usage.
+
+# Building locally
+
+Requirements: Rust, Cargo, Clang/LLVM/LibClang, CMake.
+
+ * Create a virtual environment
+```
+python3 -m venv env
+source env/bin/activate
+```
+
+ * Install maturin
+```
+pip install maturin
+```
+
+ * Build package
+```
+maturin develop
+```
+
+# Building and releasing
+
+This section is intended for package maintainers. The `pyparaspace`  package is
+released on PyPi with Python wheel packages that make it convenient to use
+`paraspace` without needing to set up Rust and C++ compilers and tools.
+Through the `z3-sys` package's static link option, we get the whole planner,
+including the Z3 solver, statically linked. This greatly increases the
+convenience for users of the library.
+
+Windows and Manylinux platforms are currently supported.
+
+
+## Windows
+
+If building and installing the local package works, then using `maturin build --release` 
+should also correctly build a wheel package, which can be uploaded to PyPi using `maturin publish`.
+
+## Manylinux
+
+`paraspace` requires an Rust version 1.60 and Clang version 3.5 (to compile the Z3 solver), 
+which makes it requires a bit of setup to correcly build the manylinux wheel. 
+There is a Dockerfile available that can be used to build a Docker image with 
+an up-to-date Rust version and version 7 of the LLVM/Clang toolchain.
+
+The builds should work using the following commands.
+```
+docker build -t mybuild .
+docker run --rm -v $(pwd):/io mybuild publish --skip-existing --compatibility manylinux2014 -i python3.10
+```
+
```

