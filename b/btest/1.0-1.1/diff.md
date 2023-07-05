# Comparing `tmp/btest-1.0.tar.gz` & `tmp/btest-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btest-1.0.tar", last modified: Tue Apr 11 23:52:04 2023, max compression
+gzip compressed data, was "btest-1.1.tar", last modified: Wed Jul  5 17:02:26 2023, max compression
```

## Comparing `btest-1.0.tar` & `btest-1.1.tar`

### file list

```diff
@@ -1,332 +1,342 @@
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.225184 btest-1.0/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.184184 btest-1.0/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t4/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1252 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t4/dots
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t5/
--rw-rw-r--   0 christian  (1000) christian  (1000)        9 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t5/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t5-2/
--rw-rw-r--   0 christian  (1000) christian  (1000)        9 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t5-2/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t6/
--rw-rw-r--   0 christian  (1000) christian  (1000)        2 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t6/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.t7/
--rw-rw-r--   0 christian  (1000) christian  (1000)      132 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.t7/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.189184 btest-1.0/Baseline/examples.unstable/
--rw-rw-r--   0 christian  (1000) christian  (1000)        2 2020-10-05 17:46:07.000000 btest-1.0/Baseline/examples.unstable/output
--rw-r--r--   0 christian  (1000) christian  (1000)    43286 2023-04-11 23:48:59.000000 btest-1.0/CHANGES
--rw-rw-r--   0 christian  (1000) christian  (1000)     1839 2020-10-05 17:46:07.000000 btest-1.0/COPYING
--rw-rw-r--   0 christian  (1000) christian  (1000)      204 2020-10-05 17:46:07.000000 btest-1.0/MANIFEST.in
--rw-r--r--   0 christian  (1000) christian  (1000)      627 2020-12-01 21:37:29.000000 btest-1.0/Makefile
--rw-r--r--   0 christian  (1000) christian  (1000)      661 2023-04-11 23:52:04.225184 btest-1.0/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)    53701 2023-04-11 23:48:59.000000 btest-1.0/README
--rw-r--r--   0 christian  (1000) christian  (1000)        4 2023-04-11 23:48:59.000000 btest-1.0/VERSION
--rwxr-xr-x   0 christian  (1000) christian  (1000)   103196 2023-04-11 23:48:59.000000 btest-1.0/btest
--rwxr-xr-x   0 christian  (1000) christian  (1000)     1145 2021-10-25 23:17:40.000000 btest-1.0/btest-ask-update
--rwxr-xr-x   0 christian  (1000) christian  (1000)      708 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-run
--rwxr-xr-x   0 christian  (1000) christian  (1000)      455 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-run-helper
--rwxr-xr-x   0 christian  (1000) christian  (1000)     3107 2021-10-25 23:17:40.000000 btest-1.0/btest-bg-wait
--rwxr-xr-x   0 christian  (1000) christian  (1000)     7836 2023-01-24 20:15:29.000000 btest-1.0/btest-diff
--rwxr-xr-x   0 christian  (1000) christian  (1000)      892 2021-10-25 23:17:40.000000 btest-1.0/btest-progress
--rwxr-xr-x   0 christian  (1000) christian  (1000)      158 2023-02-01 03:00:52.000000 btest-1.0/btest-setsid
--rw-rw-r--   0 christian  (1000) christian  (1000)      386 2020-10-20 16:43:55.000000 btest-1.0/btest.cfg.example
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.191184 btest-1.0/examples/
--rw-rw-r--   0 christian  (1000) christian  (1000)      124 2020-10-05 17:46:07.000000 btest-1.0/examples/alternative
--rwxrwxr-x   0 christian  (1000) christian  (1000)       57 2020-10-05 17:46:07.000000 btest-1.0/examples/my-filter
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.192184 btest-1.0/examples/sphinx/
--rw-rw-r--   0 christian  (1000) christian  (1000)       21 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/.gitignore
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.185184 btest-1.0/examples/sphinx/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.193184 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/
--rw-r--r--   0 christian  (1000) christian  (1000)       61 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#1
--rw-r--r--   0 christian  (1000) christian  (1000)       75 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#2
--rw-r--r--   0 christian  (1000) christian  (1000)       89 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#3
--rw-rw-r--   0 christian  (1000) christian  (1000)     5620 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/Makefile
--rw-rw-r--   0 christian  (1000) christian  (1000)      209 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/btest.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)     8021 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/conf.py
--rw-r--r--   0 christian  (1000) christian  (1000)     1316 2021-10-25 23:17:40.000000 btest-1.0/examples/sphinx/index.rst
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.185184 btest-1.0/examples/sphinx/tests/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.193184 btest-1.0/examples/sphinx/tests/sphinx/
--rw-rw-r--   0 christian  (1000) christian  (1000)       47 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest
--rw-rw-r--   0 christian  (1000) christian  (1000)       54 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest#2
--rw-rw-r--   0 christian  (1000) christian  (1000)       61 2020-10-05 17:46:07.000000 btest-1.0/examples/sphinx/tests/sphinx/hello-world.btest#3
--rw-rw-r--   0 christian  (1000) christian  (1000)       59 2020-10-05 17:46:07.000000 btest-1.0/examples/t1
--rw-rw-r--   0 christian  (1000) christian  (1000)       70 2020-10-05 17:46:07.000000 btest-1.0/examples/t2
--rw-rw-r--   0 christian  (1000) christian  (1000)       50 2020-10-05 17:46:07.000000 btest-1.0/examples/t3.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)       93 2020-10-05 17:46:07.000000 btest-1.0/examples/t4.awk
--rw-r--r--   0 christian  (1000) christian  (1000)      158 2021-10-25 23:17:40.000000 btest-1.0/examples/t5.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)      166 2020-10-05 17:46:07.000000 btest-1.0/examples/t6.sh
--rw-rw-r--   0 christian  (1000) christian  (1000)       92 2020-10-05 17:46:07.000000 btest-1.0/examples/t7
--rw-rw-r--   0 christian  (1000) christian  (1000)       44 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#1
--rw-rw-r--   0 christian  (1000) christian  (1000)       44 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#2
--rw-rw-r--   0 christian  (1000) christian  (1000)       32 2020-10-05 17:46:07.000000 btest-1.0/examples/t7.sh#3
--rw-r--r--   0 christian  (1000) christian  (1000)       78 2021-10-25 23:17:40.000000 btest-1.0/examples/unstable.sh
--rw-r--r--   0 christian  (1000) christian  (1000)      120 2023-04-11 23:52:04.225184 btest-1.0/setup.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)     1555 2023-04-11 23:48:59.000000 btest-1.0/setup.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.194184 btest-1.0/sphinx/
--rwxr-xr-x   0 christian  (1000) christian  (1000)      426 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-diff-rst
--rwxr-xr-x   0 christian  (1000) christian  (1000)     3534 2022-03-07 20:08:30.000000 btest-1.0/sphinx/btest-rst-cmd
--rwxr-xr-x   0 christian  (1000) christian  (1000)      410 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-rst-include
--rwxr-xr-x   0 christian  (1000) christian  (1000)      156 2021-10-25 23:17:40.000000 btest-1.0/sphinx/btest-rst-pipe
--rw-r--r--   0 christian  (1000) christian  (1000)     7665 2023-02-01 03:00:52.000000 btest-1.0/sphinx/btest-sphinx.py
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/sphinx/btest.egg-info/
--rw-r--r--   0 christian  (1000) christian  (1000)      661 2023-04-11 23:52:03.000000 btest-1.0/sphinx/btest.egg-info/PKG-INFO
--rw-r--r--   0 christian  (1000) christian  (1000)     8675 2023-04-11 23:52:04.000000 btest-1.0/sphinx/btest.egg-info/SOURCES.txt
--rw-r--r--   0 christian  (1000) christian  (1000)        1 2023-04-11 23:52:03.000000 btest-1.0/sphinx/btest.egg-info/dependency_links.txt
--rw-r--r--   0 christian  (1000) christian  (1000)       13 2023-04-11 23:52:04.000000 btest-1.0/sphinx/btest.egg-info/top_level.txt
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/
--rw-rw-r--   0 christian  (1000) christian  (1000)       32 2020-10-05 17:46:07.000000 btest-1.0/testing/.gitignore
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/Baseline/tests.abort-on-failure/
--rw-rw-r--   0 christian  (1000) christian  (1000)      255 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.abort-on-failure/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.195184 btest-1.0/testing/Baseline/tests.abort-on-failure-with-only-known-fails/
--rw-r--r--   0 christian  (1000) christian  (1000)      347 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-environment/
--rw-r--r--   0 christian  (1000) christian  (1000)      321 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-environment/child-output
--rw-r--r--   0 christian  (1000) christian  (1000)      463 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-environment/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-filter/
--rw-r--r--   0 christian  (1000) christian  (1000)      523 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.alternatives-filter/child-output
--rw-rw-r--   0 christian  (1000) christian  (1000)      221 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-filter/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.196184 btest-1.0/testing/Baseline/tests.alternatives-keywords/
--rw-r--r--   0 christian  (1000) christian  (1000)      289 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-keywords/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-substitution/
--rw-rw-r--   0 christian  (1000) christian  (1000)      136 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-substitution/child-output
--rw-rw-r--   0 christian  (1000) christian  (1000)      233 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.alternatives-substitution/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-testbase/
--rw-rw-r--   0 christian  (1000) christian  (1000)       58 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.alternatives-testbase/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.alternatives-undefined/
--rw-r--r--   0 christian  (1000) christian  (1000)      154 2022-12-07 22:09:21.000000 btest-1.0/testing/Baseline/tests.alternatives-undefined/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.197184 btest-1.0/testing/Baseline/tests.brief/
--rw-rw-r--   0 christian  (1000) christian  (1000)      138 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.brief/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      149 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.brief/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.btest-cfg/
--rw-rw-r--   0 christian  (1000) christian  (1000)      195 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/abspath
--rw-rw-r--   0 christian  (1000) christian  (1000)      276 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/nopath
--rw-rw-r--   0 christian  (1000) christian  (1000)      195 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.btest-cfg/relpath
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.console/
--rw-rw-r--   0 christian  (1000) christian  (1000)      119 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.console/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.198184 btest-1.0/testing/Baseline/tests.crlf-line-terminators/
--rw-r--r--   0 christian  (1000) christian  (1000)      125 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.crlf-line-terminators/crlfs.dat
--rw-r--r--   0 christian  (1000) christian  (1000)      445 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.crlf-line-terminators/input
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag/
--rw-rw-r--   0 christian  (1000) christian  (1000)      732 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag-all/
--rw-rw-r--   0 christian  (1000) christian  (1000)      264 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-all/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diag-file/
--rw-rw-r--   0 christian  (1000) christian  (1000)      216 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-file/diag
--rw-rw-r--   0 christian  (1000) christian  (1000)      155 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diag-file/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.199184 btest-1.0/testing/Baseline/tests.diff-brief/
--rw-rw-r--   0 christian  (1000) christian  (1000)      471 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-brief/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.diff-max-lines/
--rw-rw-r--   0 christian  (1000) christian  (1000)      604 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-max-lines/output1
--rw-rw-r--   0 christian  (1000) christian  (1000)      690 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.diff-max-lines/output2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.doc/
--rw-rw-r--   0 christian  (1000) christian  (1000)      864 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.doc/md
--rw-rw-r--   0 christian  (1000) christian  (1000)      998 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.doc/rst
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.environment/
--rw-rw-r--   0 christian  (1000) christian  (1000)      717 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.environment/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.environment-windows/
--rw-r--r--   0 christian  (1000) christian  (1000)      845 2023-01-24 20:15:29.000000 btest-1.0/testing/Baseline/tests.environment-windows/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.200184 btest-1.0/testing/Baseline/tests.exit-codes/
--rw-r--r--   0 christian  (1000) christian  (1000)      159 2020-12-03 19:18:53.000000 btest-1.0/testing/Baseline/tests.exit-codes/out1
--rw-r--r--   0 christian  (1000) christian  (1000)      271 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.exit-codes/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.groups/
--rw-rw-r--   0 christian  (1000) christian  (1000)      476 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.groups/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.ignore/
--rw-rw-r--   0 christian  (1000) christian  (1000)      184 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.ignore/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure/
--rw-rw-r--   0 christian  (1000) christian  (1000)      342 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure-and-success/
--rw-rw-r--   0 christian  (1000) christian  (1000)      208 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure-and-success/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.known-failure-succeeds/
--rw-rw-r--   0 christian  (1000) christian  (1000)      191 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.known-failure-succeeds/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.201184 btest-1.0/testing/Baseline/tests.list/
--rw-r--r--   0 christian  (1000) christian  (1000)      124 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.list/out
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.macros/
--rw-rw-r--   0 christian  (1000) christian  (1000)      152 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.macros/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.measure-time/
--rw-rw-r--   0 christian  (1000) christian  (1000)      504 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.measure-time/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.measure-time-options/
--rw-rw-r--   0 christian  (1000) christian  (1000)      640 2020-10-05 17:46:07.000000 btest-1.0/testing/Baseline/tests.measure-time-options/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.multiple-baseline-dirs/
--rw-r--r--   0 christian  (1000) christian  (1000)      375 2020-12-01 21:37:42.000000 btest-1.0/testing/Baseline/tests.multiple-baseline-dirs/fail.log
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.parts/
--rw-rw-r--   0 christian  (1000) christian  (1000)      227 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.202184 btest-1.0/testing/Baseline/tests.parts-error-part/
--rw-rw-r--   0 christian  (1000) christian  (1000)      196 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-error-part/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-error-start-next/
--rw-rw-r--   0 christian  (1000) christian  (1000)      180 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-error-start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-glob/
--rw-rw-r--   0 christian  (1000) christian  (1000)      243 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-glob/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-initializer-finalizer/
--rw-r--r--   0 christian  (1000) christian  (1000)      363 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.parts-initializer-finalizer/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-skipping/
--rw-rw-r--   0 christian  (1000) christian  (1000)      179 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.parts-skipping/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.parts-teardown/
--rw-r--r--   0 christian  (1000) christian  (1000)      199 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.parts-teardown/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.203184 btest-1.0/testing/Baseline/tests.progress/
--rw-rw-r--   0 christian  (1000) christian  (1000)      504 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.progress/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.progress-back-to-back/
--rw-rw-r--   0 christian  (1000) christian  (1000)      608 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.progress-back-to-back/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.quiet/
--rw-rw-r--   0 christian  (1000) christian  (1000)      115 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.quiet/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      129 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.quiet/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.requires/
--rw-rw-r--   0 christian  (1000) christian  (1000)      225 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.requires/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.requires-with-start-next/
--rw-r--r--   0 christian  (1000) christian  (1000)      229 2021-05-10 05:01:31.000000 btest-1.0/testing/Baseline/tests.requires-with-start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.rerun/
--rw-rw-r--   0 christian  (1000) christian  (1000)      202 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.rerun/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.204184 btest-1.0/testing/Baseline/tests.set-key/
--rw-r--r--   0 christian  (1000) christian  (1000)       28 2023-01-24 20:15:29.000000 btest-1.0/testing/Baseline/tests.set-key/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/
--rw-rw-r--   0 christian  (1000) christian  (1000)      926 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/
--rw-r--r--   0 christian  (1000) christian  (1000)     1390 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-file/
--rw-rw-r--   0 christian  (1000) christian  (1000)      119 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-file/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-next/
--rw-rw-r--   0 christian  (1000) christian  (1000)      125 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-next/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.start-next-dir/
--rw-rw-r--   0 christian  (1000) christian  (1000)      196 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.start-next-dir/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.205184 btest-1.0/testing/Baseline/tests.statefile/
--rw-rw-r--   0 christian  (1000) christian  (1000)      115 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.statefile/mystate1
--rw-rw-r--   0 christian  (1000) christian  (1000)      121 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.statefile/mystate2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.statefile-sorted/
--rw-r--r--   0 christian  (1000) christian  (1000)      121 2021-10-25 23:17:40.000000 btest-1.0/testing/Baseline/tests.statefile-sorted/mystate
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.teardown/
--rw-r--r--   0 christian  (1000) christian  (1000)      271 2022-03-07 20:08:30.000000 btest-1.0/testing/Baseline/tests.teardown/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.206184 btest-1.0/testing/Baseline/tests.testdirs/
--rw-rw-r--   0 christian  (1000) christian  (1000)      164 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.testdirs/out1
--rw-rw-r--   0 christian  (1000) christian  (1000)      154 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.testdirs/out2
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.threads/
--rw-rw-r--   0 christian  (1000) christian  (1000)      188 2020-12-02 21:16:24.000000 btest-1.0/testing/Baseline/tests.threads/output.j0
--rw-r--r--   0 christian  (1000) christian  (1000)      188 2020-12-07 16:45:09.000000 btest-1.0/testing/Baseline/tests.threads/output.j1
--rw-rw-r--   0 christian  (1000) christian  (1000)      120 2020-12-02 21:16:24.000000 btest-1.0/testing/Baseline/tests.threads/output.j5
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.tracing/
--rw-rw-r--   0 christian  (1000) christian  (1000)      166 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.tracing/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable/
--rw-rw-r--   0 christian  (1000) christian  (1000)      256 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.unstable/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable-dir/
--rw-rw-r--   0 christian  (1000) christian  (1000)      280 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.unstable-dir/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.207184 btest-1.0/testing/Baseline/tests.unstable-subtest/
--rw-r--r--   0 christian  (1000) christian  (1000)      209 2023-02-01 23:09:39.000000 btest-1.0/testing/Baseline/tests.unstable-subtest/.stderr
--rw-r--r--   0 christian  (1000) christian  (1000)      261 2023-02-01 23:09:39.000000 btest-1.0/testing/Baseline/tests.unstable-subtest/diag
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.verbose/
--rw-rw-r--   0 christian  (1000) christian  (1000)      354 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.verbose/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.versioning/
--rw-rw-r--   0 christian  (1000) christian  (1000)      188 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.versioning/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Baseline/tests.xml/
--rw-rw-r--   0 christian  (1000) christian  (1000)      438 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.xml/output-j2.xml
--rw-rw-r--   0 christian  (1000) christian  (1000)      438 2020-10-20 16:43:55.000000 btest-1.0/testing/Baseline/tests.xml/output.xml
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Files/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Files/local_alternative/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.186184 btest-1.0/testing/Files/local_alternative/Baseline/
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.208184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/
--rw-r--r--   0 christian  (1000) christian  (1000)      330 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/
--rw-r--r--   0 christian  (1000) christian  (1000)      255 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/output
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/
--rw-r--r--   0 christian  (1000) christian  (1000)       34 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/output
--rw-r--r--   0 christian  (1000) christian  (1000)      389 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/btest.tests.cfg
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.209184 btest-1.0/testing/Files/local_alternative/tests/
--rw-r--r--   0 christian  (1000) christian  (1000)      116 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-found.test
--rw-r--r--   0 christian  (1000) christian  (1000)      234 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-env.test
--rw-r--r--   0 christian  (1000) christian  (1000)      201 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-test-baseline.test
--rw-r--r--   0 christian  (1000) christian  (1000)      200 2021-10-25 23:17:40.000000 btest-1.0/testing/Files/local_alternative/tests/local-alternative-show-testbase.test
--rw-r--r--   0 christian  (1000) christian  (1000)      236 2022-03-07 20:08:30.000000 btest-1.0/testing/Makefile
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.211184 btest-1.0/testing/Scripts/
--rw-r--r--   0 christian  (1000) christian  (1000)      359 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/convert-path-list.sh
--rwxr-xr-x   0 christian  (1000) christian  (1000)      134 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/diff-remove-abspath
--rw-rw-r--   0 christian  (1000) christian  (1000)       48 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/dummy-script
--rw-r--r--   0 christian  (1000) christian  (1000)      153 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/is-windows
--rwxr-xr-x   0 christian  (1000) christian  (1000)      438 2023-01-26 00:06:26.000000 btest-1.0/testing/Scripts/script-command
--rwxrwxr-x   0 christian  (1000) christian  (1000)      121 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/strip-iso8601-date
--rwxr-xr-x   0 christian  (1000) christian  (1000)      352 2023-01-24 20:15:29.000000 btest-1.0/testing/Scripts/strip-test-base
--rwxrwxr-x   0 christian  (1000) christian  (1000)       74 2020-10-05 17:46:07.000000 btest-1.0/testing/Scripts/test-filter
--rwxr-xr-x   0 christian  (1000) christian  (1000)      849 2021-10-25 23:17:40.000000 btest-1.0/testing/Scripts/test-perf
--rw-r--r--   0 christian  (1000) christian  (1000)      548 2023-01-24 20:15:29.000000 btest-1.0/testing/btest.cfg
--rw-r--r--   0 christian  (1000) christian  (1000)      593 2023-01-24 20:15:29.000000 btest-1.0/testing/btest.tests.cfg
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.224184 btest-1.0/testing/tests/
--rw-r--r--   0 christian  (1000) christian  (1000)      645 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/abort-on-failure-with-only-known-fails.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      495 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/abort-on-failure.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      599 2023-01-24 23:11:59.000000 btest-1.0/testing/tests/alternatives-baseline-dir.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      428 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/alternatives-environment.test
--rw-r--r--   0 christian  (1000) christian  (1000)      204 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-filter.test
--rw-r--r--   0 christian  (1000) christian  (1000)      598 2022-12-07 22:09:21.000000 btest-1.0/testing/tests/alternatives-keywords.test
--rw-r--r--   0 christian  (1000) christian  (1000)      161 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-overwrite-env.test
--rw-r--r--   0 christian  (1000) christian  (1000)      132 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-reread-config-baselinedir.test
--rw-r--r--   0 christian  (1000) christian  (1000)      122 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-reread-config.test
--rw-r--r--   0 christian  (1000) christian  (1000)      247 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/alternatives-substitution.test
--rw-r--r--   0 christian  (1000) christian  (1000)      116 2021-10-25 23:17:37.000000 btest-1.0/testing/tests/alternatives-testbase.test
--rw-r--r--   0 christian  (1000) christian  (1000)      273 2022-12-07 22:09:21.000000 btest-1.0/testing/tests/alternatives-undefined.test
--rw-r--r--   0 christian  (1000) christian  (1000)      548 2020-12-01 21:37:42.000000 btest-1.0/testing/tests/baseline-dir-env.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      208 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/basic-fail.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      203 2020-12-05 00:33:59.000000 btest-1.0/testing/tests/basic-succeed.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1214 2023-01-24 21:25:18.000000 btest-1.0/testing/tests/binary-mode.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      310 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/brief.test
--rw-r--r--   0 christian  (1000) christian  (1000)      696 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/btest-cfg.test
--rw-r--r--   0 christian  (1000) christian  (1000)      710 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-cmdline.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1746 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-conversion.test
--rw-r--r--   0 christian  (1000) christian  (1000)      593 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier-fail.test
--rw-r--r--   0 christian  (1000) christian  (1000)      374 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/canonifier.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1089 2023-01-25 01:24:24.000000 btest-1.0/testing/tests/console.test
--rw-r--r--   0 christian  (1000) christian  (1000)      174 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/copy-file.test
--rw-r--r--   0 christian  (1000) christian  (1000)      382 2023-01-24 21:29:04.000000 btest-1.0/testing/tests/crlf-line-terminators.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      321 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag-all.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      170 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag-file.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      330 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diag.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      519 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff-brief.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      799 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff-max-lines.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      364 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/diff.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     2134 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/doc.test
--rw-r--r--   0 christian  (1000) christian  (1000)      250 2022-11-28 06:30:41.000000 btest-1.0/testing/tests/duplicate-selection.test
--rw-r--r--   0 christian  (1000) christian  (1000)      619 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/env-var-casing.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1101 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/environment-windows.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1047 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/environment.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1160 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/exit-codes.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      224 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/finalizer.test
--rw-r--r--   0 christian  (1000) christian  (1000)      772 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/groups.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      897 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/ignore.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      234 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/initializer.test
--rw-r--r--   0 christian  (1000) christian  (1000)      175 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/known-failure-and-success.btest
--rw-rw-r--   0 christian  (1000) christian  (1000)      189 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/known-failure-succeeds.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      266 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/known-failure.btest
--rw-r--r--   0 christian  (1000) christian  (1000)      259 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/list.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      223 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/macros.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1659 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/measure-time-options.test
--rw-rw-r--   0 christian  (1000) christian  (1000)     1078 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/measure-time.tests
--rw-r--r--   0 christian  (1000) christian  (1000)     1202 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/multiple-baseline-dirs.test
--rw-r--r--   0 christian  (1000) christian  (1000)      168 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/parts-error-part.test
--rw-r--r--   0 christian  (1000) christian  (1000)      285 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/parts-error-start-next.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      501 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts-glob.test
--rw-r--r--   0 christian  (1000) christian  (1000)      821 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/parts-initializer-finalizer.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      355 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts-skipping.tests
--rw-r--r--   0 christian  (1000) christian  (1000)      801 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/parts-teardown.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      468 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/parts.tests
--rw-rw-r--   0 christian  (1000) christian  (1000)      267 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/ports.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      569 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/progress-back-to-back.test
--rw-r--r--   0 christian  (1000) christian  (1000)      575 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/progress.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      310 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/quiet.test
--rw-r--r--   0 christian  (1000) christian  (1000)      433 2021-05-10 05:01:31.000000 btest-1.0/testing/tests/requires-with-start-next.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      447 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/requires.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      287 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/rerun.test
--rw-r--r--   0 christian  (1000) christian  (1000)      248 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/set-key.test
-drwxr-xr-x   0 christian  (1000) christian  (1000)        0 2023-04-11 23:52:04.225184 btest-1.0/testing/tests/sphinx/
--rwxr-xr-x   0 christian  (1000) christian  (1000)      490 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/sphinx/rst-cmd.sh
--rw-r--r--   0 christian  (1000) christian  (1000)      220 2023-01-24 20:15:29.000000 btest-1.0/testing/tests/sphinx/run-sphinx
--rw-r--r--   0 christian  (1000) christian  (1000)      301 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/start-file.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      222 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/start-next-dir.test
--rw-r--r--   0 christian  (1000) christian  (1000)      388 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/start-next-naming.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      245 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/start-next.test
--rw-r--r--   0 christian  (1000) christian  (1000)      480 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/statefile-sorted.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      545 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/statefile.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1277 2022-03-07 20:08:30.000000 btest-1.0/testing/tests/teardown.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      227 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/test-base.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      383 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/testdirs.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1662 2020-12-07 16:45:09.000000 btest-1.0/testing/tests/threads.test
--rw-r--r--   0 christian  (1000) christian  (1000)      111 2021-10-25 23:17:40.000000 btest-1.0/testing/tests/tmps.test
--rw-r--r--   0 christian  (1000) christian  (1000)      418 2022-11-28 06:30:41.000000 btest-1.0/testing/tests/tracing.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      864 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/unstable-dir.test
--rw-r--r--   0 christian  (1000) christian  (1000)     1093 2023-02-01 23:09:39.000000 btest-1.0/testing/tests/unstable-subtest.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      476 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/unstable.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      291 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/verbose.test
--rw-r--r--   0 christian  (1000) christian  (1000)      405 2022-12-09 22:08:00.000000 btest-1.0/testing/tests/versioning.test
--rw-rw-r--   0 christian  (1000) christian  (1000)      709 2020-10-05 17:46:07.000000 btest-1.0/testing/tests/xml.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.558344 btest-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.526342 btest-1.1/Baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.t4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.t4/dots
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.t5/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.t5/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.t5-2/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.t5-2/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.t6/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.t6/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.t7/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.t7/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/Baseline/examples.unstable/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-05 17:02:26.000000 btest-1.1/Baseline/examples.unstable/output
+-rw-r--r--   0 runner    (1001) docker     (123)    45170 2023-07-05 17:02:26.000000 btest-1.1/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-05 17:02:26.000000 btest-1.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 17:02:26.000000 btest-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 17:02:26.000000 btest-1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 17:02:26.558344 btest-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53948 2023-07-05 17:02:26.000000 btest-1.1/README
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-05 17:02:26.000000 btest-1.1/VERSION
+-rwxr-xr-x   0 runner    (1001) docker     (123)   104391 2023-07-05 17:02:26.000000 btest-1.1/btest
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1145 2023-07-05 17:02:26.000000 btest-1.1/btest-ask-update
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-07-05 17:02:26.000000 btest-1.1/btest-bg-run
+-rwxr-xr-x   0 runner    (1001) docker     (123)      455 2023-07-05 17:02:26.000000 btest-1.1/btest-bg-run-helper
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3107 2023-07-05 17:02:26.000000 btest-1.1/btest-bg-wait
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7972 2023-07-05 17:02:26.000000 btest-1.1/btest-diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1300 2023-07-05 17:02:26.000000 btest-1.1/btest-progress
+-rwxr-xr-x   0 runner    (1001) docker     (123)      158 2023-07-05 17:02:26.000000 btest-1.1/btest-setsid
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-05 17:02:26.000000 btest-1.1/btest.cfg.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 17:02:26.000000 btest-1.1/examples/alternative
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-05 17:02:26.000000 btest-1.1/examples/my-filter
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/examples/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.526342 btest-1.1/examples/sphinx/Baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/examples/sphinx/Baseline/tests.sphinx.hello-world/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#1
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#2
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/Baseline/tests.sphinx.hello-world/btest-tests.sphinx.hello-world#3
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/btest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.526342 btest-1.1/examples/sphinx/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/examples/sphinx/tests/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/tests/sphinx/hello-world.btest
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/tests/sphinx/hello-world.btest#2
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 17:02:26.000000 btest-1.1/examples/sphinx/tests/sphinx/hello-world.btest#3
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 17:02:26.000000 btest-1.1/examples/t1
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 17:02:26.000000 btest-1.1/examples/t2
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-05 17:02:26.000000 btest-1.1/examples/t3.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 17:02:26.000000 btest-1.1/examples/t4.awk
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-05 17:02:26.000000 btest-1.1/examples/t5.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 17:02:26.000000 btest-1.1/examples/t6.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-05 17:02:26.000000 btest-1.1/examples/t7
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 17:02:26.000000 btest-1.1/examples/t7.sh#1
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 17:02:26.000000 btest-1.1/examples/t7.sh#2
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 17:02:26.000000 btest-1.1/examples/t7.sh#3
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-05 17:02:26.000000 btest-1.1/examples/unstable.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-05 17:02:26.558344 btest-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-05 17:02:26.000000 btest-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/sphinx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest-diff-rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3534 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest-rst-cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)      410 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest-rst-include
+-rwxr-xr-x   0 runner    (1001) docker     (123)      156 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest-rst-pipe
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest-sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/sphinx/btest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 17:02:26.000000 btest-1.1/sphinx/btest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-05 17:02:26.000000 btest-1.1/testing/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/testing/Baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.abort-on-failure/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.abort-on-failure/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.abort-on-failure-with-only-known-fails/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.alternatives-environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-environment/child-output
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-environment/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.alternatives-filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-filter/child-output
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-filter/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.alternatives-keywords/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-keywords/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.538343 btest-1.1/testing/Baseline/tests.alternatives-remove-env/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-remove-env/child-output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.alternatives-remove-env-bad/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-remove-env-bad/child-output
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-remove-env-bad/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.alternatives-substitution/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-substitution/child-output
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-substitution/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.alternatives-testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-testbase/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.alternatives-undefined/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.alternatives-undefined/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.binary-diag/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.binary-diag/.stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.brief/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.brief/out1
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.brief/out2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.btest-cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.btest-cfg/abspath
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.btest-cfg/nopath
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.btest-cfg/relpath
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.console/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.console/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.crlf-line-terminators/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.crlf-line-terminators/crlfs.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.crlf-line-terminators/input
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.diag/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diag/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.diag-all/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diag-all/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.diag-file/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diag-file/diag
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diag-file/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.diff-brief/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diff-brief/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.diff-max-lines/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diff-max-lines/output1
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.diff-max-lines/output2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.doc/md
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.doc/rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.environment/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.environment/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.environment-windows/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.environment-windows/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.exit-codes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.exit-codes/out1
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.exit-codes/out2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.groups/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.ignore/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.ignore/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.known-failure/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.known-failure/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.known-failure-and-success/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.known-failure-and-success/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.known-failure-succeeds/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.known-failure-succeeds/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.list/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.list/out
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.macros/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.measure-time/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.measure-time/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.measure-time-options/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.measure-time-options/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.multiple-baseline-dirs/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.multiple-baseline-dirs/fail.log
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.parts/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.parts-error-part/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-error-part/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.542343 btest-1.1/testing/Baseline/tests.parts-error-start-next/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-error-start-next/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.parts-glob/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-glob/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.parts-initializer-finalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-initializer-finalizer/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.parts-skipping/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-skipping/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.parts-teardown/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.parts-teardown/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.progress/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.progress-back-to-back/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.progress-back-to-back/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.quiet/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.quiet/out1
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.quiet/out2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.requires/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.requires/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.requires-with-start-next/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.requires-with-start-next/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.rerun/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.rerun/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.set-key/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.set-key/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.sphinx.rst-cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.sphinx.rst-cmd/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.sphinx.run-sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.start-file/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.start-file/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.start-next/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.start-next/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.start-next-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.start-next-dir/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.statefile/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.statefile/mystate1
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.statefile/mystate2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.statefile-sorted/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.statefile-sorted/mystate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.teardown/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.teardown/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.testdirs/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.testdirs/out1
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.testdirs/out2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.threads/output.j0
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.threads/output.j1
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.threads/output.j5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.tracing/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.unstable/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.unstable/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.unstable-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.unstable-dir/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.unstable-subtest/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.unstable-subtest/.stderr
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.unstable-subtest/diag
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.verbose/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.verbose/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.versioning/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Baseline/tests.xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.xml/output-j2.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-05 17:02:26.000000 btest-1.1/testing/Baseline/tests.xml/output.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/testing/Files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Files/local_alternative/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.534342 btest-1.1/testing/Files/local_alternative/Baseline/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-env/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-test-baseline/output
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/Baseline/tests.local-alternative-show-testbase/output
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/btest.tests.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.546343 btest-1.1/testing/Files/local_alternative/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/tests/local-alternative-found.test
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/tests/local-alternative-show-env.test
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/tests/local-alternative-show-test-baseline.test
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-05 17:02:26.000000 btest-1.1/testing/Files/local_alternative/tests/local-alternative-show-testbase.test
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-05 17:02:26.000000 btest-1.1/testing/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.550343 btest-1.1/testing/Scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/convert-path-list.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/diff-remove-abspath
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/dummy-script
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/is-windows
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/script-command
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/strip-iso8601-date
+-rwxr-xr-x   0 runner    (1001) docker     (123)      352 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/strip-test-base
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/test-filter
+-rwxr-xr-x   0 runner    (1001) docker     (123)      849 2023-07-05 17:02:26.000000 btest-1.1/testing/Scripts/test-perf
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 17:02:26.000000 btest-1.1/testing/btest.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 17:02:26.000000 btest-1.1/testing/btest.tests.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.558344 btest-1.1/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/abort-on-failure-with-only-known-fails.btest
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/abort-on-failure.btest
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-baseline-dir.test
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-environment.test
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-filter.test
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-keywords.test
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-overwrite-env.test
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-remove-env-bad.test
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-remove-env.test
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-reread-config-baselinedir.test
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-reread-config.test
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-substitution.test
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-testbase.test
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/alternatives-undefined.test
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/baseline-dir-env.test
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/basic-fail.test
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/basic-succeed.test
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/binary-diag.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/binary-mode.test
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/brief.test
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/btest-cfg.test
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/canonifier-cmdline.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/canonifier-conversion.test
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/canonifier-fail.test
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/canonifier.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/console.test
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/copy-file.test
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/crlf-line-terminators.test
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diag-all.test
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diag-file.test
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diag.test
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diff-brief.test
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diff-max-lines.test
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/diff.test
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/doc.test
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/duplicate-selection.test
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/env-var-casing.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/environment-windows.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/environment.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/exit-codes.test
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/finalizer.test
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/groups.test
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/ignore.test
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/initializer.test
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/known-failure-and-success.btest
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/known-failure-succeeds.btest
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/known-failure.btest
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/list.test
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/macros.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/measure-time-options.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/measure-time.tests
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/multiple-baseline-dirs.test
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-error-part.test
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-error-start-next.test
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-glob.test
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-initializer-finalizer.test
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-skipping.tests
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts-teardown.test
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/parts.tests
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/ports.test
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/progress-back-to-back.test
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/progress.test
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/quiet.test
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/requires-with-start-next.test
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/requires.test
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/rerun.test
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/set-key.test
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 17:02:26.558344 btest-1.1/testing/tests/sphinx/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      490 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/sphinx/rst-cmd.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/sphinx/run-sphinx
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/start-file.test
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/start-next-dir.test
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/start-next-naming.test
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/start-next.test
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/statefile-sorted.test
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/statefile.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/teardown.test
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/test-base.test
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/testdirs.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/threads.test
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/tmps.test
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/tracing.test
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/unstable-dir.test
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/unstable-subtest.test
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/unstable.test
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/verbose.test
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/versioning.test
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-05 17:02:26.000000 btest-1.1/testing/tests/xml.test
```

### Comparing `btest-1.0/Baseline/examples.t4/dots` & `btest-1.1/Baseline/examples.t4/dots`

 * *Files identical despite different names*

### Comparing `btest-1.0/CHANGES` & `btest-1.1/CHANGES`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+1.1 | 2023-07-05 09:52:44 -0700
+
+  * Release 1.1.
+
+1.0-12 | 2023-07-05 09:52:33 -0700
+
+  * CI: automatically push to PyPI when pushing a git tag (Christian Kreibich, Corelight)
+
+1.0-10 | 2023-04-20 13:10:09 -0700
+
+  * Add sphinx-related directory to gitignore (Christian Kreibich, Corelight)
+
+  * Recognize "date" without nanosecond support in btest-progress (Christian Kreibich, Corelight)
+
+  * Avoid diff --strip-trailing-cr since it's not available everywhere. (Christian Kreibich, Corelight)
+
+1.0-6 | 2023-03-02 10:47:08 +0100
+
+  * GH-60: Support environment variable removal in alternatives (Arne Welzel, Corelight)
+
+1.0-4 | 2023-02-21 10:20:20 +0100
+
+  * stderr/stdout: Do not assume well-formed UTF-8 output (Arne Welzel, Corelight)
+
+    The previous code opened stdout/stderr providing an explicit encoding="utf-8"
+    argument. This has no effect when the file handles are passed as stderr/stdout
+    to a subprocess: Only the underlying fds are passed and there's no way to
+    control the encoding (if any) used by the subprocess for the bytes it
+    produces on these streams.
+
+    So, switch things around: Remove the misleading encoding arguments for the
+    stdout, stderr files, open them in binary mode and be careful when
+    opening .stderr for displaying purposes. Do try UTF-8, but also set error
+    strategy to "backslashreplace" to avoid errors.
+
+  * monitor_cb: Start thread with daemon=True (Arne Welzel, Corelight)
+
+    When an unexpected exception happened in a child process, nothing would
+    stop the monitor_cb thread and in turn the child process would never
+    finish. Use daemon=True on the monitor_cb thread to prevent this.
+
+    There should never be unhandled exceptions in child processes, because
+    it may then not close all resources properly etc, but a non-terminating
+    btest is worse, specifically when btest is run in CI unattended.
+
 1.0 | 2023-02-01 16:07:31 -0700
 
   * Release 1.0.
 
 0.72-71 | 2023-02-01 16:07:09 -0700
 
   * Fix test cloning bug that caused "subtests" to run without numeric suffix (Christian Kreibich, Corelight)
```

