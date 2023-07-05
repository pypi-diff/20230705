# Comparing `tmp/Finance-JindowinDate-0.0.2.tar.gz` & `tmp/Finance-JindowinDate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-JindowinDate-0.0.2.tar", last modified: Wed Jul  5 01:56:58 2023, max compression
+gzip compressed data, was "dist/Finance-JindowinDate-0.0.3.tar", last modified: Wed Jul  5 02:03:34 2023, max compression
```

## Comparing `Finance-JindowinDate-0.0.2.tar` & `Finance-JindowinDate-0.0.3.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1560 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-07-05 01:51:33.000000 Finance-JindowinDate-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 14:40:11.000000 Finance-JindowinDate-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/jdwdate/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/
--rw-r--r--   0 root         (0) root         (0)  1847734 2023-07-05 00:26:50.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.c
--rw-r--r--   0 root         (0) root         (0)      869 2023-07-04 15:00:48.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.pxd
--rw-r--r--   0 root         (0) root         (0)    37298 2023-07-05 00:26:46.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.pyx
--rw-r--r--   0 root         (0) root         (0)   498491 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Date.c
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Date.pxd
--rw-r--r--   0 root         (0) root         (0)    14615 2023-07-04 15:02:17.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Date.pyx
--rw-r--r--   0 root         (0) root         (0)     4418 2023-07-04 15:02:52.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/DayCounter.py
--rw-r--r--   0 root         (0) root         (0)   362552 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Period.c
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Period.pxd
--rw-r--r--   0 root         (0) root         (0)     9991 2023-07-04 15:03:01.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Period.pyx
--rw-r--r--   0 root         (0) root         (0)   500811 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.c
--rw-r--r--   0 root         (0) root         (0)      755 2023-07-04 15:03:24.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.pxd
--rw-r--r--   0 root         (0) root         (0)    14669 2023-07-04 15:04:06.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.pyx
--rw-r--r--   0 root         (0) root         (0)      415 2023-07-04 14:54:08.000000 Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/
--rw-r--r--   0 root         (0) root         (0)   306528 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/BizDayConventions.c
--rw-r--r--   0 root         (0) root         (0)      400 2023-07-04 15:04:40.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/BizDayConventions.pyx
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Compoundings.py
--rw-r--r--   0 root         (0) root         (0)   287528 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/DateGeneration.c
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-04 15:04:48.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/DateGeneration.pyx
--rw-r--r--   0 root         (0) root         (0)      250 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Factors.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Frequencies.py
--rw-r--r--   0 root         (0) root         (0)   320331 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Months.c
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-04 15:05:01.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Months.pyx
--rw-r--r--   0 root         (0) root         (0)   287248 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/NormalizingType.c
--rw-r--r--   0 root         (0) root         (0)       99 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/NormalizingType.pyx
--rw-r--r--   0 root         (0) root         (0)   282955 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/OptionType.c
--rw-r--r--   0 root         (0) root         (0)      142 2023-07-04 15:05:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/OptionType.pyx
--rw-r--r--   0 root         (0) root         (0)   294114 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/TimeUnits.c
--rw-r--r--   0 root         (0) root         (0)      206 2023-07-04 15:05:13.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/TimeUnits.pyx
--rw-r--r--   0 root         (0) root         (0)   302148 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Weekdays.c
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-04 15:05:18.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/Weekdays.pyx
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_BizDayConventions.pxd
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_DateGeneration.pxd
--rw-r--r--   0 root         (0) root         (0)      282 2023-07-04 15:04:27.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_Months.pxd
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_OptionType.pxd
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_TimeUnits.pxd
--rw-r--r--   0 root         (0) root         (0)      164 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/_Weekdays.pxd
--rw-r--r--   0 root         (0) root         (0)      561 2023-07-04 15:28:57.000000 Finance-JindowinDate-0.0.2/jdwdate/Enums/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/jdwdate/Env/
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-04 15:05:42.000000 Finance-JindowinDate-0.0.2/jdwdate/Env/Settings.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-04 14:55:24.000000 Finance-JindowinDate-0.0.2/jdwdate/Env/__init__.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 01:56:32.000000 Finance-JindowinDate-0.0.2/jdwdate/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/jdwdate/api/
--rw-r--r--   0 root         (0) root         (0)     3704 2023-07-04 23:22:51.000000 Finance-JindowinDate-0.0.2/jdwdate/api/DateUtilities.py
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-04 15:18:53.000000 Finance-JindowinDate-0.0.2/jdwdate/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-05 01:56:58.000000 Finance-JindowinDate-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3483 2023-07-04 15:23:46.000000 Finance-JindowinDate-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-05 02:00:31.000000 Finance-JindowinDate-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-04 14:40:11.000000 Finance-JindowinDate-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/jdwdate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/
+-rw-r--r--   0 root         (0) root         (0)  1847734 2023-07-05 00:26:50.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.c
+-rw-r--r--   0 root         (0) root         (0)      869 2023-07-04 15:00:48.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.pxd
+-rw-r--r--   0 root         (0) root         (0)    37298 2023-07-05 00:26:46.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.pyx
+-rw-r--r--   0 root         (0) root         (0)   498491 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Date.c
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Date.pxd
+-rw-r--r--   0 root         (0) root         (0)    14615 2023-07-04 15:02:17.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Date.pyx
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-07-04 15:02:52.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/DayCounter.py
+-rw-r--r--   0 root         (0) root         (0)   362552 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Period.c
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Period.pxd
+-rw-r--r--   0 root         (0) root         (0)     9991 2023-07-04 15:03:01.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Period.pyx
+-rw-r--r--   0 root         (0) root         (0)   500811 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.c
+-rw-r--r--   0 root         (0) root         (0)      755 2023-07-04 15:03:24.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.pxd
+-rw-r--r--   0 root         (0) root         (0)    14669 2023-07-04 15:04:06.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.pyx
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-04 14:54:08.000000 Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/
+-rw-r--r--   0 root         (0) root         (0)   306528 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/BizDayConventions.c
+-rw-r--r--   0 root         (0) root         (0)      400 2023-07-04 15:04:40.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/BizDayConventions.pyx
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Compoundings.py
+-rw-r--r--   0 root         (0) root         (0)   287528 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/DateGeneration.c
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-04 15:04:48.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/DateGeneration.pyx
+-rw-r--r--   0 root         (0) root         (0)      250 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Factors.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Frequencies.py
+-rw-r--r--   0 root         (0) root         (0)   320331 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Months.c
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-04 15:05:01.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Months.pyx
+-rw-r--r--   0 root         (0) root         (0)   287248 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/NormalizingType.c
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/NormalizingType.pyx
+-rw-r--r--   0 root         (0) root         (0)   282955 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/OptionType.c
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-04 15:05:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/OptionType.pyx
+-rw-r--r--   0 root         (0) root         (0)   294114 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/TimeUnits.c
+-rw-r--r--   0 root         (0) root         (0)      206 2023-07-04 15:05:13.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/TimeUnits.pyx
+-rw-r--r--   0 root         (0) root         (0)   302148 2023-07-04 15:24:05.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Weekdays.c
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-04 15:05:18.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/Weekdays.pyx
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_BizDayConventions.pxd
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_DateGeneration.pxd
+-rw-r--r--   0 root         (0) root         (0)      282 2023-07-04 15:04:27.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_Months.pxd
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_OptionType.pxd
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_TimeUnits.pxd
+-rw-r--r--   0 root         (0) root         (0)      164 2023-07-04 14:44:07.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/_Weekdays.pxd
+-rw-r--r--   0 root         (0) root         (0)      561 2023-07-04 15:28:57.000000 Finance-JindowinDate-0.0.3/jdwdate/Enums/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/jdwdate/Env/
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-04 15:05:42.000000 Finance-JindowinDate-0.0.3/jdwdate/Env/Settings.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-04 14:55:24.000000 Finance-JindowinDate-0.0.3/jdwdate/Env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 02:00:37.000000 Finance-JindowinDate-0.0.3/jdwdate/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/jdwdate/api/
+-rw-r--r--   0 root         (0) root         (0)     3704 2023-07-04 23:22:51.000000 Finance-JindowinDate-0.0.3/jdwdate/api/DateUtilities.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-07-04 15:18:53.000000 Finance-JindowinDate-0.0.3/jdwdate/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/requirements/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-07-04 15:23:03.000000 Finance-JindowinDate-0.0.3/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-05 02:03:34.000000 Finance-JindowinDate-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3483 2023-07-04 15:23:46.000000 Finance-JindowinDate-0.0.3/setup.py
```

### Comparing `Finance-JindowinDate-0.0.2/Finance_JindowinDate.egg-info/SOURCES.txt` & `Finance-JindowinDate-0.0.3/Finance_JindowinDate.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 jdwdate/Enums/_OptionType.pxd
 jdwdate/Enums/_TimeUnits.pxd
 jdwdate/Enums/_Weekdays.pxd
 jdwdate/Enums/__init__.py
 jdwdate/Env/Settings.py
 jdwdate/Env/__init__.py
 jdwdate/api/DateUtilities.py
