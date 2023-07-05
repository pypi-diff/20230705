# Comparing `tmp/pretix-checkinlist-net-2.0.5.tar.gz` & `tmp/pretix-checkinlist-net-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pretix-checkinlist-net-2.0.5.tar", last modified: Thu Sep 12 08:03:57 2019, max compression
+gzip compressed data, was "pretix-checkinlist-net-2.0.6.tar", last modified: Wed Jul  5 14:13:34 2023, max compression
```

## Comparing `pretix-checkinlist-net-2.0.5.tar` & `pretix-checkinlist-net-2.0.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      153 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3693 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/PKG-INFO
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1087 2019-09-12 08:02:53.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     9845 2019-09-12 06:53:09.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/exporters.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de/LC_MESSAGES/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      312 2019-09-03 09:23:20.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de_Informal/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      312 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      993 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/signals.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/static/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/static/pretix_checkinlist_net/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/static/pretix_checkinlist_net/.gitkeep
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/templates/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/templates/pretix_checkinlist_net/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/templates/pretix_checkinlist_net/.gitkeep
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       80 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/entry_points.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     3693 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       10 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      733 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       23 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/top_level.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2388 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      363 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1098 2019-09-12 08:03:01.000000 pretix-checkinlist-net-2.0.5/setup.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-09-12 08:03:57.000000 pretix-checkinlist-net-2.0.5/test/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1588 2019-09-03 08:48:33.000000 pretix-checkinlist-net-2.0.5/test/test.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.955605 pretix-checkinlist-net-2.0.6/
+-rw-r--r--   0 bsheqa     (501) staff       (20)       49 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/AUTHORS
+-rw-r--r--   0 bsheqa     (501) staff       (20)    11357 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/LICENSE
+-rw-r--r--   0 bsheqa     (501) staff       (20)      153 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/MANIFEST.in
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2823 2023-07-05 14:13:34.955782 pretix-checkinlist-net-2.0.6/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2388 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/README.md
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.949310 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)       22 2023-07-05 14:13:21.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/__init__.py
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1056 2023-07-05 14:13:03.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/apps.py
+-rw-r--r--   0 bsheqa     (501) staff       (20)     9842 2023-07-05 14:12:01.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/exporters.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.943965 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.943818 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.952911 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.953366 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de_Informal/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.953771 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 bsheqa     (501) staff       (20)      993 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/signals.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.944365 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/static/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.954274 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/static/pretix_checkinlist_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/static/pretix_checkinlist_net/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.944619 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/templates/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.954664 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/templates/pretix_checkinlist_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/templates/pretix_checkinlist_net/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.952434 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2823 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)      780 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/SOURCES.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)        1 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/dependency_links.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       81 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/entry_points.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       10 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/requires.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       23 2023-07-05 14:13:34.000000 pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/top_level.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)      363 2023-07-05 14:13:34.956561 pretix-checkinlist-net-2.0.6/setup.cfg
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1098 2023-07-05 14:12:25.000000 pretix-checkinlist-net-2.0.6/setup.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:13:34.955133 pretix-checkinlist-net-2.0.6/test/
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1588 2023-07-05 14:00:13.000000 pretix-checkinlist-net-2.0.6/test/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/__init__.py` & `pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from django.apps import AppConfig
 from django.utils.functional import cached_property
-from django.utils.translation import ugettext_lazy
+from django.utils.translation import gettext_lazy
+from . import __version__
 
 from packaging import version
 
 from pretix import __version__ as appVersion
 
 class PluginApp(AppConfig):
     name = 'pretix_checkinlist_net'
     verbose_name = 'Pretix Checkin List Exporter for NETWAYS'
     required_core_version = '2.5.0'
 
     class PretixPluginMeta:
-        name = ugettext_lazy('Pretix Checkin List Exporter for NETWAYS')
+        name = gettext_lazy('Pretix Checkin List Exporter for NETWAYS')
         author = 'NETWAYS GmbH'
-        description = ugettext_lazy('This plugins allows to create custom event exports in Excel/CSV')
+        description = gettext_lazy('This plugins allows to create custom event exports in Excel/CSV')
         visible = True
-        version = '2.0.5'
+        version = __version__
 
     def ready(self):
         from . import signals  # NOQA
 
     @cached_property
     def compatibility_warnings(self):
         errs = []
 
         if version.parse(appVersion) < version.parse(self.required_core_version):
             errs.append("Pretix version %s is too old. Minimum required is %s." % (appVersion, self.required_core_version))
 
         return errs
-
-
-default_app_config = 'pretix_checkinlist_net.PluginApp'
```

### Comparing `pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/exporters.py` & `pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/exporters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from collections import OrderedDict
 from django import forms
 from django.db.models import Max, OuterRef, Subquery
 from django.db.models.functions import Coalesce
 from django.urls import reverse
-from django.utils.translation import pgettext, ugettext as _, ugettext_lazy
+from django.utils.translation import pgettext, gettext as _, gettext_lazy
 from pretix.base.exporter import BaseExporter, ListExporter
 from pretix.base.models import (
     Checkin, InvoiceAddress, Order, OrderPosition, Question,
 )
 from pretix.base.settings import PERSON_NAME_SCHEMES
 from pretix.control.forms.widgets import Select2
 
@@ -187,15 +187,15 @@
         # return result set
         return coll, collected_product_columns, collected_question_columns
 
 
 class CSVCheckinListNet(CheckInListMixin, ListExporter):
     name = "overview"
     identifier = 'checkinlistnet'
-    verbose_name = ugettext_lazy('Check-in list for NETWAYS')
+    verbose_name = gettext_lazy('Check-in list for NETWAYS')
 
     @property
     def additional_form_fields(self):
         return self._fields
 
     def iterate_list(self, form_data):
         # Fetch data from checkin_list
```

### Comparing `pretix-checkinlist-net-2.0.5/pretix_checkinlist_net/signals.py` & `pretix-checkinlist-net-2.0.6/pretix_checkinlist_net/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-checkinlist-net-2.0.5/pretix_checkinlist_net.egg-info/SOURCES.txt` & `pretix-checkinlist-net-2.0.6/pretix_checkinlist_net.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+AUTHORS
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 pretix_checkinlist_net/__init__.py
+pretix_checkinlist_net/apps.py
 pretix_checkinlist_net/exporters.py
 pretix_checkinlist_net/signals.py
 pretix_checkinlist_net.egg-info/PKG-INFO
 pretix_checkinlist_net.egg-info/SOURCES.txt
 pretix_checkinlist_net.egg-info/dependency_links.txt
 pretix_checkinlist_net.egg-info/entry_points.txt
 pretix_checkinlist_net.egg-info/requires.txt
```

### Comparing `pretix-checkinlist-net-2.0.5/README.md` & `pretix-checkinlist-net-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pretix-checkinlist-net-2.0.5/setup.py` & `pretix-checkinlist-net-2.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except ImportError:
     long_description = open('README.md').read()
 
 setup(
     name='pretix-checkinlist-net',
-    version='2.0.5',
+    version='2.0.6',
     description='Pretix checkin list exporter for NETWAYS',
     long_description=long_description,
     url='https://github.com/NETWAYS/pretix-checkinlist-net',
     download_url='https://github.com/NETWAYS/pretix-invoice-net/archive/v2.0.5.tar.gz',
     keywords=['pretix', 'tickets', 'events', 'invoice', 'pdf'],
     author='NETWAYS GmbH',
     author_email='support@netways.de',
```

### Comparing `pretix-checkinlist-net-2.0.5/test/test.py` & `pretix-checkinlist-net-2.0.6/test/test.py`

 * *Files identical despite different names*

