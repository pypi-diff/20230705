# Comparing `tmp/Products.ExternalEditor-3.1.0.tar.gz` & `tmp/Products.ExternalEditor-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.ExternalEditor-3.1.0.tar", last modified: Fri Jun 24 08:04:53 2022, max compression
+gzip compressed data, was "Products.ExternalEditor-4.0.tar", last modified: Tue Jul  4 04:51:02 2023, max compression
```

## Comparing `Products.ExternalEditor-3.1.0.tar` & `Products.ExternalEditor-4.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.880961 Products.ExternalEditor-3.1.0/
--rw-r--r--   0 mac        (513) staff       (20)    11871 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)       62 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/CREDITS.txt
--rw-r--r--   0 mac        (513) staff       (20)      616 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/INSTALL.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      309 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    30845 2022-06-24 08:04:53.881201 Products.ExternalEditor-3.1.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)    17319 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      417 2022-06-24 08:04:53.882242 Products.ExternalEditor-3.1.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2232 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.859827 Products.ExternalEditor-3.1.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.869044 Products.ExternalEditor-3.1.0/src/Products/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.876205 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/
--rw-r--r--   0 mac        (513) staff       (20)    11973 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/ExternalEditor.py
--rw-r--r--   0 mac        (513) staff       (20)     2179 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)     1619 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)      207 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/client.txt
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.876791 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/dtml/
--rw-r--r--   0 mac        (513) staff       (20)     9262 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/dtml/findForm.dtml
--rw-r--r--   0 mac        (513) staff       (20)      502 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/edit_icon.gif
--rw-r--r--   0 mac        (513) staff       (20)     7371 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/findResult.dtml
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.879969 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/
--rw-r--r--   0 mac        (513) staff       (20)      642 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     8381 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/edit.txt
--rw-r--r--   0 mac        (513) staff       (20)     1706 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/link.txt
--rw-r--r--   0 mac        (513) staff       (20)     1439 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/test_functional.py
--rw-r--r--   0 mac        (513) staff       (20)      874 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/test_zmi.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.880563 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/zpt/
--rw-r--r--   0 mac        (513) staff       (20)    11597 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/zpt/main.zpt
--rw-r--r--   0 mac        (513) staff       (20)      244 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/src/Products/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-06-24 08:04:53.872983 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    30845 2022-06-24 08:04:52.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1086 2022-06-24 08:04:53.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-06-24 08:04:52.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2022-06-24 08:04:53.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-06-24 08:04:52.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       25 2022-06-24 08:04:53.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        9 2022-06-24 08:04:53.000000 Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1447 2022-06-24 08:04:50.000000 Products.ExternalEditor-3.1.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.213875 Products.ExternalEditor-4.0/
+-rw-r--r--   0 jens       (501) staff       (20)    12116 2023-07-04 04:47:08.000000 Products.ExternalEditor-4.0/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2023-07-03 10:08:01.000000 Products.ExternalEditor-4.0/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)       62 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/CREDITS.txt
+-rw-r--r--   0 jens       (501) staff       (20)      616 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/INSTALL.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      309 2023-07-03 10:08:01.000000 Products.ExternalEditor-4.0/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    30783 2023-07-04 04:51:02.213944 Products.ExternalEditor-4.0/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)    17319 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)      418 2023-07-04 04:51:02.214196 Products.ExternalEditor-4.0/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     1906 2023-07-04 04:47:14.000000 Products.ExternalEditor-4.0/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.209229 Products.ExternalEditor-4.0/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.211233 Products.ExternalEditor-4.0/src/Products/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.212824 Products.ExternalEditor-4.0/src/Products/ExternalEditor/
+-rw-r--r--   0 jens       (501) staff       (20)    11896 2023-07-04 04:42:51.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/ExternalEditor.py
+-rw-r--r--   0 jens       (501) staff       (20)     2179 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1619 2023-04-20 08:24:09.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      207 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/client.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.212969 Products.ExternalEditor-4.0/src/Products/ExternalEditor/dtml/
+-rw-r--r--   0 jens       (501) staff       (20)     9262 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/dtml/findForm.dtml
+-rw-r--r--   0 jens       (501) staff       (20)      502 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/edit_icon.gif
+-rw-r--r--   0 jens       (501) staff       (20)     7371 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/findResult.dtml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.213640 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/
+-rw-r--r--   0 jens       (501) staff       (20)      642 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     8381 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/edit.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1706 2021-11-02 08:51:30.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/link.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1439 2023-04-20 08:24:09.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/test_functional.py
+-rw-r--r--   0 jens       (501) staff       (20)      860 2023-04-20 08:24:09.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/test_zmi.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.213747 Products.ExternalEditor-4.0/src/Products/ExternalEditor/zpt/
+-rw-r--r--   0 jens       (501) staff       (20)    11597 2023-04-20 08:24:09.000000 Products.ExternalEditor-4.0/src/Products/ExternalEditor/zpt/main.zpt
+-rw-r--r--   0 jens       (501) staff       (20)       76 2023-04-20 08:24:09.000000 Products.ExternalEditor-4.0/src/Products/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-04 04:51:02.212029 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    30783 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1086 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        9 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-07-03 10:08:04.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)       19 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        9 2023-07-04 04:51:02.000000 Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1432 2023-07-03 10:08:01.000000 Products.ExternalEditor-4.0/tox.ini
```

### Comparing `Products.ExternalEditor-3.1.0/CHANGES.rst` & `Products.ExternalEditor-4.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 Changelog
 =========
 
 
