# Comparing `tmp/wxm_example-0.0.3.tar.gz` & `tmp/wxm_example-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wxm_example-0.0.3.tar", last modified: Tue Jan 31 12:10:51 2023, max compression
+gzip compressed data, last modified: Wed Jul  5 08:39:25 2023, from Unix
```

## Comparing `wxm_example-0.0.3.tar` & `wxm_example-0.0.31.tar`

### file list

```diff
@@ -1,12 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 12:10:51.000000 wxm_example-0.0.3/
--rw-rw-rw-   0        0        0      195 2023-01-31 12:10:51.000000 wxm_example-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-01-31 12:10:51.000000 wxm_example-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      124 2023-01-31 12:10:36.000000 wxm_example-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example/
--rw-rw-rw-   0        0        0        0 2023-01-31 07:50:48.000000 wxm_example-0.0.3/wxm_example/__init__.py
--rw-rw-rw-   0        0        0      171 2023-01-31 11:54:44.000000 wxm_example-0.0.3/wxm_example/fig.py
-drwxrwxrwx   0        0        0        0 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example.egg-info/
--rw-rw-rw-   0        0        0      195 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-01-31 12:10:51.000000 wxm_example-0.0.3/wxm_example.egg-info/top_level.txt
+-rwxr-xr-x   0 chaihj15   (501) staff       (20)      220 2023-07-05 08:37:02.000000 ./dist/._wxm_example-0.0.4
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 08:37:02.525360 ./dist/wxm_example-0.0.4/
+-rw-r--r--   0 chaihj15   (501) staff       (20)      484 2023-07-05 08:37:02.000000 ./dist/wxm_example-0.0.4/._PKG-INFO
+-rw-r--r--   0 chaihj15   (501) staff       (20)      136 2023-07-05 08:37:02.386726 ./dist/wxm_example-0.0.4/PKG-INFO
+-rw-r--r--   0 chaihj15   (501) staff       (20)       86 2023-07-05 08:36:09.000000 ./dist/wxm_example-0.0.4/setup.py
+drwxr-xr-x   0 chaihj15   (501) staff       (20)        0 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/wxm_example.egg-info/
+-rw-r--r--   0 chaihj15   (501) staff       (20)       38 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/setup.cfg
+-rw-r--r--   0 chaihj15   (501) staff       (20)      136 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/wxm_example.egg-info/PKG-INFO
+-rw-r--r--   0 chaihj15   (501) staff       (20)      148 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/wxm_example.egg-info/SOURCES.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/wxm_example.egg-info/top_level.txt
+-rw-r--r--   0 chaihj15   (501) staff       (20)        1 2023-07-05 08:36:37.000000 ./dist/wxm_example-0.0.4/wxm_example.egg-info/dependency_links.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