### Comparing `btest-1.0/COPYING` & `btest-1.1/COPYING`

 * *Files identical despite different names*

### Comparing `btest-1.0/Makefile` & `btest-1.1/Makefile`

 * *Files identical despite different names*

### Comparing `btest-1.0/PKG-INFO` & `btest-1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: btest
-Version: 1.0
+Version: 1.1
 Summary: A powerful system testing framework
 Home-page: https://github.com/zeek/btest
 Author: The Zeek Team
 Author-email: info@zeek.org
 License: 3-clause BSD License
 Keywords: system tests testing framework baselines
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 License-File: COPYING
 
 See https://github.com/zeek/btest
+
```

### Comparing `btest-1.0/README` & `btest-1.1/README`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ..	-*- mode: rst-mode -*-
 ..
 .. Version number is filled in automatically.
 
-.. |version| replace:: 1.0
+.. |version| replace:: 1.1
 
 ==================================================
 BTest - A Generic Driver for Powerful System Tests
 ==================================================
 
 BTest is a powerful framework for writing system tests. Freely
 borrowing some ideas from other packages, its main objective is to
@@ -657,14 +657,22 @@
     [environment-myalternative]
     CFLAGS=-O3
 
 Running ``btest`` with ``--alternative=myalternative`` will now make
 the ``CFLAGS`` environment variable available to all commands
 executed.
 
+Prefixing the name of an environment variable with ``-`` in an alternative
+section removes the respective variable from the environment::
+
+    [environment-myalternative]
+    -CFLAGS=
+
+It is an error to provide a value when prefixing with ``-``.
+
 As a special case, one can override two specific environment
 variables---``BTEST_TEST_BASE`` and ``BTEST_BASELINE_DIR``---inside an
 alternative's environment section to have them not only be passed on
 to child processes, but also apply to the ``btest`` process itself.
 That way, one can switch to a different base and baseline directories
 for an alternative.
```

