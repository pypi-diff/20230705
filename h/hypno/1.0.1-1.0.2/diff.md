# Comparing `tmp/hypno-1.0.1.tar.gz` & `tmp/hypno-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypno-1.0.1.tar", last modified: Sun Jul  2 23:11:44 2023, max compression
+gzip compressed data, was "hypno-1.0.2.tar", last modified: Tue Jul  4 22:34:10 2023, max compression
```

## Comparing `hypno-1.0.1.tar` & `hypno-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 23:11:44.846482 hypno-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-07-02 23:10:06.000000 hypno-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       29 2023-07-02 23:10:06.000000 hypno-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2389 2023-07-02 23:11:44.846482 hypno-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1528 2023-07-02 23:10:06.000000 hypno-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 23:11:44.841269 hypno-1.0.1/hypno/
--rw-rw-rw-   0        0        0       50 2023-07-02 23:10:06.000000 hypno-1.0.1/hypno/__init__.py
--rw-rw-rw-   0        0        0      675 2023-07-02 23:10:06.000000 hypno-1.0.1/hypno/__main__.py
--rw-rw-rw-   0        0        0     2185 2023-07-02 23:10:06.000000 hypno-1.0.1/hypno/api.py
--rw-rw-rw-   0        0        0     1009 2023-07-02 23:10:06.000000 hypno-1.0.1/hypno/injection.c
-drwxrwxrwx   0        0        0        0 2023-07-02 23:11:44.845441 hypno-1.0.1/hypno.egg-info/
--rw-rw-rw-   0        0        0     2389 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-02 23:10:47.000000 hypno-1.0.1/hypno.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-02 23:11:44.000000 hypno-1.0.1/hypno.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      948 2023-07-02 23:11:44.846482 hypno-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      203 2023-07-02 23:10:06.000000 hypno-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-02 23:11:44.845441 hypno-1.0.1/tests/
--rw-rw-rw-   0        0        0     1114 2023-07-02 23:10:06.000000 hypno-1.0.1/tests/test_hypno.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.568107 hypno-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-04 22:32:36.000000 hypno-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       29 2023-07-04 22:32:36.000000 hypno-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2706 2023-07-04 22:34:10.568107 hypno-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1793 2023-07-04 22:32:36.000000 hypno-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.562203 hypno-1.0.2/hypno/
+-rw-rw-rw-   0        0        0       50 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/__init__.py
+-rw-rw-rw-   0        0        0      675 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/__main__.py
+-rw-rw-rw-   0        0        0     2636 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/api.py
+-rw-rw-rw-   0        0        0     1054 2023-07-04 22:32:36.000000 hypno-1.0.2/hypno/injection.c
+drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.566821 hypno-1.0.2/hypno.egg-info/
+-rw-rw-rw-   0        0        0     2706 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-04 22:33:30.000000 hypno-1.0.2/hypno.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-04 22:34:10.000000 hypno-1.0.2/hypno.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      989 2023-07-04 22:34:10.570202 hypno-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-07-04 22:32:36.000000 hypno-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-04 22:34:10.568107 hypno-1.0.2/tests/
+-rw-rw-rw-   0        0        0     1114 2023-07-04 22:32:36.000000 hypno-1.0.2/tests/test_hypno.py
```

### Comparing `hypno-1.0.1/LICENSE.txt` & `hypno-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hypno-1.0.1/PKG-INFO` & `hypno-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 
 # Hypno
 
@@ -54,7 +55,12 @@
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
 injects it with another print statement using hypno.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
+
+### Security
+Hypno briefly generates a temporary file containing the requested python code.
+This file is given 644 permissions by default, which means all users can read it.
+To use custom permissions, you can pass the `permissions` argument to `inject_py()`.
```

### Comparing `hypno-1.0.1/README.md` & `hypno-1.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -33,7 +33,12 @@
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
 injects it with another print statement using hypno.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
