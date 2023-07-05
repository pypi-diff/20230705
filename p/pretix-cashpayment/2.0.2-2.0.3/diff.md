# Comparing `tmp/pretix-cashpayment-2.0.2.tar.gz` & `tmp/pretix-cashpayment-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pretix-cashpayment-2.0.2.tar", last modified: Fri Apr 17 14:08:36 2020, max compression
+gzip compressed data, was "pretix-cashpayment-2.0.3.tar", last modified: Wed Jul  5 14:58:07 2023, max compression
```

## Comparing `pretix-cashpayment-2.0.2.tar` & `pretix-cashpayment-2.0.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     4685 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     3705 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/README.rst
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/
--rw-rw-r--   0 martin    (1000) martin    (1000)      597 2020-04-17 14:02:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     2673 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1722 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     2660 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1823 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 martin    (1000) martin    (1000)     2721 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 martin    (1000) martin    (1000)     2655 2020-04-17 14:01:43.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/payment.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      624 2020-04-17 14:01:43.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/signals.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/
--rw-rw-r--   0 martin    (1000) martin    (1000)       82 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/checkout_payment_form.html
--rw-rw-r--   0 martin    (1000) martin    (1000)      998 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/control.html
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/email/
--rw-rw-r--   0 martin    (1000) martin    (1000)      262 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      401 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/pending.html
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     4685 2020-04-17 14:08:35.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      944 2020-04-17 14:08:35.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2020-04-17 14:08:35.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       72 2020-04-17 14:08:35.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       19 2020-04-17 14:08:35.000000 pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/top_level.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      363 2020-04-17 14:08:36.000000 pretix-cashpayment-2.0.2/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     1098 2020-04-17 14:02:25.000000 pretix-cashpayment-2.0.2/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      553 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)      141 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4064 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3705 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/README.rst
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       22 2023-07-05 14:50:25.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      575 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/apps.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1735 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3103 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1722 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3087 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1823 2020-04-17 14:06:38.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2721 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2694 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/payment.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      917 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/signals.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.187715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      100 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/checkout_payment_form.html
+-rw-rw-r--   0 martin    (1000) martin    (1000)      998 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/control.html
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/email/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      262 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      401 2019-02-20 10:36:33.000000 pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/pending.html
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4064 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      979 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       72 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       19 2023-07-05 14:58:07.000000 pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/top_level.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      363 2023-07-05 14:58:07.191715 pretix-cashpayment-2.0.3/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1145 2023-07-05 14:50:21.000000 pretix-cashpayment-2.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pretix-cashpayment-2.0.2/README.rst` & `pretix-cashpayment-2.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/__init__.py` & `pretix-cashpayment-2.0.3/pretix_cashpayment/apps.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from django.apps import AppConfig
 from django.utils.translation import gettext_lazy as _
+from . import __version__
 
 class PluginApp(AppConfig):
     name = 'pretix_cashpayment'
     verbose_name = 'Pretix Cash Payment plugin'
 
     class PretixPluginMeta:
         name = _('Cash Payment')
         author = 'Martin Gross'
         description = _('This plugin allows you to offer your customers a "pay with cash at the venue" option.')
         category = 'PAYMENT'
         visible = True
-        version = '2.0.2'
+        version = __version__
 
     def ready(self):
         from . import signals  # NOQA
 
 
-default_app_config = 'pretix_cashpayment.PluginApp'
```

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/LC_MESSAGES/django.mo` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de/LC_MESSAGES/django.po` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 msgid ""
 msgstr ""
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2021-11-29 20:53+0100\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Project-Id-Version: \n"
+"PO-Revision-Date: \n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"X-Generator: Poedit 3.0\n"
 
-#: pretix_cashpayment/__init__.py:9 pretix_cashpayment/payment.py:14
+#: pretix_cashpayment/__init__.py:9 pretix_cashpayment/payment.py:15
 msgid "Cash Payment"
 msgstr "Barzahlung"
 
 #: pretix_cashpayment/__init__.py:11
 msgid ""
 "This plugin allows you to offer your customers a \"pay with cash at the venue"
 "\" option."
 msgstr ""
 "Dieses Plugin ermöglicht es Ihnen, Ihren Kunden die Barzahlung vor Ort "
 "anzubieten"
 
-#: pretix_cashpayment/payment.py:19
+#: pretix_cashpayment/payment.py:17
+msgid "Confirm"
+msgstr "Bestätigen"
+
+#: pretix_cashpayment/payment.py:21
+msgid ""
+"In test mode, you can just manually mark this order as paid in the backend "
+"after it has been created."
+msgstr ""
+
+#: pretix_cashpayment/payment.py:27
 msgid "Payment information text"
 msgstr "Informationstext zur Zahlungsart"
 
-#: pretix_cashpayment/signals.py:13
+#: pretix_cashpayment/signals.py:24
 msgid "You can pay your order by cash at the venue."
 msgstr "Sie können Ihre Bestellung vor Ort in Bar bezahlen."
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:4
 msgid "This order has been paid via Cash Payment."
 msgstr "Diese Bestellung wurde in Bar bezahlt."
 
@@ -47,16 +64,16 @@
 msgstr "Diese Bezahlung wurde manuell als per Barzahlung bezahlt markiert"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:22
 msgid ""
 "This order has been planned to be paid via Cash Payment, but no payment has "
 "been received yet."
 msgstr ""
-"Diese Bestellung soll in Bar bezahlt werden, aber noch ist "
-"keine Zahlung eingegangen."
+"Diese Bestellung soll in Bar bezahlt werden, aber noch ist keine Zahlung "
+"eingegangen."
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:27
 msgid "Reference code"
 msgstr "Verwendungszweck"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt:1
 #, python-format
@@ -72,15 +89,16 @@
 "Verwendungszweck: %(code)s\n"
 "\n"
 "Betrag: %(total)s %(currency)s\n"
 "%(additional_details)s"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/pending.html:4
 msgid "Please print out this page and bring it with you when paying."
-msgstr "Bitte drucken Sie diese Seite aus und bringen Sie diese beim Bezahlen mit."
+msgstr ""
+"Bitte drucken Sie diese Seite aus und bringen Sie diese beim Bezahlen mit."
 
 #: pretix_cashpayment/templates/pretix_cashpayment/pending.html:11
 msgid "Amount:"
 msgstr "Betrag:"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/pending.html:12
 msgid "Reference code (important):"
```

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/de_Informal/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 msgid ""
 msgstr ""
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2021-11-29 20:53+0100\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Project-Id-Version: \n"
+"PO-Revision-Date: \n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"X-Generator: Poedit 3.0\n"
 