### Comparing `btest-1.0/btest` & `btest-1.1/btest`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             file=sys.stderr,
         )
 else:
     import multiprocessing as mp
     import multiprocessing.managers as mp_managers
     import multiprocessing.sharedctypes as mp_sharedctypes
 
-VERSION = "1.0"  # Automatically filled in.
+VERSION = "1.1"  # Automatically filled in.
 
 Name = "btest"
 Config = None
 
 try:
     ConfigDefault = os.environ["BTEST_CFG"]
 except KeyError:
@@ -1206,16 +1206,24 @@
                     out.write(line)
             except UnicodeEncodeError as e:
                 error(f"unicode encode error in file {localfile}: {e}")
 
             out.close()
 
         self.log = open(os.path.join(self.tmpdir, ".log"), "w", encoding="utf-8")
-        self.stdout = open(os.path.join(self.tmpdir, ".stdout"), "a", encoding="utf-8")
-        self.stderr = open(os.path.join(self.tmpdir, ".stderr"), "a", encoding="utf-8")
+
+        # These file handles are given to child processes as stdout/stderr
+        # when executing CmdLine instances. In fact, just the underlying fd
+        # is used as stdout/stderr of the child (see subprocess.py).
+        # Therefore, we do neither control nor can we assume any encoding
+        # the child process may produce. Consequently, care has to be taken
+        # reading these files. So, while not strictly necessary, open them
+        # in binary mode for documentation purposes.
+        self.stdout = open(os.path.join(self.tmpdir, ".stdout"), "ab")
+        self.stderr = open(os.path.join(self.tmpdir, ".stderr"), "ab")
 
         for cmd in self.requires:
             (success, rc) = self.execute(cmd, apply_alternative=self.alternative)
 
             if not success:
                 self.mgr.testSkipped(self)
                 if not Options.tmps:
