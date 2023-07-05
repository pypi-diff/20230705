# Comparing `tmp/irene_pro-0.0.82.tar.gz` & `tmp/irene_pro-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.82.tar", last modified: Wed Jul  5 12:29:54 2023, max compression
+gzip compressed data, was "irene_pro-0.0.83.tar", last modified: Wed Jul  5 13:29:36 2023, max compression
```

## Comparing `irene_pro-0.0.82.tar` & `irene_pro-0.0.83.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 12:29:54.211655 irene_pro-0.0.82/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.82/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.82/MANIFEST.in
--rw-rw-rw-   0        0        0     1280 2023-07-05 12:29:54.210658 irene_pro-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.82/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 12:29:54.022365 irene_pro-0.0.82/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.82/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8171 2023-07-05 12:28:28.000000 irene_pro-0.0.82/irene_pro/logics.py
--rw-rw-rw-   0        0        0    35748 2023-07-05 08:54:43.000000 irene_pro-0.0.82/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-05 12:29:54.206669 irene_pro-0.0.82/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1280 2023-07-05 12:29:53.000000 irene_pro-0.0.82/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-05 12:29:53.000000 irene_pro-0.0.82/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 12:29:53.000000 irene_pro-0.0.82/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-05 12:29:53.000000 irene_pro-0.0.82/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 12:29:53.000000 irene_pro-0.0.82/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 12:29:54.212653 irene_pro-0.0.82/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-07-05 12:28:59.000000 irene_pro-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:29:36.827701 irene_pro-0.0.83/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.0.83/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.0.83/MANIFEST.in
+-rw-rw-rw-   0        0        0     1280 2023-07-05 13:29:36.826702 irene_pro-0.0.83/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.0.83/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 13:29:36.584879 irene_pro-0.0.83/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.0.83/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8171 2023-07-05 12:28:28.000000 irene_pro-0.0.83/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    35791 2023-07-05 13:27:38.000000 irene_pro-0.0.83/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-05 13:29:36.823711 irene_pro-0.0.83/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1280 2023-07-05 13:29:36.000000 irene_pro-0.0.83/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-05 13:29:36.000000 irene_pro-0.0.83/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 13:29:36.000000 irene_pro-0.0.83/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-05 13:29:36.000000 irene_pro-0.0.83/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-05 13:29:36.000000 irene_pro-0.0.83/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 13:29:36.827701 irene_pro-0.0.83/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-07-05 13:28:27.000000 irene_pro-0.0.83/setup.py
```

### Comparing `irene_pro-0.0.82/PKG-INFO` & `irene_pro-0.0.83/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene_pro
-Version: 0.0.82
+Name: irene-pro
+Version: 0.0.83
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.82/README.md` & `irene_pro-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.82/irene_pro/logics.py` & `irene_pro-0.0.83/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.82/irene_pro/widgets.py` & `irene_pro-0.0.83/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,17 +474,17 @@
         return self.Scrol_frame
 
 class label(Label):
     def __init__(self, master, **kwargs):
         super().__init__(master=master, font = ('arial', w(12)), bg = master['bg'], **kwargs)
 
 class Textb(Text):
-    def __init__(self, master, hbg = "gray80", default = None, **kwargs):
+    def __init__(self, master, hbg = "gray80", default = None, keep_default = False, **kwargs):
         super().__init__(master, font = ('arial', w(12)), highlightbackground=hbg, highlightcolor=hbg, highlightthickness=1, bg = master['bg'],fg = "gray30", bd = 0, **kwargs)
-        if default:
+        if default and not keep_default:
             self.bind("<KeyPress>", lambda e: remove_txt())
             self.bind("<Leave>", lambda e: add_txt())
 
             self.delete(0.0, END)
             self.insert(END, default)
             
         def remove_txt():
```

### Comparing `irene_pro-0.0.82/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.83/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene-pro
-Version: 0.0.82
+Name: irene_pro
+Version: 0.0.83
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.82/setup.py` & `irene_pro-0.0.83/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3832 270d 0a44 4553 4352   '0.0.82'..DESCR
+00000100: 2027 302e 302e 3833 270d 0a44 4553 4352   '0.0.83'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

