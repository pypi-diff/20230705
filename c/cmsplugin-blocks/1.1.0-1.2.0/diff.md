# Comparing `tmp/cmsplugin-blocks-1.1.0.tar.gz` & `tmp/cmsplugin-blocks-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmsplugin-blocks-1.1.0.tar", last modified: Sun May 21 00:04:46 2023, max compression
+gzip compressed data, was "cmsplugin-blocks-1.2.0.tar", last modified: Wed Jul  5 00:47:40 2023, max compression
```

## Comparing `cmsplugin-blocks-1.1.0.tar` & `cmsplugin-blocks-1.2.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/LICENCE.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.1.0/MANIFEST.in
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1853 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/README.rst
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      179 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/__init__.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1365 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/slider.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      598 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/apps.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1782 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/choices_helpers.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      839 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/cms_plugins.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2317 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/django_configuration.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3546 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/defaults.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/exceptions.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1752 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1297 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1119 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1028 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2090 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/slider.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/user.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3554 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1217 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1197 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1141 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2145 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/django.pot
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3817 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2318 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4533 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     6408 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0001_initial.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      447 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0003_slideitem_title.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)    10292 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-25 23:04:05.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2925 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/modelfields.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      271 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5641 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3668 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3358 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3098 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     5939 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2142 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/album.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1840 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/card.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1646 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/container.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1433 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/hero.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1643 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/slider.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1246 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2577 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.217660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.225660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       49 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      856 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      980 2023-05-20 20:36:28.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       53 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       50 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     1266 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/__init__.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4372 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/archive.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4859 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/cms_tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2558 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/factories.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     7647 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/tests.py
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     4058 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/validators.py
-drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-05-21 00:04:46.221660 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/PKG-INFO
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     3504 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/SOURCES.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/dependency_links.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)      219 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/requires.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2023-05-21 00:04:46.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/top_level.txt
--rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-24 20:19:54.000000 cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/zip-safe
--rw-rw-r--   0 emencia   (1001) emencia   (1001)     2266 2023-05-21 00:04:46.229660 cmsplugin-blocks-1.1.0/setup.cfg
--rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.1.0/setup.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1057 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/LICENCE.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      337 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.2.0/MANIFEST.in
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1853 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/README.rst
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      179 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/__init__.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1365 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1854 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      598 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/apps.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1782 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/choices_helpers.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      839 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/cms_plugins.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/contrib/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/contrib/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2317 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/contrib/django_configuration.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3546 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/defaults.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      756 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/exceptions.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      418 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1752 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1297 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1119 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1028 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2090 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/slider.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      387 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/user.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      327 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3554 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1217 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1197 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1141 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2145 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3770 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/django.pot
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/en/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      380 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3817 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2318 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4533 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     6408 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0001_initial.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      447 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0002_add_slide_item_order.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      432 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0003_slideitem_title.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1690 2023-04-26 20:09:50.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)    10292 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      423 2023-07-05 00:47:20.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0006_alter_card_content.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-25 23:04:05.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2925 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/modelfields.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      271 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5641 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3667 2023-07-05 00:47:20.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3358 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3098 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     5939 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        0 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2142 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/album.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1840 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/card.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1646 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/container.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1433 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/hero.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1643 2023-05-21 00:04:26.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/slider.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1246 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1181 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2577 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1557 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/js/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2612 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.724177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4081 2023-04-17 01:02:12.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.732177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       49 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      856 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      980 2023-05-20 20:36:28.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       53 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1037 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       48 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      492 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/hero/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       50 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/default.html
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     1266 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      385 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/__init__.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4372 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/archive.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4859 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/cms_tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2558 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/factories.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     7647 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/tests.py
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     4058 2023-04-26 20:11:04.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/validators.py
+drwxrwxr-x   0 emencia   (1001) emencia   (1001)        0 2023-07-05 00:47:40.728177 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3353 2023-07-05 00:47:40.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/PKG-INFO
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     3559 2023-07-05 00:47:40.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/SOURCES.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-07-05 00:47:40.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/dependency_links.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)      219 2023-07-05 00:47:40.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/requires.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       25 2023-07-05 00:47:40.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/top_level.txt
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)        1 2023-04-24 20:19:54.000000 cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/zip-safe
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)     2266 2023-07-05 00:47:40.736177 cmsplugin-blocks-1.2.0/setup.cfg
+-rw-rw-r--   0 emencia   (1001) emencia   (1001)       84 2021-08-10 12:34:03.000000 cmsplugin-blocks-1.2.0/setup.py
```

### Comparing `cmsplugin-blocks-1.1.0/LICENCE.txt` & `cmsplugin-blocks-1.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/PKG-INFO` & `cmsplugin-blocks-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsplugin-blocks
-Version: 1.1.0
+Version: 1.2.0
 Summary: A set of DjangoCMS plugins for structured contents in CMS pages
 Home-page: https://github.com/emencia/cmsplugin-blocks
 Author: David Thenon
 Author-email: dthenon@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/cmsplugin-blocks
 Project-URL: Issue Tracker, https://github.com/emencia/cmsplugin-blocks/issues
