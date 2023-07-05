# Comparing `tmp/fuzzy-hash-0.0.2.tar.gz` & `tmp/fuzzy-hash-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuzzy-hash-0.0.2.tar", last modified: Fri Jun 30 11:05:42 2023, max compression
+gzip compressed data, was "dist/fuzzy-hash-0.0.3.tar", last modified: Wed Jul  5 03:30:42 2023, max compression
```

## Comparing `fuzzy-hash-0.0.2.tar` & `fuzzy-hash-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.695262 fuzzy-hash-0.0.2/
--rw-r--r--   0 guofei     (501) staff       (20)       26 2023-06-30 10:56:15.000000 fuzzy-hash-0.0.2/MANIFEST.in
--rw-r--r--   0 guofei     (501) staff       (20)      107 2023-06-30 11:05:42.695016 fuzzy-hash-0.0.2/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)     1898 2023-06-30 03:28:20.000000 fuzzy-hash-0.0.2/README.md
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.692405 fuzzy-hash-0.0.2/fuzzy_hash/
--rw-r--r--   0 guofei     (501) staff       (20)      711 2023-06-30 10:56:52.000000 fuzzy-hash-0.0.2/fuzzy_hash/__init__.py
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.694735 fuzzy-hash-0.0.2/fuzzy_hash/lib/
--rw-r--r--   0 guofei     (501) staff       (20)      270 2023-06-29 02:01:03.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/__init__.py
--rw-r--r--   0 guofei     (501) staff       (20)     2792 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.c
--rw-r--r--   0 guofei     (501) staff       (20)      497 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.h
--rw-r--r--   0 guofei     (501) staff       (20)    29209 2023-06-27 09:54:55.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.c
--rw-r--r--   0 guofei     (501) staff       (20)     8004 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.h
--rw-r--r--   0 guofei     (501) staff       (20)      220 2023-06-29 01:42:31.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/setup.py
--rw-r--r--   0 guofei     (501) staff       (20)    26778 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.2/fuzzy_hash/lib/sum_table.h
-drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-06-30 11:05:42.693257 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/
--rw-r--r--   0 guofei     (501) staff       (20)      107 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/PKG-INFO
--rw-r--r--   0 guofei     (501) staff       (20)      367 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/SOURCES.txt
--rw-r--r--   0 guofei     (501) staff       (20)        1 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/dependency_links.txt
--rw-r--r--   0 guofei     (501) staff       (20)       11 2023-06-30 11:05:42.000000 fuzzy-hash-0.0.2/fuzzy_hash.egg-info/top_level.txt
--rw-r--r--   0 guofei     (501) staff       (20)       38 2023-06-30 11:05:42.695340 fuzzy-hash-0.0.2/setup.cfg
--rw-r--r--   0 guofei     (501) staff       (20)      775 2023-06-30 11:05:26.000000 fuzzy-hash-0.0.2/setup.py
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-07-05 03:30:42.476640 fuzzy-hash-0.0.3/
+-rw-r--r--   0 guofei     (501) staff       (20)       26 2023-06-30 10:56:15.000000 fuzzy-hash-0.0.3/MANIFEST.in
+-rw-r--r--   0 guofei     (501) staff       (20)      107 2023-07-05 03:30:42.476480 fuzzy-hash-0.0.3/PKG-INFO
+-rw-r--r--   0 guofei     (501) staff       (20)     2123 2023-07-03 11:27:46.000000 fuzzy-hash-0.0.3/README.md
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-07-05 03:30:42.473856 fuzzy-hash-0.0.3/fuzzy_hash/
+-rw-r--r--   0 guofei     (501) staff       (20)      688 2023-07-03 11:27:29.000000 fuzzy-hash-0.0.3/fuzzy_hash/__init__.py
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-07-05 03:30:42.476118 fuzzy-hash-0.0.3/fuzzy_hash/lib/
+-rw-r--r--   0 guofei     (501) staff       (20)      270 2023-06-29 02:01:03.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/__init__.py
+-rw-r--r--   0 guofei     (501) staff       (20)     2449 2023-07-01 12:08:19.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/edit_dist.c
+-rw-r--r--   0 guofei     (501) staff       (20)      207 2023-07-01 12:08:19.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/edit_dist.h
+-rw-r--r--   0 guofei     (501) staff       (20)    28083 2023-07-01 12:08:19.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/fuzzy.c
+-rw-r--r--   0 guofei     (501) staff       (20)     6265 2023-07-01 12:08:19.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/fuzzy.h
+-rw-r--r--   0 guofei     (501) staff       (20)      220 2023-06-29 01:42:31.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/setup.py
+-rw-r--r--   0 guofei     (501) staff       (20)    26778 2023-06-25 07:21:36.000000 fuzzy-hash-0.0.3/fuzzy_hash/lib/sum_table.h
+drwxr-xr-x   0 guofei     (501) staff       (20)        0 2023-07-05 03:30:42.474507 fuzzy-hash-0.0.3/fuzzy_hash.egg-info/
+-rw-r--r--   0 guofei     (501) staff       (20)      107 2023-07-05 03:30:42.000000 fuzzy-hash-0.0.3/fuzzy_hash.egg-info/PKG-INFO
+-rw-r--r--   0 guofei     (501) staff       (20)      367 2023-07-05 03:30:42.000000 fuzzy-hash-0.0.3/fuzzy_hash.egg-info/SOURCES.txt
+-rw-r--r--   0 guofei     (501) staff       (20)        1 2023-07-05 03:30:42.000000 fuzzy-hash-0.0.3/fuzzy_hash.egg-info/dependency_links.txt
+-rw-r--r--   0 guofei     (501) staff       (20)       11 2023-07-05 03:30:42.000000 fuzzy-hash-0.0.3/fuzzy_hash.egg-info/top_level.txt
+-rw-r--r--   0 guofei     (501) staff       (20)       38 2023-07-05 03:30:42.476682 fuzzy-hash-0.0.3/setup.cfg
+-rw-r--r--   0 guofei     (501) staff       (20)      775 2023-07-05 03:30:36.000000 fuzzy-hash-0.0.3/setup.py
```

### Comparing `fuzzy-hash-0.0.2/README.md` & `fuzzy-hash-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # fuzzy-hash
 
 This project computes fuzzy hash.  
 