@@ -1228,15 +1236,15 @@
         # that the callback can modify the test object to maintain
         # state.
         def monitor_cb():
             while not self.monitor_quit.is_set():
                 self.parseProgress()
                 time.sleep(0.1)
 
-        self.monitor = threading.Thread(target=monitor_cb)
+        self.monitor = threading.Thread(target=monitor_cb, daemon=True)
         self.monitor_quit = threading.Event()
         self.monitor.start()
 
         # Run test's commands. First, construct a series of command sequences:
         # each sequence consists of test commands with an optional teardown that
         # always runs, regardless of prior test failures.
 
@@ -1518,17 +1526,25 @@
         env["TEST_MODE"] = Options.mode.upper()
         env["TEST_NAME"] = self.name
         env["TEST_VERBOSE"] = self.verbose
         env["TEST_PART"] = str(cmd.part)
         env["TEST_BASE"] = TestBase
 
         for key, val in addl.items():
-            # Convert val to string since otherwise os.environ (and our clone)
-            # trigger a TypeError upon insertion, and the caller may be unaware.
-            env[key] = str(val)
+            # Environment variables with a leading "-" are to be
+            # removed from the environment.
+            if key.startswith("-"):
+                try:
+                    env.pop(key[1:])
+                except KeyError:
+                    pass
+            else:
+                # Convert val to string since otherwise os.environ (and our clone)
+                # trigger a TypeError upon insertion, and the caller may be unaware.
+                env[key] = str(val)
 
         for idx, key in enumerate(sorted(self.ports)):
             env[key] = str(self.bound_ports[idx]) + "/tcp"
 
         return env
 
     def addFiles(self, files):