```

### Comparing `cmsplugin-blocks-1.1.0/README.rst` & `cmsplugin-blocks-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/album.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/admin/slider.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/admin/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/apps.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/apps.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/choices_helpers.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/choices_helpers.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/cms_plugins.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/contrib/django_configuration.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/contrib/django_configuration.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/defaults.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/defaults.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/exceptions.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/exceptions.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/album.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/card.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/card.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/container.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/container.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/hero.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/hero.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/factories/slider.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/factories/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/album.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/card.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/card.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/container.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/container.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/hero.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/hero.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/forms/slider.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/forms/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/django.pot` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/django.pot`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.po` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0001_initial.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/migrations/0005_v1-0-0_changes.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/modelfields.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/modelfields.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/album.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/card.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,19 +75,19 @@
     """
     Optional image file, limited to enabled image formats from settings
     ``BLOCKS_ALLOWED_IMAGE_EXTENSIONS``.
     """
 
     content = models.TextField(
         _("Content"),
-        blank=False,
+        blank=True,
         default="",
     )
     """
-    Required long text, it will be editable through CKeditor on plugin form.
+    Optional long text, it will be editable through CKeditor on plugin form.
     """
 
     link_url = models.CharField(
         _("Link url"),
         blank=True,
         max_length=255,
     )
```

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/container.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/container.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/hero.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/hero.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/models/slider.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/models/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/album.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/album.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/card.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/card.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/container.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/container.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/hero.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/hero.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/plugins/slider.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/plugins/slider.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/album.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/albumitem.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/card.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/container.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/hero.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/admin/slider.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/css/fileinputbutton.css`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/static/cmsplugin_blocks/js/fileinputbutton.js`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/admin/albumitem_edit_tabular.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/album/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/card/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/container/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/templates/cmsplugin_blocks/slider/test.html`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/archive.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/archive.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/cms_tests.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/cms_tests.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/factories.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/factories.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/tests.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/tests.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks/utils/validators.py` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks/utils/validators.py`

 * *Files identical despite different names*

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/PKG-INFO` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsplugin-blocks
-Version: 1.1.0
+Version: 1.2.0
 Summary: A set of DjangoCMS plugins for structured contents in CMS pages
 Home-page: https://github.com/emencia/cmsplugin-blocks
 Author: David Thenon
 Author-email: dthenon@emencia.com
 License: MIT
 Project-URL: Source Code, https://github.com/emencia/cmsplugin-blocks
 Project-URL: Issue Tracker, https://github.com/emencia/cmsplugin-blocks/issues
```

### Comparing `cmsplugin-blocks-1.1.0/cmsplugin_blocks.egg-info/SOURCES.txt` & `cmsplugin-blocks-1.2.0/cmsplugin_blocks.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.mo
 cmsplugin_blocks/locale/fr/LC_MESSAGES/django.po
 cmsplugin_blocks/migrations/0001_initial.py
 cmsplugin_blocks/migrations/0002_add_slide_item_order.py
 cmsplugin_blocks/migrations/0003_slideitem_title.py
 cmsplugin_blocks/migrations/0004_change_image_as_filefield_.py
 cmsplugin_blocks/migrations/0005_v1-0-0_changes.py
+cmsplugin_blocks/migrations/0006_alter_card_content.py
 cmsplugin_blocks/migrations/__init__.py
 cmsplugin_blocks/models/__init__.py
 cmsplugin_blocks/models/album.py
 cmsplugin_blocks/models/card.py
 cmsplugin_blocks/models/container.py
 cmsplugin_blocks/models/hero.py
 cmsplugin_blocks/models/slider.py
```

### Comparing `cmsplugin-blocks-1.1.0/setup.cfg` & `cmsplugin-blocks-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cmsplugin-blocks
-version = 1.1.0
+version = 1.2.0
 description = A set of DjangoCMS plugins for structured contents in CMS pages
 long_description = file:README.rst
 long_description_content_type = text/x-rst
 author = David Thenon
 author_email = dthenon@emencia.com
 url = https://github.com/emencia/cmsplugin-blocks
 project_urls =
```