+## install
+
+
+If `gcc` is not installed, execute the following command to install `gcc`:
+
+```bach
+apt update
+apt install gcc -y
+```
+
+Then install `fuzzy-hash`
+```bash
+pip install fuzzy-hash
+```
 
 
 
 ```python
 from fuzzy_hash import fuzzy_hash, fuzzy_compare
 
 sentence = '''
@@ -19,16 +33,16 @@
 而《许你万家灯火》的创作题材，便是中国完全自主知识产权的三代核电技术——“华龙一号”。
 从核潜艇研发起步的中国核工业
 如何实现拥有世界一流核电站的梦想？
 '''
 sentence2 = sentence.replace('电视剧', '视频')
 sentence2 += "添加几句结尾"
 
-hash1 = fuzzy_hash(sentence)
-hash2 = fuzzy_hash(sentence2)
+hash1 = fuzzy_hash(sentence.encode('utf-8'))
+hash2 = fuzzy_hash(sentence2.encode('utf-8'))
 
 print(hash1)
 print(hash2)
 
 corr = fuzzy_compare(hash1, hash2)
 print('corr = {}%'.format(corr))
 ```
```

### Comparing `fuzzy-hash-0.0.2/fuzzy_hash/lib/edit_dist.c` & `fuzzy-hash-0.0.3/fuzzy_hash/lib/edit_dist.c`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-/**
- * Modified levenshtein distance calculation
- *
- * This program can be used, redistributed or modified under any of
- * Boost Software License 1.0, GPL v2 or GPL v3
- * See the file COPYING for details.
- *
- * $Id$
- *
- * Copyright (C) 2014 kikairoya <kikairoya@gmail.com>
- * Copyright (C) 2014 Jesse Kornblum <research@jessekornblum.com>
- */
 #include <stddef.h>
 
 #define EDIT_DISTN_MAXLEN 64 /* MAX_SPAMSUM */
 #define EDIT_DISTN_INSERT_COST 1
 #define EDIT_DISTN_REMOVE_COST 1
 #define EDIT_DISTN_REPLACE_COST 2
```