+4.0 (2023-07-04)
+----------------
+
+- Ensure an object's editable body is cast to bytes
+  (`#20 <https://github.com/zopefoundation/Products.ExternalEditor/issues/20>`_)
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 3.1.0 (2022-06-24)
 ------------------
 
 - Add support for Python 3.9, 3.10.
 
 - Change package structure to move package code into a ``src`` subfolder.
 
 - Fix bug which prevented ZMI from rendering, when Products.ExternalEdit was
   installed.
   (`#18 <https://github.com/zopefoundation/Products.ExternalEditor/pull/18>`_)
 
+
 3.0.1 (2020-10-30)
 ------------------
 
 Bug fixes:
 
 - Add support for recent Python 3 versions [ale-rt]
```

### Comparing `Products.ExternalEditor-3.1.0/CONTRIBUTING.md` & `Products.ExternalEditor-4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/INSTALL.txt` & `Products.ExternalEditor-4.0/INSTALL.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/LICENSE.txt` & `Products.ExternalEditor-4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/PKG-INFO` & `Products.ExternalEditor-4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 Metadata-Version: 2.1
 Name: Products.ExternalEditor
-Version: 3.1.0
+Version: 4.0
 Summary: Zope External Editor
 Home-page: https://github.com/zopefoundation/Products.ExternalEditor
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
-Maintainer: Chris McDonough
-Maintainer-email: chrism@plope.com
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.ExternalEditor/issues
 Project-URL: Sources, https://github.com/zopefoundation/Products.ExternalEditor
 Keywords: zope external editor WebDAV
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors :: Text Processing
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Products.ExternalEditor/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Products.ExternalEditor/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/Products.ExternalEditor/badge.svg
         :target: https://coveralls.io/github/zopefoundation/Products.ExternalEditor
@@ -454,25 +447,37 @@
 
 Casey Duncan
 
 Changelog
 =========
 
 
+4.0 (2023-07-04)
+----------------
+
+- Ensure an object's editable body is cast to bytes
+  (`#20 <https://github.com/zopefoundation/Products.ExternalEditor/issues/20>`_)
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 3.1.0 (2022-06-24)
 ------------------
 
 - Add support for Python 3.9, 3.10.
 
 - Change package structure to move package code into a ``src`` subfolder.
 
 - Fix bug which prevented ZMI from rendering, when Products.ExternalEdit was
   installed.
   (`#18 <https://github.com/zopefoundation/Products.ExternalEditor/pull/18>`_)
 
+
 3.0.1 (2020-10-30)
 ------------------
 
 Bug fixes:
 
 - Add support for recent Python 3 versions [ale-rt]
 
@@ -856,9 +861,7 @@
 
 - Fixed product uninstallation bug
 
 5/15/02 - 0.1
 -------------
 
 - Initial release