-jdwdate/api/__init__.py
+jdwdate/api/__init__.py
+requirements/py3.txt
```

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.c` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.pxd` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.pxd`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Calendar.pyx` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Calendar.pyx`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Date.c` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Date.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Date.pyx` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Date.pyx`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/DayCounter.py` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/DayCounter.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Period.c` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Period.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Period.pyx` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Period.pyx`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.c` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.pxd` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.pxd`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/DateUtilities/Schedule.pyx` & `Finance-JindowinDate-0.0.3/jdwdate/DateUtilities/Schedule.pyx`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/BizDayConventions.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/BizDayConventions.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/DateGeneration.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/DateGeneration.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/Months.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/Months.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/NormalizingType.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/NormalizingType.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/OptionType.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/OptionType.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/TimeUnits.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/TimeUnits.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/Weekdays.c` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/Weekdays.c`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Enums/__init__.py` & `Finance-JindowinDate-0.0.3/jdwdate/Enums/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/Env/Settings.py` & `Finance-JindowinDate-0.0.3/jdwdate/Env/Settings.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/api/DateUtilities.py` & `Finance-JindowinDate-0.0.3/jdwdate/api/DateUtilities.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/jdwdate/api/__init__.py` & `Finance-JindowinDate-0.0.3/jdwdate/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-JindowinDate-0.0.2/setup.py` & `Finance-JindowinDate-0.0.3/setup.py`

 * *Files identical despite different names*