@@ -2025,15 +2041,15 @@
 
         for f in (test.diag, os.path.join(test.tmpdir, ".stderr")):
             if not f:
                 continue
 
             if os.path.isfile(f):
                 self.output(test, "  % cat " + os.path.basename(f), True, self._file)
-                for line in open(f):
+                for line in open(f, encoding="utf-8", errors="backslashreplace"):
                     self.output(test, "  " + line.rstrip(), True, self._file)
                 self.output(test, "", True, self._file)
 
         if self.options().wait and not self._file:
             self.output(test, "<Enter> ...")
             try:
                 sys.stdin.readline()
@@ -2121,15 +2137,17 @@
 
         for f in (test.diag, os.path.join(test.tmpdir, ".stderr")):
             if not f:
                 continue
 
             if os.path.isfile(f):
                 print("  % cat " + os.path.basename(f), file=out)
-                for line in open(f, newline="\n"):
+                for line in open(
+                    f, newline="\n", encoding="utf-8", errors="backslashreplace"
+                ):
                     print("   %s" % line.strip(), file=out)
                 print(file=out)
 
     def testUnstable(self, test, msg):
         pass
 
     def testSkipped(self, test, msg):
@@ -2190,15 +2208,17 @@
 
         for f in (test.diag, os.path.join(test.tmpdir, context_file)):
             if not f:
                 continue
 
             if os.path.isfile(f):
                 context += "  % cat " + os.path.basename(f) + "\n"
