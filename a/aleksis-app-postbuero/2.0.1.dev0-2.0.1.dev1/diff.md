# Comparing `tmp/aleksis_app_postbuero-2.0.1.dev0.tar.gz` & `tmp/aleksis_app_postbuero-2.0.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_postbuero-2.0.1.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_postbuero-2.0.1.dev1.tar", max compression
```

## Comparing `aleksis_app_postbuero-2.0.1.dev0.tar` & `aleksis_app_postbuero-2.0.1.dev1.tar`

### file list

```diff
@@ -1,35 +1,29 @@
--rw-r--r--   0        0        0     1582 2022-08-10 18:23:31.273177 aleksis_app_postbuero-2.0.1.dev0/README.rst
--rw-r--r--   0        0        0      223 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/__init__.py
--rw-r--r--   0        0        0     1578 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/apps.py
--rw-r--r--   0        0        0     1346 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/forms.py
--rw-r--r--   0        0        0     2881 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_addresses/MailAddressCRUDList.vue
--rw-r--r--   0        0        0      612 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_addresses/mailAddresses.graphql
--rw-r--r--   0        0        0     3218 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_domains/MailDomainCRUDList.vue
--rw-r--r--   0        0        0      716 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_domains/mailDomains.graphql
--rw-r--r--   0        0        0      982 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/index.js
--rw-r--r--   0        0        0     1094 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/messages/en.json
--rw-r--r--   0        0        0     3356 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3224 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3269 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3224 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3224 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3224 2023-07-02 13:38:01.020861 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1640 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0001_initial.py
--rw-r--r--   0        0        0     1501 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0002_maildomain.py
--rw-r--r--   0        0        0      378 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0003_alter_maildomain_options.py
--rw-r--r--   0        0        0      547 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0004_domain_is_public.py
--rw-r--r--   0        0        0     3442 2022-08-10 18:23:31.273177 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0005_group_address.py
--rw-r--r--   0        0        0        0 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/__init__.py
--rw-r--r--   0        0        0     3698 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/models.py
--rw-r--r--   0        0        0     1427 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/preferences.py
--rw-r--r--   0        0        0     1061 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/rules.py
--rw-r--r--   0        0        0     5215 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/schema.py
--rw-r--r--   0        0        0      450 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/serializers.py
--rw-r--r--   0        0        0        0 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/static/.keepdir
--rw-r--r--   0        0        0      770 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/templates/templated_email/mail_added.email
--rw-r--r--   0        0        0      412 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/urls.py
--rw-r--r--   0        0        0      454 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/util/predicates.py
--rw-r--r--   0        0        0     2152 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/views.py
--rw-r--r--   0        0        0     1110 2023-07-02 13:38:21.360878 aleksis_app_postbuero-2.0.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 aleksis_app_postbuero-2.0.1.dev0/setup.py
--rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 aleksis_app_postbuero-2.0.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1582 2022-08-10 18:23:31.273177 aleksis_app_postbuero-2.0.1.dev1/README.rst
+-rw-r--r--   0        0        0      223 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/__init__.py
+-rw-r--r--   0        0        0     1578 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/apps.py
+-rw-r--r--   0        0        0     1346 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/forms.py
+-rw-r--r--   0        0        0     2881 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_addresses/MailAddressCRUDList.vue
+-rw-r--r--   0        0        0      612 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_addresses/mailAddresses.graphql
+-rw-r--r--   0        0        0     3218 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_domains/MailDomainCRUDList.vue
+-rw-r--r--   0        0        0      716 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_domains/mailDomains.graphql
+-rw-r--r--   0        0        0      982 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/index.js
+-rw-r--r--   0        0        0     1094 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/messages/en.json
+-rw-r--r--   0        0        0     1640 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1501 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0002_maildomain.py
+-rw-r--r--   0        0        0      378 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0003_alter_maildomain_options.py
+-rw-r--r--   0        0        0      547 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0004_domain_is_public.py
+-rw-r--r--   0        0        0     3442 2022-08-10 18:23:31.273177 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0005_group_address.py
+-rw-r--r--   0        0        0        0 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/__init__.py
+-rw-r--r--   0        0        0     3698 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/models.py
+-rw-r--r--   0        0        0     1427 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/preferences.py
+-rw-r--r--   0        0        0     1061 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/rules.py
+-rw-r--r--   0        0        0     5223 2023-07-05 13:08:55.007398 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/schema.py
+-rw-r--r--   0        0        0      450 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/serializers.py
+-rw-r--r--   0        0        0        0 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/static/.keepdir
+-rw-r--r--   0        0        0      770 2022-07-13 19:21:08.458482 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/templates/templated_email/mail_added.email
+-rw-r--r--   0        0        0      412 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/urls.py
+-rw-r--r--   0        0        0      454 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/util/predicates.py
+-rw-r--r--   0        0        0     2152 2023-07-02 13:35:21.048732 aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/views.py
+-rw-r--r--   0        0        0     1110 2023-07-05 13:12:13.423606 aleksis_app_postbuero-2.0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 aleksis_app_postbuero-2.0.1.dev1/setup.py
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 aleksis_app_postbuero-2.0.1.dev1/PKG-INFO
```

### Comparing `aleksis_app_postbuero-2.0.1.dev0/README.rst` & `aleksis_app_postbuero-2.0.1.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/apps.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/forms.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_addresses/MailAddressCRUDList.vue` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_addresses/MailAddressCRUDList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_addresses/mailAddresses.graphql` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_addresses/mailAddresses.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_domains/MailDomainCRUDList.vue` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_domains/MailDomainCRUDList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/components/mail_domains/mailDomains.graphql` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/components/mail_domains/mailDomains.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/index.js` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/frontend/messages/en.json` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0001_initial.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0002_maildomain.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0002_maildomain.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0004_domain_is_public.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0004_domain_is_public.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/migrations/0005_group_address.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/migrations/0005_group_address.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/models.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/preferences.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/rules.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/schema.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     @classmethod
     def before_save(cls, root, info, input, obj):  # noqa
         obj.person = info.context.user.person
         return obj
 
     @classmethod
     def check_permissions(cls, root, info, input):  # noqa