-
-
```

### Comparing `Products.ExternalEditor-3.1.0/README.rst` & `Products.ExternalEditor-4.0/README.rst`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/setup.py` & `Products.ExternalEditor-4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,49 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(name='Products.ExternalEditor',
-      version='3.1.0',
+      version='4.0',
       description="Zope External Editor",
       long_description=(open("README.rst").read() + "\n" +
                         open("CHANGES.rst").read()),
       classifiers=[
           'Development Status :: 6 - Mature',
           'Environment :: Web Environment',
           'Framework :: Plone',
-          'Framework :: Zope :: 4',
           'Framework :: Zope :: 5',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: Zope Public License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 2',
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
           'Topic :: Software Development',
           'Topic :: Text Editors :: Text Processing',
       ],
       author="Zope Foundation and Contributors",
-      author_email="zope-dev@zope.org",
-      maintainer="Chris McDonough",
-      maintainer_email="chrism@plope.com",
+      author_email="zope-dev@zope.dev",
       license="ZPL 2.1",
       keywords="zope external editor WebDAV",
       url="https://github.com/zopefoundation/Products.ExternalEditor",
       project_urls={
         'Issue Tracker': ('https://github.com/zopefoundation/'
                           'Products.ExternalEditor/issues'),
         'Sources': 'https://github.com/zopefoundation/Products.ExternalEditor',
       },
       packages=find_packages('src'),
       package_dir={'': 'src'},
       namespace_packages=['Products'],
       include_package_data=True,
       zip_safe=False,
-      python_requires='>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*',
+      python_requires='>=3.7',
       install_requires=[
           'setuptools',
-          'Zope >= 4.3',
-          'six',
+          'Zope >= 5',
       ],
       )
```

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/ExternalEditor.py` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/ExternalEditor.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,31 @@
 # Version 2.1 (ZPL).  A copy of the ZPL should accompany this distribution.
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
-"""$Id$
-"""
+"""Zope External Editor Product by Casey Duncan."""
 
-# Zope External Editor Product by Casey Duncan
-
-import six
-from six.moves import urllib
+import urllib
 
 from AccessControl.class_init import InitializeClass
 from AccessControl.SecurityInfo import ClassSecurityInfo
 from AccessControl.SecurityManagement import getSecurityManager
 from Acquisition import Implicit
 from Acquisition import aq_base
 from Acquisition import aq_inner
 from Acquisition import aq_parent
 from OFS import Image
 from OFS.Lockable import wl_isLocked
 from zExceptions import BadRequest
 from zope.datetime import rfc1123_date
 from zope.interface import implementer
+from ZPublisher.HTTPRequest import default_encoding
 from ZPublisher.Iterators import IStreamIterator
 
 
 ExternalEditorPermission = 'Use external editor'
 
 _callbacks = []
 
@@ -45,23 +42,20 @@
     def __init__(self, data):
         self.data = data
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        # Python 3
         if self.data is None:
             raise StopIteration
         data = self.data.data
         self.data = next(self.data)
         return data
 
-    next = __next__  # Python 2
-
 
 def registerCallback(cb):
     """Register a callback to be called by the External Editor when
     it's about to be finished with collecting metadata for the
     to-be-edited file to allow actions to be taken, like for example
     inserting more metadata headers or enabling response compression
     or anything.
@@ -120,16 +114,14 @@
         r.append('url:%s' % ob.absolute_url())
         r.append('meta_type:%s' % ob.meta_type)
 
         title = getattr(aq_base(ob), 'title', None)
         if title is not None:
             if callable(title):
                 title = title()
-            if six.PY2 and isinstance(title, six.text_type):
-                title = title.encode('utf-8')
             r.append('title:%s' % title)
 
         if hasattr(aq_base(ob), 'content_type'):
             if callable(ob.content_type):
                 r.append('content_type:%s' % ob.content_type())
             else:
                 r.append('content_type:%s' % ob.content_type)
@@ -161,16 +153,15 @@
 
         # Apply any extra callbacks that might have been registered.
         applyCallbacks(ob, r, REQUEST, RESPONSE)
 
         # Finish metadata with an empty line.
         r.append('')
         metadata = '\n'.join(r)
-        if not six.PY2:
-            metadata = metadata.encode()
+        metadata = metadata.encode()
         metadata_len = len(metadata)
 
         # Check if we should send the file's data down the response.
         if REQUEST.get('skip_data'):
             # We've been requested to send only the metadata. The
             # client will presumably fetch the data itself.
             self._write_metadata(RESPONSE, metadata, metadata_len)
@@ -215,14 +206,17 @@
             body = ob.read()
         elif ob_data is not None:
             body = ob_data
         else:
             # can't read it!
             raise BadRequest('Object does not support external editing')
 
+        if isinstance(body, str):
+            body = body.encode(default_encoding)
+
         if IStreamIterator.providedBy(body):
             # We need to manage our content-length because we're streaming.
             # The content-length should have been set in the response by
             # the method that returns the iterator, but we need to fix it up
             # here because we insert metadata before the body.
             clen = RESPONSE.headers.get('content-length', None)
             assert clen is not None
@@ -286,15 +280,15 @@
         # launch the ZopeEditManager helper app
         # this is a workaround for limited MIME type
         ext = '.zem'
         if borrow_lock:
             query['borrow_lock'] = 1
         if skip_data:
             query['skip_data'] = 1
-        url = "%s/externalEdit_/%s%s%s" % (
+        url = "{}/externalEdit_/{}{}{}".format(
             aq_parent(aq_inner(object)).absolute_url(),
             urllib.parse.quote(object.getId()),
             ext, querystr(query))
         return ('<a href="%s" '
                 'title="Edit using external editor">'
                 '<img src="%s/misc_/ExternalEditor/edit_icon" '
                 'align="middle" hspace="2" border="0" alt="External Editor" />'
@@ -304,10 +298,10 @@
         return ''
 
 
 def querystr(d):
     """Create a query string from a dict"""
     if d:
         return '?' + '&'.join(
-            ['%s=%s' % (name, val) for name, val in d.items()])
+            ['{}={}'.format(name, val) for name, val in d.items()])
     else:
         return ''
```

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/LICENSE.txt` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/__init__.py` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/dtml/findForm.dtml` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/dtml/findForm.dtml`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/findResult.dtml` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/findResult.dtml`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/__init__.py` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/edit.txt` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/edit.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/link.txt` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/link.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/test_functional.py` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/tests/test_zmi.py` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/tests/test_zmi.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import Zope2.App
 
 
 class ZMITests(Testing.ZopeTestCase.FunctionalTestCase):
     """Testing the ZMI rendering."""
 
     def setUp(self):
-        super(ZMITests, self).setUp()
+        super().setUp()
 
         Zope2.App.zcml.load_site(force=True)
 
         uf = self.app.acl_users
         uf.userFolderAddUser('manager', 'manager_pass', ['Manager'], [])
         self.app.manage_addProduct['OFSP'].addDTMLMethod('meth')
```