+
+### Security
+Hypno briefly generates a temporary file containing the requested python code.
+This file is given 644 permissions by default, which means all users can read it.
+To use custom permissions, you can pass the `permissions` argument to `inject_py()`.
```

### Comparing `hypno-1.0.1/hypno/__main__.py` & `hypno-1.0.2/hypno/__main__.py`

 * *Files identical despite different names*

### Comparing `hypno-1.0.1/hypno/api.py` & `hypno-1.0.2/hypno/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-import os
+import sys
 from importlib.util import find_spec
 from typing import AnyStr
 from pyinjector import inject, InjectorError
 from tempfile import NamedTemporaryFile
 from pathlib import Path
 
 
 INJECTION_LIB_PATH = Path(find_spec('.injection', __package__).origin)
 MAGIC = b'--- hypno code start ---'
-WINDOWS = os.name == 'nt'
+WINDOWS = sys.platform == 'win32'
 
 
 class CodeTooLongException(Exception):
     def __init__(self, code: bytes, max_size: int):
         super().__init__(f'The given python code is too long ({len(code)}). The maximum length is {max_size}.\n'
                          f'Consider writing the code to a file and executing it with runpy.run_path.\n'
                          f'Also, please report this on https://github.com/kmaork/hypno/issues/new')
 
 
-def inject_py(pid: int, python_code: AnyStr) -> None:
+def inject_py(pid: int, python_code: AnyStr, permissions=0o644) -> None:
+    """
+    :param pid: PID of target python process
+    :param python_code: Python code to inject to the target process.
+    :param permissions: Permissions of the generated shared library file that will be injected to the target process.
+                        Make sure the file is readable from the target process. By default, all users can read the file.
+    """
     if isinstance(python_code, str):
         python_code = python_code.encode()
     lib = INJECTION_LIB_PATH.read_bytes()
     magic_addr = lib.find(MAGIC)
     code_addr = magic_addr - 1
     max_size_addr = magic_addr + len(MAGIC)
     max_size_end_addr = lib.find(b'\0', max_size_addr)
     max_size = int(lib[max_size_addr:max_size_end_addr])
     if len(python_code) > max_size:
         raise CodeTooLongException(python_code, max_size)
-    name = None
+    path = None
     try:
-        # Can't delete a loaded shared library on Windows
+        # delete=False because can't delete a loaded shared library on Windows
         with NamedTemporaryFile(prefix='hypno', suffix=INJECTION_LIB_PATH.suffix, delete=False) as temp:
-            name = temp.name
+            path = Path(temp.name)
             temp.write(lib[:code_addr])
             temp.write(python_code)
             temp.write(b'\0')
             temp.write(lib[code_addr + len(python_code) + 1:])
+        path.chmod(permissions)
         try:
             inject(pid, str(temp.name))
         except InjectorError as e:
             # On Windows we are failing the load on purpose so the library will be immediately unloaded
             if not WINDOWS or e.ret_val != -5 or e.error_str != \
                     "LoadLibrary in the target process failed: " \
                     "A dynamic link library (DLL) initialization routine failed.":
                 raise
     finally:
-        if name is not None and Path(name).exists():
-            Path(name).unlink()
+        if path is not None and path.exists():
+            path.unlink()
```

### Comparing `hypno-1.0.1/hypno/injection.c` & `hypno-1.0.2/hypno/injection.c`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 #ifdef _WIN32
     #include <windows.h>
 
     BOOL WINAPI DllMain(HINSTANCE hinstDLL, DWORD fdwReason, LPVOID lpReserved) {
         switch( fdwReason ) {
             case DLL_PROCESS_ATTACH:
                 run_python_code();
+                // "Failing" so the library is immediately unloaded
                 return FALSE;
-                break;
         }
         return TRUE;
     }
 #else
     __attribute__((constructor))
     static void init(void) {
         run_python_code();
```

### Comparing `hypno-1.0.1/hypno.egg-info/PKG-INFO` & `hypno-1.0.2/hypno.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hypno
-Version: 1.0.1
+Version: 1.0.2
 Summary: A tool/library allowing to inject python code into a running python process.
 Home-page: https://github.com/kmaork/hypno
 Author: Maor Kleinberger
 Author-email: kmaork@gmail.com
 Keywords: injection library
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE.txt
 
 # Hypno
 
