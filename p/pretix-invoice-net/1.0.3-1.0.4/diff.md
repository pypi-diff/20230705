# Comparing `tmp/pretix-invoice-net-1.0.3.tar.gz` & `tmp/pretix-invoice-net-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-invoice-net-1.0.3.tar", last modified: Wed Jul  5 14:06:09 2023, max compression
+gzip compressed data, was "pretix-invoice-net-1.0.4.tar", last modified: Wed Jul  5 14:10:37 2023, max compression
```

## Comparing `pretix-invoice-net-1.0.3.tar` & `pretix-invoice-net-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.526563 pretix-invoice-net-1.0.3/
--rw-r--r--   0 bsheqa     (501) staff       (20)    11357 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/LICENSE
--rw-r--r--   0 bsheqa     (501) staff       (20)      141 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/MANIFEST.in
--rw-r--r--   0 bsheqa     (501) staff       (20)     2807 2023-07-05 14:06:09.526733 pretix-invoice-net-1.0.3/PKG-INFO
--rw-r--r--   0 bsheqa     (501) staff       (20)     2400 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/README.md
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.521880 pretix-invoice-net-1.0.3/pretix_invoice_net/
--rw-r--r--   0 bsheqa     (501) staff       (20)       22 2023-07-05 14:04:16.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/__init__.py
--rw-r--r--   0 bsheqa     (501) staff       (20)      568 2023-07-05 14:05:54.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/apps.py
--rw-r--r--   0 bsheqa     (501) staff       (20)    17056 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/invoice.py
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.517406 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.517259 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.524647 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de/LC_MESSAGES/
--rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.525065 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de_Informal/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de_Informal/.gitkeep
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.525421 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de_Informal/LC_MESSAGES/
--rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/locale/de_Informal/LC_MESSAGES/django.po
--rw-r--r--   0 bsheqa     (501) staff       (20)      967 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/signals.py
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.517810 pretix-invoice-net-1.0.3/pretix_invoice_net/static/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.525908 pretix-invoice-net-1.0.3/pretix_invoice_net/static/pretix_invoice_net/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/static/pretix_invoice_net/.gitkeep
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.518059 pretix-invoice-net-1.0.3/pretix_invoice_net/templates/
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.526208 pretix-invoice-net-1.0.3/pretix_invoice_net/templates/pretix_invoice_net/
--rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.3/pretix_invoice_net/templates/pretix_invoice_net/.gitkeep
-drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:06:09.524216 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/
--rw-r--r--   0 bsheqa     (501) staff       (20)     2807 2023-07-05 14:06:09.000000 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/PKG-INFO
--rw-r--r--   0 bsheqa     (501) staff       (20)      648 2023-07-05 14:06:09.000000 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/SOURCES.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)        1 2023-07-05 14:06:09.000000 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/dependency_links.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)       73 2023-07-05 14:06:09.000000 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/entry_points.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)       19 2023-07-05 14:06:09.000000 pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/top_level.txt
--rw-r--r--   0 bsheqa     (501) staff       (20)      404 2023-07-05 14:06:09.527462 pretix-invoice-net-1.0.3/setup.cfg
--rw-r--r--   0 bsheqa     (501) staff       (20)     1112 2023-07-05 14:04:08.000000 pretix-invoice-net-1.0.3/setup.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.621695 pretix-invoice-net-1.0.4/
+-rw-r--r--   0 bsheqa     (501) staff       (20)    11357 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/LICENSE
+-rw-r--r--   0 bsheqa     (501) staff       (20)      141 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/MANIFEST.in
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2807 2023-07-05 14:10:37.621862 pretix-invoice-net-1.0.4/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2400 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/README.md
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.616773 pretix-invoice-net-1.0.4/pretix_invoice_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)       22 2023-07-05 14:10:29.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/__init__.py
+-rw-r--r--   0 bsheqa     (501) staff       (20)      565 2023-07-05 14:09:53.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/apps.py
+-rw-r--r--   0 bsheqa     (501) staff       (20)    17056 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/invoice.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.612157 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.611999 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.619689 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.620172 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de_Informal/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de_Informal/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.620545 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de_Informal/LC_MESSAGES/
+-rw-r--r--   0 bsheqa     (501) staff       (20)      312 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/locale/de_Informal/LC_MESSAGES/django.po
+-rw-r--r--   0 bsheqa     (501) staff       (20)      967 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/signals.py
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.612559 pretix-invoice-net-1.0.4/pretix_invoice_net/static/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.621003 pretix-invoice-net-1.0.4/pretix_invoice_net/static/pretix_invoice_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/static/pretix_invoice_net/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.612805 pretix-invoice-net-1.0.4/pretix_invoice_net/templates/
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.621430 pretix-invoice-net-1.0.4/pretix_invoice_net/templates/pretix_invoice_net/
+-rw-r--r--   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:01:33.000000 pretix-invoice-net-1.0.4/pretix_invoice_net/templates/pretix_invoice_net/.gitkeep
+drwxr-xr-x   0 bsheqa     (501) staff       (20)        0 2023-07-05 14:10:37.619209 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/
+-rw-r--r--   0 bsheqa     (501) staff       (20)     2807 2023-07-05 14:10:37.000000 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/PKG-INFO
+-rw-r--r--   0 bsheqa     (501) staff       (20)      648 2023-07-05 14:10:37.000000 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/SOURCES.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)        1 2023-07-05 14:10:37.000000 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/dependency_links.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       73 2023-07-05 14:10:37.000000 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/entry_points.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)       19 2023-07-05 14:10:37.000000 pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/top_level.txt
+-rw-r--r--   0 bsheqa     (501) staff       (20)      404 2023-07-05 14:10:37.622639 pretix-invoice-net-1.0.4/setup.cfg
+-rw-r--r--   0 bsheqa     (501) staff       (20)     1112 2023-07-05 14:10:22.000000 pretix-invoice-net-1.0.4/setup.py
```

### Comparing `pretix-invoice-net-1.0.3/LICENSE` & `pretix-invoice-net-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-invoice-net-1.0.3/PKG-INFO` & `pretix-invoice-net-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-invoice-net
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pretix invoice renderer plugin for NETWAYS
 Home-page: https://github.com/NETWAYS/pretix-invoice-net
 Download-URL: https://github.com/NETWAYS/pretix-invoice-net/archive/v1.0.2.tar.gz
 Author: NETWAYS GmbH
 Author-email: support@netways.de
 License: Apache Software License
 Keywords: pretix,tickets,events,invoice,pdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pretix-invoice-net Version: 1.0.3 Summary: Pretix