### Comparing `fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.c` & `fuzzy-hash-0.0.3/fuzzy_hash/lib/fuzzy.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-/* ssdeep
- * Copyright (C) 2002 Andrew Tridgell <tridge@samba.org>
- * Copyright (C) 2006 ManTech International Corporation
- * Copyright (C) 2013 Helmut Grohne <helmut@subdivi.de>
- * Copyright (C) 2017 Tsukasa OI <floss_ssdeep@irq.a4lg.com>
- *
- * This program is free software; you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation; either version 2 of the License, or
- * (at your option) any later version.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
- *
- * Earlier versions of this code were named fuzzy.c and can be found at:
- *     http://www.samba.org/ftp/unpacked/junkcode/spamsum/
- *     http://ssdeep.sf.net/
- */
-
 #ifndef MIN
 #define MIN(a, b) ((a)<(b)?(a):(b))
 #endif
 
 #ifndef MAX
 #define MAX(a, b) ((a)>(b)?(a):(b))
 #endif
```

### Comparing `fuzzy-hash-0.0.2/fuzzy_hash/lib/fuzzy.h` & `fuzzy-hash-0.0.3/fuzzy_hash/lib/fuzzy.h`

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,12 @@
 #ifndef FUZZY_H
 #define FUZZY_H
 
-/*
- * Copyright (C) ManTech International Corporation 2010
- * Copyright (C) Kyrus 2012
- * Copyright (C) 2013 Helmut Grohne <helmut@subdivi.de>
- *
- * $Id$
- *
- * This program is free software; you can redistribute it and/or modify
- * it under the terms of the GNU General Public License as published by
- * the Free Software Foundation; either version 2 of the License, or
- * (at your option) any later version.
- *
- * This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of
- * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
- * GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License
- * along with this program; if not, write to the Free Software
- * Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA  02110-1301  USA
- *
- * Earlier versions of this code can be found at:
- *     http://ssdeep.sf.net/
- */
-
-/// \mainpage
-/// This is the documentation for the fuzzy hashing API from ssdeep.
-///
-/// There is a complete function reference in fuzzy.h.
-///
-/// The most recent version of this documentation can be found
-/// at http://ssdeep.sourceforge.net/.
-///
-/// \copydoc fuzzy.h
-///
-/// \version 3.0
-///
-/// \author Jesse Kornblum, research@jessekornblum.com
-/// \author Helmut Grohne, helmut@subdivi.de
-
-/// \file fuzzy.h
-/// \brief
 /// These functions allow a programmer to compute the fuzzy hashes
-/// (also called the context-triggered piecewise hashes) of
-/// \link fuzzy_hash_buf() a buffer
-/// of text @endlink,
-/// \link fuzzy_hash_filename() the contents of a file on the disk @endlink,
-/// and
-/// @link fuzzy_hash_file() the contents of
-/// an open file handle @endlink .
-/// There is also a function to
-/// @link fuzzy_compare() compute the
-/// similarity between any two fuzzy signatures @endlink.
+/// (also called the context-triggered piecewise hashes)
 
 
 #include <stdint.h>
 #include <stdio.h>
 
 #ifdef __cplusplus
 extern "C" {
```

### Comparing `fuzzy-hash-0.0.2/fuzzy_hash/lib/sum_table.h` & `fuzzy-hash-0.0.3/fuzzy_hash/lib/sum_table.h`

 * *Files identical despite different names*

### Comparing `fuzzy-hash-0.0.2/setup.py` & `fuzzy-hash-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     with open(os.path.join(this_directory, filename), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
 setup(
     name='fuzzy-hash',
-    version='0.0.2',
+    version='0.0.3',
     python_requires='>=3.5',
     packages=find_packages(),
     ext_modules=[
         Extension(
             name="fuzzy_hash.lib.core",
             sources=[
                 'fuzzy_hash/lib/fuzzy.c',
                 'fuzzy_hash/lib/edit_dist.c',
             ])
     ],
-    description='fuzzy hash in python',
+    description='Fuzzy Hash in python',
     # long_description=read_file('README.md'),
 )
```

