# Comparing `tmp/safeeyes-2.1.5.tar.gz` & `tmp/safeeyes-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeeyes-2.1.5.tar", last modified: Fri Jan  6 00:19:47 2023, max compression
+gzip compressed data, was "safeeyes-2.1.6.tar", last modified: Wed Jul  5 00:12:06 2023, max compression
```

## Comparing `safeeyes-2.1.5.tar` & `safeeyes-2.1.6.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.639541 safeeyes-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-01-06 00:19:37.000000 safeeyes-2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-06 00:19:37.000000 safeeyes-2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-01-06 00:19:47.635542 safeeyes-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-01-06 00:19:37.000000 safeeyes-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5999 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.603542 safeeyes-2.1.5/safeeyes/config/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ar/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/bg/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ca/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/cs/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/da/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/da/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/de/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/en_US/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/en_US/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/en_US/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/eo/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/es/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/et/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/et/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/eu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/eu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/eu/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.607542 safeeyes-2.1.5/safeeyes/config/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/fa/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/fr/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/he/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/hi/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/hu/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/hu/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/id/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/config/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/it/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/kn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/kn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/kn/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.611542 safeeyes-2.1.5/safeeyes/config/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ko/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/lt/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/lv/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/mk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/mk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/mk/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/mr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/mr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/mr/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/nb/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/nl/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/pl/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/pt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/pt/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/pt_BR/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ru/LC_MESSAGES/safeeyes.po
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/safeeyes.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.615542 safeeyes-2.1.5/safeeyes/config/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/sk/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/sr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/sr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/sr/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/sv/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12041 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/sv/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/ta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/ta/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ta/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/tr/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/ug/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/ug/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/ug/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/uk/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/uz_Latn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/uz_Latn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/uz_Latn/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/vi/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/zh_CN/LC_MESSAGES/safeeyes.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/config/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/locale/zh_TW/LC_MESSAGES/safeeyes.po
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/safeeyes.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/config/style/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/config/style/safeeyes_style.css
--rw-r--r--   0 runner    (1001) docker     (123)    11198 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/glade/
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/about_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/break_screen.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/item_bool.glade
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/item_break.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/item_int.glade
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/item_plugin.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/item_text.glade
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/new_break.glade
--rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/settings_break.glade
--rw-r--r--   0 runner    (1001) docker     (123)    70106 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/settings_dialog.glade
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/glade/settings_plugin.glade
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/platform/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.623542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.619542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/128x128/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/128x128/apps/
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/128x128/apps/safeeyes.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.623542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/apps/safeeyes.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_enabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_timer.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.623542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/apps/safeeyes.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_enabled.png
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_timer.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.623542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.631542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/apps/safeeyes.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/status/safeeyes_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/status/safeeyes_enabled.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.623542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/apps/safeeyes.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/status/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/status/safeeyes_disabled.png
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/status/safeeyes_enabled.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/64x64/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/64x64/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/icons/hicolor/64x64/apps/safeeyes.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/platform/safeeyes.desktop
--rw-r--r--   0 runner    (1001) docker     (123)    14444 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/audiblealert/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/audiblealert/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/audiblealert/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/audiblealert/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/donotdisturb/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/donotdisturb/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/donotdisturb/dependency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/donotdisturb/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/donotdisturb/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/healthstats/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/healthstats/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/healthstats/dependency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/healthstats/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/healthstats/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/mediacontrol/resource/pause.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/notification/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/notification/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/notification/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/screensaver/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/screensaver/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/screensaver/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/screensaver/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/screensaver/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/screensaver/resource/lock.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/smartpause/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/smartpause/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/smartpause/dependency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/smartpause/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/smartpause/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/plugins/trayicon/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/trayicon/config.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/trayicon/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    15933 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/plugins/trayicon/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/resource/ic_plugin.png
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/resource/ic_warning.png
--rw-r--r--   0 runner    (1001) docker     (123)    96082 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/resource/on_pre_break.wav
--rw-r--r--   0 runner    (1001) docker     (123)    66194 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/resource/on_stop_break.wav
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/rpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/safeeyes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.635542 safeeyes-2.1.5/safeeyes/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/ui/about_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/ui/break_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/ui/settings_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-01-06 00:19:37.000000 safeeyes-2.1.5/safeeyes/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 00:19:47.627542 safeeyes-2.1.5/safeeyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-06 00:19:47.000000 safeeyes-2.1.5/safeeyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 00:19:47.639541 safeeyes-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-01-06 00:19:37.000000 safeeyes-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35145 2023-07-05 00:11:48.000000 safeeyes-2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 00:11:48.000000 safeeyes-2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-05 00:12:06.378126 safeeyes-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-05 00:11:48.000000 safeeyes-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5999 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/config/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/config/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/config/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14253 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ar/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/bg/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ca/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/cs/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/da/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/da/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/de/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/en_US/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/en_US/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/en_US/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/eo/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/es/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/et/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/et/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/eu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/eu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/eu/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    14360 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/fa/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/fr/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13310 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/he/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.354126 safeeyes-2.1.6/safeeyes/config/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11547 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/hi/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/hu/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11228 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/hu/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/id/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/it/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/kn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/kn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/kn/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ko/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12581 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/lt/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/lv/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/mk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/mk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/mk/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/mr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/mr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/mr/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/nb/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12355 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/nl/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/pl/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.366126 safeeyes-2.1.6/safeeyes/config/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/pt/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12470 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/pt_BR/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ru/LC_MESSAGES/safeeyes.po
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/safeeyes.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/sk/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/sr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/sr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/sr/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/sv/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/sv/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/ta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/ta/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ta/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/tr/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/ug/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/ug/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/ug/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/uk/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/uz_Latn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/uz_Latn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/uz_Latn/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/vi/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11476 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/zh_CN/LC_MESSAGES/safeeyes.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/config/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/locale/zh_TW/LC_MESSAGES/safeeyes.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/safeeyes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/config/style/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/config/style/safeeyes_style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/glade/
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/about_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/break_screen.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/item_bool.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/item_break.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/item_int.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/item_plugin.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/item_text.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/new_break.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    29000 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/settings_break.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    70106 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/settings_dialog.glade
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/glade/settings_plugin.glade
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/platform/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/platform/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/128x128/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.370126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/128x128/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/128x128/apps/io.github.slgobinath.SafeEyes.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/apps/io.github.slgobinath.SafeEyes.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-enabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-timer.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/apps/io.github.slgobinath.SafeEyes.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-enabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-timer.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.358126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/apps/io.github.slgobinath.SafeEyes.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-enabled.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/apps/io.github.slgobinath.SafeEyes.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/status/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-enabled.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/64x64/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/64x64/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/icons/hicolor/64x64/apps/io.github.slgobinath.SafeEyes.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/io.github.slgobinath.SafeEyes.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/platform/io.github.slgobinath.SafeEyes.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/plugins/audiblealert/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/audiblealert/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/audiblealert/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/audiblealert/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/plugins/donotdisturb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/donotdisturb/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/donotdisturb/dependency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/donotdisturb/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/donotdisturb/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/plugins/healthstats/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/healthstats/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/healthstats/dependency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/healthstats/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/healthstats/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.374126 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/mediacontrol/resource/pause.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/notification/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/notification/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/notification/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/screensaver/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/screensaver/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/screensaver/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/screensaver/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/screensaver/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/screensaver/resource/lock.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/smartpause/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/smartpause/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/smartpause/dependency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/smartpause/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/smartpause/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/plugins/trayicon/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/trayicon/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/trayicon/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17272 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/plugins/trayicon/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/resource/ic_plugin.png
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/resource/ic_warning.png
+-rw-r--r--   0 runner    (1001) docker     (123)    96082 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/resource/on_pre_break.wav
+-rw-r--r--   0 runner    (1001) docker     (123)    66194 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/resource/on_stop_break.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/rpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/safeeyes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.378126 safeeyes-2.1.6/safeeyes/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/ui/about_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/ui/break_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/ui/settings_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22742 2023-07-05 00:11:48.000000 safeeyes-2.1.6/safeeyes/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 00:12:06.362125 safeeyes-2.1.6/safeeyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 00:12:06.000000 safeeyes-2.1.6/safeeyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 00:12:06.378126 safeeyes-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-05 00:11:48.000000 safeeyes-2.1.6/setup.py
```

### Comparing `safeeyes-2.1.5/LICENSE` & `safeeyes-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/PKG-INFO` & `safeeyes-2.1.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,14 @@
-Metadata-Version: 2.1
-Name: safeeyes
-Version: 2.1.5
-Summary: Protect your eyes from eye strain using this continuous breaks reminder.
-Home-page: https://github.com/slgobinath/SafeEyes
-Download-URL: https://github.com/slgobinath/SafeEyes/archive/v2.1.5.tar.gz
-Author: Gobinath Loganathan
-Author-email: slgobinath@gmail.com
-Keywords: linux utility health eye-strain safe-eyes
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: X11 Applications :: GTK
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Safe Eyes
 
 [![Release](https://img.shields.io/github/v/release/slgobinath/SafeEyes)](https://github.com/slgobinath/SafeEyes/releases)
 [![PyPI version](https://badge.fury.io/py/safeeyes.svg)](https://badge.fury.io/py/safeeyes)
 [![Debian](https://badges.debian.net/badges/debian/unstable/safeeyes/version.svg)](https://packages.debian.org/unstable/safeeyes)
 [![AUR](https://img.shields.io/aur/version/safeeyes)](https://aur.archlinux.org/packages/safeeyes)
+[![Flathub](https://img.shields.io/flathub/v/io.github.slgobinath.SafeEyes)](https://flathub.org/apps/details/io.github.slgobinath.SafeEyes)
 [![Translation status](https://hosted.weblate.org/widgets/safe-eyes/-/translations/svg-badge.svg)](https://hosted.weblate.org/engage/safe-eyes/?utm_source=widget)
 [![Awesome Humane Tech](https://raw.githubusercontent.com/humanetech-community/awesome-humane-tech/main/humane-tech-badge.svg?sanitize=true)](https://github.com/humanetech-community/awesome-humane-tech)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/slgobinath)
 
 Protect your eyes from eye strain using this simple and beautiful, yet extensible break reminder.
 
 Visit the official site: https://slgobinath.github.io/SafeEyes/ for more details.
@@ -104,14 +81,20 @@
 
 ### Alpine Linux
 
 ```bash
 sudo apk add safeeyes
 ```
 
+### Flatpak
+
+```bash
+flatpak install flathub io.github.slgobinath.SafeEyes
+```
+
 ### Other Linux & Run from source
 
 Ensure to meet the following dependencies:
 
 - gir1.2-appindicator3-0.1 or gir1.2-ayatanaappindicator3-0.1
 - gir1.2-notify-0.7
 - libappindicator-gtk3
@@ -181,14 +164,30 @@
 - Command-line arguments to control the running instance
 - Customizable using plug-ins
 
 ## Third-party Plugins
 
 Thirdparty plugins are available at another GitHub repository: [safeeyes-plugins](https://github.com/slgobinath/safeeyes-plugins). More details about how to write your own plugin and how to install third-party plugin are available there.
 
+## How to Release?
+
+1. Checkout the latest commits from the `master` branch
+2. Run `python3 -m safeeyes` to make sure nothing is broken
+3. Update the Safe Eyes version in the following places (Open the project in VSCode and search for the current version):
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L81)
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L88)
+    - [safeeyes.py](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/safeeyes.py#L43)
+    - [io.github.slgobinath.SafeEyes.metainfo.xml](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/platform/io.github.slgobinath.SafeEyes.metainfo.xml#L50)
+    - [about_dialog.glade](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/glade/about_dialog.glade#L74)
+4. Update the [changelog](https://github.com/slgobinath/SafeEyes/blob/master/debian/changelog) (for Ubuntu release)
+5. Commit the changes to `master`
+6. Create a pull-request from `master` to `release`
+7. Merge the PR to release **with merge commit** (Important to merge with merge commit)
+
+
 ## License
 
 GNU General Public License v3
 
 ## IDE Support
 
 <p align="center">Thanks to JetBrains for offering IDE support to develop this Open Source project.</p>
```

### Comparing `safeeyes-2.1.5/README.md` & `safeeyes-2.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,38 @@
+Metadata-Version: 2.1
+Name: safeeyes
+Version: 2.1.6
+Summary: Protect your eyes from eye strain using this continuous breaks reminder.
+Home-page: https://github.com/slgobinath/SafeEyes
+Download-URL: https://github.com/slgobinath/SafeEyes/archive/v2.1.6.tar.gz
+Author: Gobinath Loganathan
+Author-email: slgobinath@gmail.com
+Keywords: linux utility health eye-strain safe-eyes
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: X11 Applications :: GTK
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Safe Eyes
 
 [![Release](https://img.shields.io/github/v/release/slgobinath/SafeEyes)](https://github.com/slgobinath/SafeEyes/releases)
 [![PyPI version](https://badge.fury.io/py/safeeyes.svg)](https://badge.fury.io/py/safeeyes)
 [![Debian](https://badges.debian.net/badges/debian/unstable/safeeyes/version.svg)](https://packages.debian.org/unstable/safeeyes)
 [![AUR](https://img.shields.io/aur/version/safeeyes)](https://aur.archlinux.org/packages/safeeyes)
+[![Flathub](https://img.shields.io/flathub/v/io.github.slgobinath.SafeEyes)](https://flathub.org/apps/details/io.github.slgobinath.SafeEyes)
 [![Translation status](https://hosted.weblate.org/widgets/safe-eyes/-/translations/svg-badge.svg)](https://hosted.weblate.org/engage/safe-eyes/?utm_source=widget)
 [![Awesome Humane Tech](https://raw.githubusercontent.com/humanetech-community/awesome-humane-tech/main/humane-tech-badge.svg?sanitize=true)](https://github.com/humanetech-community/awesome-humane-tech)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/slgobinath)
 
 Protect your eyes from eye strain using this simple and beautiful, yet extensible break reminder.
 
 Visit the official site: https://slgobinath.github.io/SafeEyes/ for more details.
@@ -80,14 +105,20 @@
 
 ### Alpine Linux
 
 ```bash
 sudo apk add safeeyes
 ```
 
+### Flatpak
+
+```bash
+flatpak install flathub io.github.slgobinath.SafeEyes
+```
+
 ### Other Linux & Run from source
 
 Ensure to meet the following dependencies:
 
 - gir1.2-appindicator3-0.1 or gir1.2-ayatanaappindicator3-0.1
 - gir1.2-notify-0.7
 - libappindicator-gtk3
@@ -157,14 +188,30 @@
 - Command-line arguments to control the running instance
 - Customizable using plug-ins
 
 ## Third-party Plugins
 
 Thirdparty plugins are available at another GitHub repository: [safeeyes-plugins](https://github.com/slgobinath/safeeyes-plugins). More details about how to write your own plugin and how to install third-party plugin are available there.
 
+## How to Release?
+
+1. Checkout the latest commits from the `master` branch
+2. Run `python3 -m safeeyes` to make sure nothing is broken
+3. Update the Safe Eyes version in the following places (Open the project in VSCode and search for the current version):
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L81)
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L88)
+    - [safeeyes.py](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/safeeyes.py#L43)
+    - [io.github.slgobinath.SafeEyes.metainfo.xml](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/platform/io.github.slgobinath.SafeEyes.metainfo.xml#L50)
+    - [about_dialog.glade](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/glade/about_dialog.glade#L74)
+4. Update the [changelog](https://github.com/slgobinath/SafeEyes/blob/master/debian/changelog) (for Ubuntu release)
+5. Commit the changes to `master`
+6. Create a pull-request from `master` to `release`
+7. Merge the PR to release **with merge commit** (Important to merge with merge commit)
+
+
 ## License
 
 GNU General Public License v3
 
 ## IDE Support
 
 <p align="center">Thanks to JetBrains for offering IDE support to develop this Open Source project.</p>
```

### Comparing `safeeyes-2.1.5/safeeyes/__main__.py` & `safeeyes-2.1.6/safeeyes/__main__.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ar/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ar/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/bg/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/bg/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ca/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ca/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/cs/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/cs/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/da/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/da/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/de/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/de/LC_MESSAGES/safeeyes.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) 2017 Gobinath
 # Gobinath slgobinath@gmail.com, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: \n"
-"PO-Revision-Date: 2021-03-07 09:50+0000\n"
-"Last-Translator: J. Lavoie <j.lavoie@net-c.ca>\n"
+"PO-Revision-Date: 2023-07-04 20:53+0000\n"
+"Last-Translator: Sebastian Pipping <sebastian@pipping.org>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/safe-eyes/"
 "translations/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.5.1\n"
+"X-Generator: Weblate 5.0-dev\n"
 
 # Short break
 msgid "Tightly close your eyes"
 msgstr "Augen fest schließen"
 
 # Short break
 msgid "Roll your eyes a few times to each side"
@@ -98,15 +98,18 @@
 msgstr "Schließen"
 
 # Description in about dialog
 # Safe Eyes protects your eyes from eye strain (asthenopia) by reminding you to take breaks while you're working long hours at the computer
 msgid ""
 "Safe Eyes protects your eyes from eye strain (asthenopia) by reminding you "
 "to take breaks while you're working long hours at the computer"
-msgstr "Beschreibung"
+msgstr ""
+"Safe Eyes schützt Ihre Augen vor Beschwerden (Asthenopie), indem es Sie "
+"regelmäßig erinnert, Pausen zu machen, wenn Sie längere Zeit am Bildschirm "
+"verbringen"
 
 # About dialog
 msgid "License"
 msgstr "Lizenz"
 
 # Break screen
 msgid "Skip"
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/en_US/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/en_US/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/eo/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/eo/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/es/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/es/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/et/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/et/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/eu/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/eu/LC_MESSAGES/safeeyes.po`

 * *Files 9% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 # Copyright (C) 2017 Gobinath
 # Gobinath slgobinath@gmail.com, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: \n"
-"PO-Revision-Date: 2022-09-28 22:17+0000\n"
-"Last-Translator: Gontzal Manuel Pujana Onaindia <thadahdenyse@gmail.com>\n"
+"PO-Revision-Date: 2023-01-07 11:49+0000\n"
+"Last-Translator: Porrumentzio <porrumentzio@riseup.net>\n"
 "Language-Team: Basque <https://hosted.weblate.org/projects/safe-eyes/"
 "translations/eu/>\n"
 "Language: eu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 4.15.1-dev\n"
 
 # Short break
 msgid "Tightly close your eyes"
 msgstr "Itxi begiak indarrez"
 
 # Short break
 msgid "Roll your eyes a few times to each side"
-msgstr "Mugitu begiak alde bakoitzera pare bat aldiz"
+msgstr "Mugitu begiak aldez alde"
 
 # Short break
 msgid "Rotate your eyes in clockwise direction"
-msgstr "Biratu begiak erlojuaren noranzkoan"
+msgstr "Biratu begiak erloju-orratzen noranzkoan"
 
 # Short break
 msgid "Rotate your eyes in counterclockwise direction"
-msgstr "Biratu begiak erlojuaren aurkako noranzkoan"
+msgstr "Biratu begiak erloju-orratzen kontrako noranzkoan"
 
 # Short break
 msgid "Blink your eyes"
 msgstr "Kliskatu begiak"
 
 # Short break
 msgid "Focus on a point in the far distance"
@@ -67,15 +67,15 @@
 
 # Commandline arg description
 msgid "quit the running safeeyes instance and exit"
 msgstr "itxi uneko safeeyes instantzia eta irten"
 
 # Commandline arg description
 msgid "show the settings dialog"
-msgstr "erakutsi ezarpenen elkarrizketa-koadroa"
+msgstr "erakutsi ezarpenak"
 
 # Commandline arg description
 msgid "start safeeyes in debug mode"
 msgstr "abiarazi safeeyes arazketa moduan"
 
 # Commandline arg description
 msgid "print the status of running safeeyes instance and exit"
@@ -86,29 +86,29 @@
 msgstr "Safe Eyes ez dago martxan"
 
 # RPC not enabled message
 msgid ""
 "Safe Eyes is running without an RPC server. Turn it on to use command-line "
 "arguments."
 msgstr ""
-"Safe Eyes RPC zerbitzaririk gabe exekutatzen ari da. Piztu ezazu komando-"
-"lerroko argumentuak erabiltzeko."
+"RPC zerbitzaririk gabe ari da exekutatzen Safe Eyes. Piztu zerbitzaria "
+"komando-lerroko argumentuak erabiltzeko."
 
 # About dialog
 msgid "Close"
 msgstr "Itxi"
 
 # Description in about dialog
 # Safe Eyes protects your eyes from eye strain (asthenopia) by reminding you to take breaks while you're working long hours at the computer
 msgid ""
 "Safe Eyes protects your eyes from eye strain (asthenopia) by reminding you "
 "to take breaks while you're working long hours at the computer"
 msgstr ""
-"Safe Eyes-ek zure begiak begi-neketik (astenopia) babesten ditu "
-"ordenagailuan ordu luzez zabiltzanean atsedenaldiak hartzeaz gogoraraziz"
+"Safe Eyes-ek begi-neketik (astenopiatik) babesten zaitu ordenagailuan ordu "
+"luzez zabiltzanean etenaldiak egiteko gogoraraziz"
 
 # About dialog
 msgid "License"
 msgstr "Lizentzia"
 
 # Break screen
 msgid "Skip"
@@ -116,43 +116,43 @@
 
 # Break screen
 msgid "Postpone"
 msgstr "Atzeratu"
 
 # Settings dialog
 msgid "Break duration (in seconds)"
-msgstr "Atsedenaldiaren iraupena (segundotan)"
+msgstr "Etenaldiaren iraupena (segundotan)"
 
 # Settings dialog
 msgid "Interval between two breaks (in minutes)"
-msgstr "Bi atsedenaldien arteko tartea (minututan)"
+msgstr "Bi etenaldiren arteko tartea (minututan)"
 
 # Settings dialog
 msgid "Time to prepare for a break (in seconds)"
-msgstr "Atsedenaldirako prestatzeko denbora (segundotan)"
+msgstr "Etenaldirako prestatzeko denbora (segundotan)"
 
 # Settings dialog
 msgid "Keyboard shortcuts disabled period (in seconds)"
-msgstr "Laster-teklak desgaitutako unea (segundotan)"
+msgstr "Laster-teklak desgaitutako aldia (segundotan)"
 
 # Settings dialog
 msgid "Postponement duration (in minutes)"
 msgstr "Atzerapenaren iraupena (minututan)"
 
 # Settings dialog
 msgid "Show breaks in random order"
-msgstr "Erakutsi atsedenaldiak ausazko ordenean"
+msgstr "Erakutsi etenaldiak ausazko ordenan"
 
 # Settings dialog
 msgid "Strict break (No way to skip breaks)"
-msgstr "Atsedenaldi zorrotza (saltatzeko modurik ez)"
+msgstr "Etenaldi zorrotza (saltatzeko modurik ez)"
 
 # Settings dialog
 msgid "Allow postponing breaks"
-msgstr "Baimendu atsedenaldiak atzeratzea"
+msgstr "Baimendu etenaldiak atzeratzea"
 
 # Settings dialog
 msgid "Persist the internal state"
 msgstr "Eutsi barruko egoerari"
 
 # Settings dialog
 msgid "Use RPC server to receive runtime commands"
@@ -160,55 +160,57 @@
 
 # Settings dialog
 msgid "Without the RPC server, command-line commands may not work"
 msgstr "RPC zerbitzaririk gabe, komandu-lineako komanduek ez dute funtzionatuko"
 
 # Settings dialog
 msgid "Long break interval must be a multiple of short break interval"
-msgstr "Atsedenaldik luzeak, motzen multzoa izan behar du"
+msgstr ""
+"Etenaldi luzeen arteko tarteak motzen arteko tartearen multiploa izan behar "
+"du"
 
 # Settings dialog
 msgid "Reset"
 msgstr "Berrezarri"
 
 # Settings dialog
 msgid "Are you sure you want to reset all settings to default?"
-msgstr "Ziur ezarpen guztiak lehenetsitakoetara berrezarri nahi dituzula?"
+msgstr "Ziur ezarpen guztiak lehenetsietara berrezarri nahi dituzula?"
 
 # Settings dialog
 msgid "Options"
 msgstr "Aukerak"
 
 # Settings dialog
 msgid "Short Breaks"
-msgstr "Atsedenaldi motzak"
+msgstr "Etenaldi motzak"
 
 # Settings dialog
 msgid "Long Breaks"
-msgstr "Atsedenaldi luzeak"
+msgstr "Etenaldi luzeak"
 
 # Settings dialog
 msgid "Delete"
 msgstr "Ezabatu"
 
 # Settings dialog
 msgid "Are you sure you want to delete this break?"
-msgstr "Ziur atsedenaldi hau ezabatu nahi duzula?"
+msgstr "Ziur etenaldi hau ezabatu nahi duzula?"
 
 # Settings dialog
 msgid "You can't undo this action."
 msgstr "Ekintza hau ezin da desegin."
 
 # Settings dialog
 msgid "Break"
-msgstr "Atsedenaldia"
+msgstr "Etenaldia"
 
 # Settings dialog
 msgid "Breaks"
-msgstr "Atsedenaldiak"
+msgstr "Etenaldiak"
 
 # Settings dialog
 msgid "Plugins"
 msgstr "Gehigarriak"
 
 # Settings dialog
 msgid "Type"
@@ -252,15 +254,15 @@
 
 # Settings dialog
 msgid "Time (in minutes)"
 msgstr "Denbora (minututan)"
 
 # Settings dialog
 msgid "Break Settings"
-msgstr "Atsedenaldien ezarpenak"
+msgstr "Etenaldien ezarpenak"
 
 # Settings dialog
 msgid "Plugin Settings"
 msgstr "Gehigarriaren ezarpenak"
 
 # Settings dialog
 msgid "Plugin does not support %s desktop environment"
@@ -280,15 +282,15 @@
 
 # Settings dialog
 msgid "Please add the resource %(resource)s to %(config_resource)s directory"
 msgstr "Gehitu %(resource)s baliabidea %(config_resource)s direktorioan"
 
 # Settings dialog
 msgid "New Break"
-msgstr "Atsedenaldi berria"
+msgstr "Etenaldi berria"
 
 # Settings dialog
 msgid "Remove"
 msgstr "Kendu"
 
 # Settings dialog
 msgid "Discard"
@@ -300,35 +302,35 @@
 
 # plugin/audiblealert
 msgid "Audible Alert"
 msgstr "Abisu entzungarria"
 
 # plugin/audiblealert
 msgid "Play audible alert before and after breaks"
-msgstr "Erreproduzitu abisu entzungarria atsedenaldien aurretik eta ondoren"
+msgstr "Erreproduzitu abisu entzungarri bat etenaldien aurretik eta ondoren"
 
 # plugin/audiblealert
 msgid "Play audible alert before breaks"
-msgstr "Erreproduzitu abisu entzungarria atsedenaldien aurretik"
+msgstr "Erreproduzitu abisu entzungarria etenaldien aurretik"
 
 # plugin/audiblealert
 msgid "Play audible alert after breaks"
-msgstr "Erreproduzitu abisu entzungarria atsedenaldien ondoren"
+msgstr "Erreproduzitu abisu entzungarria etenaldien ondoren"
 
 # plugin/donotdisturb
 msgid "Do Not Disturb"
 msgstr "Ez molestatu"
 
 # plugin/donotdisturb
 msgid "Skip break if the active window is in fullscreen mode"
-msgstr "Saltatu atsedenaldia uneko leihoa pantaila osoan badago"
+msgstr "Saltatu etenaldia leiho aktiboa pantaila osoan badago"
 
 # plugin/donotdisturb
 msgid "Do not interrupt these windows anytime"
-msgstr "Ez eten honako leihoetan edonola ere"
+msgstr "Ez eten honako leihoetan inoiz ere"
 
 # plugin/donotdisturb
 msgid "Interrupt these windows regardless of their state"
 msgstr "Eten honako leihoetan haien egoerari erreparatu gabe"
 
 # plugin/donotdisturb
 msgid "Switch the interruptible windows to normal mode"
@@ -352,40 +354,40 @@
 
 # plugin/notification
 msgid "Notification"
 msgstr "Jakinarazpena"
 
 # plugin/notification
 msgid "Show a system notification before breaks"
-msgstr "Erakutsi sistemako jakinarazpena atsedenaldien aurretik"
+msgstr "Erakutsi sistemako jakinarazpen bat etenaldien aurretik"
 
 # plugin/notification
 msgid "Ready for a short break in %s seconds"
-msgstr "Prestatu %s segundo barru atsedenaldi motza egiteko"
+msgstr "Prestatu %s segundo barru etenaldi motza egiteko"
 
 # plugin/notification
 msgid "Ready for a long break in %s seconds"
-msgstr "Prestatu %s segundo barru atsedenaldi luzea egiteko"
+msgstr "Prestatu %s segundo barru etenaldi luzea egiteko"
 
 # plugin/screensaver
 msgid "Screensaver"
 msgstr "Pantaila babeslea"
 
 # plugin/screensaver
 msgid "Lock the screen after long breaks by starting screensaver"
 msgstr ""
-"Blokeatu pantaila atsedenaldi luzeen ondoren pantaila-babeslea erakutsiz"
+"Blokeatu pantaila etenaldi luzeen ondoren eta erakutsi pantaila-babeslea"
 
 # plugin/screensaver
 msgid "Custom screensaver command"
 msgstr "Pantaila-babeslearentzako komando pertsonalizatua"
 
 # plugin/screensaver
 msgid "Minimum seconds to skip without screensaver"
-msgstr "Pantaila-babeslerik gabe saltatzeko gutxieneko segundoak"
+msgstr "Pantaila-babesle erakutsi gabe saltatzeko segundoak"
 
 # plugin/screensaver
 msgid "Lock screen"
 msgstr "Blokeatu pantaila"
 
 # plugin/smartpause
 msgid "Smart Pause"
@@ -393,37 +395,37 @@
 
 # plugin/smartpause
 msgid "Pause Safe Eyes if the system is idle"
 msgstr "Pausatu Safe Eyes sistema inaktibo badago"
 
 # plugin/smartpause
 msgid "Minimum idle time to pause Safe Eyes (in seconds)"
-msgstr "Safe Eyes pausatzeko gutxieneko denbora inaktiboa (segundotan)"
+msgstr "Safe Eyes pausatzeko pasa behar den denbora inaktiboa (segundotan)"
 
 # plugin/smartpause
 msgid "Interpret idle time equivalent to upcoming break duration as a break"
 msgstr ""
-"Interpretatu hurrengo atsedenaldiaren iraupenaren baliokidea den denbora "
-"inaktiboa atsedenaldi gisa"
+"Tratatu denbora inaktiboa etenaldi gisa, inaktibo emandako denbora datorren "
+"etenaldiaren iraupen berekoa izan bada"
 
 # plugin/smartpause
 msgid "Postpone the next break until the system becomes idle"
-msgstr "Atzeratu hurrengo atsedenaldia sistema inaktibo egon arte"
+msgstr "Atzeratu hurrengo etenaldia sistema inaktibo egon arte"
 
 #: plugins/trayicon
 msgid "Tray Icon"
 msgstr "Erretiluko ikonoa"
 
 #: plugins/trayicon
 msgid "Show a tray icon in the notification area"
 msgstr "Erakutsi erretiluko ikonoa jakinarazpenen eremuan"
 
 #: plugins/trayicon
 msgid "Show next break time in tray icon"
-msgstr "Erakutsi hurrengo atsedenaldia erretiluko ikonoan"
+msgstr "Erakutsi hurrengo etenaldia erretiluko ikonoan"
 
 #: plugins/trayicon
 msgid "Allow disabling Safe Eyes"
 msgstr "Baimendu Safe Eyes desgaitzea"
 
 #: plugins/trayicon
 msgid "About"
@@ -444,57 +446,57 @@
 #: plugins/trayicon
 msgid "Enable Safe Eyes"
 msgstr "Gaitu Safe Eyes"
 
 #: plugins/trayicon
 msgid "For %d Hour"
 msgid_plural "For %d Hours"
-msgstr[0] "Ordu %derako"
-msgstr[1] "%d ordurako"
+msgstr[0] "Ordu %dez"
+msgstr[1] "%d orduz"
 
 #: plugins/trayicon
 msgid "For %d Minute"
 msgid_plural "For %d Minutes"
-msgstr[0] "Minutu %derako"
-msgstr[1] "%d minuturako"
+msgstr[0] "Minutu %dez"
+msgstr[1] "%d minutuz"
 
 #: plugins/trayicon
 msgid "For %d Second"
 msgid_plural "For %d Seconds"
-msgstr[0] "Segundo %derako"
-msgstr[1] "%d segundorako"
+msgstr[0] "Segundo %dez"
+msgstr[1] "%d segundoz"
 
 #: plugins/trayicon
 msgid "Next break at %s"
-msgstr "Hurrengo atsedenaldia: %s"
+msgstr "Hurrengo etenaldia: %s"
 
 #: plugins/trayicon
 msgid "No Breaks Available"
-msgstr "Atsedenaldirik ez erabilgarri"
+msgstr "Etenaldirik ez erabilgarri"
 
 #: plugins/trayicon
 msgid "Settings"
 msgstr "Ezarpenak"
 
 #: plugins/trayicon
 msgid "Take a break now"
-msgstr "Hartu atsedenaldia orain"
+msgstr "Egin orain etenaldia"
 
 #: plugins/trayicon
 msgid "Until restart"
 msgstr "Berrabiarazi arte"
 
 #: plugins/trayicon
 msgid "Quit"
-msgstr "Utzi"
+msgstr "Irten"
 
 # plugin/mediacontrol
 msgid "Media Control"
 msgstr "Multimediaren kontrola"
 
 # plugin/mediacontrol
 msgid "Pause media players from the break screen"
-msgstr "Pausatu multimedia erreproduzitzaileak atsedenaldiaren pantailatik"
+msgstr "Pausatu multimedia etenaldiaren pantailatik"
 
 # plugin/mediacontrol
 msgid "Pause media"
 msgstr "Pausatu multimedia"
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/fa/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/fa/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/fr/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/fr/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/he/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/he/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/hi/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/hi/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/hu/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/hu/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/id/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/id/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/it/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/it/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/kn/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/kn/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ko/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ko/LC_MESSAGES/safeeyes.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) 2017 Gobinath
 # Gobinath slgobinath@gmail.com, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: \n"
-"PO-Revision-Date: 2021-02-24 07:50+0000\n"
-"Last-Translator: Lee Yunseok <ironyunseok@protonmail.com>\n"
+"PO-Revision-Date: 2023-02-17 05:35+0000\n"
+"Last-Translator: Yi Yunseok <ironyunseok@protonmail.com>\n"
 "Language-Team: Korean <https://hosted.weblate.org/projects/safe-eyes/"
 "translations/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.5\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 # Short break
 msgid "Tightly close your eyes"
 msgstr "눈을 꼭 감으세요"
 
 # Short break
 msgid "Roll your eyes a few times to each side"
@@ -342,15 +342,15 @@
 
 # plugin/healthstats
 msgid "Show statistics based on how you use Safe Eyes"
 msgstr "세이프 아이즈 사용에 기반한 통계 표시"
 
 # plugin/healthstats
 msgid "Statistics reset interval (cron expression)"
-msgstr "통계 재설정 간격 (크론 표현식)"
+msgstr "통계 초기화 간격 (크론 표현식)"
 
 # plugin/notification
 msgid "Notification"
 msgstr "알림"
 
 # plugin/notification
 msgid "Show a system notification before breaks"
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/lt/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/lt/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/lv/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/lv/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/mk/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/mk/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/mr/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/mr/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/nb/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/nb/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/nl/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/nl/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/pl/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/pl/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/pt/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/pt/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/pt_BR/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/pt_BR/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ru/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ru/LC_MESSAGES/safeeyes.po`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 # Copyright (C) 2017 Gobinath
 # Gobinath slgobinath@gmail.com, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: \n"
-"PO-Revision-Date: 2022-12-21 05:47+0000\n"
-"Last-Translator: Dmitriy Q <krotesk@mail.ru>\n"
+"PO-Revision-Date: 2023-03-22 16:41+0000\n"
+"Last-Translator: AHOHNMYC <lqwh2h2cwa@protonmail.com>\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/safe-eyes/"
 "translations/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.15.1-dev\n"
+"X-Generator: Weblate 4.16.2-dev\n"
 
 # Short break
 msgid "Tightly close your eyes"
 msgstr "Плотно закройте глаза"
 
 # Short break
 msgid "Roll your eyes a few times to each side"
@@ -153,19 +153,19 @@
 
 # Settings dialog
 msgid "Persist the internal state"
 msgstr "Сохранять внутреннее состояние"
 
 # Settings dialog
 msgid "Use RPC server to receive runtime commands"
-msgstr "Использовать RPC-сервер для получения запущенных команд"
+msgstr "Используйте RPC сервер для получения команд во время работы приложения"
 
 # Settings dialog
 msgid "Without the RPC server, command-line commands may not work"
-msgstr "Без RPC сервера команды из командной строки могут не работать"
+msgstr "Без RPC сервера команды из командной строки могут не сработать"
 
 # Settings dialog
 msgid "Long break interval must be a multiple of short break interval"
 msgstr "Время длинного перерыва должно быть кратно времени короткого перерыва"
 
 # Settings dialog
 msgid "Reset"
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/safeeyes.pot` & `safeeyes-2.1.6/safeeyes/config/locale/safeeyes.pot`

 * *Files 2% similar despite different names*

```diff
@@ -453,14 +453,26 @@
 msgstr ""
 
 #: plugins/trayicon
 msgid "Take a break now"
 msgstr ""
 
 #: plugins/trayicon
+msgid "Any break"
+msgstr ""
+
+#: plugins/trayicon
+msgid "Short break"
+msgstr ""
+
+#: plugins/trayicon
+msgid "Long break"
+msgstr ""
+
+#: plugins/trayicon
 msgid "Until restart"
 msgstr ""
 
 #: plugins/trayicon
 msgid "Quit"
 msgstr ""
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/sk/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/sk/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/sr/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/sr/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/sv/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/sv/LC_MESSAGES/safeeyes.po`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # Copyright (C) 2017 Gobinath
 # Gobinath slgobinath@gmail.com, 2017.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "POT-Creation-Date: \n"
-"PO-Revision-Date: 2021-08-18 00:37+0000\n"
+"PO-Revision-Date: 2023-02-11 11:39+0000\n"
 "Last-Translator: Luna Jernberg <droidbittin@gmail.com>\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/safe-eyes/"
 "translations/sv/>\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.8-dev\n"
+"X-Generator: Weblate 4.16-dev\n"
 
 # Short break
 msgid "Tightly close your eyes"
 msgstr "Stäng ögonen tätt"
 
 # Short break
 msgid "Roll your eyes a few times to each side"
@@ -134,15 +134,15 @@
 
 # Settings dialog
 msgid "Postponement duration (in minutes)"
 msgstr "Uppskjutningsvaraktighet (i minuter)"
 
 # Settings dialog
 msgid "Show breaks in random order"
-msgstr ""
+msgstr "Visa avbrott i slumpmässig ordning"
 
 # Settings dialog
 msgid "Strict break (No way to skip breaks)"
 msgstr "Strikt paus (inget sätt att hoppa över pauser)"
 
 # Settings dialog
 msgid "Allow postponing breaks"
```

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ta/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ta/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/tr/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/tr/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/ug/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/ug/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/uk/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/uk/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/uz_Latn/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/uz_Latn/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/vi/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/vi/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/zh_CN/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/zh_CN/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/locale/zh_TW/LC_MESSAGES/safeeyes.po` & `safeeyes-2.1.6/safeeyes/config/locale/zh_TW/LC_MESSAGES/safeeyes.po`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/safeeyes.json` & `safeeyes-2.1.6/safeeyes/config/safeeyes.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/config/style/safeeyes_style.css` & `safeeyes-2.1.6/safeeyes/config/style/safeeyes_style.css`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/core.py` & `safeeyes-2.1.6/safeeyes/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -127,31 +127,31 @@
         if duration > 0:
             self.postpone_duration = duration
         else:
             self.postpone_duration = self.default_postpone_duration
         logging.debug("Postpone the break for %d seconds", self.postpone_duration)
         self.context['postponed'] = True
 
-    def take_break(self):
+    def take_break(self, break_type = None):
         """
         Calling this method stops the scheduler and show the next break screen
         """
         if self.break_queue.is_empty():
             return
         if not self.context['state'] == State.WAITING:
             return
-        utility.start_thread(self.__take_break)
+        utility.start_thread(self.__take_break, break_type=break_type)
 
-    def has_breaks(self):
+    def has_breaks(self, break_type = None):
         """
-        Check whether Safe Eyes has breaks or not.
+        Check whether Safe Eyes has breaks or not. Use the break_type to check for either short or long break.
         """
-        return not self.break_queue.is_empty()
+        return not self.break_queue.is_empty(break_type)
 
-    def __take_break(self):
+    def __take_break(self, break_type = None):
         """
         Show the next break screen
         """
         logging.info('Take a break due to external request')
 
         with self.lock:
             if not self.running:
@@ -163,14 +163,16 @@
             self.waiting_condition.acquire()
             self.running = False
             self.waiting_condition.notify_all()
             self.waiting_condition.release()
             time.sleep(1)  # Wait for 1 sec to ensure the sceduler is dead
             self.running = True
 
+        if break_type is not None and self.break_queue.get_break().type != break_type:
+            self.break_queue.next(break_type)
         utility.execute_main_thread(self.__fire_start_break)
 
     def __scheduler_job(self):
         """
         Scheduler task to execute during every interval
         """
         if not self.running:
@@ -240,29 +242,30 @@
         utility.execute_main_thread(self.__fire_start_break)
 
     def __postpone_break(self):
         self.__wait_for(self.postpone_duration)
         utility.execute_main_thread(self.__fire_start_break)
 
     def __fire_start_break(self):
+        break_obj = self.break_queue.get_break()
         # Show the break screen
-        if not self.on_start_break.fire(self.break_queue.get_break()):
+        if not self.on_start_break.fire(break_obj):
             # Plugins want to ignore this break
             self.__start_next_break()
             return
         if self.context['postponed']:
             # Plugins want to postpone this break
             self.context['postponed'] = False
             # Update the next break time
             self.scheduled_next_break_time = self.scheduled_next_break_time + datetime.timedelta(seconds=self.postpone_duration)
             self.__fire_on_update_next_break(self.scheduled_next_break_time)
             # Wait in user thread
             utility.start_thread(self.__postpone_break)
         else:
-            self.start_break.fire(self.break_queue.get_break())
+            self.start_break.fire(break_obj)
             utility.start_thread(self.__start_break)
 
     def __start_break(self):
         """
         Start the break screen.
         """
         self.context['state'] = State.BREAK
```

### Comparing `safeeyes-2.1.5/safeeyes/glade/about_dialog.glade` & `safeeyes-2.1.6/safeeyes/glade/about_dialog.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/break_screen.glade` & `safeeyes-2.1.6/safeeyes/glade/break_screen.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/item_bool.glade` & `safeeyes-2.1.6/safeeyes/glade/item_bool.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/item_break.glade` & `safeeyes-2.1.6/safeeyes/glade/item_break.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/item_int.glade` & `safeeyes-2.1.6/safeeyes/glade/item_int.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/item_plugin.glade` & `safeeyes-2.1.6/safeeyes/glade/item_plugin.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/item_text.glade` & `safeeyes-2.1.6/safeeyes/glade/item_text.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/new_break.glade` & `safeeyes-2.1.6/safeeyes/glade/new_break.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/settings_break.glade` & `safeeyes-2.1.6/safeeyes/glade/settings_break.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/settings_dialog.glade` & `safeeyes-2.1.6/safeeyes/glade/settings_dialog.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/glade/settings_plugin.glade` & `safeeyes-2.1.6/safeeyes/glade/settings_plugin.glade`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/model.py` & `safeeyes-2.1.6/safeeyes/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
 class BreakQueue:
     def __init__(self, config, context):
         self.context = context
         self.__current_break = None
         self.__current_long = 0
         self.__current_short = 0
-        self.__shorts_taken = 0
         self.__short_break_time = config.get('short_break_interval')
         self.__long_break_time = config.get('long_break_interval')
         self.__is_random_order = config.get('random_order')
         self.__config = config
 
         self.__build_longs()
         self.__build_shorts()
@@ -109,101 +108,101 @@
             if last_break is not None:
                 current_break = self.get_break()
                 if last_break != current_break.name:
                     brk = self.next()
                     while brk != current_break and brk.name != last_break:
                         brk = self.next()
 
-    def get_break(self):
+    def get_break(self, break_type = None):
         if self.__current_break is None:
             self.__current_break = self.next()
-        return self.__current_break
+
+        if break_type is None or self.__current_break.type == break_type:
+            return self.__current_break
+
+        if break_type == BreakType.LONG_BREAK:
+            return self.__long_queue[self.__current_long]
+
+        return self.__short_queue[self.__current_short]
 
     def is_long_break(self):
         return self.__current_break is not None and self.__current_break.type == BreakType.LONG_BREAK
 
-    def next(self):
+    def next(self, break_type = None):
         break_obj = None
         shorts = self.__short_queue
         longs  = self.__long_queue
 
+        # Reset break that has just ended
+        if self.is_long_break():
+            self.__current_break.time = self.__long_break_time
+            if self.__current_long == 0 and self.__is_random_order:
+                # Shuffle queue
+                self.__build_longs()
+        elif self.__current_break:
+            # Reduce the break time from the next long break (default)
+            if longs:
+                longs[self.__current_long].time -= shorts[self.__current_short].time
+            if self.__current_short == 0 and self.__is_random_order:
+                self.__build_shorts()
+
         if self.is_empty():
             return None
 
         if shorts is None:
             break_obj = self.__next_long()
         elif longs is None:
             break_obj = self.__next_short()
-        elif longs[self.__current_long].time <= shorts[self.__current_short].time:
+        elif break_type == BreakType.LONG_BREAK or longs[self.__current_long].time <= shorts[self.__current_short].time:
             break_obj = self.__next_long()
         else:
             break_obj = self.__next_short()
 
-        # Shorts and longs exist -> set cycle on every long
-        if break_obj.type == BreakType.LONG_BREAK:
-            self.context['new_cycle'] = True
-            self.__shorts_taken = 0
-        # Only shorts exist -> set cycle when enough short breaks pass
-        elif self.__shorts_taken  == self.__cycle_len:
-            self.context['new_cycle'] = True
-            self.__shorts_taken = 0
-        else:
-            self.context['new_cycle'] = False
-
-        if self.__current_break is not None:
-            # Reset the time of long breaks
-            if self.__current_break.type == BreakType.LONG_BREAK:
-                self.__current_break.time = self.__long_break_time
-
         self.__current_break = break_obj
         self.context['session']['break'] = self.__current_break.name
 
         return break_obj
 
     def reset(self):
         for break_object in self.__short_queue:
             break_object.time = self.__short_break_time
-        
+
         for break_object in self.__long_queue:
             break_object.time = self.__long_break_time
 
-    def is_empty(self):
-        return self.__short_queue is None and self.__long_queue is None
+    def is_empty(self, break_type = None):
+        """
+        Check if the given break type is empty or not. If the break_type is None, check for both short and long breaks.
+        """
+        if break_type == BreakType.SHORT_BREAK:
+            return self.__short_queue is None
+        elif break_type == BreakType.LONG_BREAK:
+            return self.__long_queue is None
+        else:
+            return self.__short_queue is None and self.__long_queue is None
 
     def __next_short(self):
         longs  = self.__long_queue
         shorts = self.__short_queue
         break_obj = shorts[self.__current_short]
         self.context['break_type'] = 'short'
-        # Reduce the break time from the next long break (default)
-        if longs:
-            longs[self.__current_long].time -= shorts[self.__current_short].time
 
         # Update the index to next
         self.__current_short = (self.__current_short + 1) % len(shorts)
 
-        # Shuffle queue
-        if self.__current_short == 0 and self.__is_random_order:
-            self.__build_shorts()
-
-        self.__shorts_taken += 1
         return break_obj
 
     def __next_long(self):
         longs  = self.__long_queue
         break_obj = longs[self.__current_long]
         self.context['break_type'] = 'long'
 
         # Update the index to next
         self.__current_long = (self.__current_long + 1) % len(longs)
 
-        # Shuffle queue
-        if self.__current_long == 0 and self.__is_random_order:
-            self.__build_longs()
-
         return break_obj
 
     def __build_queue(self, break_type, break_configs, break_time, break_duration):
         """
         Build a queue of breaks.
         """
         size = len(break_configs)
```

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/128x128/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/128x128/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_disabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-disabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_enabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-enabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/16x16/status/safeeyes_timer.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-timer.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_disabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-disabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_enabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-enabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/24x24/status/safeeyes_timer.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-timer.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/status/safeeyes_disabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-disabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/32x32/status/safeeyes_enabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-enabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/status/safeeyes_disabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-disabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/48x48/status/safeeyes_enabled.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-enabled.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/icons/hicolor/64x64/apps/safeeyes.png` & `safeeyes-2.1.6/safeeyes/platform/icons/hicolor/64x64/apps/io.github.slgobinath.SafeEyes.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/platform/safeeyes.desktop` & `safeeyes-2.1.6/safeeyes/platform/io.github.slgobinath.SafeEyes.desktop`

 * *Files 3% similar despite different names*

```diff
@@ -21,11 +21,11 @@
 Comment[ru]=Защитите свои глаза от зрительного перенапряжения
 Comment[sk]=Chráňte svoje oči pred únavou
 Comment[ta]=உங்கள் கண்களை சோர்வடையாது பாதுகாத்திடுங்கள்
 Comment[tr]=Gözünüzü yorgunluğa karşı koruyun
 Comment[uk]=Захистіть свої очі від втоми
 Comment[vi]=Bảo vệ đôi mắt của bạn khỏi sự mệt mỏi
 Exec=env GDK_BACKEND=x11 safeeyes
-Icon=safeeyes
+Icon=io.github.slgobinath.SafeEyes
 Terminal=false
 Type=Application
 Categories=Utility;
```

### Comparing `safeeyes-2.1.5/safeeyes/plugin_manager.py` & `safeeyes-2.1.6/safeeyes/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,20 @@
         """
         Initialize all the plugins with init(context, safe_eyes_config, plugin_config) function.
         """
         # Load the plugins
         for plugin in config.get('plugins'):
             try:
                 self.__load_plugin(plugin)
-            except BaseException:
-                logging.error('Error in loading the plugin: %s', plugin['id'])
+            except BaseException as e:
+                traceback_wanted = logging.getLogger().getEffectiveLevel() == logging.DEBUG
+                if traceback_wanted:
+                    import traceback
+                    traceback.print_exc()
+                logging.error('Error in loading the plugin %s: %s', plugin['id'], e)
                 continue
         # Initialize the plugins
         for plugin in self.__plugins_on_init:
             plugin['module'].init(context, config, plugin['config'])
         return True
 
     def start(self):
```

### Comparing `safeeyes-2.1.5/safeeyes/plugins/audiblealert/config.json` & `safeeyes-2.1.6/safeeyes/plugins/audiblealert/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/audiblealert/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/audiblealert/plugin.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/donotdisturb/config.json` & `safeeyes-2.1.6/safeeyes/plugins/donotdisturb/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/donotdisturb/dependency_checker.py` & `safeeyes-2.1.6/safeeyes/plugins/donotdisturb/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/donotdisturb/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/donotdisturb/plugin.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/healthstats/config.json` & `safeeyes-2.1.6/safeeyes/plugins/healthstats/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/healthstats/dependency_checker.py` & `safeeyes-2.1.6/safeeyes/plugins/healthstats/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/healthstats/icon.png` & `safeeyes-2.1.6/safeeyes/plugins/healthstats/icon.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/healthstats/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/healthstats/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import croniter
 import datetime
 import logging
 
 context = None
 no_of_skipped_breaks = 0
 no_of_breaks = 0
-no_of_cycles = -1
 session = None
 safe_eyes_start_time = datetime.datetime.now()
 total_idle_time = 0
 last_screen_time = -1
 statistics_reset_cron = '0 0 * * *'  # Every midnight
 time_to_reset_break = datetime.datetime.now()
 next_reset_time = None
@@ -42,15 +41,14 @@
     Initialize the plugin.
     """
     global enabled
     global context
     global session
     global no_of_skipped_breaks
     global no_of_breaks
-    global no_of_cycles
     global statistics_reset_cron
     global safe_eyes_start_time
     global total_idle_time
     global last_screen_time
     global next_reset_time
 
     logging.debug('Initialize Health Stats plugin')
@@ -67,23 +65,21 @@
 
     if session is None:
         # Read the session
         session = context['session']['plugin'].get('healthstats', None)
         if session is None:
             session = {'no_of_skipped_breaks': 0,
                        'no_of_breaks': 0,
-                       'no_of_cycles': -1,
                        'safe_eyes_start_time': safe_eyes_start_time.strftime("%Y-%m-%d %H:%M:%S"),
                        'total_idle_time': 0,
                        'last_screen_time': -1,
                        'next_reset_time': next_reset_time.strftime("%Y-%m-%d %H:%M:%S")}
             context['session']['plugin']['healthstats'] = session
         no_of_skipped_breaks = session.get('no_of_skipped_breaks', 0)
         no_of_breaks = session.get('no_of_breaks', 0)
-        no_of_cycles = session.get('no_of_cycles', -1)
         total_idle_time = session.get('total_idle_time', 0)
         last_screen_time = session.get('last_screen_time', -1)
         str_time = session.get('safe_eyes_start_time', None)
         str_next_reset_time = session.get('next_reset_time', None)
         if str_time:
             safe_eyes_start_time = datetime.datetime.strptime(str_time, "%Y-%m-%d %H:%M:%S")
         if str_next_reset_time:
@@ -111,29 +107,24 @@
     Return the widget title.
     """
     # Check if the plugin is enabled
     if not enabled:
         return ""
 
     global no_of_breaks
-    global no_of_cycles
     no_of_breaks += 1
-    if context['new_cycle']:
-        no_of_cycles += 1
     session['no_of_breaks'] = no_of_breaks
-    session['no_of_cycles'] = no_of_cycles
     session['safe_eyes_start_time'] = safe_eyes_start_time.strftime("%Y-%m-%d %H:%M:%S")
     session['total_idle_time'] = total_idle_time
     session['last_screen_time'] = last_screen_time
     return _('Health Statistics')
 
 
 def _reset_stats():
     global no_of_breaks
-    global no_of_cycles
     global safe_eyes_start_time
     global total_idle_time
     global no_of_skipped_breaks
     global last_screen_time
     global next_reset_time
 
     # Check if the reset time has passed
@@ -150,18 +141,16 @@
 
         # Update the next_reset_time
         next_reset_time = _get_next_reset_time(current_time, statistics_reset_cron)
 
         last_screen_time = round((total_duration_sec - total_idle_time) / 60)
         total_idle_time = 0
         no_of_breaks = 0
-        no_of_cycles = 0
         no_of_skipped_breaks = 0
         session['no_of_breaks'] = 0
-        session['no_of_cycles'] = 0
         session['no_of_skipped_breaks'] = 0
         session['safe_eyes_start_time'] = safe_eyes_start_time.strftime("%Y-%m-%d %H:%M:%S")
         session['total_idle_time'] = total_idle_time
         session['last_screen_time'] = last_screen_time
         session['next_reset_time'] = next_reset_time.strftime("%Y-%m-%d %H:%M:%S")
 
     return total_duration_sec
@@ -191,15 +180,15 @@
         hrs_diff, mins_diff = divmod(abs(screen_time - last_screen_time), 60)
         symbol = ''
         if screen_time > last_screen_time:
             symbol = '+'
         elif screen_time < last_screen_time:
             symbol = '-'
         screen_time_diff = ' ( {}{:02d}:{:02d} )'.format(symbol, hrs_diff, mins_diff)
-    return "{}\tBREAKS: {}\tSKIPPED: {}\tCYCLES: {}\tSCREEN TIME: {}{}".format(heart, no_of_breaks, no_of_skipped_breaks, no_of_cycles, time_format, screen_time_diff)
+    return "{}\tBREAKS: {}\tSKIPPED: {}\tSCREEN TIME: {}{}".format(heart, no_of_breaks, no_of_skipped_breaks, time_format, screen_time_diff)
 
 
 def on_start():
     """
     Add the idle period to the total idle time.
     """
     # Check if the plugin is enabled
```

### Comparing `safeeyes-2.1.5/safeeyes/plugins/mediacontrol/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/mediacontrol/plugin.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/notification/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/notification/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     logging.info('Show the notification')
     message = '\n'
     if break_obj.type == BreakType.SHORT_BREAK:
         message += (_('Ready for a short break in %s seconds') % warning_time)
     else:
         message += (_('Ready for a long break in %s seconds') % warning_time)
 
-    notification = Notify.Notification.new('Safe Eyes', message, icon='safeeyes_enabled')
+    notification = Notify.Notification.new('Safe Eyes', message, icon='io.github.slgobinath.SafeEyes-enabled')
     try:
         notification.show()
     except BaseException:
         logging.error('Failed to show the notification')
 
 
 def on_start_break(break_obj):
```

### Comparing `safeeyes-2.1.5/safeeyes/plugins/screensaver/config.json` & `safeeyes-2.1.6/safeeyes/plugins/screensaver/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/screensaver/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/screensaver/plugin.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/smartpause/config.json` & `safeeyes-2.1.6/safeeyes/plugins/smartpause/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/smartpause/dependency_checker.py` & `safeeyes-2.1.6/safeeyes/plugins/smartpause/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/smartpause/icon.png` & `safeeyes-2.1.6/safeeyes/plugins/smartpause/icon.png`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/smartpause/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/smartpause/plugin.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/trayicon/config.json` & `safeeyes-2.1.6/safeeyes/plugins/trayicon/config.json`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/plugins/trayicon/plugin.py` & `safeeyes-2.1.6/safeeyes/plugins/trayicon/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import datetime
+from safeeyes.model import BreakType
 import gi
 gi.require_version('Gtk', '3.0')
 try:
     gi.require_version('AppIndicator3', '0.1')
     from gi.repository import AppIndicator3 as appindicator
 except:
     #fall back to Ayatana
@@ -63,36 +64,34 @@
         self.idle_condition = threading.Condition()
         self.lock = threading.Lock()
         self.allow_disabling = plugin_config['allow_disabling']
         self.animate = False
 
         # Construct the tray icon
         self.indicator = appindicator.Indicator.new(
-            APPINDICATOR_ID, "safeeyes_enabled", appindicator.IndicatorCategory.APPLICATION_STATUS)
+            APPINDICATOR_ID, "io.github.slgobinath.SafeEyes-enabled", appindicator.IndicatorCategory.APPLICATION_STATUS)
         self.indicator.set_status(appindicator.IndicatorStatus.ACTIVE)
 
         # Construct the context menu
         self.menu = Gtk.Menu()
 
         # Next break info menu item
         self.item_info = Gtk.ImageMenuItem()
         img_timer = Gtk.Image()
-        img_timer.set_from_icon_name("safeeyes_timer", 16)
+        img_timer.set_from_icon_name("io.github.slgobinath.SafeEyes-timer", 16)
         self.item_info.set_image(img_timer)
 
         self.item_separator = Gtk.SeparatorMenuItem()
 
         self.item_enable = Gtk.MenuItem()
         self.item_enable.connect('activate', self.on_enable_clicked)
 
         self.item_disable = Gtk.MenuItem()
-        self.item_disable.connect('activate', self.on_disable_clicked)
-
         self.sub_menu_disable = Gtk.Menu()
-        self.sub_menu_items = []
+        self.sub_menu_disable_items = []
 
         # Read disable options and build the sub menu
         for disable_option in plugin_config['disable_options']:
             time_in_minutes = disable_option['time']
             label = []
             # Validate time value
             if not isinstance(time_in_minutes, int) or time_in_minutes <= 0:
@@ -112,28 +111,40 @@
                 # Invalid unit
                 logging.error('Invalid unit in disable option: ' + str(disable_option))
                 continue
 
             # Create submenu
             sub_menu_item = Gtk.MenuItem()
             sub_menu_item.connect('activate', self.on_disable_clicked, time_in_minutes)
-            self.sub_menu_items.append([sub_menu_item, label, disable_option['time']])
+            self.sub_menu_disable_items.append([sub_menu_item, label, disable_option['time']])
             self.sub_menu_disable.append(sub_menu_item)
 
         # Disable until restart submenu
         self.sub_menu_item_until_restart = Gtk.MenuItem()
         self.sub_menu_item_until_restart.connect('activate', self.on_disable_clicked, -1)
         self.sub_menu_disable.append(self.sub_menu_item_until_restart)
 
         # Add the sub menu to the enable/disable menu
         self.item_disable.set_submenu(self.sub_menu_disable)
 
         # Settings menu item
         self.item_manual_break = Gtk.MenuItem()
-        self.item_manual_break.connect('activate', self.on_manual_break_clicked)
+
+        self.sub_menu_manual_next_break = Gtk.MenuItem()
+        self.sub_menu_manual_next_break.connect('activate', self.on_manual_break_clicked, None)
+        self.sub_menu_manual_next_short_break = Gtk.MenuItem()
+        self.sub_menu_manual_next_short_break.connect('activate', self.on_manual_break_clicked, BreakType.SHORT_BREAK)
+        self.sub_menu_manual_next_long_break = Gtk.MenuItem()
+        self.sub_menu_manual_next_long_break.connect('activate', self.on_manual_break_clicked, BreakType.LONG_BREAK)
+
+        self.sub_menu_manual_break = Gtk.Menu()
+        self.sub_menu_manual_break.append(self.sub_menu_manual_next_break)
+        self.sub_menu_manual_break.append(self.sub_menu_manual_next_short_break)
+        self.sub_menu_manual_break.append(self.sub_menu_manual_next_long_break)
+        self.item_manual_break.set_submenu(self.sub_menu_manual_break)
 
         # Settings menu item
         self.item_settings = Gtk.MenuItem()
         self.item_settings.connect('activate', self.show_settings)
 
         # About menu item
         self.item_about = Gtk.MenuItem()
@@ -178,45 +189,48 @@
         self.item_quit.set_visible(self.allow_disabling)
         self.item_quit.set_visible(self.allow_disabling)
 
     def set_labels(self):
         """
         Update the text of menu items based on the selected language.
         """
-        for entry in self.sub_menu_items:
+        for entry in self.sub_menu_disable_items:
             # print(self.context['locale'].ngettext('For %d Hour', 'For %d Hours', 1) % 1)
             entry[0].set_label(self.context['locale'].ngettext(entry[1][0], entry[1][1], entry[2]) % entry[2])
 
         self.sub_menu_item_until_restart.set_label(_('Until restart'))
         self.item_enable.set_label(_('Enable Safe Eyes'))
         self.item_disable.set_label(_('Disable Safe Eyes'))
 
         breaks_found = self.has_breaks()
         if breaks_found:
             if self.active:
                 if self.date_time:
                     self.__set_next_break_info()
-                self.indicator.set_icon("safeeyes_enabled")
+                self.indicator.set_icon("io.github.slgobinath.SafeEyes-enabled")
             else:
                 if self.wakeup_time:
                     self.item_info.set_label(_('Disabled until %s') % utility.format_time(self.wakeup_time))
                 else:
                     self.item_info.set_label(_('Disabled until restart'))
                 self.indicator.set_label('', '')
-                self.indicator.set_icon("safeeyes_disabled")
+                self.indicator.set_icon("io.github.slgobinath.SafeEyes-disabled")
         else:
             self.item_info.set_label(_('No Breaks Available'))
             self.indicator.set_label('', '')
-            self.indicator.set_icon("safeeyes_disabled")
+            self.indicator.set_icon("io.github.slgobinath.SafeEyes-disabled")
         self.item_info.set_sensitive(breaks_found and self.active)
         self.item_enable.set_sensitive(breaks_found and not self.active)
         self.item_disable.set_sensitive(breaks_found and self.active)
         self.item_manual_break.set_sensitive(breaks_found and self.active)
 
         self.item_manual_break.set_label(_('Take a break now'))
+        self.sub_menu_manual_next_break.set_label(_('Any break'))
+        self.sub_menu_manual_next_short_break.set_label(_('Short break'))
+        self.sub_menu_manual_next_long_break.set_label(_('Long break'))
         self.item_settings.set_label(_('Settings'))
         self.item_about.set_label(_('About'))
         self.item_quit.set_label(_('Quit'))
 
     def show_icon(self):
         """
         Show the tray icon.
@@ -278,15 +292,19 @@
         else:
             self.indicator.set_label('', '')
 
     def on_manual_break_clicked(self, *args):
         """
         Trigger a break manually.
         """
-        self.take_break()
+        if len(args) > 1:
+            break_type = args[1]
+            self.take_break(break_type)
+        else:
+            self.take_break()
 
     def on_enable_clicked(self, *args):
         """
         Handle 'Enable Safe Eyes' menu action.
         This action enables the application if it is currently disabled.
         """
         # active = self.item_enable.get_active()
@@ -338,30 +356,30 @@
     def disable_ui(self):
         """
         Change the UI to disabled state.
         """
         if self.active:
             logging.info('Disable Safe Eyes')
             self.active = False
-            self.indicator.set_icon("safeeyes_disabled")
+            self.indicator.set_icon("io.github.slgobinath.SafeEyes-disabled")
             self.item_info.set_label(_('Disabled until restart'))
             self.indicator.set_label('', '')
             self.item_info.set_sensitive(False)
             self.item_enable.set_sensitive(True)
             self.item_disable.set_sensitive(False)
             self.item_manual_break.set_sensitive(False)
 
     def enable_ui(self):
         """
         Change the UI to enabled state.
         """
         if not self.active:
             logging.info('Enable Safe Eyes')
             self.active = True
-            self.indicator.set_icon("safeeyes_enabled")
+            self.indicator.set_icon("io.github.slgobinath.SafeEyes-enabled")
             self.item_info.set_sensitive(True)
             self.item_enable.set_sensitive(False)
             self.item_disable.set_sensitive(True)
             self.item_manual_break.set_sensitive(True)
 
     def __schedule_resume(self, time_minutes):
         """
@@ -374,28 +392,28 @@
         with self.lock:
             if not self.active:
                 utility.execute_main_thread(self.item_enable.activate)
 
     def start_animation(self):
         if not self.active or not self.animate:
             return
-        utility.execute_main_thread(lambda: self.indicator.set_icon("safeeyes_disabled"))
+        utility.execute_main_thread(lambda: self.indicator.set_icon("io.github.slgobinath.SafeEyes-disabled"))
         time.sleep(0.5)
-        utility.execute_main_thread(lambda: self.indicator.set_icon("safeeyes_enabled"))
+        utility.execute_main_thread(lambda: self.indicator.set_icon("io.github.slgobinath.SafeEyes-enabled"))
         if self.animate and self.active:
             time.sleep(0.5)
             if self.animate and self.active:
                 utility.start_thread(self.start_animation)
 
     def stop_animation(self):
         self.animate = False
         if self.active:
-            utility.execute_main_thread(lambda: self.indicator.set_icon("safeeyes_enabled"))
+            utility.execute_main_thread(lambda: self.indicator.set_icon("io.github.slgobinath.SafeEyes-enabled"))
         else:
-            utility.execute_main_thread(lambda: self.indicator.set_icon("safeeyes_disabled"))
+            utility.execute_main_thread(lambda: self.indicator.set_icon("io.github.slgobinath.SafeEyes-disabled"))
 
 def init(ctx, safeeyes_cfg, plugin_config):
     """
     Initialize the tray icon.
     """
     global context
     global tray_icon
```

### Comparing `safeeyes-2.1.5/safeeyes/resource/on_pre_break.wav` & `safeeyes-2.1.6/safeeyes/resource/on_pre_break.wav`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/resource/on_stop_break.wav` & `safeeyes-2.1.6/safeeyes/resource/on_stop_break.wav`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/rpc.py` & `safeeyes-2.1.6/safeeyes/rpc.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/safeeyes.py` & `safeeyes-2.1.6/safeeyes/safeeyes.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from safeeyes.plugin_manager import PluginManager
 from safeeyes.core import SafeEyesCore
 from safeeyes.ui.settings_dialog import SettingsDialog
 
 gi.require_version('Gtk', '3.0')
 from gi.repository import Gtk
 
-SAFE_EYES_VERSION = "2.1.5"
+SAFE_EYES_VERSION = "2.1.6"
 
 
 class SafeEyes:
     """
     This class represents a runnable Safe Eyes instance.
     """
 
@@ -89,16 +89,15 @@
         self.safe_eyes_core.on_pre_break += self.plugins_manager.pre_break
         self.safe_eyes_core.on_start_break += self.on_start_break
         self.safe_eyes_core.start_break += self.start_break
         self.safe_eyes_core.on_count_down += self.countdown
         self.safe_eyes_core.on_stop_break += self.stop_break
         self.safe_eyes_core.on_update_next_break += self.update_next_break
         self.safe_eyes_core.initialize(self.config)
-        self.context['api']['take_break'] = lambda: utility.execute_main_thread(
-            self.safe_eyes_core.take_break)
+        self.context['api']['take_break'] = self.take_break
         self.context['api']['has_breaks'] = self.safe_eyes_core.has_breaks
         self.context['api']['postpone'] = self.safe_eyes_core.postpone
         self.plugins_manager.init(self.context, self.config)
         atexit.register(self.persist_session)
 
     def start(self):
         """
@@ -291,19 +290,19 @@
         """
         Stop the current break.
         """
         self.break_screen.close()
         self.plugins_manager.stop_break()
         return True
 
-    def take_break(self):
+    def take_break(self, break_type = None):
         """
         Take a break now.
         """
-        self.safe_eyes_core.take_break()
+        utility.execute_main_thread(self.safe_eyes_core.take_break, break_type)
 
     def status(self):
         """
         Return the status of Safe Eyes.
         """
         return self._status
```

### Comparing `safeeyes-2.1.5/safeeyes/ui/about_dialog.py` & `safeeyes-2.1.6/safeeyes/ui/about_dialog.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/ui/break_screen.py` & `safeeyes-2.1.6/safeeyes/ui/break_screen.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/ui/settings_dialog.py` & `safeeyes-2.1.6/safeeyes/ui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `safeeyes-2.1.5/safeeyes/utility.py` & `safeeyes-2.1.6/safeeyes/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,26 +47,27 @@
 
 gi.require_version('Gdk', '3.0')
 
 BIN_DIRECTORY = os.path.dirname(os.path.realpath(__file__))
 HOME_DIRECTORY = os.environ.get('HOME') or os.path.expanduser('~')
 CONFIG_DIRECTORY = os.path.join(os.environ.get(
     'XDG_CONFIG_HOME') or os.path.join(HOME_DIRECTORY, '.config'), 'safeeyes')
+STYLE_SHEET_DIRECTORY = os.path.join(CONFIG_DIRECTORY, 'style')
 CONFIG_FILE_PATH = os.path.join(CONFIG_DIRECTORY, 'safeeyes.json')
 CONFIG_RESOURCE = os.path.join(CONFIG_DIRECTORY, 'resource')
 SESSION_FILE_PATH = os.path.join(CONFIG_DIRECTORY, 'session.json')
-STYLE_SHEET_PATH = os.path.join(CONFIG_DIRECTORY, 'style/safeeyes_style.css')
+STYLE_SHEET_PATH = os.path.join(STYLE_SHEET_DIRECTORY, 'safeeyes_style.css')
 SYSTEM_CONFIG_FILE_PATH = os.path.join(BIN_DIRECTORY, "config/safeeyes.json")
 SYSTEM_STYLE_SHEET_PATH = os.path.join(
     BIN_DIRECTORY, "config/style/safeeyes_style.css")
 LOG_FILE_PATH = os.path.join(HOME_DIRECTORY, 'safeeyes.log')
 SYSTEM_PLUGINS_DIR = os.path.join(BIN_DIRECTORY, 'plugins')
 USER_PLUGINS_DIR = os.path.join(CONFIG_DIRECTORY, 'plugins')
 LOCALE_PATH = os.path.join(BIN_DIRECTORY, 'config/locale')
-SYSTEM_DESKTOP_FILE = os.path.join(BIN_DIRECTORY, "platform/safeeyes.desktop")
+SYSTEM_DESKTOP_FILE = os.path.join(BIN_DIRECTORY, "platform/io.github.slgobinath.SafeEyes.desktop")
 SYSTEM_ICONS = os.path.join(BIN_DIRECTORY, "platform/icons")
 DESKTOP_ENVIRONMENT = None
 IS_WAYLAND = False
 
 
 def get_resource_path(resource_name):
     """
@@ -367,25 +368,23 @@
     new_config = new_config.copy()
     new_config.update(old_config)
     return new_config
 
 
 def initialize_safeeyes():
     """
-    Create the config file and style sheet in ~/.config/safeeyes directory.
+    Create the config file and style sheet in XDG_CONFIG_HOME(or ~/.config)/safeeyes directory.
     """
-    logging.info('Copy the config files to ~/.config/safeeyes')
-
-    style_dir_path = os.path.join(HOME_DIRECTORY, '.config/safeeyes/style')
+    logging.info('Copy the config files to XDG_CONFIG_HOME(or ~/.config)/safeeyes')
     
     # Remove the ~/.config/safeeyes/safeeyes.json file
     delete(CONFIG_FILE_PATH)
 
-    # Create the ~/.config/safeeyes/style directory
-    mkdir(style_dir_path)
+    # Create the XDG_CONFIG_HOME(or ~/.config)/safeeyes/style directory
+    mkdir(STYLE_SHEET_DIRECTORY)
 
     # Copy the safeeyes.json
     shutil.copy2(SYSTEM_CONFIG_FILE_PATH, CONFIG_FILE_PATH)
     os.chmod(CONFIG_FILE_PATH, 0o777)
 
     # Copy the new style sheet
     if not os.path.isfile(STYLE_SHEET_PATH):
@@ -396,15 +395,15 @@
 
 
 def create_startup_entry():
     """
     Create start up entry.
     """
     startup_dir_path = os.path.join(HOME_DIRECTORY, '.config/autostart')
-    startup_entry = os.path.join(startup_dir_path, 'safeeyes.desktop')
+    startup_entry = os.path.join(startup_dir_path, 'io.github.slgobinath.SafeEyes.desktop')
 
     # Create the folder if not exist
     mkdir(startup_dir_path)
 
     # Remove existing files
     delete(startup_entry)
 
@@ -419,21 +418,21 @@
     """
     Copy icons and generate desktop entries.
     """
     logging.debug("Initialize the platform")
 
     applications_dir_path = os.path.join(HOME_DIRECTORY, '.local/share/applications')
     icons_dir_path = os.path.join(HOME_DIRECTORY, '.local/share/icons')
-    desktop_entry = os.path.join(applications_dir_path, 'safeeyes.desktop')
+    desktop_entry = os.path.join(applications_dir_path, 'io.github.slgobinath.SafeEyes.desktop')
 
     # Create the folder if not exist
     mkdir(icons_dir_path)
 
     # Create a desktop entry
-    if not os.path.exists(os.path.join(sys.prefix, "share/applications/safeeyes.desktop")):
+    if not os.path.exists(os.path.join(sys.prefix, "share/applications/io.github.slgobinath.SafeEyes.desktop")):
         # Create the folder if not exist
         mkdir(applications_dir_path)
         
         # Remove existing file
         delete(desktop_entry)
 
         # Create a link
@@ -662,15 +661,15 @@
 
 
 def has_method(module, method_name, no_of_args=0):
     """
     Check whether the given function is defined in the module or not.
     """
     if hasattr(module, method_name):
-        if len(inspect.getargspec(getattr(module, method_name)).args) == no_of_args:
+        if len(inspect.getfullargspec(getattr(module, method_name)).args) == no_of_args:
             return True
     return False
 
 
 def remove_if_exists(list_of_items, item):
     """
     Remove the item from the list_of_items it it exists.
```

### Comparing `safeeyes-2.1.5/safeeyes.egg-info/PKG-INFO` & `safeeyes-2.1.6/safeeyes.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: safeeyes
-Version: 2.1.5
+Version: 2.1.6
 Summary: Protect your eyes from eye strain using this continuous breaks reminder.
 Home-page: https://github.com/slgobinath/SafeEyes
-Download-URL: https://github.com/slgobinath/SafeEyes/archive/v2.1.5.tar.gz
+Download-URL: https://github.com/slgobinath/SafeEyes/archive/v2.1.6.tar.gz
 Author: Gobinath Loganathan
 Author-email: slgobinath@gmail.com
 Keywords: linux utility health eye-strain safe-eyes
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
@@ -24,14 +24,15 @@
 
 # Safe Eyes
 
 [![Release](https://img.shields.io/github/v/release/slgobinath/SafeEyes)](https://github.com/slgobinath/SafeEyes/releases)
 [![PyPI version](https://badge.fury.io/py/safeeyes.svg)](https://badge.fury.io/py/safeeyes)
 [![Debian](https://badges.debian.net/badges/debian/unstable/safeeyes/version.svg)](https://packages.debian.org/unstable/safeeyes)
 [![AUR](https://img.shields.io/aur/version/safeeyes)](https://aur.archlinux.org/packages/safeeyes)
+[![Flathub](https://img.shields.io/flathub/v/io.github.slgobinath.SafeEyes)](https://flathub.org/apps/details/io.github.slgobinath.SafeEyes)
 [![Translation status](https://hosted.weblate.org/widgets/safe-eyes/-/translations/svg-badge.svg)](https://hosted.weblate.org/engage/safe-eyes/?utm_source=widget)
 [![Awesome Humane Tech](https://raw.githubusercontent.com/humanetech-community/awesome-humane-tech/main/humane-tech-badge.svg?sanitize=true)](https://github.com/humanetech-community/awesome-humane-tech)
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/slgobinath)
 
 Protect your eyes from eye strain using this simple and beautiful, yet extensible break reminder.
 
 Visit the official site: https://slgobinath.github.io/SafeEyes/ for more details.
@@ -104,14 +105,20 @@
 
 ### Alpine Linux
 
 ```bash
 sudo apk add safeeyes
 ```
 
+### Flatpak
+
+```bash
+flatpak install flathub io.github.slgobinath.SafeEyes
+```
+
 ### Other Linux & Run from source
 
 Ensure to meet the following dependencies:
 
 - gir1.2-appindicator3-0.1 or gir1.2-ayatanaappindicator3-0.1
 - gir1.2-notify-0.7
 - libappindicator-gtk3
@@ -181,14 +188,30 @@
 - Command-line arguments to control the running instance
 - Customizable using plug-ins
 
 ## Third-party Plugins
 
 Thirdparty plugins are available at another GitHub repository: [safeeyes-plugins](https://github.com/slgobinath/safeeyes-plugins). More details about how to write your own plugin and how to install third-party plugin are available there.
 
+## How to Release?
+
+1. Checkout the latest commits from the `master` branch
+2. Run `python3 -m safeeyes` to make sure nothing is broken
+3. Update the Safe Eyes version in the following places (Open the project in VSCode and search for the current version):
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L81)
+    - [setup.py](https://github.com/slgobinath/SafeEyes/blob/master/setup.py#L88)
+    - [safeeyes.py](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/safeeyes.py#L43)
+    - [io.github.slgobinath.SafeEyes.metainfo.xml](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/platform/io.github.slgobinath.SafeEyes.metainfo.xml#L50)
+    - [about_dialog.glade](https://github.com/slgobinath/SafeEyes/blob/master/safeeyes/glade/about_dialog.glade#L74)
+4. Update the [changelog](https://github.com/slgobinath/SafeEyes/blob/master/debian/changelog) (for Ubuntu release)
+5. Commit the changes to `master`
+6. Create a pull-request from `master` to `release`
+7. Merge the PR to release **with merge commit** (Important to merge with merge commit)
+
+
 ## License
 
 GNU General Public License v3
 
 ## IDE Support
 
 <p align="center">Thanks to JetBrains for offering IDE support to develop this Open Source project.</p>
```

### Comparing `safeeyes-2.1.5/safeeyes.egg-info/SOURCES.txt` & `safeeyes-2.1.6/safeeyes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -67,31 +67,32 @@
 safeeyes/glade/item_int.glade
 safeeyes/glade/item_plugin.glade
 safeeyes/glade/item_text.glade
 safeeyes/glade/new_break.glade
 safeeyes/glade/settings_break.glade
 safeeyes/glade/settings_dialog.glade
 safeeyes/glade/settings_plugin.glade
-safeeyes/platform/safeeyes.desktop
-safeeyes/platform/icons/hicolor/128x128/apps/safeeyes.png
-safeeyes/platform/icons/hicolor/16x16/apps/safeeyes.png
-safeeyes/platform/icons/hicolor/16x16/status/safeeyes_disabled.png
-safeeyes/platform/icons/hicolor/16x16/status/safeeyes_enabled.png
-safeeyes/platform/icons/hicolor/16x16/status/safeeyes_timer.png
-safeeyes/platform/icons/hicolor/24x24/apps/safeeyes.png
-safeeyes/platform/icons/hicolor/24x24/status/safeeyes_disabled.png
-safeeyes/platform/icons/hicolor/24x24/status/safeeyes_enabled.png
-safeeyes/platform/icons/hicolor/24x24/status/safeeyes_timer.png
-safeeyes/platform/icons/hicolor/32x32/apps/safeeyes.png
-safeeyes/platform/icons/hicolor/32x32/status/safeeyes_disabled.png
-safeeyes/platform/icons/hicolor/32x32/status/safeeyes_enabled.png
-safeeyes/platform/icons/hicolor/48x48/apps/safeeyes.png
-safeeyes/platform/icons/hicolor/48x48/status/safeeyes_disabled.png
-safeeyes/platform/icons/hicolor/48x48/status/safeeyes_enabled.png
-safeeyes/platform/icons/hicolor/64x64/apps/safeeyes.png
+safeeyes/platform/io.github.slgobinath.SafeEyes.desktop
+safeeyes/platform/io.github.slgobinath.SafeEyes.metainfo.xml
+safeeyes/platform/icons/hicolor/128x128/apps/io.github.slgobinath.SafeEyes.png
+safeeyes/platform/icons/hicolor/16x16/apps/io.github.slgobinath.SafeEyes.png
+safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-disabled.png
+safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-enabled.png
+safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-timer.png
+safeeyes/platform/icons/hicolor/24x24/apps/io.github.slgobinath.SafeEyes.png
+safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-disabled.png
+safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-enabled.png
+safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-timer.png
+safeeyes/platform/icons/hicolor/32x32/apps/io.github.slgobinath.SafeEyes.png
+safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-disabled.png
+safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-enabled.png
+safeeyes/platform/icons/hicolor/48x48/apps/io.github.slgobinath.SafeEyes.png
+safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-disabled.png
+safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-enabled.png
+safeeyes/platform/icons/hicolor/64x64/apps/io.github.slgobinath.SafeEyes.png
 safeeyes/plugins/audiblealert/config.json
 safeeyes/plugins/audiblealert/icon.png
 safeeyes/plugins/audiblealert/plugin.py
 safeeyes/plugins/donotdisturb/config.json
 safeeyes/plugins/donotdisturb/dependency_checker.py
 safeeyes/plugins/donotdisturb/icon.png
 safeeyes/plugins/donotdisturb/plugin.py
```

### Comparing `safeeyes-2.1.5/setup.py` & `safeeyes-2.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,25 +37,25 @@
 
 
 def __data_files():
     """
     Collect the data files.
     """
     root_dir = sys.prefix
-    return [(os.path.join(root_dir, "share/applications"), ["safeeyes/platform/safeeyes.desktop"]),
-    (os.path.join(root_dir, "share/icons/hicolor/24x24/status"), ["safeeyes/platform/icons/hicolor/24x24/status/safeeyes_disabled.png", "safeeyes/platform/icons/hicolor/24x24/status/safeeyes_enabled.png", "safeeyes/platform/icons/hicolor/24x24/status/safeeyes_timer.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/24x24/apps"), ["safeeyes/platform/icons/hicolor/24x24/apps/safeeyes.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/16x16/status"), ["safeeyes/platform/icons/hicolor/16x16/status/safeeyes_disabled.png", "safeeyes/platform/icons/hicolor/16x16/status/safeeyes_enabled.png", "safeeyes/platform/icons/hicolor/16x16/status/safeeyes_timer.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/16x16/apps"), ["safeeyes/platform/icons/hicolor/16x16/apps/safeeyes.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/32x32/status"), ["safeeyes/platform/icons/hicolor/32x32/status/safeeyes_disabled.png", "safeeyes/platform/icons/hicolor/32x32/status/safeeyes_enabled.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/32x32/apps"), ["safeeyes/platform/icons/hicolor/32x32/apps/safeeyes.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/64x64/apps"), ["safeeyes/platform/icons/hicolor/64x64/apps/safeeyes.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/128x128/apps"), ["safeeyes/platform/icons/hicolor/128x128/apps/safeeyes.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/48x48/status"), ["safeeyes/platform/icons/hicolor/48x48/status/safeeyes_disabled.png", "safeeyes/platform/icons/hicolor/48x48/status/safeeyes_enabled.png"]),
-    (os.path.join(root_dir, "share/icons/hicolor/48x48/apps"), ["safeeyes/platform/icons/hicolor/48x48/apps/safeeyes.png"]),]
+    return [(os.path.join(root_dir, "share/applications"), ["safeeyes/platform/io.github.slgobinath.SafeEyes.desktop"]),
+    (os.path.join(root_dir, "share/icons/hicolor/24x24/status"), ["safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-disabled.png", "safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-enabled.png", "safeeyes/platform/icons/hicolor/24x24/status/io.github.slgobinath.SafeEyes-timer.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/24x24/apps"), ["safeeyes/platform/icons/hicolor/24x24/apps/io.github.slgobinath.SafeEyes.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/16x16/status"), ["safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-disabled.png", "safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-enabled.png", "safeeyes/platform/icons/hicolor/16x16/status/io.github.slgobinath.SafeEyes-timer.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/16x16/apps"), ["safeeyes/platform/icons/hicolor/16x16/apps/io.github.slgobinath.SafeEyes.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/32x32/status"), ["safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-disabled.png", "safeeyes/platform/icons/hicolor/32x32/status/io.github.slgobinath.SafeEyes-enabled.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/32x32/apps"), ["safeeyes/platform/icons/hicolor/32x32/apps/io.github.slgobinath.SafeEyes.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/64x64/apps"), ["safeeyes/platform/icons/hicolor/64x64/apps/io.github.slgobinath.SafeEyes.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/128x128/apps"), ["safeeyes/platform/icons/hicolor/128x128/apps/io.github.slgobinath.SafeEyes.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/48x48/status"), ["safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-disabled.png", "safeeyes/platform/icons/hicolor/48x48/status/io.github.slgobinath.SafeEyes-enabled.png"]),
+    (os.path.join(root_dir, "share/icons/hicolor/48x48/apps"), ["safeeyes/platform/icons/hicolor/48x48/apps/io.github.slgobinath.SafeEyes.png"]),]
 
 
 def __package_files(directory):
     """
     Collect the package files.
     """
     paths = []
@@ -74,22 +74,22 @@
     data.extend(__package_files('safeeyes/config'))
     data.extend(__package_files('safeeyes/plugins'))
     data.extend(__package_files('safeeyes/platform'))
     return data
 
 setuptools.setup(
     name="safeeyes",
-    version="2.1.5",
+    version="2.1.6",
     description="Protect your eyes from eye strain using this continuous breaks reminder.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Gobinath Loganathan",
     author_email="slgobinath@gmail.com",
     url="https://github.com/slgobinath/SafeEyes",
-    download_url="https://github.com/slgobinath/SafeEyes/archive/v2.1.5.tar.gz",
+    download_url="https://github.com/slgobinath/SafeEyes/archive/v2.1.6.tar.gz",
     packages=setuptools.find_packages(),
     package_data={'safeeyes': __package_data()},
     data_files=__data_files(),
     install_requires=requires,
     entry_points={'console_scripts': ['safeeyes = safeeyes.__main__:main']},
     keywords='linux utility health eye-strain safe-eyes',
     classifiers=[
```