-                for line in open(f, newline="\n"):
+                for line in open(
+                    f, newline="\n", encoding="utf-8", errors="backslashreplace"
+                ):
                     context += "  " + line.strip() + "\n"
 
         return context
 
     def addTestResult(self, test, status):
         context = ""
 
@@ -3092,14 +3112,19 @@
                     a.substitutions[name] = value
 
             except configparser.NoSectionError:
                 pass
 
             try:
                 for name, value in Config.itemsNoDefaults("environment-%s" % tag):
+                    if name.startswith("-") and value.strip():
+                        error(
+                            f'expected empty value for "{name}" in section environment-{tag}'
+                        )
+
                     a.envs[name] = value
 
             except configparser.NoSectionError:
                 pass
 
             if a.is_empty() and not a.is_default():
                 error('alternative "%s" is undefined' % tag)
```

### Comparing `btest-1.0/btest-ask-update` & `btest-1.1/btest-ask-update`

 * *Files identical despite different names*

### Comparing `btest-1.0/btest-bg-run` & `btest-1.1/btest-bg-run`

 * *Files identical despite different names*

### Comparing `btest-1.0/btest-bg-wait` & `btest-1.1/btest-bg-wait`

 * *Files identical despite different names*

### Comparing `btest-1.0/btest-diff` & `btest-1.1/btest-diff`

 * *Files 4% similar despite different names*

```diff
@@ -221,15 +221,18 @@
     fi
 
     if [ $error -eq 0 ]; then
         echo "== Diff ===============================" >>$TEST_DIAGNOSTICS
         if is_binary_mode; then
             diff -s "$@" "$canon_baseline" "$canon_output" >>$TEST_DIAGNOSTICS
         else