-        domain = MailDomain.get(id=input.domain)
+        domain = MailDomain.objects.get(id=input.domain)
         if info.context.user.has_perm("postbuero.can_use_domain_rule", domain):
             return
         raise PermissionDenied()
 
     @classmethod
     def validate_local_part(cls, root, info, value, input, **kwargs):  # noqa
         if value in get_site_preferences()["postbuero__disallowed_local_parts"].split(","):
```

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/templates/templated_email/mail_added.email` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/templates/templated_email/mail_added.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/aleksis/apps/postbuero/views.py` & `aleksis_app_postbuero-2.0.1.dev1/aleksis/apps/postbuero/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_postbuero-2.0.1.dev0/pyproject.toml` & `aleksis_app_postbuero-2.0.1.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Postbuero"
-version = "2.0.1.dev0"
+version = "2.0.1.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 
 description = "AlekSIS (School Information System) — App Postbuero (Mail server management)"
 authors = ["Tom Teichler <tom.teichler@teckids.org>"]
```

### Comparing `aleksis_app_postbuero-2.0.1.dev0/setup.py` & `aleksis_app_postbuero-2.0.1.dev1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,32 +9,26 @@
 
 package_data = \
 {'': ['*'],
  'aleksis.apps.postbuero': ['frontend/*',
                             'frontend/components/mail_addresses/*',
                             'frontend/components/mail_domains/*',
                             'frontend/messages/*',
-                            'locale/ar/LC_MESSAGES/*',
-                            'locale/de_DE/LC_MESSAGES/*',
-                            'locale/fr/LC_MESSAGES/*',
-                            'locale/la/LC_MESSAGES/*',
-                            'locale/nb_NO/LC_MESSAGES/*',
-                            'locale/tr_TR/LC_MESSAGES/*',
                             'static/*',
                             'templates/templated_email/*']}
 
 install_requires = \
 ['AlekSIS-Core>=3.0b0,<4.0']
 
 entry_points = \
 {'aleksis.app': ['postbuero = aleksis.apps.postbuero.apps:PostBueroConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-postbuero',
-    'version': '2.0.1.dev0',
+    'version': '2.0.1.dev1',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Postbuero (Mail server management)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Postbuero (Mail server management)\n============================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\nPostbuero provides integration with various mail server functionality, among which are:\n\n * Management of supported mail domains\n * Management of mail addresses (mailboxes) for persons\n\n   * Public registration for domains allowing it\n\n * Management of mail addresses (aliases) for groups\n\n   * Including support for members, owners, and guardians\n\n * `WebMilter`_ support for Postfix\n\n   * Alias resolution for persons and groups\n\nLicence\n-------\n\n::\n\n  Copyright © 2020 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2022 Tom Teichler <tom.teichler@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/official/AlekSIS\n.. _WebMilter: https://docs.bergblau.io/concepts/webmilter/\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Tom Teichler',
     'author_email': 'tom.teichler@teckids.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_postbuero-2.0.1.dev0/PKG-INFO` & `aleksis_app_postbuero-2.0.1.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-postbuero
-Version: 2.0.1.dev0
+Version: 2.0.1.dev1
 Summary: AlekSIS (School Information System) — App Postbuero (Mail server management)
 Home-page: https://aleksis.org
 License: EUPL-1.2
 Author: Tom Teichler
 Author-email: tom.teichler@teckids.org
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
```

