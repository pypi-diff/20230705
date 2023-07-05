# Comparing `tmp/django_one_time_notices-0.1.1.tar.gz` & `tmp/django_one_time_notices-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_one_time_notices-0.1.1.tar", max compression
+gzip compressed data, was "django_one_time_notices-0.1.2.tar", max compression
```

## Comparing `django_one_time_notices-0.1.1.tar` & `django_one_time_notices-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1965 2022-10-17 17:38:17.433667 django_one_time_notices-0.1.1/README.md
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/__init__.py
--rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/admin.py
--rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/apps.py
--rw-r--r--   0        0        0      750 2022-10-17 17:40:31.745581 django_one_time_notices-0.1.1/notices/context_processors.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_app/templates/example_app/home.html
--rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_app/views.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_project/__init__.py
--rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_project/asgi.py
--rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.1/notices/example_project/example_project/settings.py
--rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_project/urls.py
--rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/example_project/wsgi.py
--rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/example_project/manage.py
--rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/migrations/0001_initial.py
--rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/migrations/0002_alter_notice_version.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/migrations/__init__.py
--rw-r--r--   0        0        0     1676 2022-10-17 17:45:21.377334 django_one_time_notices-0.1.1/notices/models.py
--rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.1/notices/static/notices/css/notices.css
--rw-r--r--   0        0        0     1059 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/static/notices/js/notices.js
--rw-r--r--   0        0        0      569 2022-10-17 17:41:19.381545 django_one_time_notices-0.1.1/notices/templates/notices/notices.html
--rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/templates/notices/notices_clear.html
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/templatetags/__init__.py
--rw-r--r--   0        0        0     1643 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.1/notices/templatetags/notices_tags.py
--rw-r--r--   0        0        0     1482 2022-10-17 17:46:09.649287 django_one_time_notices-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.1/setup.py
--rw-r--r--   0        0        0     2564 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2166 2023-07-05 09:12:05.416089 django_one_time_notices-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/__init__.py
+-rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/admin.py
+-rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/apps.py
+-rw-r--r--   0        0        0     1078 2023-07-05 10:24:30.076861 django_one_time_notices-0.1.2/notices/context_processors.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/templates/example_app/home.html
+-rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/views.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/__init__.py
+-rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/asgi.py
+-rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.2/notices/example_project/example_project/settings.py
+-rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/urls.py
+-rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/wsgi.py
+-rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/manage.py
+-rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/0001_initial.py
+-rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/0002_alter_notice_version.py
+-rw-r--r--   0        0        0      414 2023-07-05 08:34:05.713146 django_one_time_notices-0.1.2/notices/migrations/0003_notice_timeout_seconds.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/__init__.py
+-rw-r--r--   0        0        0     2080 2023-07-05 10:24:30.092861 django_one_time_notices-0.1.2/notices/models.py
+-rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.2/notices/static/notices/css/notices.css
+-rw-r--r--   0        0        0     1101 2023-07-05 08:24:49.738939 django_one_time_notices-0.1.2/notices/static/notices/js/notices.js
+-rw-r--r--   0        0        0      909 2023-07-05 08:53:25.144794 django_one_time_notices-0.1.2/notices/templates/notices/notices.html
+-rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templates/notices/notices_clear.html
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templatetags/__init__.py
+-rw-r--r--   0        0        0     1643 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templatetags/notices_tags.py
+-rw-r--r--   0        0        0     1482 2023-07-05 09:13:02.068042 django_one_time_notices-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.2/PKG-INFO
```

### Comparing `django_one_time_notices-0.1.1/README.md` & `django_one_time_notices-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: django-one-time-notices
+Version: 0.1.2
+Summary: 
+License: MIT
+Author: Becky Smith
+Author-email: rebkwok@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Django (>=4.1,<5.0)
+Requires-Dist: django-classy-tags (>=3.0.1,<4.0.0)
+Description-Content-Type: text/markdown
+
 # django-one-time-notices
 
 Displays a modal with notice content if a user hasn't seen it yet.
 
 ## Install
 ```
 pip install django-one-time-notices
@@ -36,15 +54,15 @@
         }
     }
 ]
 ```             
 
 To customise the notice colour (button and title border), add
 ```
-NOTICES_COLOR=<color>  # any css-acceptable colour
+NOTICES_COLOUR=<colour>  # any css-acceptable colour
 ```
 
 ## Static assets
 Add `notices/css/notices.css` and `notices/js/notices.js` to your markup.
 
 ## Usage
 In templates, load the tags:
@@ -53,28 +71,32 @@
 ```
 
 and add the modal:
 ```
 {% NoticesModal %} 
 ```
 
-The modal will be shown.  Once it has been dismissed it won't be shown again unless the notice version changes (see below) or the `notice_seen` cookie is deleted.
+The modal will be shown.  Once it has been dismissed it won't be shown again unless the notice version changes (see below), the `notice_seen` cookie is deleted, or the notice timeout is reached.
 
 ## Setting/updating the notice
 
 ### via models and django admin
 Add a `Notice` instance in the django admin. 
 
-Notices have `title`, `content`, `version` and optional `expires_at` fields.
+Notices have `title`, `content`, `version` and optional `timeout_seconds` and `expires_at` fields.
 
 Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it.
 
+Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
+
 To show a new notice, add another Notice instance with an incremented version number.
 
 ### via django settings
 
 Override the Notice model by adding to your `settings.py`:
 `NOTICES_VERSION` # an integer
 `NOTICES_TITLE`  # optional, default = "New!"
 `NOTICES_CONTENT`  # optional, default = ""
+`NOTICES_TIMEOUT_SECONDS`  # optional, default = None
 
 Set `NOTICES_VERSION = 0` to clear the cookie and disable showing notices at all.
+
```

### Comparing `django_one_time_notices-0.1.1/notices/example_project/example_app/templates/example_app/home.html` & `django_one_time_notices-0.1.2/notices/example_project/example_app/templates/example_app/home.html`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/example_project/example_project/settings.py` & `django_one_time_notices-0.1.2/notices/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/example_project/example_project/urls.py` & `django_one_time_notices-0.1.2/notices/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/example_project/manage.py` & `django_one_time_notices-0.1.2/notices/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/migrations/0001_initial.py` & `django_one_time_notices-0.1.2/notices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/models.py` & `django_one_time_notices-0.1.2/notices/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 class Notice(models.Model):
 
     title = models.CharField(max_length=255, default="New!")
     content = models.TextField()
     version = models.PositiveIntegerField(blank=True, unique=True)
     expires_at = models.DateTimeField(null=True, blank=True)
+    timeout_seconds = models.PositiveIntegerField(blank=True, null=True)
 
     def __str__(self):
         return (
             f"v{self.version} - "
             f"expires: {self.expires_at.strftime('%d-%b-%Y %H:%M UTC') if self.expires_at else 'never'}"
         )
 
@@ -30,19 +31,27 @@
     def from_settings(cls):
         if hasattr(settings, "NOTICES_VERSION"):
             try:
                 version = int(settings.NOTICES_VERSION)
             except (TypeError, ValueError):
                 ...
             else:
+                if hasattr(settings, "NOTICES_COLOUR"):
+                    colour_setting = "NOTICES_COLOUR"
+                else:
+                    colour_setting = "NOTICES_COLOR"
+
                 return {
                     "notices_version": version,
                     "notices_title": getattr(settings, "NOTICES_TITLE", "New!"),
                     "notices_content": getattr(settings, "NOTICES_CONTENT", ""),
-                    "notices_color": getattr(settings, "NOTICES_COLOR", None),
+                    "notices_colour": getattr(settings, colour_setting, None),
+                    "notices_timeout_seconds": getattr(
+                        settings, "NOTICES_TIMEOUT_SECONDS", None
+                    ),
                 }
 
     def has_expired(self):
         if not self.expires_at:
             return False
         return self.expires_at < timezone.now()
```

### Comparing `django_one_time_notices-0.1.1/notices/static/notices/css/notices.css` & `django_one_time_notices-0.1.2/notices/static/notices/css/notices.css`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/notices/static/notices/js/notices.js` & `django_one_time_notices-0.1.2/notices/static/notices/js/notices.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -5,34 +5,34 @@
             document.cookie = "notices_seen=; Max-Age=-99999999;"
             clear.remove()
         };
     }
 )();
 
 var noticesCookie = {
-    createCookie: function(value, days) {
+    createCookie: function(value, timeout_seconds) {
         var date = new Date(),
             expires = '';
-        if (days) {
-            date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
+        if (timeout_seconds) {
+            date.setTime(date.getTime() + (timeout_seconds * 1000));
             expires = "; expires=" + date.toGMTString();
         } else {
             expires = "";
         }
 
         var secureString = "";
         if (window.isSecureContext) {
             secureString = "; Secure";
         }
 
         document.cookie = "notices_seen" + "=" + value + expires + "; path=/" + secureString;
     },
 
-    setCookie: function(version) {
-        this.createCookie(version, 10 * 365);
+    setCookie: function(version, timeout_seconds) {
+        this.createCookie(version, timeout_seconds);
         this.hidenoticedModal()
     },
 
     hidenoticedModal: function() {
         document.getElementById('noticesModal').remove();
         document.getElementById('noticesModalFader').remove();
     },
```