-            diff -au --strip-trailing-cr "$@" "$canon_baseline" "$canon_output" >>$TEST_DIAGNOSTICS
+            # We'd use --strip-trailing-cr in the following, but it's not guaranteed.
+            diff -au "$@" \
+                <(sed 's/\r$//' "$canon_baseline") \
+                <(sed 's/\r$//' "$canon_output") >>$TEST_DIAGNOSTICS
         fi
         result=$?
     fi
 elif [ "$TEST_MODE" = "TEST" ]; then
     echo "== Error ==============================" >>$TEST_DIAGNOSTICS
     echo "test-diff: no baseline found." >>$TEST_DIAGNOSTICS
     result=100
```

### Comparing `btest-1.0/examples/sphinx/Makefile` & `btest-1.1/examples/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `btest-1.0/examples/sphinx/conf.py` & `btest-1.1/examples/sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `btest-1.0/examples/sphinx/index.rst` & `btest-1.1/examples/sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `btest-1.0/setup.py` & `btest-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 if sys.platform == "win32":
     install_requires = ["multiprocess"]
 else:
     install_requires = []
 
 setup(
     name="btest",
-    version="1.0",  # Filled in automatically.
+    version="1.1",  # Filled in automatically.
     description="A powerful system testing framework",
     long_description="See https://github.com/zeek/btest",
     author="The Zeek Team",
     author_email="info@zeek.org",
     url="https://github.com/zeek/btest",
     scripts=scripts,
     package_dir={"": "sphinx"},
```

### Comparing `btest-1.0/sphinx/btest-rst-cmd` & `btest-1.1/sphinx/btest-rst-cmd`

 * *Files identical despite different names*

### Comparing `btest-1.0/sphinx/btest-sphinx.py` & `btest-1.1/sphinx/btest-sphinx.py`

 * *Files identical despite different names*