+Metadata-Version: 2.1 Name: pretix-invoice-net Version: 1.0.4 Summary: Pretix
 invoice renderer plugin for NETWAYS Home-page: https://github.com/NETWAYS/
 pretix-invoice-net Download-URL: https://github.com/NETWAYS/pretix-invoice-net/
 archive/v1.0.2.tar.gz Author: NETWAYS GmbH Author-email: support@netways.de
 License: Apache Software License Keywords: pretix,tickets,events,invoice,pdf
 License-File: LICENSE # Pretix Invoice Renderer Plugin for NETWAYS This plugin
 adds a custom invoice renderer for NETWAYS hosted events and conferences using
 [https://github.com/NETWAYS/pretix-invoice-net/blob/master/res/logo.png].
```

### Comparing `pretix-invoice-net-1.0.3/README.md` & `pretix-invoice-net-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pretix-invoice-net-1.0.3/pretix_invoice_net/apps.py` & `pretix-invoice-net-1.0.4/pretix_invoice_net/apps.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from django.apps import AppConfig
-from django.utils.translation import ugettext_lazy
+from django.utils.translation import gettext_lazy
 from . import __version__
 
 
 class PluginApp(AppConfig):
     name = 'pretix_invoice_net'
     verbose_name = 'Pretix invoice renderer plugin for NETWAYS'
 
     class PretixPluginMeta:
-        name = ugettext_lazy('Pretix invoice renderer plugin for NETWAYS')
+        name = gettext_lazy('Pretix invoice renderer plugin for NETWAYS')
         author = 'NETWAYS GmbH'
-        description = ugettext_lazy('Pretix invoice renderer plugin for NETWAYS')
+        description = gettext_lazy('Pretix invoice renderer plugin for NETWAYS')
         visible = True
         version = __version__
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretix-invoice-net-1.0.3/pretix_invoice_net/invoice.py` & `pretix-invoice-net-1.0.4/pretix_invoice_net/invoice.py`

 * *Files identical despite different names*

### Comparing `pretix-invoice-net-1.0.3/pretix_invoice_net/signals.py` & `pretix-invoice-net-1.0.4/pretix_invoice_net/signals.py`

 * *Files identical despite different names*

### Comparing `pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/PKG-INFO` & `pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-invoice-net
-Version: 1.0.3
+Version: 1.0.4
 Summary: Pretix invoice renderer plugin for NETWAYS
 Home-page: https://github.com/NETWAYS/pretix-invoice-net
 Download-URL: https://github.com/NETWAYS/pretix-invoice-net/archive/v1.0.2.tar.gz
 Author: NETWAYS GmbH
 Author-email: support@netways.de
 License: Apache Software License
 Keywords: pretix,tickets,events,invoice,pdf
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pretix-invoice-net Version: 1.0.3 Summary: Pretix
+Metadata-Version: 2.1 Name: pretix-invoice-net Version: 1.0.4 Summary: Pretix
 invoice renderer plugin for NETWAYS Home-page: https://github.com/NETWAYS/
 pretix-invoice-net Download-URL: https://github.com/NETWAYS/pretix-invoice-net/
 archive/v1.0.2.tar.gz Author: NETWAYS GmbH Author-email: support@netways.de
 License: Apache Software License Keywords: pretix,tickets,events,invoice,pdf
 License-File: LICENSE # Pretix Invoice Renderer Plugin for NETWAYS This plugin
 adds a custom invoice renderer for NETWAYS hosted events and conferences using
 [https://github.com/NETWAYS/pretix-invoice-net/blob/master/res/logo.png].
```

### Comparing `pretix-invoice-net-1.0.3/pretix_invoice_net.egg-info/SOURCES.txt` & `pretix-invoice-net-1.0.4/pretix_invoice_net.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretix-invoice-net-1.0.3/setup.py` & `pretix-invoice-net-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     import pypandoc
     long_description = pypandoc.convert('README.md', 'rst')
 except:
     long_description = open('README.md').read()
 
 setup(
     name = 'pretix-invoice-net',
-    version = '1.0.3',
+    version = '1.0.4',
     description = 'Pretix invoice renderer plugin for NETWAYS',
     long_description = long_description,
     url = 'https://github.com/NETWAYS/pretix-invoice-net',
     download_url = 'https://github.com/NETWAYS/pretix-invoice-net/archive/v1.0.2.tar.gz',
     keywords = [ 'pretix', 'tickets', 'events', 'invoice', 'pdf' ],
     author = 'NETWAYS GmbH',
     author_email = 'support@netways.de',
```