-#: pretix_cashpayment/__init__.py:9 pretix_cashpayment/payment.py:14
+#: pretix_cashpayment/__init__.py:9 pretix_cashpayment/payment.py:15
 msgid "Cash Payment"
 msgstr "Barzahlung"
 
 #: pretix_cashpayment/__init__.py:11
 msgid ""
 "This plugin allows you to offer your customers a \"pay with cash at the venue"
 "\" option."
 msgstr ""
 "Dieses Plugin ermöglicht es dir, deinen Kunden die Barzahlung vor Ort "
 "anzubieten"
 
-#: pretix_cashpayment/payment.py:19
+#: pretix_cashpayment/payment.py:17
+msgid "Confirm"
+msgstr "Bestätigen"
+
+#: pretix_cashpayment/payment.py:21
+msgid ""
+"In test mode, you can just manually mark this order as paid in the backend "
+"after it has been created."
+msgstr ""
+
+#: pretix_cashpayment/payment.py:27
 msgid "Payment information text"
 msgstr "Informationstext zur Zahlungsart"
 
-#: pretix_cashpayment/signals.py:13
+#: pretix_cashpayment/signals.py:24
 msgid "You can pay your order by cash at the venue."
 msgstr "Du kannst deine Bestellung vor Ort in Bar bezahlen."
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:4
 msgid "This order has been paid via Cash Payment."
 msgstr "Diese Bestellung wurde in Bar bezahlt."
 
@@ -47,16 +64,16 @@
 msgstr "Diese Bezahlung wurde manuell als per Barzahlung bezahlt markiert"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:22
 msgid ""
 "This order has been planned to be paid via Cash Payment, but no payment has "
 "been received yet."
 msgstr ""
-"Diese Bestellung soll in Bar bezahlt werden, aber noch ist "
-"keine Zahlung eingegangen."
+"Diese Bestellung soll in Bar bezahlt werden, aber noch ist keine Zahlung "
+"eingegangen."
 
 #: pretix_cashpayment/templates/pretix_cashpayment/control.html:27
 msgid "Reference code"
 msgstr "Verwendungszweck"
 
 #: pretix_cashpayment/templates/pretix_cashpayment/email/order_pending.txt:1
 #, python-format
```

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po` & `pretix-cashpayment-2.0.3/pretix_cashpayment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/payment.py` & `pretix-cashpayment-2.0.3/pretix_cashpayment/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pretix.base.payment import BasePaymentProvider
 
 
 class CashPayment(BasePaymentProvider):
     identifier = 'cashpayment'
     verbose_name = _('Cash Payment')
     abort_pending_allowed = True
+    confirm_button_name = _('Confirm')
 
     @property
     def test_mode_message(self):
         return _('In test mode, you can just manually mark this order as paid in the backend after it has been '
                  'created.')
 
     @property
```

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment/templates/pretix_cashpayment/control.html` & `pretix-cashpayment-2.0.3/pretix_cashpayment/templates/pretix_cashpayment/control.html`

 * *Files identical despite different names*

### Comparing `pretix-cashpayment-2.0.2/pretix_cashpayment.egg-info/SOURCES.txt` & `pretix-cashpayment-2.0.3/pretix_cashpayment.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 pretix_cashpayment/__init__.py
+pretix_cashpayment/apps.py
 pretix_cashpayment/payment.py
 pretix_cashpayment/signals.py
 pretix_cashpayment.egg-info/PKG-INFO
 pretix_cashpayment.egg-info/SOURCES.txt
 pretix_cashpayment.egg-info/dependency_links.txt
 pretix_cashpayment.egg-info/entry_points.txt
 pretix_cashpayment.egg-info/top_level.txt
```

### Comparing `pretix-cashpayment-2.0.2/setup.py` & `pretix-cashpayment-2.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from distutils.command.build import build
 
 from django.core import management
 from setuptools import setup, find_packages
+from pretix_cashpayment import __version__
 
 
 try:
     with open(os.path.join(os.path.dirname(__file__), 'README.rst'), encoding='utf-8') as f:
         long_description = f.read()
 except:
     long_description = ''
@@ -21,15 +22,15 @@
 cmdclass = {
     'build': CustomBuild
 }
 
 
 setup(
     name='pretix-cashpayment',
-    version='2.0.2',
+    version=__version__,
     description='pretix plugin that allows you to offer your customers a "pay with cash at the venue" option.',
     long_description=long_description,
     url='http://www.github.com/pc-coholic/pretix-cashpayment',
     author='Martin Gross',
     author_email='martin@pc-coholic.de',
     license='Apache Software License',
```