### Comparing `btest-1.0/sphinx/btest.egg-info/PKG-INFO` & `btest-1.1/sphinx/btest.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: btest
-Version: 1.0
+Version: 1.1
 Summary: A powerful system testing framework
 Home-page: https://github.com/zeek/btest
 Author: The Zeek Team
 Author-email: info@zeek.org
 License: 3-clause BSD License
 Keywords: system tests testing framework baselines
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 License-File: COPYING
 
 See https://github.com/zeek/btest
+
```

### Comparing `btest-1.0/sphinx/btest.egg-info/SOURCES.txt` & `btest-1.1/sphinx/btest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,22 @@
 testing/Baseline/tests.abort-on-failure/output
 testing/Baseline/tests.abort-on-failure-with-only-known-fails/output
 testing/Baseline/tests.alternatives-environment/child-output
 testing/Baseline/tests.alternatives-environment/output
 testing/Baseline/tests.alternatives-filter/child-output
 testing/Baseline/tests.alternatives-filter/output
 testing/Baseline/tests.alternatives-keywords/output
+testing/Baseline/tests.alternatives-remove-env/child-output
+testing/Baseline/tests.alternatives-remove-env-bad/child-output
+testing/Baseline/tests.alternatives-remove-env-bad/output
 testing/Baseline/tests.alternatives-substitution/child-output
 testing/Baseline/tests.alternatives-substitution/output
 testing/Baseline/tests.alternatives-testbase/output
 testing/Baseline/tests.alternatives-undefined/output
+testing/Baseline/tests.binary-diag/.stdout
 testing/Baseline/tests.brief/out1
 testing/Baseline/tests.brief/out2
 testing/Baseline/tests.btest-cfg/abspath
 testing/Baseline/tests.btest-cfg/nopath
 testing/Baseline/tests.btest-cfg/relpath
 testing/Baseline/tests.console/output
 testing/Baseline/tests.crlf-line-terminators/crlfs.dat
@@ -158,22 +162,25 @@
 testing/tests/abort-on-failure-with-only-known-fails.btest
 testing/tests/abort-on-failure.btest
 testing/tests/alternatives-baseline-dir.test
 testing/tests/alternatives-environment.test
 testing/tests/alternatives-filter.test
 testing/tests/alternatives-keywords.test
 testing/tests/alternatives-overwrite-env.test
+testing/tests/alternatives-remove-env-bad.test
+testing/tests/alternatives-remove-env.test
 testing/tests/alternatives-reread-config-baselinedir.test
 testing/tests/alternatives-reread-config.test
 testing/tests/alternatives-substitution.test
 testing/tests/alternatives-testbase.test
 testing/tests/alternatives-undefined.test
 testing/tests/baseline-dir-env.test
 testing/tests/basic-fail.test
 testing/tests/basic-succeed.test
+testing/tests/binary-diag.test
 testing/tests/binary-mode.test
 testing/tests/brief.test
 testing/tests/btest-cfg.test
 testing/tests/canonifier-cmdline.test
 testing/tests/canonifier-conversion.test
 testing/tests/canonifier-fail.test
 testing/tests/canonifier.test
```

### Comparing `btest-1.0/testing/Baseline/tests.alternatives-filter/child-output` & `btest-1.1/testing/Baseline/tests.alternatives-filter/child-output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.diag/output` & `btest-1.1/testing/Baseline/tests.diag/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.diff-max-lines/output1` & `btest-1.1/testing/Baseline/tests.diff-max-lines/output1`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.diff-max-lines/output2` & `btest-1.1/testing/Baseline/tests.diff-max-lines/output2`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.doc/md` & `btest-1.1/testing/Baseline/tests.doc/md`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.doc/rst` & `btest-1.1/testing/Baseline/tests.doc/rst`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.environment/output` & `btest-1.1/testing/Baseline/tests.environment/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.environment-windows/output` & `btest-1.1/testing/Baseline/tests.environment-windows/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.measure-time-options/output` & `btest-1.1/testing/Baseline/tests.measure-time-options/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.progress-back-to-back/output` & `btest-1.1/testing/Baseline/tests.progress-back-to-back/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.sphinx.rst-cmd/output` & `btest-1.1/testing/Baseline/tests.sphinx.rst-cmd/output`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt` & `btest-1.1/testing/Baseline/tests.sphinx.run-sphinx/_build.text.index.txt`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/Scripts/test-perf` & `btest-1.1/testing/Scripts/test-perf`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/btest.cfg` & `btest-1.1/testing/btest.cfg`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/btest.tests.cfg` & `btest-1.1/testing/btest.tests.cfg`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/abort-on-failure-with-only-known-fails.btest` & `btest-1.1/testing/tests/abort-on-failure-with-only-known-fails.btest`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/alternatives-baseline-dir.test` & `btest-1.1/testing/tests/alternatives-baseline-dir.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/alternatives-keywords.test` & `btest-1.1/testing/tests/alternatives-keywords.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/baseline-dir-env.test` & `btest-1.1/testing/tests/baseline-dir-env.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/binary-mode.test` & `btest-1.1/testing/tests/binary-mode.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/btest-cfg.test` & `btest-1.1/testing/tests/btest-cfg.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/canonifier-cmdline.test` & `btest-1.1/testing/tests/canonifier-cmdline.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/canonifier-conversion.test` & `btest-1.1/testing/tests/canonifier-conversion.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/canonifier-fail.test` & `btest-1.1/testing/tests/canonifier-fail.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/console.test` & `btest-1.1/testing/tests/console.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/diff-brief.test` & `btest-1.1/testing/tests/diff-brief.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/diff-max-lines.test` & `btest-1.1/testing/tests/diff-max-lines.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/doc.test` & `btest-1.1/testing/tests/doc.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/env-var-casing.test` & `btest-1.1/testing/tests/env-var-casing.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/environment-windows.test` & `btest-1.1/testing/tests/environment-windows.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/environment.test` & `btest-1.1/testing/tests/environment.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/exit-codes.test` & `btest-1.1/testing/tests/exit-codes.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/groups.test` & `btest-1.1/testing/tests/groups.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/ignore.test` & `btest-1.1/testing/tests/ignore.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/measure-time-options.test` & `btest-1.1/testing/tests/measure-time-options.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/measure-time.tests` & `btest-1.1/testing/tests/measure-time.tests`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/multiple-baseline-dirs.test` & `btest-1.1/testing/tests/multiple-baseline-dirs.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/parts-initializer-finalizer.test` & `btest-1.1/testing/tests/parts-initializer-finalizer.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/parts-teardown.test` & `btest-1.1/testing/tests/parts-teardown.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/progress-back-to-back.test` & `btest-1.1/testing/tests/progress-back-to-back.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/progress.test` & `btest-1.1/testing/tests/progress.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/statefile.test` & `btest-1.1/testing/tests/statefile.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/teardown.test` & `btest-1.1/testing/tests/teardown.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/threads.test` & `btest-1.1/testing/tests/threads.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/unstable-dir.test` & `btest-1.1/testing/tests/unstable-dir.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/unstable-subtest.test` & `btest-1.1/testing/tests/unstable-subtest.test`

 * *Files identical despite different names*

### Comparing `btest-1.0/testing/tests/xml.test` & `btest-1.1/testing/tests/xml.test`

 * *Files identical despite different names*

