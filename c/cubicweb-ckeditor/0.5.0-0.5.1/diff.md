# Comparing `tmp/cubicweb-ckeditor-0.5.0.tar.gz` & `tmp/cubicweb-ckeditor-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-ckeditor-0.5.0.tar", last modified: Mon Feb  6 09:57:13 2023, max compression
+gzip compressed data, was "cubicweb-ckeditor-0.5.1.tar", last modified: Wed Jul  5 12:17:53 2023, max compression
```

## Comparing `cubicweb-ckeditor-0.5.0.tar` & `cubicweb-ckeditor-0.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      684 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.093607 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/data/
--rw-rw-rw-   0 root         (0) root         (0)     1284 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/data/ckeditor-config.js
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/data/initwysiwyg.js
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      684 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      778 2023-02-06 09:57:13.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       36 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-02-06 09:57:12.000000 cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2650 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 09:57:13.097607 cubicweb-ckeditor-0.5.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     2519 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/test/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/test/test_ckeditor.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-02-06 09:57:00.000000 cubicweb-ckeditor-0.5.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.246258 cubicweb-ckeditor-0.5.1/
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-05 12:17:53.246258 cubicweb-ckeditor-0.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.238258 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/
+-rw-rw-rw-   0 root         (0) root         (0)     1532 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.242258 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/data/ckeditor-config.js
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/data/initwysiwyg.js
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.242258 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.242258 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.242258 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      778 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-05 12:17:53.000000 cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 12:17:53.246258 cubicweb-ckeditor-0.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.246258 cubicweb-ckeditor-0.5.1/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 12:17:53.246258 cubicweb-ckeditor-0.5.1/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/test/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/test/test_ckeditor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-05 12:17:33.000000 cubicweb-ckeditor-0.5.1/tox.ini
```

### Comparing `cubicweb-ckeditor-0.5.0/PKG-INFO` & `cubicweb-ckeditor-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-ckeditor
-Version: 0.5.0
+Version: 0.5.1
 Summary: WYSIWYG js editor with ckeditor
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-ckeditor
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -18,9 +17,7 @@
 
 
 If don't want to use ckeditor from //cdn set following variables in
 uiprops of your main cube:
 
   CKEDITOR_URL = data('ckeditor/ckeditor.js')
   CKEDITOR_BASEPATH = data('ckeditor/')
-
-
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/__init__.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 WYSIWYG js editor with ckeditor
 """
 
 from logilab.common.decorators import monkeypatch, cached
 
 from cubicweb_web.webconfig import WebConfiguration
-from cubicweb_web.request import _CubicWebRequestBase
+from cubicweb_web.request import CubicWebRequestBase
 
 
-@monkeypatch(_CubicWebRequestBase)
+@monkeypatch(CubicWebRequestBase)
 @cached  # so it's writed only once
 def fckeditor_config(self):
     ckeditor_url = self.uiprops.get(
         "CKEDITOR_URL", "//cdn.ckeditor.com/4.5.7/standard/ckeditor.js"
     )
     self.add_js(ckeditor_url, localfile=False)
     self.add_js("initwysiwyg.js")
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/__pkginfo__.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/__pkginfo__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from os import listdir as _listdir
 from os.path import join, isdir
 from glob import glob
 
 modname = "ckeditor"
 distname = "cubicweb-ckeditor"
 
-numversion = (0, 5, 0)
+numversion = (0, 5, 1)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "WYSIWYG js editor with ckeditor"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {"cubicweb": ">= 3.38.0, < 3.39.0", "six": ">= 1.4.0"}
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/data/ckeditor-config.js` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/data/ckeditor-config.js`

 * *Files identical despite different names*

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/data/initwysiwyg.js` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/data/initwysiwyg.js`

 * *Files identical despite different names*

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/entities.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -11,8 +11,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""cubicweb-ckeditor entity's classes"""
+"""cubicweb-ckeditor specific hooks and operations"""
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/hooks.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -11,8 +11,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""cubicweb-ckeditor specific hooks and operations"""
+"""cubicweb-ckeditor schema"""
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/migration/postcreate.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/migration/postcreate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/schema.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -11,8 +11,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""cubicweb-ckeditor schema"""
+"""cubicweb-ckeditor views/forms/actions/components for web ui"""
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor/views.py` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
@@ -11,8 +11,8 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-"""cubicweb-ckeditor views/forms/actions/components for web ui"""
+"""cubicweb-ckeditor entity's classes"""
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/PKG-INFO` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-ckeditor
-Version: 0.5.0
+Version: 0.5.1
 Summary: WYSIWYG js editor with ckeditor
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-ckeditor
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -18,9 +17,7 @@
 
 
 If don't want to use ckeditor from //cdn set following variables in
 uiprops of your main cube:
 
   CKEDITOR_URL = data('ckeditor/ckeditor.js')
   CKEDITOR_BASEPATH = data('ckeditor/')
-
-
```

### Comparing `cubicweb-ckeditor-0.5.0/cubicweb_ckeditor.egg-info/SOURCES.txt` & `cubicweb-ckeditor-0.5.1/cubicweb_ckeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-ckeditor-0.5.0/setup.py` & `cubicweb-ckeditor-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # pylint: disable=W0142,W0403,W0404,W0613,W0622,W0622,W0704,R0904,C0103,E0611
 #
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of CubicWeb.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -52,17 +52,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{0} {1}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-ckeditor-0.5.0/test/pytestconf.py` & `cubicweb-ckeditor-0.5.1/test/pytestconf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of CubicWeb.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
```

### Comparing `cubicweb-ckeditor-0.5.0/test/test_ckeditor.py` & `cubicweb-ckeditor-0.5.1/test/test_ckeditor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2016-2022 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2016-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr -- mailto:contact@logilab.fr
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
 # any later version.
 #
```

### Comparing `cubicweb-ckeditor-0.5.0/tox.ini` & `cubicweb-ckeditor-0.5.1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     safety
 commands =
     safety check
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -65,8 +65,8 @@
 commands = black --check .
 
 [testenv:black-run]
 basepython = python3
 skip_install = true
 deps =
   black >= 22.12
-commands = black .
+commands = black .
```

