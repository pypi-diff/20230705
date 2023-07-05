# Comparing `tmp/kero-0.0.0.post1.tar.gz` & `tmp/kero-0.0.0.post2.tar.gz`

## Comparing `kero-0.0.0.post1.tar` & `kero-0.0.0.post2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 kero-0.0.0.post1/.gitattributes
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 kero-0.0.0.post1/env.yml
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kero-0.0.0.post1/projects/_tests01.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kero-0.0.0.post1/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kero-0.0.0.post1/src/kero/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 kero-0.0.0.post1/src/kero/dummy.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 kero-0.0.0.post1/src/kero/utils.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 kero-0.0.0.post1/LICENSE
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 kero-0.0.0.post1/README.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 kero-0.0.0.post1/pyproject.toml
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 kero-0.0.0.post1/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 kero-0.0.0.post2/.gitattributes
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 kero-0.0.0.post2/env.yml
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kero-0.0.0.post2/projects/_tests01.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 kero-0.0.0.post2/projects/dataframeutest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/kero/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/kero/directory.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/kero/dummy.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/kero/pandas.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 kero-0.0.0.post2/src/kero/utils.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 kero-0.0.0.post2/LICENSE
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 kero-0.0.0.post2/README.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 kero-0.0.0.post2/pyproject.toml
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 kero-0.0.0.post2/PKG-INFO
```

### Comparing `kero-0.0.0.post1/projects/_tests01.py` & `kero-0.0.0.post2/projects/_tests01.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 """ Assume code is executed in "projects" folder.
-python _tests01.py --TOGGLES 1
+python _tests01.py --TOGGLES 11
 """
 
 import argparse
 
 def test_dummy_df(parser):
+    # python _tests01.py --TOGGLES 10
     parser.add_argument('--n', default=77, type=int, help=None)
     args, unknown = parser.parse_known_args()
     kwargs = vars(args)  # is a dictionary    
 
     import kero.dummy
-    df = kero.dummy.get_df(kwargs['n'], selection="01")
+    df = kero.dummy.get_random_dataframe(kwargs['n'], selection="01")
     print('='*47)
     print(df)
 
     import kero.dummy as kdum
-    df2 = kdum.get_df(4, selection="01")
+    df2 = kdum.get_random_dataframe(4, selection="01")
     print('\n','='*47)
     print(df2)
 
-    from kero.dummy import get_df
+    from kero.dummy import get_random_dataframe
     print('\n','='*47)
-    print(get_df(2, selection="01"))
+    print(get_random_dataframe(2, selection="01"))
+
+def test_dummy_df2(parser):
+    # python _tests01.py --TOGGLES 01
+    parser.add_argument('--n', default=77, type=int, help=None)
+    args, unknown = parser.parse_known_args()
+    kwargs = vars(args)  # is a dictionary    
+
+    from kero.dummy import get_random_dataframe
+    df = get_random_dataframe(kwargs['n'],nx=2,nt=3, selection="02")
+    print(df)
 
 if __name__=='__main__':
     parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=None)
     parser.add_argument('--TOGGLES', default='1', type=str, help=None)
     # parser.add_argument('-m','--mode', default=None, type=str, help=None)
     # parser.add_argument('--id', nargs='+', default=['a','b']) # for list args
     args, unknown = parser.parse_known_args()
     kwargs = vars(args)  # is a dictionary    
 
     TOGGLES = kwargs['TOGGLES']
     if TOGGLES[0] == '1':
         test_dummy_df(parser)
+    if len(TOGGLES)<=1: exit()
+    
+    if TOGGLES[1] == '1':
+        test_dummy_df2(parser)
+    if len(TOGGLES)<=2: exit()
```

### Comparing `kero-0.0.0.post1/LICENSE` & `kero-0.0.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `kero-0.0.0.post1/pyproject.toml` & `kero-0.0.0.post2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "kero"
-version = "0.0.0-1"
+version = "0.0.0-2"
 authors = [
   {name="Erico Tjoa", email="ericotjoa@gmail.com"},
 ]
 description = "Utilities and things."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

