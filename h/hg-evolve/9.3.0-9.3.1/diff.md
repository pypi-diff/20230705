# Comparing `tmp/hg-evolve-9.3.0.tar.gz` & `tmp/hg-evolve-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hg-evolve-9.3.0.tar", last modified: Wed Mar  4 17:04:49 2020, max compression
+gzip compressed data, was "dist/hg-evolve-9.3.1.tar", last modified: Wed Apr  8 14:19:04 2020, max compression
```

## Comparing `hg-evolve-9.3.0.tar` & `hg-evolve-9.3.1.tar`

### file list

```diff
@@ -1,309 +1,330 @@
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/figures/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2442 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg01-ab.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4259 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg02-b.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3069 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg03.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4898 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg04-a.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4897 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg04-b.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1971 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg05.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2984 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg06.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5690 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg07-a.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1991 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg07-b.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6677 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg08-a.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2591 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg08-b.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6840 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg09.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7324 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-sg10.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15771 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug01.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20777 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug02.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16730 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug03.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22903 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug04.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30464 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug05.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32650 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug06.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25240 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug07.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    19226 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug08.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14111 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug09.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    41987 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug10.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    29239 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug11.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25991 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/figures/figure-ug12.svg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)   217868 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/figures/hgview-example.png
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/static/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)   107444 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/static/logo-evolve.svg
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/tutorial/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/tutorial/mypandocfilters/
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     1147 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/mypandocfilters/graphviz-file.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      483 2019-12-18 13:10:57.000000 hg-evolve-9.3.0/docs/tutorial/mypandocfilters/raw-file.py
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/tutorial/testlib/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      496 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/arguments_printer.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      772 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/common.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)       85 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/docgraph_setup.sh
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     3568 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/exchange-obsmarker-util.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      524 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/push-checkheads-util.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      256 2019-12-18 13:10:57.000000 hg-evolve-9.3.0/docs/tutorial/testlib/pythonpath.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      331 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/testlib/topic_setup.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1706 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/README.rst
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      338 2019-12-18 13:10:57.000000 hg-evolve-9.3.0/docs/tutorial/compile.sh
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      125 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/deploy.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    33685 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/tutorial/draft.md
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7839 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/jquery.sticky-kit.js
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      884 2019-12-18 13:10:57.000000 hg-evolve-9.3.0/docs/tutorial/prepare.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3662 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/scripts.js
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    70943 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/tutorial/slides.md
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3266 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/standalone.html
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      596 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/style.css
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)   106829 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/tutorial/test-training.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)   167005 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/uikit.css
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)   114616 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorial/uikit.js
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/docs/tutorials/
-lrwxrwxrwx   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorials/topic-tutorial.t -> ../../tests/test-topic-tutorial.t
-lrwxrwxrwx   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/tutorials/tutorial.t -> ../../tests/test-tutorial.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      647 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/README
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      548 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/commands.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8419 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/concepts.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5077 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/conf.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5579 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/evolve-faq.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1537 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/evolve-good-practice.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4193 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/from-mq.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7223 2019-12-18 13:10:57.000000 hg-evolve-9.3.0/docs/index.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1173 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/docs/known-doc-issues.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      443 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/makefile
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13333 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/obs-terms.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    28938 2020-01-23 10:10:57.000000 hg-evolve-9.3.0/docs/sharing.rst
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2315 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/test2rst.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22827 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/docs/user-guide.rst
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/hgext3rd/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/hgext3rd/evolve/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/hgext3rd/evolve/thirdparty/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/hgext3rd/evolve/thirdparty/__init__.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16189 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/thirdparty/cbor.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    51816 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/__init__.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    62239 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/cmdrewrite.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    17457 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/compat.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8535 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/dagutil.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6280 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/debugcmd.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7149 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/depthcache.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    94031 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/evolvecmd.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    12319 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/exthelper.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4862 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/firstmergecache.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5709 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/genericcaches.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7619 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/legacy.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      402 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/hgext3rd/evolve/metadata.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    17940 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/obscache.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    31008 2020-03-04 15:33:35.000000 hg-evolve-9.3.0/hgext3rd/evolve/obsdiscovery.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6163 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/obsexchange.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3093 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/obshashtree.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    27515 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/obshistory.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8535 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/rewind.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11898 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/rewriteutil.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2122 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/safeguard.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1775 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/serveronly.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    47252 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/evolve/stablerange.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    18829 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/stablerangecache.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32146 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/stablesort.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4878 2020-01-23 10:10:57.000000 hg-evolve-9.3.0/hgext3rd/evolve/state.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6871 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/templatekw.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8029 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/evolve/utility.py
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/hgext3rd/topic/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1306 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/hgext3rd/topic/README
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    48868 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/hgext3rd/topic/__init__.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      326 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/common.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1125 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/topic/compat.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)       50 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/constants.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3957 2020-01-23 10:10:57.000000 hg-evolve-9.3.0/hgext3rd/topic/destination.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8011 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/topic/discovery.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3810 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/topic/evolvebits.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3955 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/flow.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16414 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/randomname.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5433 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/revset.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4177 2020-03-04 16:48:10.000000 hg-evolve-9.3.0/hgext3rd/topic/server.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13342 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/stack.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8082 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/hgext3rd/topic/topicmap.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      157 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/hgext3rd/__init__.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22432 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/pullbundle.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7924 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/hgext3rd/serverminitopic.py
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/tests/
-drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/tests/testlib/
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      239 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/testlib/common.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)       85 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/testlib/docgraph_setup.sh
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     3568 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/testlib/exchange-obsmarker-util.sh
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      244 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/testlib/map-hg-rev.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      217 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/testlib/obshistory_setup.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      524 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/testlib/push-checkheads-util.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      363 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/testlib/pythonpath.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      331 2020-02-19 00:25:36.000000 hg-evolve-9.3.0/tests/testlib/topic_setup.sh
--rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)       40 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/fake-editor.sh
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      395 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/hghaveaddon.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25405 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-amend-patch.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7640 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-amend.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      688 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-check-commit.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      452 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-check-flake8.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      325 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-check-pyflakes.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      371 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-check-setup-manifest.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2845 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-corrupt.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6337 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-discovery-obshashrange-cache.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    85871 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-discovery-obshashrange.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7336 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-drop.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13681 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-abort-orphan.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8658 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-abort-phasediv.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    26878 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-basic.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9583 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-corner-cases.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1104 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-first-changeset.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16119 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-interrupted.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11992 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-meta.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13837 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-relocation.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    31029 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-content-divergent-stack.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10227 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-continue.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13325 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-cycles.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7356 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-effectflags.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3037 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/tests/test-evolve-interrupted.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10765 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-issue5832.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1610 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-issue5881.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2655 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-issue5958.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1940 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-issue5966.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1747 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/tests/test-evolve-issue5967.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2659 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-issue6097.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2170 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-list.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3184 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-noupdate.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7731 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-amend-then-fold.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15024 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-amend.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13710 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-complex.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10691 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-content-divergent.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10701 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-fold.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7913 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-lots-of-splits.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6743 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-phase-divergent.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3280 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-prune.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7765 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory-split.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5469 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-obshistory.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6978 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-order.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3443 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-orphan-corner-cases.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15165 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-orphan-merge.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6946 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-orphan-split.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    49809 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-phase-divergence.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2468 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-phase.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5746 2020-03-04 17:04:18.000000 hg-evolve-9.3.0/tests/test-evolve-progress.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20667 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-corner-cases.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15889 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-discard.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14111 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-main.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5453 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-serveronly-bundle2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1622 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-evolve-serveronly-legacy.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1393 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-split.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9199 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-stop-orphan.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2836 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-evolve-stop-phasediv.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    43002 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-templates.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11889 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve-topic.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    37402 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-evolve.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10999 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4875 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10544 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5405 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5850 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A5.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5535 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A6.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3032 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A7.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3300 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5273 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3941 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6392 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7320 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B5.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5127 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B6.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3343 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B7.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7720 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8256 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9844 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5946 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8252 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4818 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4192 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6936 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4814 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/tests/test-extension-isolation.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10925 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-fold.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2346 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-import.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1641 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-issue-5720.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4498 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-issue-6028.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7090 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-metaedit.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7318 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-minitopic.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3538 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-obsconvert.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2715 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-obsolete-push.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    24469 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-obsolete.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3574 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-oldconvert.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      611 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-options.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9655 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-pick.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14411 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-prev-next.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20876 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-prune.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    39301 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-pullbundle.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1965 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-partial-C1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2067 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-partial-C2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1926 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-partial-C3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1969 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-partial-C4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1608 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2163 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2129 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2087 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2340 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B5.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1938 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B6.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1934 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B7.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2706 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B8.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1598 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2179 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2253 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1717 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1715 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A5.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2670 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A6.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2672 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A7.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1962 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A8.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1869 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2453 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D2.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2992 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D3.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3273 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D4.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3116 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D5.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2078 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D6.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2507 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D7.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    37937 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-rewind.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      455 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-share.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14787 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-sharing.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30996 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-split.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6647 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stabilize-conflict.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6371 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stabilize-order.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32009 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-stablerange-branchpoint.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32080 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-stablerange.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20483 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stablesort-branchpoint-criss-cross.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20589 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stablesort-branchpoint.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22242 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stablesort-criss-cross.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    27110 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stablesort.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6405 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-stack-branch.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7846 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-change.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7246 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-debugcb.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10062 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-dest.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9223 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-flow-publish-bare.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11605 2020-02-25 00:28:41.000000 hg-evolve-9.3.0/tests/test-topic-flow-publish-flag.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3831 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-flow-reject-untopiced.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4901 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-flow-single-head.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3214 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-topic-fold.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9542 2020-02-25 00:28:41.000000 hg-evolve-9.3.0/tests/test-topic-mode.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1771 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-multiple.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10641 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-push-concurrent-on.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11790 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-push.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4732 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-rebase.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5745 2020-03-04 16:48:10.000000 hg-evolve-9.3.0/tests/test-topic-server.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1193 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/tests/test-topic-shelve.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4281 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-stack-complex.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6699 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-topic-stack-data.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    24167 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-stack.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    46932 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic-tutorial.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30035 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-topic.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4640 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-touch.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    46441 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-tutorial.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16512 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-uncommit-interactive.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10789 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-uncommit.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5825 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-unstability-resolution-result.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3329 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-unstable-orphan.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9261 2020-02-25 00:28:41.000000 hg-evolve-9.3.0/tests/test-userguide.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      785 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/tests/test-version-install.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2265 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-wireproto-bundle1.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7667 2020-03-04 16:32:40.000000 hg-evolve-9.3.0/tests/test-wireproto.t
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    40918 2020-03-04 16:48:10.000000 hg-evolve-9.3.0/CHANGELOG
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)    18095 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/COPYING
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      894 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/MANIFEST.in
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7230 2020-03-04 16:27:37.000000 hg-evolve-9.3.0/README
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)      909 2019-09-21 15:30:33.000000 hg-evolve-9.3.0/setup.cfg
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1601 2020-01-23 10:10:45.000000 hg-evolve-9.3.0/setup.py
--rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9411 2020-03-04 17:04:49.000000 hg-evolve-9.3.0/PKG-INFO
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/figures/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2442 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg01-ab.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4259 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg02-b.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3069 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg03.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4898 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg04-a.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4897 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg04-b.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1971 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg05.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2984 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg06.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5690 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg07-a.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1991 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg07-b.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6677 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg08-a.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2591 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg08-b.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6840 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg09.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7324 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-sg10.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15771 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug01.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20777 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug02.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16730 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug03.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22903 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug04.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30464 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug05.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32650 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug06.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25240 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug07.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    19226 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug08.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14111 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug09.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    41987 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug10.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    29239 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug11.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25991 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/figures/figure-ug12.svg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)   217868 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/figures/hgview-example.png
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/static/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)   107444 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/static/logo-evolve.svg
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/tutorial/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/tutorial/mypandocfilters/
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     1147 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/mypandocfilters/graphviz-file.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      483 2019-12-18 13:10:57.000000 hg-evolve-9.3.1/docs/tutorial/mypandocfilters/raw-file.py
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/tutorial/testlib/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      496 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/arguments_printer.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      772 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/common.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)       85 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/docgraph_setup.sh
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     3568 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/exchange-obsmarker-util.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      524 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/push-checkheads-util.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      256 2019-12-18 13:10:57.000000 hg-evolve-9.3.1/docs/tutorial/testlib/pythonpath.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      331 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/testlib/topic_setup.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1706 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/README.rst
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      338 2019-12-18 13:10:57.000000 hg-evolve-9.3.1/docs/tutorial/compile.sh
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      125 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/deploy.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    33685 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/tutorial/draft.md
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7839 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/jquery.sticky-kit.js
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      884 2019-12-18 13:10:57.000000 hg-evolve-9.3.1/docs/tutorial/prepare.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3662 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/scripts.js
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    70943 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/tutorial/slides.md
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3266 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/standalone.html
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      596 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/style.css
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)   106829 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/tutorial/test-training.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)   167005 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/uikit.css
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)   114616 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorial/uikit.js
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/docs/tutorials/
+lrwxrwxrwx   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorials/topic-tutorial.t -> ../../tests/test-topic-tutorial.t
+lrwxrwxrwx   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/tutorials/tutorial.t -> ../../tests/test-tutorial.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      647 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/README
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      548 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/commands.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8419 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/concepts.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5077 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/conf.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5579 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/evolve-faq.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1537 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/evolve-good-practice.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4193 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/from-mq.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7223 2019-12-18 13:10:57.000000 hg-evolve-9.3.1/docs/index.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1173 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/docs/known-doc-issues.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      443 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/makefile
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13333 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/obs-terms.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    28938 2020-01-23 10:10:57.000000 hg-evolve-9.3.1/docs/sharing.rst
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2315 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/test2rst.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22827 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/docs/user-guide.rst
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/hgext3rd/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/hgext3rd/evolve/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/hgext3rd/evolve/thirdparty/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)        0 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/hgext3rd/evolve/thirdparty/__init__.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16189 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/thirdparty/cbor.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    51860 2020-04-08 14:18:57.000000 hg-evolve-9.3.1/hgext3rd/evolve/__init__.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    62247 2020-04-08 14:18:57.000000 hg-evolve-9.3.1/hgext3rd/evolve/cmdrewrite.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    17457 2020-04-08 14:18:57.000000 hg-evolve-9.3.1/hgext3rd/evolve/compat.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8535 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/dagutil.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6280 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/debugcmd.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7149 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/depthcache.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    94032 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/evolvecmd.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    12319 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/hgext3rd/evolve/exthelper.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4862 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/firstmergecache.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5709 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/hgext3rd/evolve/genericcaches.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6459 2020-04-07 17:32:53.000000 hg-evolve-9.3.1/hgext3rd/evolve/headchecking.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7619 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/legacy.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      402 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/metadata.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    17940 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/obscache.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    31628 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/obsdiscovery.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7060 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/obsexchange.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3093 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/obshashtree.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    27515 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/obshistory.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8551 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/rewind.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11898 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/hgext3rd/evolve/rewriteutil.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2080 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/safeguard.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1775 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/evolve/serveronly.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    47252 2020-03-11 14:26:26.000000 hg-evolve-9.3.1/hgext3rd/evolve/stablerange.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    18828 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/stablerangecache.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32146 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/stablesort.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4878 2020-01-23 10:10:57.000000 hg-evolve-9.3.1/hgext3rd/evolve/state.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6871 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/evolve/templatekw.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7982 2020-04-07 16:24:54.000000 hg-evolve-9.3.1/hgext3rd/evolve/utility.py
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/hgext3rd/topic/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1306 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/hgext3rd/topic/README
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    49599 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/__init__.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      326 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/topic/common.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1125 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/compat.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)       50 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/topic/constants.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3957 2020-01-23 10:10:57.000000 hg-evolve-9.3.1/hgext3rd/topic/destination.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9414 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/discovery.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3810 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/hgext3rd/topic/evolvebits.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5832 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/flow.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16414 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/topic/randomname.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5433 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/revset.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4177 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/server.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13342 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/hgext3rd/topic/stack.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8082 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/topic/topicmap.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      157 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/hgext3rd/__init__.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22432 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/pullbundle.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7924 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/hgext3rd/serverminitopic.py
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/tests/
+drwxr-xr-x   0 marmoute  (1000) marmoute  (1000)        0 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/tests/testlib/
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      239 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/testlib/common.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)       85 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/testlib/docgraph_setup.sh
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)     3568 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/testlib/exchange-obsmarker-util.sh
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)      244 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/testlib/map-hg-rev.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      217 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/testlib/obshistory_setup.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1000 2020-04-07 17:32:53.000000 hg-evolve-9.3.1/tests/testlib/push-checkheads-util.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      363 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/testlib/pythonpath.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      331 2020-02-19 00:25:36.000000 hg-evolve-9.3.1/tests/testlib/topic_setup.sh
+-rwxr-xr-x   0 marmoute  (1000) marmoute  (1000)       40 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/fake-editor.sh
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      395 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/hghaveaddon.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    25405 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-amend-patch.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7640 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-amend.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      688 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-check-commit.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      452 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-check-flake8.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      325 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-check-pyflakes.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      371 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-check-setup-manifest.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2845 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-corrupt.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2535 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-discovery-hidden-common.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6294 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-discovery-obshashrange-cache.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    85884 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-discovery-obshashrange.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7336 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-drop.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13681 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-abort-orphan.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8658 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-abort-phasediv.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    26878 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-basic.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9583 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-corner-cases.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1104 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-first-changeset.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16119 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-interrupted.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11992 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-meta.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13837 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-relocation.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    31029 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-content-divergent-stack.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10227 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-continue.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13325 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-cycles.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7356 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-effectflags.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3037 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-interrupted.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10774 2020-04-07 16:24:54.000000 hg-evolve-9.3.1/tests/test-evolve-issue5832.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1610 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-issue5881.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2655 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-issue5958.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1940 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-issue5966.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1747 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-issue5967.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2659 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-issue6097.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2170 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-list.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3184 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-noupdate.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7729 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-amend-then-fold.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15024 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-amend.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    13710 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-complex.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10691 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-content-divergent.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10701 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-fold.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7913 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-lots-of-splits.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6743 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-phase-divergent.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3280 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-prune.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7765 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory-split.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5467 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-obshistory.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6978 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-order.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3443 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-orphan-corner-cases.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15165 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-orphan-merge.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6967 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-orphan-split.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    49809 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-phase-divergence.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2468 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-phase.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5746 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-evolve-progress.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20667 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-corner-cases.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    15889 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-discard.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14111 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-main.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5458 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-serveronly-bundle2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1622 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-evolve-serveronly-legacy.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2803 2020-04-06 02:20:20.000000 hg-evolve-9.3.1/tests/test-evolve-split.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9199 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-stop-orphan.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2836 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-evolve-stop-phasediv.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    43002 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-templates.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11889 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve-topic.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    37402 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-evolve.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10999 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4875 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10544 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5405 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5850 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5535 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A6.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3032 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A7.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3300 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5273 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3941 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6392 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7320 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5127 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B6.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3343 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B7.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7720 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8256 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9844 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5946 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     8252 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4818 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4192 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6936 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4814 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/tests/test-extension-isolation.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10925 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-fold.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2346 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-import.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1641 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-issue-5720.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4498 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-issue-6028.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7090 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-metaedit.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7318 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-minitopic.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3538 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-obsconvert.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2715 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-obsolete-push.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    24469 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-obsolete.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3574 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-oldconvert.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      611 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-options.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9655 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-pick.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14411 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-prev-next.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20876 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-prune.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    39301 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-pullbundle.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2183 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-mixed-branch-topic-G1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2693 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-mixed-branch-topic-G2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2471 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-mixed-branch-topic-G3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2310 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multi-topics-F1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2821 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multi-topics-F2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2618 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multi-topics-F3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2247 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multibranches-E1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2693 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multibranches-E2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2468 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-multibranches-E3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1965 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-partial-C1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2067 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-partial-C2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1926 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-partial-C3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1969 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-partial-C4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1608 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2163 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2129 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2087 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2340 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1938 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B6.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1934 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B7.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2706 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B8.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1598 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2179 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2253 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1717 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1715 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2670 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A6.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2672 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A7.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1962 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A8.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1869 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2453 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2992 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3273 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3116 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2078 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D6.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2507 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D7.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    37937 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-rewind.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      455 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-share.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    14787 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-sharing.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2789 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-named-branch-A1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2740 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-named-branch-A2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3121 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-named-branch-A3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3045 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-named-branch-A4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3042 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-named-branch-A5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3086 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-topic-B1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3078 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-topic-B2.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3144 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-topic-B3.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3045 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-topic-B4.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3232 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-single-head-obsolescence-topic-B5.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30996 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-split.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6647 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stabilize-conflict.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6371 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stabilize-order.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32009 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-stablerange-branchpoint.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    32080 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-stablerange.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20483 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stablesort-branchpoint-criss-cross.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    20589 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stablesort-branchpoint.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    22242 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stablesort-criss-cross.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    27110 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stablesort.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6405 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-stack-branch.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7846 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-topic-change.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7246 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-topic-debugcb.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10062 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-dest.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10570 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-flow-publish-bare.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11605 2020-02-25 00:28:41.000000 hg-evolve-9.3.1/tests/test-topic-flow-publish-flag.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3831 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-flow-reject-untopiced.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4901 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-flow-single-head.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3214 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-topic-fold.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9542 2020-02-25 00:28:41.000000 hg-evolve-9.3.1/tests/test-topic-mode.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1771 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-topic-multiple.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10645 2020-04-06 02:20:20.000000 hg-evolve-9.3.1/tests/test-topic-push-concurrent-on.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    11794 2020-04-06 02:20:20.000000 hg-evolve-9.3.1/tests/test-topic-push.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4732 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-topic-rebase.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5745 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-server.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1193 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/tests/test-topic-shelve.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4281 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-stack-complex.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     6699 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-topic-stack-data.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    24167 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-stack.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    46932 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic-tutorial.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    30035 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-topic.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     4640 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-touch.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    46441 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-tutorial.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    16512 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-uncommit-interactive.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    10789 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-uncommit.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     5825 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-unstability-resolution-result.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     3329 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-unstable-orphan.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9261 2020-02-25 00:28:41.000000 hg-evolve-9.3.1/tests/test-userguide.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      785 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/tests/test-version-install.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     2270 2020-04-08 13:34:48.000000 hg-evolve-9.3.1/tests/test-wireproto-bundle1.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7672 2020-04-08 14:18:58.000000 hg-evolve-9.3.1/tests/test-wireproto.t
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    41612 2020-04-08 14:18:57.000000 hg-evolve-9.3.1/CHANGELOG
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)    18095 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/COPYING
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      894 2020-03-04 16:27:37.000000 hg-evolve-9.3.1/MANIFEST.in
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     7230 2020-04-08 14:18:57.000000 hg-evolve-9.3.1/README
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)      909 2019-09-21 15:30:33.000000 hg-evolve-9.3.1/setup.cfg
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     1601 2020-01-23 10:10:45.000000 hg-evolve-9.3.1/setup.py
+-rw-r--r--   0 marmoute  (1000) marmoute  (1000)     9411 2020-04-08 14:19:04.000000 hg-evolve-9.3.1/PKG-INFO
```

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg01-ab.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg01-ab.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg02-b.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg02-b.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg03.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg03.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg04-a.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg04-a.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg04-b.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg04-b.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg05.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg05.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg06.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg06.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg07-a.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg07-a.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg07-b.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg07-b.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg08-a.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg08-a.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg08-b.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg08-b.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg09.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg09.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-sg10.svg` & `hg-evolve-9.3.1/docs/figures/figure-sg10.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug01.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug01.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug02.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug02.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug03.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug03.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug04.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug04.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug05.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug05.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug06.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug06.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug07.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug07.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug08.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug08.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug09.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug09.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug10.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug10.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug11.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug11.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/figure-ug12.svg` & `hg-evolve-9.3.1/docs/figures/figure-ug12.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/figures/hgview-example.png` & `hg-evolve-9.3.1/docs/figures/hgview-example.png`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/static/logo-evolve.svg` & `hg-evolve-9.3.1/docs/static/logo-evolve.svg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/mypandocfilters/graphviz-file.py` & `hg-evolve-9.3.1/docs/tutorial/mypandocfilters/graphviz-file.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/testlib/common.sh` & `hg-evolve-9.3.1/docs/tutorial/testlib/common.sh`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/testlib/exchange-obsmarker-util.sh` & `hg-evolve-9.3.1/docs/tutorial/testlib/exchange-obsmarker-util.sh`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/testlib/push-checkheads-util.sh` & `hg-evolve-9.3.1/docs/tutorial/testlib/push-checkheads-util.sh`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/README.rst` & `hg-evolve-9.3.1/docs/tutorial/README.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/draft.md` & `hg-evolve-9.3.1/docs/tutorial/draft.md`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/jquery.sticky-kit.js` & `hg-evolve-9.3.1/docs/tutorial/jquery.sticky-kit.js`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/prepare.sh` & `hg-evolve-9.3.1/docs/tutorial/prepare.sh`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/scripts.js` & `hg-evolve-9.3.1/docs/tutorial/scripts.js`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/slides.md` & `hg-evolve-9.3.1/docs/tutorial/slides.md`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/standalone.html` & `hg-evolve-9.3.1/docs/tutorial/standalone.html`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/style.css` & `hg-evolve-9.3.1/docs/tutorial/style.css`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/test-training.t` & `hg-evolve-9.3.1/docs/tutorial/test-training.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/uikit.css` & `hg-evolve-9.3.1/docs/tutorial/uikit.css`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/tutorial/uikit.js` & `hg-evolve-9.3.1/docs/tutorial/uikit.js`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/README` & `hg-evolve-9.3.1/docs/README`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/commands.rst` & `hg-evolve-9.3.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/concepts.rst` & `hg-evolve-9.3.1/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/conf.py` & `hg-evolve-9.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/evolve-faq.rst` & `hg-evolve-9.3.1/docs/evolve-faq.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/evolve-good-practice.rst` & `hg-evolve-9.3.1/docs/evolve-good-practice.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/from-mq.rst` & `hg-evolve-9.3.1/docs/from-mq.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/index.rst` & `hg-evolve-9.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/known-doc-issues.rst` & `hg-evolve-9.3.1/docs/known-doc-issues.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/obs-terms.rst` & `hg-evolve-9.3.1/docs/obs-terms.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/sharing.rst` & `hg-evolve-9.3.1/docs/sharing.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/test2rst.py` & `hg-evolve-9.3.1/docs/test2rst.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/docs/user-guide.rst` & `hg-evolve-9.3.1/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/thirdparty/cbor.py` & `hg-evolve-9.3.1/hgext3rd/evolve/thirdparty/cbor.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/__init__.py` & `hg-evolve-9.3.1/hgext3rd/evolve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,14 +288,15 @@
 from . import (
     compat,
     debugcmd,
     cmdrewrite,
     state,
     evolvecmd,
     exthelper,
+    headchecking,
     metadata,
     obscache,
     obsexchange,
     obshashtree,
     obshistory,
     rewind,
     safeguard,
@@ -342,14 +343,15 @@
 eh.merge(safeguard.eh)
 eh.merge(obscache.eh)
 eh.merge(obshistory.eh)
 eh.merge(templatekw.eh)
 eh.merge(compat.eh)
 eh.merge(cmdrewrite.eh)
 eh.merge(rewind.eh)
+eh.merge(headchecking.eh)
 uisetup = eh.finaluisetup
 extsetup = eh.finalextsetup
 reposetup = eh.finalreposetup
 cmdtable = eh.cmdtable
 configtable = eh.configtable
 revsetpredicate = eh.revsetpredicate
 templatekeyword = eh.templatekeyword
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/cmdrewrite.py` & `hg-evolve-9.3.1/hgext3rd/evolve/cmdrewrite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1403,15 +1403,15 @@
     duplicate = opts['duplicate']
     allowdivergence = opts['allowdivergence']
     revs.sort() # ensure parent are run first
     newmapping = {}
     for r in revs:
         ctx = repo[r]
         extra = ctx.extra().copy()
-        extra[b'__touch-noise__'] = random.randint(0, 0xffffffff)
+        extra[b'__touch-noise__'] = b'%d' % random.randint(0, 0xffffffff)
         # search for touched parent
         p1 = ctx.p1().node()
         p2 = ctx.p2().node()
         p1 = newmapping.get(p1, p1)
         p2 = newmapping.get(p2, p2)
 
         if not (duplicate or allowdivergence):
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/compat.py` & `hg-evolve-9.3.1/hgext3rd/evolve/compat.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/dagutil.py` & `hg-evolve-9.3.1/hgext3rd/evolve/dagutil.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/debugcmd.py` & `hg-evolve-9.3.1/hgext3rd/evolve/debugcmd.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/depthcache.py` & `hg-evolve-9.3.1/hgext3rd/evolve/depthcache.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/evolvecmd.py` & `hg-evolve-9.3.1/hgext3rd/evolve/evolvecmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1614,17 +1614,17 @@
     repository by using the --list flag. You can choose to display only some
     categories of troubles with the --orphan, --content-divergent or
     --phase-divergent flags.
 
     Interrupted
     ===========
 
-    The `hg evolve` command is an all purpose tool that solve all kind of
+    The `hg evolve` command is an all purpose tool that solves all kinds of
     instabilities in your repository. Sometimes, instability resolution will lead
-    to merge conflict that cannot be solved without a human intervention (same as
+    to merge conflicts that cannot be solved without human intervention (same as
     `hg merge`). This can lead to an "interrupted state" where human assistance is
     requested. There are three things which you can do when you face a similar
     situation:
 
       - `hg evolve --continue`:
          resolve all the conflicts using `hg resolve` and then run this to
          continue the interrupted evolve
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/exthelper.py` & `hg-evolve-9.3.1/hgext3rd/evolve/exthelper.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/firstmergecache.py` & `hg-evolve-9.3.1/hgext3rd/evolve/firstmergecache.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/genericcaches.py` & `hg-evolve-9.3.1/hgext3rd/evolve/genericcaches.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/legacy.py` & `hg-evolve-9.3.1/hgext3rd/evolve/legacy.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/obscache.py` & `hg-evolve-9.3.1/hgext3rd/evolve/obscache.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/obsdiscovery.py` & `hg-evolve-9.3.1/hgext3rd/evolve/obsdiscovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -840,30 +840,41 @@
     """small function returning the argument for pull markers call
     may to contains 'heads' and 'common'. skip the key for None.
 
     It is a separed function to play around with strategy for that."""
     repo = pullop.repo
     remote = pullop.remote
     unfi = repo.unfiltered()
-    revs = unfi.revs(b'::(%ln - null)', pullop.common)
+    # Also exclude filtered revisions. Working on unfiltered repository can
+    # give a bit more precise view of the repository. However it makes the
+    # overall operation more complicated.
+    filteredrevs = repo.changelog.filteredrevs
+    # XXX probably not very efficient
+    revs = unfi.revs(b'::(%ln - null) - %ld', pullop.common, filteredrevs)
     boundaries = {b'heads': pullop.pulledsubset}
     if not revs: # nothing common
         boundaries[b'common'] = [node.nullid]
         return boundaries
 
     if not usediscovery(repo):
         # discovery disabled by users.
         repo.ui.status(obsdiscovery_skip_message)
         boundaries[b'common'] = [node.nullid]
         return boundaries
 
     if bundle2 and _canobshashrange(repo, remote):
         obsexcmsg(repo.ui, b"looking for common markers in %i nodes\n"
                   % len(revs))
-        boundaries[b'missing'] = findmissingrange(repo.ui, unfi, pullop.remote,
-                                                  revs)
+        missing = findmissingrange(repo.ui, repo, pullop.remote, revs)
+        boundaries[b'missing'] = missing
+        # using getattr since `limitedarguments` is missing
+        # hg <= 5.0 (69921d02daaf)
+        if getattr(pullop.remote, 'limitedarguments', False):
+            # prepare for a possible fallback to common
+            common = repo.set("heads(only(%ld, %ln))", revs, missing)
+            boundaries[b'common'] = [c.node() for c in common]
     else:
         boundaries[b'common'] = [node.nullid]
     return boundaries
 
 # merge later for outer layer wrapping
 eh.merge(stablerangecache.eh)
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/obsexchange.py` & `hg-evolve-9.3.1/hgext3rd/evolve/obsexchange.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,47 +50,70 @@
     except (ImportError, AttributeError):
         # <= hg 4.5
         from mercurial import wireproto
         gboptsmap = wireproto.gboptsmap
     gboptsmap[b'evo_obscommon'] = b'nodes'
     gboptsmap[b'evo_missing_nodes'] = b'nodes'
 
+ARGUMENTS_LIMIT = 200
+
+OVERFLOW_MSG = """obsmarkers differ for %d common nodes
+|
+| This might be too much for the remote HTTP server that doesn't accept
+| arguments through POST request. (config: experimental.httppostargs=yes)
+|
+| Falling back to a less efficient fetching method.
+|
+| More efficient fetching method is possible and will be used in the future.
+"""
+
 @eh.wrapfunction(exchange, '_pullbundle2extraprepare')
 def _addobscommontob2pull(orig, pullop, kwargs):
     ret = orig(pullop, kwargs)
     ui = pullop.repo.ui
     if (b'obsmarkers' in kwargs
         and pullop.remote.capable(b'_evoext_getbundle_obscommon')):
         boundaries = obsdiscovery.buildpullobsmarkersboundaries(pullop)
-        if b'common' in boundaries:
+        use_common = True
+        if b'missing' in boundaries:
+            use_common = False
+            missing = boundaries[b'missing']
+            # using getattr since `limitedarguments` is missing
+            # hg <= 5.0 (69921d02daaf)
+            limitedarguments = getattr(pullop.remote, 'limitedarguments', False)
+            if limitedarguments and len(missing) > ARGUMENTS_LIMIT:
+                obsexcmsg(ui, OVERFLOW_MSG % len(missing))
+                use_common = True
+            else:
+                if missing:
+                    obsexcmsg(ui, b'request obsmarkers for %d common nodes\n'
+                              % len(missing))
+                kwargs[b'evo_missing_nodes'] = missing
+        if use_common and b'common' in boundaries:
             common = boundaries[b'common']
             if common != pullop.common:
                 obsexcmsg(ui, b'request obsmarkers for some common nodes\n')
             if common != [node.nullid]:
                 kwargs[b'evo_obscommon'] = common
-        elif b'missing' in boundaries:
-            missing = boundaries[b'missing']
-            if missing:
-                obsexcmsg(ui, b'request obsmarkers for %d common nodes\n'
-                          % len(missing))
-            kwargs[b'evo_missing_nodes'] = missing
     return ret
 
 def _getbundleobsmarkerpart(orig, bundler, repo, source, **kwargs):
     if not (set([r'evo_obscommon', r'evo_missing_nodes']) & set(kwargs)):
         return orig(bundler, repo, source, **kwargs)
 
     if kwargs.get('obsmarkers', False):
         heads = kwargs.get('heads')
         if r'evo_obscommon' in kwargs:
             if heads is None:
                 heads = repo.heads()
             obscommon = kwargs.get('evo_obscommon', ())
-            assert obscommon
-            obsset = repo.unfiltered().set(b'::%ln - ::%ln', heads, obscommon)
+            if obscommon:
+                obsset = repo.unfiltered().set(b'::%ln - ::%ln', heads, obscommon)
+            else:
+                obsset = repo.unfiltered().set(b'::%ln', heads)
             subset = [c.node() for c in obsset]
         else:
             common = kwargs.get('common')
             subset = [c.node() for c in repo.unfiltered().set(b'only(%ln, %ln)', heads, common)]
             subset += kwargs['evo_missing_nodes']
         markers = repo.obsstore.relevantmarkers(subset)
         if util.safehasattr(bundle2, 'buildobsmarkerspart'):
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/obshashtree.py` & `hg-evolve-9.3.1/hgext3rd/evolve/obshashtree.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/obshistory.py` & `hg-evolve-9.3.1/hgext3rd/evolve/obshistory.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/rewind.py` & `hg-evolve-9.3.1/hgext3rd/evolve/rewind.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
     user = unfi.ui.config(b'devel', b'user.obsmarker')
     if not user:
         user = unfi.ui.username()
     date = unfi.ui.configdate(b'devel', b'default-date')
     if date is None:
         date = compat.makedate()
     noise = b"%s\0%s\0%d\0%d" % (ctx.node(), user, date[0], date[1])
-    extra[b'__rewind-hash__'] = hashlib.sha256(noise).hexdigest()
+    extra[b'__rewind-hash__'] = hashlib.sha256(noise).hexdigest().encode('ascii')
 
     p1 = ctx.p1().node()
     p1 = rewindmap.get(p1, p1)
     p2 = ctx.p2().node()
     p2 = rewindmap.get(p2, p2)
 
     updates = []
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/rewriteutil.py` & `hg-evolve-9.3.1/hgext3rd/evolve/rewriteutil.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/safeguard.py` & `hg-evolve-9.3.1/hgext3rd/evolve/safeguard.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,41 +15,46 @@
     error,
 )
 
 from . import exthelper
 
 eh = exthelper.exthelper()
 
-# hg <= 4.8
+# hg <= 4.8 (33d30fb1e4ae)
 if b'auto-publish' not in configitems.coreitems.get(b'experimental', {}):
 
     eh.configitem(b'experimental', b'auto-publish', b'publish')
 
+    def _checkpublish(pushop):
+        repo = pushop.repo
+        ui = repo.ui
+        behavior = ui.config(b'experimental', b'auto-publish')
+        nocheck = behavior not in (b'warn', b'abort')
+        if nocheck or getattr(pushop, 'publish', False):
+            return
+        remotephases = pushop.remote.listkeys(b'phases')
+        publishing = remotephases.get(b'publishing', False)
+        if publishing:
+            if pushop.revs is None:
+                published = repo.filtered(b'served').revs(b"not public()")
+            else:
+                published = repo.revs(b"::%ln - public()", pushop.revs)
+            if published:
+                if behavior == b'warn':
+                    ui.warn(_(b'%i changesets about to be published\n')
+                            % len(published))
+                elif behavior == b'abort':
+                    msg = _(b'push would publish 1 changesets')
+                    hint = _(b"behavior controlled by "
+                             b"'experimental.auto-publish' config")
+                    raise error.Abort(msg, hint=hint)
+
     @eh.reposetup
     def setuppublishprevention(ui, repo):
 
         class noautopublishrepo(repo.__class__):
 
             def checkpush(self, pushop):
                 super(noautopublishrepo, self).checkpush(pushop)
-                behavior = self.ui.config(b'experimental', b'auto-publish')
-                nocheck = behavior not in (b'warn', b'abort')
-                if nocheck or getattr(pushop, 'publish', False):
-                    return
-                remotephases = pushop.remote.listkeys(b'phases')
-                publishing = remotephases.get(b'publishing', False)
-                if publishing:
-                    if pushop.revs is None:
-                        published = self.filtered(b'served').revs(b"not public()")
-                    else:
-                        published = self.revs(b"::%ln - public()", pushop.revs)
-                    if published:
-                        if behavior == b'warn':
-                            self.ui.warn(_(b'%i changesets about to be published\n')
-                                         % len(published))
-                        elif behavior == b'abort':
-                            msg = _(b'push would publish 1 changesets')
-                            hint = _(b"behavior controlled by "
-                                     b"'experimental.auto-publish' config")
-                            raise error.Abort(msg, hint=hint)
+                _checkpublish(pushop)
 
         repo.__class__ = noautopublishrepo
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/serveronly.py` & `hg-evolve-9.3.1/hgext3rd/evolve/serveronly.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/stablerange.py` & `hg-evolve-9.3.1/hgext3rd/evolve/stablerange.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/stablerangecache.py` & `hg-evolve-9.3.1/hgext3rd/evolve/stablerangecache.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,28 +42,28 @@
 
 LONG_WARNING_TIME = 60
 
 LONG_MESSAGE = b"""Stable range cache is taking a while to load
 
 Your repository is probably big.
 
-Stable range are used for discovery missing osbsolescence markers during
+Stable ranges are used for discovery missing obsolescence markers during
 exchange. While the algorithm we use can scale well for large repositories, the
 naive python implementation that you are using is not very efficient, the
 storage backend for that cache neither.
 
 This computation will finish in a finite amount of time, even for repositories
-with millions of revision and many merges. However It might take multiple tens
+with millions of revisions and many merges. However it might take multiple tens
 of minutes to complete in such case.
 
 In the future, better implementation of the algorithm in a more appropriate
 language than Python will make it much faster. This data should also get
 exchanged between server and clients removing recomputation needs.
 
-In the mean time, got take a break while this cache is warming.
+In the meantime, go take a break while this cache is warming.
 
 See `hg help -e evolve` for details about how to control obsmarkers discovery and
 the update of related cache.
 
 --- Sorry for the delay ---
 """
```

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/stablesort.py` & `hg-evolve-9.3.1/hgext3rd/evolve/stablesort.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/state.py` & `hg-evolve-9.3.1/hgext3rd/evolve/state.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/templatekw.py` & `hg-evolve-9.3.1/hgext3rd/evolve/templatekw.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/evolve/utility.py` & `hg-evolve-9.3.1/hgext3rd/evolve/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,17 @@
     Return (True, succ) unless split targets are split over multiple
     topological branches and user didn't choose any evolve destination,
     in which case return (False, '.')
     """
     targets = obsutil.successorssets(repo, ctx.node())[0]
     assert targets
     targetrevs = [repo[r].rev() for r in targets]
-    roots = repo.revs(b'roots(%ld)', targetrevs)
-    heads = repo.revs(b'heads(%ld)', targetrevs)
-    if len(roots) > 1 or len(heads) > 1:
-        cheader = (_(b"ancestor '%s' split over multiple topological"
+    heads = repo.revs(b'heads(%ld::%ld)', targetrevs, targetrevs)
+    if len(heads) > 1:
+        cheader = (_(b"ancestor of '%s' split over multiple topological"
                      b" branches.\nchoose an evolve destination:") %
                    evolvecand)
         selectedrev = revselectionprompt(ui, repo, list(heads), cheader)
         if selectedrev is None:
             return (False, '.')
         succ = repo[selectedrev]
     else:
```

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/README` & `hg-evolve-9.3.1/hgext3rd/topic/README`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/__init__.py` & `hg-evolve-9.3.1/hgext3rd/topic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 from mercurial import (
     bookmarks,
     changelog,
     cmdutil,
     commands,
     context,
     error,
+    exchange,
     extensions,
     hg,
     localrepo,
     lock as lockmod,
     merge,
     namespaces,
     node,
@@ -198,15 +199,15 @@
               b'stack.summary.headcount.multiple': b'yellow',
               # default color to help log output and thg
               # (first pick I could think off, update as needed
               b'log.topic': b'green_background',
               b'topic.active': b'green',
               }
 
-__version__ = b'0.18.0'
+__version__ = b'0.18.1'
 
 testedwith = b'4.6.2 4.7 4.8 4.9 5.0 5.1 5.2 5.3'
 minimumhgversion = b'4.6'
 buglink = b'https://bz.mercurial-scm.org/'
 
 if util.safehasattr(registrar, 'configitem'):
 
@@ -376,14 +377,26 @@
     if not post45template:
         templatekw.keywords[b'topic'] = topickw
         templatekw.keywords[b'topicidx'] = topicidxkw
     # Wrap workingctx extra to return the topic name
     extensions.wrapfunction(context.workingctx, '__init__', wrapinit)
     # Wrap changelog.add to drop empty topic
     extensions.wrapfunction(changelog.changelog, 'add', wrapadd)
+    # Make exchange._checkpublish handle experimental.topic.publish-bare-branch
+    if util.safehasattr(exchange, '_checkpublish'):
+        extensions.wrapfunction(exchange, '_checkpublish',
+                                flow.replacecheckpublish)
+    else:
+        # hg <= 4.8 (33d30fb1e4ae)
+        try:
+            evolve = extensions.find(b'evolve')
+            extensions.wrapfunction(evolve.safeguard, '_checkpublish',
+                                    flow.replacecheckpublish)
+        except (KeyError, AttributeError):
+            pass
 
     server.setupserver(ui)
 
 def reposetup(ui, repo):
     if not isinstance(repo, localrepo.localrepository):
         return # this can be a peer in the ssh case (puzzling)
 
@@ -397,14 +410,17 @@
 
         # attribute for other code to distinct between repo with topic and repo without
         hastopicext = True
 
         def _restrictcapabilities(self, caps):
             caps = super(topicrepo, self)._restrictcapabilities(caps)
             caps.add(b'topics')
+            if self.ui.configbool(b'experimental',
+                                  b'topic.publish-bare-branch'):
+                caps.add(b'ext-topics-publish=auto')
             return caps
 
         def commit(self, *args, **kwargs):
             configoverride = util.nullcontextmanager()
             if self.currenttopic != self[b'.'].topic():
                 # bypass the core "nothing changed" logic
                 configoverride = self.ui.configoverride({
```

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/compat.py` & `hg-evolve-9.3.1/hgext3rd/topic/compat.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/destination.py` & `hg-evolve-9.3.1/hgext3rd/topic/destination.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/discovery.py` & `hg-evolve-9.3.1/hgext3rd/topic/discovery.py`

 * *Files 11% similar despite different names*

```diff
@@ -135,26 +135,68 @@
                 return super(repocls, self).branchmap(topic=usetopic)
         repo.__class__ = repocls
         return orig(repo, proto)
     finally:
         repo.__class__ = oldrepo
 
 
+def _get_branch_name(ctx):
+    # make it easy for extension with the branch logic there
+    return ctx.branch()
+
+
+def _filter_obsolete_heads(repo, heads):
+    """filter heads to return non-obsolete ones
+
+    Given a list of heads (on the same named branch) return a new list of heads
+    where the obsolete part have been skimmed out.
+    """
+    new_heads = []
+    old_heads = heads[:]
+    while old_heads:
+        rh = old_heads.pop()
+        ctx = repo[rh]
+        current_name = _get_branch_name(ctx)
+        # run this check early to skip the evaluation of the whole branch
+        if not ctx.obsolete():
+            new_heads.append(rh)
+            continue
+
+        # Get all revs/nodes on the branch exclusive to this head
+        # (already filtered heads are "ignored"))
+        sections_revs = repo.revs(
+            b'only(%d, (%ld+%ld))', rh, old_heads, new_heads,
+        )
+        keep_revs = []
+        for r in sections_revs:
+            ctx = repo[r]
+            if ctx.obsolete():
+                continue
+            if _get_branch_name(ctx) != current_name:
+                continue
+            keep_revs.append(r)
+        for h in repo.revs(b'heads(%ld and (::%ld))', sections_revs, keep_revs):
+            new_heads.append(h)
+    new_heads.sort()
+    return new_heads
+
 # Discovery have deficiency around phases, branch can get new heads with pure
 # phases change. This happened with a changeset was allowed to be pushed
 # because it had a topic, but it later become public and create a new branch
 # head.
 #
 # Handle this by doing an extra check for new head creation server side
 def _nbheads(repo):
     data = {}
     for b in repo.branchmap().iterbranches():
         if b':' in b[0]:
             continue
-        data[b[0]] = len(b[1])
+        oldheads = [repo[n].rev() for n in b[1]]
+        newheads = _filter_obsolete_heads(repo, oldheads)
+        data[b[0]] = len(newheads)
     return data
 
 def handlecheckheads(orig, op, inpart):
     """This is used to check for new heads when publishing changeset"""
     orig(op, inpart)
     if not common.hastopicext(op.repo) or op.repo.publishing():
         return
```

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/evolvebits.py` & `hg-evolve-9.3.1/hgext3rd/topic/evolvebits.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/flow.py` & `hg-evolve-9.3.1/hgext3rd/topic/flow.py`

 * *Files 24% similar despite different names*

```diff
@@ -104,7 +104,61 @@
     if not any(opt for opt in entry[1] if opt[1] == b'publish'): # hg <= 4.9
         entry[1].append((b'', b'publish', False,
                          _(b'push the changeset as public')))
     extensions.wrapfunction(exchange.pushoperation, '__init__',
                             extendpushoperation)
     extensions.wrapfunction(exchange, '_pushdiscoveryphase', wrapphasediscovery)
     exchange.pushdiscoverymapping[b'phase'] = exchange._pushdiscoveryphase
+
+def replacecheckpublish(orig, pushop):
+    listkeys = exchange.listkeys
+    repo = pushop.repo
+    ui = repo.ui
+    behavior = ui.config(b'experimental', b'auto-publish')
+    if pushop.publish or behavior not in (b'warn', b'confirm', b'abort'):
+        return
+
+    # possible modes are:
+    #
+    # none -> nothing is published on push
+    # all  -> everything is published on push
+    # auto -> only changeset without topic are published on push
+    #
+    # Unknown mode is assumed "all" for safety.
+    #
+    # TODO: do a wider brain storming about mode names.
+
+    mode = b'all'
+    remotephases = listkeys(pushop.remote, b'phases')
+    if not remotephases.get(b'publishing', False):
+        mode = b'none'
+        for c in pushop.remote.capabilities():
+            if c.startswith(b'ext-topics-publish'):
+                mode = c.split(b'=', 1)[1]
+                break
+    if mode == b'none':
+        return
+
+    if pushop.revs is None:
+        published = repo.filtered(b'served').revs(b'not public()')
+    else:
+        published = repo.revs(b'::%ln - public()', pushop.revs)
+    if mode == b'auto':
+        published = repo.revs(b'%ld::(%ld - topic())', published, published)
+    if published:
+        if behavior == b'warn':
+            ui.warn(
+                _(b'%i changesets about to be published\n') % len(published)
+            )
+        elif behavior == b'confirm':
+            if ui.promptchoice(
+                _(b'push and publish %i changesets (yn)?$$ &Yes $$ &No')
+                % len(published)
+            ):
+                raise error.Abort(_(b'user quit'))
+        elif behavior == b'abort':
+            msg = _(b'push would publish %i changesets') % len(published)
+            hint = _(
+                b"use --publish or adjust 'experimental.auto-publish'"
+                b" config"
+            )
+            raise error.Abort(msg, hint=hint)
```

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/randomname.py` & `hg-evolve-9.3.1/hgext3rd/topic/randomname.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/revset.py` & `hg-evolve-9.3.1/hgext3rd/topic/revset.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/server.py` & `hg-evolve-9.3.1/hgext3rd/topic/server.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/stack.py` & `hg-evolve-9.3.1/hgext3rd/topic/stack.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/topic/topicmap.py` & `hg-evolve-9.3.1/hgext3rd/topic/topicmap.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/pullbundle.py` & `hg-evolve-9.3.1/hgext3rd/pullbundle.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/hgext3rd/serverminitopic.py` & `hg-evolve-9.3.1/hgext3rd/serverminitopic.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/testlib/exchange-obsmarker-util.sh` & `hg-evolve-9.3.1/tests/testlib/exchange-obsmarker-util.sh`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-amend-patch.t` & `hg-evolve-9.3.1/tests/test-amend-patch.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-amend.t` & `hg-evolve-9.3.1/tests/test-amend.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-check-commit.t` & `hg-evolve-9.3.1/tests/test-check-commit.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-corrupt.t` & `hg-evolve-9.3.1/tests/test-corrupt.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-discovery-obshashrange-cache.t` & `hg-evolve-9.3.1/tests/test-discovery-obshashrange-cache.t`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,17 @@
   > [defaults]
   > blackbox = -l 100
   > [experimental]
   > obshashrange=1
   > verbose-obsolescence-exchange=1
   > [ui]
   > logtemplate = "{rev} {node|short} {desc} {tags}\n"
-  > ssh=python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [alias]
   > debugobsolete=debugobsolete -d '0 0'
-  > [ui]
-  > ssh=$PYTHON "$RUNTESTDIR/dummyssh"
   > EOF
 
   $ hg init main
 
   $ hg -R main debugbuilddag '.+7'
 
   $ for node in `hg -R main log -T '{node}\n'`; do
```

### Comparing `hg-evolve-9.3.0/tests/test-discovery-obshashrange.t` & `hg-evolve-9.3.1/tests/test-discovery-obshashrange.t`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   >         commandfinish, debug, discovery, evoext-cache, evoext-obsdiscovery,
   >         incoming, tagscache
   > [experimental]
   > obshashrange=1
   > verbose-obsolescence-exchange=1
   > [ui]
   > logtemplate = "{rev} {node|short} {desc} {tags}\n"
-  > ssh=python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [alias]
   > debugobsolete=debugobsolete -d '0 0'
   > EOF
 
   $ getid() {
   >     hg log --hidden --template '{node}\n' --rev "$1" --config 'extensions.blackbox=!'
   > }
@@ -189,15 +189,15 @@
   $ hg commit -m foo
   $ hg debugobsolete ffffffffffffffffffffffffffffffffffffffff `getid '.'`
   1 new obsolescence markers
   $ hg push -f --debug
   could not import hgext.hgext3rd.evolve (No module named hgext3rd.evolve): trying hgext3rd.hgext3rd.evolve (?)
   could not import hgext3rd.hgext3rd.evolve (No module named hgext3rd.evolve): trying hgext3rd.evolve (?)
   pushing to ssh://user@dummy/server
-  running python "*/dummyssh" *user@dummy* *hg -R server serve --stdio* (glob)
+  running "*python*" "*/dummyssh" *user@dummy* *hg -R server serve --stdio* (glob)
   sending hello command
   sending between command
   remote: * (glob)
   remote: capabilities: _evoext_getbundle_obscommon _evoext_obshashrange_v1 batch * (glob)
   remote: 1
   sending protocaps command
   query 1; heads
@@ -320,15 +320,15 @@
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> updated evo-ext-obscache in *.???? seconds (1r, 0o) (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> commit -m foo exited 0 after *.?? seconds (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> debugobsolete ffffffffffffffffffffffffffffffffffffffff 45f8b879de922f6a6e620ba04205730335b6fc7e (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> alias 'debugobsolete' expands to 'debugobsolete -d '0 0'' (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> updated evo-ext-obscache in *.???? seconds (0r, 1o) (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> debugobsolete ffffffffffffffffffffffffffffffffffffffff 45f8b879de922f6a6e620ba04205730335b6fc7e exited 0 after *.?? seconds (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> push -f --debug (glob)
-  * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> running python "*/dummyssh" *user@dummy* *hg -R server serve --stdio* (glob)
+  * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> running "*python*" "*/dummyssh" *user@dummy* *hg -R server serve --stdio* (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> sending hello command (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> sending between command (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> remote: * (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> remote: capabilities: _evoext_getbundle_obscommon _evoext_obshashrange_v1 batch branchmap bundle2=HG20%0Abookmarks%0Achangegroup%3D01%2C02%0Adigests%3Dmd5%2Csha1%2Csha512%0Aerror%3Dabort%2Cunsupportedcontent%2Cpushraced%2Cpushkey%0Ahgtagsfnodes%0Alistkeys%0Aobsmarkers%3DV0%2CV1%0Aphases%3Dheads%0Apushkey%0Aremote-changegroup%3Dhttp%2Chttps%0Arev-branch-cache%0Astream%3Dv2 changegroupsubset getbundle known lookup protocaps pushkey streamreqs=generaldelta,revlogv1,sparserevlog unbundle=HG10GZ,HG10BZ,HG10UN unbundlehash (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> remote: 1 (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> sending protocaps command (glob)
   * @45f8b879de922f6a6e620ba04205730335b6fc7e (*)> query 1; heads (glob)
```

### Comparing `hg-evolve-9.3.0/tests/test-drop.t` & `hg-evolve-9.3.1/tests/test-drop.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-abort-orphan.t` & `hg-evolve-9.3.1/tests/test-evolve-abort-orphan.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-abort-phasediv.t` & `hg-evolve-9.3.1/tests/test-evolve-abort-phasediv.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-basic.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-basic.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-corner-cases.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-corner-cases.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-first-changeset.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-first-changeset.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-interrupted.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-interrupted.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-meta.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-meta.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-relocation.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-relocation.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-content-divergent-stack.t` & `hg-evolve-9.3.1/tests/test-evolve-content-divergent-stack.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-continue.t` & `hg-evolve-9.3.1/tests/test-evolve-continue.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-cycles.t` & `hg-evolve-9.3.1/tests/test-evolve-cycles.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-effectflags.t` & `hg-evolve-9.3.1/tests/test-evolve-effectflags.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-interrupted.t` & `hg-evolve-9.3.1/tests/test-evolve-interrupted.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue5832.t` & `hg-evolve-9.3.1/tests/test-evolve-issue5832.t`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
   $ hg evolve --any --all --config ui.interactive=True <<EOF
   > 1
   > EOF
   move:[2] added b
   atop:[5] added a
   move:[4] merge commit
-  ancestor '7235ef625ea3' split over multiple topological branches.
+  ancestor of '7235ef625ea3' split over multiple topological branches.
   choose an evolve destination:
   1: [62fb70414f99] added c
   2: [5841d7cf9893] added d
   q: quit the prompt
   enter the index of the revision you want to select: 1
   move:[9] merge commit
   atop:[6] added c
@@ -253,15 +253,15 @@
 
   $ hg evolve --any --all --config ui.interactive=True <<EOF
   > 2
   > EOF
   move:[2] added b
   atop:[6] added a
   move:[4] merge commit
-  ancestor 'cdf2ea1b9312' split over multiple topological branches.
+  ancestor of 'cdf2ea1b9312' split over multiple topological branches.
   choose an evolve destination:
   1: [62fb70414f99] added c
   2: [5841d7cf9893] added d
   q: quit the prompt
   enter the index of the revision you want to select: 2
   move:[10] merge commit
   atop:[8] added d
@@ -398,15 +398,15 @@
   could not solve instability, ambiguous destination: parent split across two branches
 
   $ hg evolve --any --all --config ui.interactive=True <<EOF
   > 2
   > EOF
   move:[2] added b
   atop:[6] added a
-  ancestor 'b9b387427a53' split over multiple topological branches.
+  ancestor of 'b9b387427a53' split over multiple topological branches.
   choose an evolve destination:
   1: [62fb70414f99] added c
   2: [5841d7cf9893] added d
   q: quit the prompt
   enter the index of the revision you want to select: 2
   move:[4] merge commit
   atop:[8] added d
```

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue5881.t` & `hg-evolve-9.3.1/tests/test-evolve-issue5881.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue5958.t` & `hg-evolve-9.3.1/tests/test-evolve-issue5958.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue5966.t` & `hg-evolve-9.3.1/tests/test-evolve-issue5966.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue5967.t` & `hg-evolve-9.3.1/tests/test-evolve-issue5967.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-issue6097.t` & `hg-evolve-9.3.1/tests/test-evolve-issue6097.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-list.t` & `hg-evolve-9.3.1/tests/test-evolve-list.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-noupdate.t` & `hg-evolve-9.3.1/tests/test-evolve-noupdate.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-amend-then-fold.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-amend-then-fold.t`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
   |    summary:     A0
   |
   o  changeset:   0:ea207398892e
      user:        test
      date:        Thu Jan 01 00:00:00 1970 +0000
      summary:     ROOT
   
- Actual test
- -----------
+Actual test
+-----------
 
 Check that debugobshistory on head show a coherent graph
   $ hg obslog eb5a0daa2192 --patch
   @    eb5a0daa2192 (4) C0
   |\
   x |  471f378eab4c (1) A0
    /     folded(description, content) as eb5a0daa2192 using fold by test (Thu Jan 01 00:00:00 1970 +0000)
```

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-amend.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-amend.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-complex.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-complex.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-content-divergent.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-content-divergent.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-fold.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-fold.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-lots-of-splits.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-lots-of-splits.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-phase-divergent.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-phase-divergent.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-prune.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-prune.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory-split.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory-split.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-obshistory.t` & `hg-evolve-9.3.1/tests/test-evolve-obshistory.t`

 * *Files 1% similar despite different names*

```diff
@@ -86,16 +86,16 @@
   |    summary:     A0
   |
   o  changeset:   0:ea207398892e
      user:        test
      date:        Thu Jan 01 00:00:00 1970 +0000
      summary:     ROOT
   
- Actual test
- -----------
+Actual test
+-----------
 
   $ hg obslog 7a230b46bf61 --patch
   @  7a230b46bf61 (3) A2
   |
   x  fdf9bde5129a (2) A1
   |    reworded(description) as 7a230b46bf61 using amend by test (Thu Jan 01 00:00:00 1970 +0000)
   |      diff -r fdf9bde5129a -r 7a230b46bf61 changeset-description
```

### Comparing `hg-evolve-9.3.0/tests/test-evolve-order.t` & `hg-evolve-9.3.1/tests/test-evolve-order.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-orphan-corner-cases.t` & `hg-evolve-9.3.1/tests/test-evolve-orphan-corner-cases.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-orphan-merge.t` & `hg-evolve-9.3.1/tests/test-evolve-orphan-merge.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-orphan-split.t` & `hg-evolve-9.3.1/tests/test-evolve-orphan-split.t`

 * *Files 2% similar despite different names*

```diff
@@ -189,28 +189,28 @@
   |/    () draft
   o  0:8fa14d15e168 added hgignore
       () draft
 
   $ hg evolve --dry-run <<EOF
   > 1
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: 1
   move:[7] added d
   atop:[8] added a b c
   hg rebase -r d48a30875f01 -d f2632392aefe
 
   $ hg evolve --dry-run <<EOF
   > 2
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: 2
   move:[7] added d
   atop:[10] added a b c
@@ -218,64 +218,64 @@
 
 Testing the interactive prompt with invalid values first
 (this should move its own test file when we use it at multiple places)
 
   $ hg evolve --all <<EOF
   > foo
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: foo
   invalid value 'foo' entered for index
   could not solve instability, ambiguous destination: parent split across two branches
 
   $ hg evolve --all <<EOF
   > 4
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: 4
   invalid value '4' entered for index
   could not solve instability, ambiguous destination: parent split across two branches
 
   $ hg evolve --all <<EOF
   > -1
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: -1
   invalid value '-1' entered for index
   could not solve instability, ambiguous destination: parent split across two branches
 
   $ hg evolve --all <<EOF
   > q
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: q
   could not solve instability, ambiguous destination: parent split across two branches
 
 Doing the evolve with the interactive prompt
 
   $ hg evolve --all <<EOF
   > 1
   > EOF
-  ancestor 'd48a30875f01' split over multiple topological branches.
+  ancestor of 'd48a30875f01' split over multiple topological branches.
   choose an evolve destination:
   1: [f2632392aefe] added a b c
   2: [7f87764e5b64] added a b c
   q: quit the prompt
   enter the index of the revision you want to select: 1
   move:[7] added d
   atop:[8] added a b c
```

### Comparing `hg-evolve-9.3.0/tests/test-evolve-phase-divergence.t` & `hg-evolve-9.3.1/tests/test-evolve-phase-divergence.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-phase.t` & `hg-evolve-9.3.1/tests/test-evolve-phase.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-progress.t` & `hg-evolve-9.3.1/tests/test-evolve-progress.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-corner-cases.t` & `hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-corner-cases.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-discard.t` & `hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-discard.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-public-content-divergent-main.t` & `hg-evolve-9.3.1/tests/test-evolve-public-content-divergent-main.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-serveronly-bundle2.t` & `hg-evolve-9.3.1/tests/test-evolve-serveronly-bundle2.t`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   $ cat >> $HGRCPATH <<EOF
   > [defaults]
   > amend=-d "0 0"
   > [web]
   > push_ssl = false
   > allow_push = *
   > [ui]
-  > ssh=python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [phases]
   > publish = False
   > [experimental]
   > bundle2-exp=True
   > EOF
 
   $ mkcommit() {
```

### Comparing `hg-evolve-9.3.0/tests/test-evolve-serveronly-legacy.t` & `hg-evolve-9.3.1/tests/test-evolve-serveronly-legacy.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-stop-orphan.t` & `hg-evolve-9.3.1/tests/test-evolve-stop-orphan.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-stop-phasediv.t` & `hg-evolve-9.3.1/tests/test-evolve-stop-phasediv.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-templates.t` & `hg-evolve-9.3.1/tests/test-evolve-templates.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve-topic.t` & `hg-evolve-9.3.1/tests/test-evolve-topic.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-evolve.t` & `hg-evolve-9.3.1/tests/test-evolve.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A1.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A2.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A3.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A4.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A5.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A5.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A6.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A6.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-A7.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-A7.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B1.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B2.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B3.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B4.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B5.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B5.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B6.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B6.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-B7.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-B7.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C1.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C2.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C3.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-C4.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-C4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D1.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D2.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D3.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-exchange-obsmarkers-case-D4.t` & `hg-evolve-9.3.1/tests/test-exchange-obsmarkers-case-D4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-extension-isolation.t` & `hg-evolve-9.3.1/tests/test-extension-isolation.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-fold.t` & `hg-evolve-9.3.1/tests/test-fold.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-import.t` & `hg-evolve-9.3.1/tests/test-import.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-issue-5720.t` & `hg-evolve-9.3.1/tests/test-issue-5720.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-issue-6028.t` & `hg-evolve-9.3.1/tests/test-issue-6028.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-metaedit.t` & `hg-evolve-9.3.1/tests/test-metaedit.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-minitopic.t` & `hg-evolve-9.3.1/tests/test-minitopic.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-obsconvert.t` & `hg-evolve-9.3.1/tests/test-obsconvert.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-obsolete-push.t` & `hg-evolve-9.3.1/tests/test-obsolete-push.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-obsolete.t` & `hg-evolve-9.3.1/tests/test-obsolete.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-oldconvert.t` & `hg-evolve-9.3.1/tests/test-oldconvert.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-options.t` & `hg-evolve-9.3.1/tests/test-options.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-pick.t` & `hg-evolve-9.3.1/tests/test-pick.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-prev-next.t` & `hg-evolve-9.3.1/tests/test-prev-next.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-prune.t` & `hg-evolve-9.3.1/tests/test-prune.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-pullbundle.t` & `hg-evolve-9.3.1/tests/test-pullbundle.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-partial-C1.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-partial-C1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-partial-C2.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-partial-C2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-partial-C3.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-partial-C3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-partial-C4.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-partial-C4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B1.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B2.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B3.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B4.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B5.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B5.t`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 ..
 .. expected-result:
 ..
 .. * push allowed
 ..
 .. graph-summary:
 ..
-..   B ⊗
+..   C ⊗
 ..     |
-..   A ø⇠◔ A'
+..   B ø⇠◔ B'
 ..     | |
-..   B ⊗ |
+..   A ⊗ |
 ..     |/
 ..     ●
 
   $ . $TESTDIR/testlib/push-checkheads-util.sh
 
 Test setup
 ----------
```

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B6.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B6.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B7.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B7.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-pruned-B8.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-pruned-B8.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A1.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A2.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A3.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A4.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A5.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A5.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A6.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A6.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A7.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A7.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-superceed-A8.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-superceed-A8.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D1.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D1.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D2.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D2.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D3.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D3.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D4.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D4.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D5.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D5.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D6.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D6.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-push-checkheads-unpushed-D7.t` & `hg-evolve-9.3.1/tests/test-push-checkheads-unpushed-D7.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-rewind.t` & `hg-evolve-9.3.1/tests/test-rewind.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-sharing.t` & `hg-evolve-9.3.1/tests/test-sharing.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-split.t` & `hg-evolve-9.3.1/tests/test-split.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stabilize-conflict.t` & `hg-evolve-9.3.1/tests/test-stabilize-conflict.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stabilize-order.t` & `hg-evolve-9.3.1/tests/test-stabilize-order.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablerange-branchpoint.t` & `hg-evolve-9.3.1/tests/test-stablerange-branchpoint.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablerange.t` & `hg-evolve-9.3.1/tests/test-stablerange.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablesort-branchpoint-criss-cross.t` & `hg-evolve-9.3.1/tests/test-stablesort-branchpoint-criss-cross.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablesort-branchpoint.t` & `hg-evolve-9.3.1/tests/test-stablesort-branchpoint.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablesort-criss-cross.t` & `hg-evolve-9.3.1/tests/test-stablesort-criss-cross.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stablesort.t` & `hg-evolve-9.3.1/tests/test-stablesort.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-stack-branch.t` & `hg-evolve-9.3.1/tests/test-stack-branch.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-change.t` & `hg-evolve-9.3.1/tests/test-topic-change.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-debugcb.t` & `hg-evolve-9.3.1/tests/test-topic-debugcb.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-dest.t` & `hg-evolve-9.3.1/tests/test-topic-dest.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-flow-publish-bare.t` & `hg-evolve-9.3.1/tests/test-topic-flow-publish-bare.t`

 * *Files 4% similar despite different names*

```diff
@@ -317,7 +317,47 @@
   
   $ hg phase --public -r 8 --config experimental.topic.allow-publish=no
   abort: rejecting publishing of changeset 858be9a8daaf
   [255]
   $ hg phase --public -r 10 --config experimental.topic.allow-publish=no
   abort: rejecting publishing of changeset 858be9a8daaf and 1 others
   [255]
+
+Checking the option to prevent automatic publishing
+===================================================
+
+  $ hg up branchA
+  2 files updated, 0 files merged, 5 files removed, 0 files unresolved
+
+Trying to push changeset without topic (would publish them)
+
+  $ mkcommit c_aM0
+  $ hg debugcapabilities $TESTTMP/bare-branch-server | grep topics
+    ext-topics-publish=auto
+    topics
+  $ hg push --config experimental.auto-publish=abort -r .
+  pushing to $TESTTMP/bare-branch-server
+  abort: push would publish 1 changesets
+  (use --publish or adjust 'experimental.auto-publish' config)
+  [255]
+  $ hg push --config experimental.auto-publish=abort -r . --publish
+  pushing to $TESTTMP/bare-branch-server
+  searching for changes
+  adding changesets
+  adding manifests
+  adding file changes
+  added 1 changesets with 1 changes to 1 files
+
+Pushing a changeset with topic (not publishing, no warning)
+
+  $ hg topic test-push-protection
+  marked working directory as topic: test-push-protection
+  $ mkcommit c_aL0
+  active topic 'test-push-protection' grew its first changeset
+  (see 'hg help topics' for more information)
+  $ hg push --config experimental.auto-publish=abort -r .
+  pushing to $TESTTMP/bare-branch-server
+  searching for changes
+  adding changesets
+  adding manifests
+  adding file changes
+  added 1 changesets with 1 changes to 1 files
```

### Comparing `hg-evolve-9.3.0/tests/test-topic-flow-publish-flag.t` & `hg-evolve-9.3.1/tests/test-topic-flow-publish-flag.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-flow-reject-untopiced.t` & `hg-evolve-9.3.1/tests/test-topic-flow-reject-untopiced.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-flow-single-head.t` & `hg-evolve-9.3.1/tests/test-topic-flow-single-head.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-fold.t` & `hg-evolve-9.3.1/tests/test-topic-fold.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-mode.t` & `hg-evolve-9.3.1/tests/test-topic-mode.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-multiple.t` & `hg-evolve-9.3.1/tests/test-topic-multiple.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-push-concurrent-on.t` & `hg-evolve-9.3.1/tests/test-topic-push-concurrent-on.t`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # same as test-topic-push but with the concurrent push feature on
 
   $ . "$TESTDIR/testlib/topic_setup.sh"
 
   $ cat << EOF >> $HGRCPATH
   > [ui]
   > logtemplate = {rev} {branch} {get(namespaces, "topics")} {phase} {desc|firstline}\n
-  > ssh =python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [server]
   > concurrent-push-mode=check-related
   > EOF
 
   $ hg init main
   $ hg init draft
   $ cat << EOF >> draft/.hg/hgrc
```

### Comparing `hg-evolve-9.3.0/tests/test-topic-push.t` & `hg-evolve-9.3.1/tests/test-topic-push.t`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
   $ . "$TESTDIR/testlib/topic_setup.sh"
 
   $ cat << EOF >> $HGRCPATH
   > [ui]
   > logtemplate = {rev} {branch} {get(namespaces, "topics")} {phase} {desc|firstline}\n
-  > ssh =python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > EOF
 
   $ hg init main
   $ hg init draft
   $ cat << EOF >> draft/.hg/hgrc
   > [phases]
   > publish=False
```

### Comparing `hg-evolve-9.3.0/tests/test-topic-rebase.t` & `hg-evolve-9.3.1/tests/test-topic-rebase.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-server.t` & `hg-evolve-9.3.1/tests/test-topic-server.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-shelve.t` & `hg-evolve-9.3.1/tests/test-topic-shelve.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-stack-complex.t` & `hg-evolve-9.3.1/tests/test-topic-stack-complex.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-stack-data.t` & `hg-evolve-9.3.1/tests/test-topic-stack-data.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-stack.t` & `hg-evolve-9.3.1/tests/test-topic-stack.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic-tutorial.t` & `hg-evolve-9.3.1/tests/test-topic-tutorial.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-topic.t` & `hg-evolve-9.3.1/tests/test-topic.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-touch.t` & `hg-evolve-9.3.1/tests/test-touch.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-tutorial.t` & `hg-evolve-9.3.1/tests/test-tutorial.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-uncommit-interactive.t` & `hg-evolve-9.3.1/tests/test-uncommit-interactive.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-uncommit.t` & `hg-evolve-9.3.1/tests/test-uncommit.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-unstability-resolution-result.t` & `hg-evolve-9.3.1/tests/test-unstability-resolution-result.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-unstable-orphan.t` & `hg-evolve-9.3.1/tests/test-unstable-orphan.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-userguide.t` & `hg-evolve-9.3.1/tests/test-userguide.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-version-install.t` & `hg-evolve-9.3.1/tests/test-version-install.t`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/tests/test-wireproto-bundle1.t` & `hg-evolve-9.3.1/tests/test-wireproto-bundle1.t`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
   $ cat >> $HGRCPATH <<EOF
   > [defaults]
   > amend=-d "0 0"
   > [ui]
-  > ssh=python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [phases]
   > publish = False
   > [extensions]
   > EOF
   $ echo "evolve=$(echo $(dirname $TESTDIR))/hgext3rd/evolve/" >> $HGRCPATH
 
   $ mkcommit() {
```

### Comparing `hg-evolve-9.3.0/tests/test-wireproto.t` & `hg-evolve-9.3.1/tests/test-wireproto.t`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   $ cat >> $HGRCPATH <<EOF
   > [defaults]
   > amend=-d "0 0"
   > [experimental]
   > obsmarkers-exchange-debug=true
   > bundle2-exp=true
   > [ui]
-  > ssh=python "$RUNTESTDIR/dummyssh"
+  > ssh = "$PYTHON" "$RUNTESTDIR/dummyssh"
   > [phases]
   > publish = False
   > [extensions]
   > EOF
   $ echo "evolve=$(echo $(dirname $TESTDIR))/hgext3rd/evolve/" >> $HGRCPATH
 
   $ mkcommit() {
```

### Comparing `hg-evolve-9.3.0/CHANGELOG` & `hg-evolve-9.3.1/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changelog
 =========
 
+9.3.1 -- 2020-04-08
+-------------------
+
+  * compat: make __touch-noise__ and __rewind-hash__ extra field be bytes
+
+  * obsexchange: avoid sending too large request to http server
+  * obsdiscovery: server no longer aborts with a 500 error if client sends a
+    request without obscommon
+  * obsdiscovery: avoid considering locally hidden changeset
+  * single-heads: ignore obsolete section when enforcing one head per branch
+
+  * evolve: improved behavior when evolving above the result of a split
+  * evolve: checking for new head on push is no longer confused by mixed
+    branches (or topics)
+
+topic (0.18.1)
+
+  * topic: fix auto-publish=abort with server that auto-publishes bare branches
+
 9.3.0 -- 2020-03-04
 -------------------
 
   * compat: compatibility with Mercurial 5.3
   * compat: drop compatibility with Mercurial 4.5
   * compat: cleanup old compatibility code for Mercurial < 4.5
```

### Comparing `hg-evolve-9.3.0/COPYING` & `hg-evolve-9.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/MANIFEST.in` & `hg-evolve-9.3.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/README` & `hg-evolve-9.3.1/README`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/setup.cfg` & `hg-evolve-9.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/setup.py` & `hg-evolve-9.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `hg-evolve-9.3.0/PKG-INFO` & `hg-evolve-9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: hg-evolve
-Version: 9.3.0
+Version: 9.3.1
 Summary: Flexible evolution of Mercurial history.
 Home-page: https://www.mercurial-scm.org/doc/evolution/
 Author: Pierre-Yves David
 Author-email: pierre-yves.david@ens-lyon.org
 License: GPLv2+
 Description: =============================
         Mutable History For Mercurial
```

