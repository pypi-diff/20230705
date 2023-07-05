# Comparing `tmp/crc8-0.1.0.tar.gz` & `tmp/crc8-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crc8-0.1.0.tar", last modified: Fri Nov  1 19:51:57 2019, max compression
+gzip compressed data, was "crc8-0.2.0.tar", last modified: Wed Jul  5 12:51:21 2023, max compression
```

## Comparing `crc8-0.1.0.tar` & `crc8-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 19:51:57.000000 crc8-0.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2019-11-01 19:51:57.000000 crc8-0.1.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6151 2019-11-01 19:51:39.000000 crc8-0.1.0/crc8.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-01 19:51:57.000000 crc8-0.1.0/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2739 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      162 2019-11-01 19:51:57.000000 crc8-0.1.0/crc8.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1353 2019-11-01 19:51:39.000000 crc8-0.1.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4783 2019-11-01 19:51:39.000000 crc8-0.1.0/setup.py
+drwxrwxr-x   0 sabin     (1000) sabin     (1000)        0 2023-07-05 12:51:21.077939 crc8-0.2.0/
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     1081 2023-07-05 12:31:34.000000 crc8-0.2.0/LICENSE
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     2580 2023-07-05 12:51:21.077939 crc8-0.2.0/PKG-INFO
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     1631 2023-07-05 12:47:55.000000 crc8-0.2.0/README.rst
+drwxrwxr-x   0 sabin     (1000) sabin     (1000)        0 2023-07-05 12:51:21.077939 crc8-0.2.0/crc8.egg-info/
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     2580 2023-07-05 12:51:20.000000 crc8-0.2.0/crc8.egg-info/PKG-INFO
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)      170 2023-07-05 12:51:20.000000 crc8-0.2.0/crc8.egg-info/SOURCES.txt
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)        1 2023-07-05 12:51:20.000000 crc8-0.2.0/crc8.egg-info/dependency_links.txt
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)        5 2023-07-05 12:51:20.000000 crc8-0.2.0/crc8.egg-info/top_level.txt
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)        1 2023-07-05 12:36:11.000000 crc8-0.2.0/crc8.egg-info/zip-safe
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     6316 2023-07-05 12:32:23.000000 crc8-0.2.0/crc8.py
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)       38 2023-07-05 12:51:21.077939 crc8-0.2.0/setup.cfg
+-rw-rw-r--   0 sabin     (1000) sabin     (1000)     4783 2023-07-05 12:31:34.000000 crc8-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crc8-0.1.0/crc8.py` & `crc8-0.2.0/crc8.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 and gave credit "From the PyPy project" and the link
     http://snippets.dzone.com/posts/show/3543
 
 """
 import sys
 
 __author__="Nicco Kunzmann"
-__version__="0.1.0"
+__version__="0.2.0"
 
 PY2 = sys.version_info[0] == 2
 
 
 class crc8(object):
 
     digest_size = 1
@@ -76,14 +76,15 @@
                 0x96, 0x91, 0x98, 0x9f, 0x8a, 0x8d, 0x84, 0x83,
                 0xde, 0xd9, 0xd0, 0xd7, 0xc2, 0xc5, 0xcc, 0xcb,
                 0xe6, 0xe1, 0xe8, 0xef, 0xfa, 0xfd, 0xf4, 0xf3]
 
     def __init__(self, initial_string=b'', initial_start=0x00):
         """Create a new crc8 hash instance."""
         self._sum = initial_start
+        self._initial_start = initial_start
         self._update(initial_string)
 
     def update(self, bytes_):
         """Update the hash object with the string arg.
 
         Repeated calls are equivalent to a single call with the concatenation
         of all the arguments: m.update(a); m.update(b) is equivalent
@@ -144,8 +145,12 @@
         This can be used to efficiently compute the digests of strings that
         share a common initial substring.
         """
         crc = crc8()
         crc._sum = self._sum
         return crc
 
+    def reset(self):
+        """Resets the hash object to its initial state."""
+        self._sum = self._initial_start
+
 __all__ = ['crc8']
```

### Comparing `crc8-0.1.0/README.rst` & `crc8-0.2.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -39,18 +39,34 @@
 .. code:: python
 
     import crc8
     hash = crc8.crc8()
     hash.update(b'123')
     assert hash.hexdigest() == 'c0'
     assert hash.digest() == b'\xc0'
+    hash.reset()
+    assert hash.hexdigest() == '00'
 
 Contribute
 ----------
 
 If something s not there that you would like to have, 
 `open an issue <https://github.com/niccokunzmann/crc8/issues>`__, 
 `create a pull request <https://github.com/niccokunzmann/crc8/pulls>`__.
 
 The license is `MIT
 <https://github.com/niccokunzmann/crc8/blob/master/LICENSE>`__ and
 I value contributions if you modify the code.
+
+
+Release
+-------
+
+Install `twine <https://twine.readthedocs.io/en/stable/>`_.
+
+.. code:: sh
+
+    python setup.py sdist
+    source .env # if you have stored TWINE_USERNAME and TWINE_PASSWORD
+    twine upload dist/*
+    
+
```

### Comparing `crc8-0.1.0/setup.py` & `crc8-0.2.0/setup.py`

 * *Files identical despite different names*