### Comparing `django_one_time_notices-0.1.1/notices/templatetags/notices_tags.py` & `django_one_time_notices-0.1.2/notices/templatetags/notices_tags.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.1/pyproject.toml` & `django_one_time_notices-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-one-time-notices"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Becky Smith <rebkwok@gmail.com>"]
 readme = "README.md"
 packages = [{include = "notices"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `django_one_time_notices-0.1.1/setup.py` & `django_one_time_notices-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# django-one-time-notices
 
-packages = \
-['notices',
- 'notices.example_project',
- 'notices.example_project.example_app',
- 'notices.example_project.example_app.migrations',
- 'notices.example_project.example_project',
- 'notices.migrations',
- 'notices.templatetags']
-
-package_data = \
-{'': ['*'],
- 'notices': ['static/notices/css/*',
-             'static/notices/js/*',
-             'templates/notices/*'],
- 'notices.example_project.example_app': ['templates/example_app/*']}
-
-install_requires = \
-['Django>=4.1,<5.0', 'django-classy-tags>=3.0.1,<4.0.0']
-
-setup_kwargs = {
-    'name': 'django-one-time-notices',
-    'version': '0.1.1',
-    'description': '',
-    'long_description': '# django-one-time-notices\n\nDisplays a modal with notice content if a user hasn\'t seen it yet.\n\n## Install\n```\npip install django-one-time-notices\n```\n\n## Settings\n\nAdd to `INSTALLED_APPS`:\n\n```\ndjango.contrib.auth\ndjango.contrib.admin\n...\nnotices\n```\n\n\nAdd to `TEMPLATES[\'OPTIONS\']`:\n```\nTEMPLATES = [\n    {\n        \'BACKEND\': \'django.template.backends.django.DjangoTemplates\',\n        \'DIRS\': [],\n        \'APP_DIRS\': True,\n        \'OPTIONS\': {\n            \'context_processors\': [\n                ...\n                \'django.core.context_processors.request\'\n                ...\n                \'notices.context_processors.notices\',\n            ]\n        }\n    }\n]\n```             \n\nTo customise the notice colour (button and title border), add\n```\nNOTICES_COLOR=<color>  # any css-acceptable colour\n```\n\n## Static assets\nAdd `notices/css/notices.css` and `notices/js/notices.js` to your markup.\n\n## Usage\nIn templates, load the tags:\n```\n{% load notices_tags %}\n```\n\nand add the modal:\n```\n{% NoticesModal %} \n```\n\nThe modal will be shown.  Once it has been dismissed it won\'t be shown again unless the notice version changes (see below) or the `notice_seen` cookie is deleted.\n\n## Setting/updating the notice\n\n### via models and django admin\nAdd a `Notice` instance in the django admin. \n\nNotices have `title`, `content`, `version` and optional `expires_at` fields.\n\nVersion can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it.\n\nTo show a new notice, add another Notice instance with an incremented version number.\n\n### via django settings\n\nOverride the Notice model by adding to your `settings.py`:\n`NOTICES_VERSION` # an integer\n`NOTICES_TITLE`  # optional, default = "New!"\n`NOTICES_CONTENT`  # optional, default = ""\n\nSet `NOTICES_VERSION = 0` to clear the cookie and disable showing notices at all.\n',
-    'author': 'Becky Smith',
-    'author_email': 'rebkwok@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+Displays a modal with notice content if a user hasn't seen it yet.
 
+## Install
+```
+pip install django-one-time-notices
+```
 
-setup(**setup_kwargs)
+## Settings
+
+Add to `INSTALLED_APPS`:
+
+```
+django.contrib.auth
+django.contrib.admin
+...
+notices
+```
+
+
+Add to `TEMPLATES['OPTIONS']`:
+```
+TEMPLATES = [
+    {
+        'BACKEND': 'django.template.backends.django.DjangoTemplates',
+        'DIRS': [],
+        'APP_DIRS': True,
+        'OPTIONS': {
+            'context_processors': [
+                ...
+                'django.core.context_processors.request'
+                ...
+                'notices.context_processors.notices',
+            ]
+        }
+    }
+]
+```             
+
+To customise the notice colour (button and title border), add
+```
+NOTICES_COLOUR=<colour>  # any css-acceptable colour
+```
+
+## Static assets
+Add `notices/css/notices.css` and `notices/js/notices.js` to your markup.
+
+## Usage
+In templates, load the tags:
+```
+{% load notices_tags %}
+```
+
+and add the modal:
+```
+{% NoticesModal %} 
+```
+
+The modal will be shown.  Once it has been dismissed it won't be shown again unless the notice version changes (see below), the `notice_seen` cookie is deleted, or the notice timeout is reached.
+
+## Setting/updating the notice
+
+### via models and django admin
+Add a `Notice` instance in the django admin. 
+
+Notices have `title`, `content`, `version` and optional `timeout_seconds` and `expires_at` fields.
+
+Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it.
+
+Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
+
+To show a new notice, add another Notice instance with an incremented version number.
+
+### via django settings
+
+Override the Notice model by adding to your `settings.py`:
+`NOTICES_VERSION` # an integer
+`NOTICES_TITLE`  # optional, default = "New!"
+`NOTICES_CONTENT`  # optional, default = ""
+`NOTICES_TIMEOUT_SECONDS`  # optional, default = None
+
+Set `NOTICES_VERSION = 0` to clear the cookie and disable showing notices at all.
```