### Comparing `Products.ExternalEditor-3.1.0/src/Products/ExternalEditor/zpt/main.zpt` & `Products.ExternalEditor-4.0/src/Products/ExternalEditor/zpt/main.zpt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/PKG-INFO` & `Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 Metadata-Version: 2.1
 Name: Products.ExternalEditor
-Version: 3.1.0
+Version: 4.0
 Summary: Zope External Editor
 Home-page: https://github.com/zopefoundation/Products.ExternalEditor
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
-Maintainer: Chris McDonough
-Maintainer-email: chrism@plope.com
+Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Project-URL: Issue Tracker, https://github.com/zopefoundation/Products.ExternalEditor/issues
 Project-URL: Sources, https://github.com/zopefoundation/Products.ExternalEditor
 Keywords: zope external editor WebDAV
-Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Text Editors :: Text Processing
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://github.com/zopefoundation/Products.ExternalEditor/actions/workflows/tests.yml/badge.svg
         :target: https://github.com/zopefoundation/Products.ExternalEditor/actions/workflows/tests.yml
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/Products.ExternalEditor/badge.svg
         :target: https://coveralls.io/github/zopefoundation/Products.ExternalEditor
@@ -454,25 +447,37 @@
 
 Casey Duncan
 
 Changelog
 =========
 
 
+4.0 (2023-07-04)
+----------------
+
+- Ensure an object's editable body is cast to bytes
+  (`#20 <https://github.com/zopefoundation/Products.ExternalEditor/issues/20>`_)
+
+- Add support for Python 3.11.
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 3.1.0 (2022-06-24)
 ------------------
 
 - Add support for Python 3.9, 3.10.
 
 - Change package structure to move package code into a ``src`` subfolder.
 
 - Fix bug which prevented ZMI from rendering, when Products.ExternalEdit was
   installed.
   (`#18 <https://github.com/zopefoundation/Products.ExternalEditor/pull/18>`_)
 
+
 3.0.1 (2020-10-30)
 ------------------
 
 Bug fixes:
 
 - Add support for recent Python 3 versions [ale-rt]
 
@@ -856,9 +861,7 @@
 
 - Fixed product uninstallation bug
 
 5/15/02 - 0.1
 -------------
 
 - Initial release
-
-
```

### Comparing `Products.ExternalEditor-3.1.0/src/Products.ExternalEditor.egg-info/SOURCES.txt` & `Products.ExternalEditor-4.0/src/Products.ExternalEditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Products.ExternalEditor-3.1.0/tox.ini` & `Products.ExternalEditor-4.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
+    py311
     coverage
 
 [testenv]
 usedevelop = true
 deps =
     zope.testrunner
 commands =
@@ -35,37 +33,36 @@
     check-python-versions >= 0.19.1
     wheel
     flake8
     isort
 
 [testenv:isort-apply]
 basepython = python3
+skip_install = true
 commands_pre =
 deps =
     isort
 commands =
     isort {toxinidir}/src {toxinidir}/setup.py []
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
     zope.testrunner
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
-    coverage html
-    coverage report -m --fail-under=78
+    coverage html --ignore-errors
+    coverage report --ignore-errors --show-missing --fail-under=78
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = Products.ExternalEditor
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```