@@ -54,7 +55,12 @@
 #### Example
 This example runs a python program that prints its pid, and then attaches to the newly created process and
 injects it with another print statement using hypno.
 ```shell script
 python -c "import os, time; print('Hello from', os.getpid()); time.sleep(0.5)" &\
 hypno $! "import os; print('Hello again from', os.getpid())"
 ```
+
+### Security
+Hypno briefly generates a temporary file containing the requested python code.
+This file is given 644 permissions by default, which means all users can read it.
+To use custom permissions, you can pass the `permissions` argument to `inject_py()`.
```

### Comparing `hypno-1.0.1/setup.cfg` & `hypno-1.0.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 00000020: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
 00000030: 3d33 2e37 0d0a 7061 636b 6167 6573 203d  =3.7..packages =
 00000040: 2068 7970 6e6f 0d0a 696e 7374 616c 6c5f   hypno..install_
 00000050: 7265 7175 6972 6573 203d 200d 0a09 7079  requires = ...py
 00000060: 696e 6a65 6374 6f72 3e3d 302e 312e 320d  injector>=0.1.2.
 00000070: 0a0d 0a5b 6d65 7461 6461 7461 5d0d 0a6e  ...[metadata]..n
 00000080: 616d 6520 3d20 6879 706e 6f0d 0a76 6572  ame = hypno..ver
-00000090: 7369 6f6e 203d 2031 2e30 2e31 0d0a 6465  sion = 1.0.1..de
+00000090: 7369 6f6e 203d 2031 2e30 2e32 0d0a 6465  sion = 1.0.2..de
 000000a0: 7363 7269 7074 696f 6e20 3d20 4120 746f  scription = A to
 000000b0: 6f6c 2f6c 6962 7261 7279 2061 6c6c 6f77  ol/library allow
 000000c0: 696e 6720 746f 2069 6e6a 6563 7420 7079  ing to inject py
 000000d0: 7468 6f6e 2063 6f64 6520 696e 746f 2061  thon code into a
 000000e0: 2072 756e 6e69 6e67 2070 7974 686f 6e20   running python 
 000000f0: 7072 6f63 6573 732e 0d0a 6175 7468 6f72  process...author
 00000100: 203d 204d 616f 7220 4b6c 6569 6e62 6572   = Maor Kleinber
@@ -46,15 +46,17 @@
 000002d0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 000002e0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 000002f0: 3a3a 2033 2e38 0d0a 0950 726f 6772 616d  :: 3.8...Program
 00000300: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 00000310: 2050 7974 686f 6e20 3a3a 2033 2e39 0d0a   Python :: 3.9..
 00000320: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
 00000330: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000340: 3a3a 2033 2e31 300d 0a09 546f 7069 6320  :: 3.10...Topic 
-00000350: 3a3a 2053 6f66 7477 6172 6520 4465 7665  :: Software Deve
-00000360: 6c6f 706d 656e 7420 3a3a 204c 6962 7261  lopment :: Libra
-00000370: 7269 6573 203a 3a20 5079 7468 6f6e 204d  ries :: Python M
-00000380: 6f64 756c 6573 0d0a 0d0a 5b65 6767 5f69  odules....[egg_i
-00000390: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000003a0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000003b0: 0d0a 0d0a                                ....
+00000340: 3a3a 2033 2e31 300d 0a09 5072 6f67 7261  :: 3.10...Progra
+00000350: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000360: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
+00000370: 0d0a 0954 6f70 6963 203a 3a20 536f 6674  ...Topic :: Soft
+00000380: 7761 7265 2044 6576 656c 6f70 6d65 6e74  ware Development
+00000390: 203a 3a20 4c69 6272 6172 6965 7320 3a3a   :: Libraries ::
+000003a0: 2050 7974 686f 6e20 4d6f 6475 6c65 730d   Python Modules.
+000003b0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000003c0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000003d0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `hypno-1.0.1/tests/test_hypno.py` & `hypno-1.0.2/tests/test_hypno.py`

 * *Files identical despite different names*

