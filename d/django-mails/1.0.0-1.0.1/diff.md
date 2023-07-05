# Comparing `tmp/django-mails-1.0.0.tar.gz` & `tmp/django-mails-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mails-1.0.0.tar", last modified: Wed Jun 14 05:07:00 2023, max compression
+gzip compressed data, was "django-mails-1.0.1.tar", last modified: Wed Jul  5 07:58:03 2023, max compression
```

## Comparing `django-mails-1.0.0.tar` & `django-mails-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-06-14 05:07:00.391786 django-mails-1.0.0/
--rw-rw-r--   0 manish    (1000) manish    (1000)     1093 2023-05-30 07:22:53.000000 django-mails-1.0.0/LICENSE
--rw-rw-r--   0 manish    (1000) manish    (1000)     3380 2023-06-14 05:07:00.391786 django-mails-1.0.0/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)     2530 2023-06-06 05:08:16.000000 django-mails-1.0.0/README.md
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-06-14 05:07:00.387786 django-mails-1.0.0/django_mails.egg-info/
--rw-rw-r--   0 manish    (1000) manish    (1000)     3380 2023-06-14 05:07:00.000000 django-mails-1.0.0/django_mails.egg-info/PKG-INFO
--rw-rw-r--   0 manish    (1000) manish    (1000)      594 2023-06-14 05:07:00.000000 django-mails-1.0.0/django_mails.egg-info/SOURCES.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-06-14 05:07:00.000000 django-mails-1.0.0/django_mails.egg-info/dependency_links.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       76 2023-06-14 05:07:00.000000 django-mails-1.0.0/django_mails.egg-info/requires.txt
--rw-rw-r--   0 manish    (1000) manish    (1000)       26 2023-06-14 05:07:00.000000 django-mails-1.0.0/django_mails.egg-info/top_level.txt
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-06-14 05:07:00.387786 django-mails-1.0.0/djangomails/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:11:12.000000 django-mails-1.0.0/djangomails/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      399 2023-05-22 11:19:50.000000 django-mails-1.0.0/djangomails/asgi.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     4187 2023-06-13 11:45:02.000000 django-mails-1.0.0/djangomails/settings.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      276 2023-05-31 09:51:28.000000 django-mails-1.0.0/djangomails/test_settings.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      893 2023-05-25 08:01:42.000000 django-mails-1.0.0/djangomails/urls.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      399 2023-05-22 11:19:50.000000 django-mails-1.0.0/djangomails/wsgi.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-06-14 05:07:00.391786 django-mails-1.0.0/email_service/
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-1.0.0/email_service/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      350 2023-06-09 07:11:49.000000 django-mails-1.0.0/email_service/admin.py
--rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-05-22 11:19:50.000000 django-mails-1.0.0/email_service/apps.py
-drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-06-14 05:07:00.391786 django-mails-1.0.0/email_service/migrations/
--rw-rw-r--   0 manish    (1000) manish    (1000)     5582 2023-05-22 11:19:50.000000 django-mails-1.0.0/email_service/migrations/0001_initial.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-03-24 10:30:19.000000 django-mails-1.0.0/email_service/migrations/__init__.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     2926 2023-06-13 12:53:39.000000 django-mails-1.0.0/email_service/models.py
--rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-05-30 09:39:25.000000 django-mails-1.0.0/email_service/tests.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     5921 2023-06-13 12:53:39.000000 django-mails-1.0.0/email_service/utils.py
--rw-rw-r--   0 manish    (1000) manish    (1000)       26 2023-05-22 11:20:52.000000 django-mails-1.0.0/email_service/views.py
--rw-rw-r--   0 manish    (1000) manish    (1000)     1297 2023-06-14 05:07:00.391786 django-mails-1.0.0/setup.cfg
--rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-05-22 11:19:50.000000 django-mails-1.0.0/setup.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-05 07:58:03.918216 django-mails-1.0.1/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1093 2023-06-22 05:00:04.000000 django-mails-1.0.1/LICENSE
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3383 2023-07-05 07:58:03.918216 django-mails-1.0.1/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2533 2023-07-05 06:53:49.000000 django-mails-1.0.1/README.md
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-05 07:58:03.914218 django-mails-1.0.1/django_mails.egg-info/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     3383 2023-07-05 07:58:03.000000 django-mails-1.0.1/django_mails.egg-info/PKG-INFO
+-rw-rw-r--   0 manish    (1000) manish    (1000)      594 2023-07-05 07:58:03.000000 django-mails-1.0.1/django_mails.egg-info/SOURCES.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)        1 2023-07-05 07:58:03.000000 django-mails-1.0.1/django_mails.egg-info/dependency_links.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       76 2023-07-05 07:58:03.000000 django-mails-1.0.1/django_mails.egg-info/requires.txt
+-rw-rw-r--   0 manish    (1000) manish    (1000)       26 2023-07-05 07:58:03.000000 django-mails-1.0.1/django_mails.egg-info/top_level.txt
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-05 07:58:03.914218 django-mails-1.0.1/djangomails/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      399 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/asgi.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     4187 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/settings.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      276 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/test_settings.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      893 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/urls.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      399 2023-06-22 05:00:04.000000 django-mails-1.0.1/djangomails/wsgi.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-05 07:58:03.918216 django-mails-1.0.1/email_service/
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      350 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/admin.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)      157 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/apps.py
+drwxrwxr-x   0 manish    (1000) manish    (1000)        0 2023-07-05 07:58:03.918216 django-mails-1.0.1/email_service/migrations/
+-rw-rw-r--   0 manish    (1000) manish    (1000)     5582 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/migrations/0001_initial.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/migrations/__init__.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     2926 2023-06-26 05:17:08.000000 django-mails-1.0.1/email_service/models.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)        0 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/tests.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     6087 2023-07-05 06:53:49.000000 django-mails-1.0.1/email_service/utils.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)       26 2023-06-22 05:00:04.000000 django-mails-1.0.1/email_service/views.py
+-rw-rw-r--   0 manish    (1000) manish    (1000)     1297 2023-07-05 07:58:03.918216 django-mails-1.0.1/setup.cfg
+-rw-rw-r--   0 manish    (1000) manish    (1000)       38 2023-06-22 05:00:04.000000 django-mails-1.0.1/setup.py
```

### Comparing `django-mails-1.0.0/LICENSE` & `django-mails-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/PKG-INFO` & `django-mails-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Hashtrust Technologies Private Limited
 Author-email: support@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -61,27 +61,27 @@
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
     attachment: any = None,
-    attachment_path : str | None = None,
+    parts:list[dict] = None,
     enable_logo : bool = False
 )
 ```
 * recipient : List of Receivers emails
 * path : path to html file for email content and subject (path should be upto parent folder of html file inside template folder)
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email as string
 * body : content of email as string
 * attachment: attach file to send email as attachement
-* attachment_path : send string path of attachment,
+* parts (list[dict]): list of dictionaries with part name and data
 * enable_logo : set true to enable logo in email
 
 
 # Setup guideline
 
 - build: Create the build and runtime images
 ```
```

### Comparing `django-mails-1.0.0/README.md` & `django-mails-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -38,27 +38,27 @@
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
     attachment: any = None,
-    attachment_path : str | None = None,
+    parts:list[dict] = None,
     enable_logo : bool = False
 )
 ```
 * recipient : List of Receivers emails
 * path : path to html file for email content and subject (path should be upto parent folder of html file inside template folder)
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email as string
 * body : content of email as string
 * attachment: attach file to send email as attachement
-* attachment_path : send string path of attachment,
+* parts (list[dict]): list of dictionaries with part name and data
 * enable_logo : set true to enable logo in email
 
 
 # Setup guideline
 
 - build: Create the build and runtime images
 ```
```

### Comparing `django-mails-1.0.0/django_mails.egg-info/PKG-INFO` & `django-mails-1.0.1/django_mails.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mails
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Django Library to Send Simple/HTML Emails
 Home-page: https://www.example.com/
 Author: Hashtrust Technologies Private Limited
 Author-email: support@hashtrust.in
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.1
@@ -61,27 +61,27 @@
     path: str | None = None,
     template: any = None,
     template_prefix: str | None = None,
     context: Dict = {},
     subject: str | None = None,
     body: str | None = None,
     attachment: any = None,
-    attachment_path : str | None = None,
+    parts:list[dict] = None,
     enable_logo : bool = False
 )
 ```
 * recipient : List of Receivers emails
 * path : path to html file for email content and subject (path should be upto parent folder of html file inside template folder)
 * template : Object of Template Model if exists (Optional)
 * template_prefix : html file name
 * context : context to replace variable name in template
 * subject : subject of email as string
 * body : content of email as string
 * attachment: attach file to send email as attachement
-* attachment_path : send string path of attachment,
+* parts (list[dict]): list of dictionaries with part name and data
 * enable_logo : set true to enable logo in email
 
 
 # Setup guideline
 
 - build: Create the build and runtime images
 ```
```

### Comparing `django-mails-1.0.0/django_mails.egg-info/SOURCES.txt` & `django-mails-1.0.1/django_mails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/djangomails/settings.py` & `django-mails-1.0.1/djangomails/settings.py`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/djangomails/urls.py` & `django-mails-1.0.1/djangomails/urls.py`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/email_service/migrations/0001_initial.py` & `django-mails-1.0.1/email_service/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/email_service/models.py` & `django-mails-1.0.1/email_service/models.py`

 * *Files identical despite different names*

### Comparing `django-mails-1.0.0/email_service/utils.py` & `django-mails-1.0.1/email_service/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import mimetypes
 import os
 from email.mime.image import MIMEImage
 
 import html2text
 from django.conf import settings
 from django.core.files.base import ContentFile
 from django.core.mail.message import EmailMultiAlternatives
@@ -18,29 +19,29 @@
     path: str = None,
     template: any = None,
     template_prefix: str = None,
     context=None,
     subject: str = None,
     body: str = None,
     attachments: list[ContentFile] = None,
-    attachment_path: str = None,
+    parts: list[dict] = None,
     enable_logo: bool = False,
 ) -> str:
     """This function is responsible to send emails and create emails in database model.
 
     Parameters:
     recipient (list[str]): List of Receivers emails
     path (str): path to html file for email content and subject (path should be upto parent folder of html file inside template folder)
     template (any): Object of Template Model if exists (Optional)
     template_prefix (str): html file name
     context (dict): context to replace variable name in template
     subject (str): subject of email as string
     body (str): content of email as string
     attachment (list[ContentFile]): attach file to send email as attachement
-    attachment_path (str): send string path of attachment,
+    parts (list[dict]): list of dictionaries with part name and data
     enable_logo (bool): set true to enable logo in email
 
     Returns:
     str : email success or error message
     """
     from email_service.models import Attachment, Email
 
@@ -106,29 +107,34 @@
     )
     text_content = html2text.HTML2Text().handle(html_content)
     msg = EmailMultiAlternatives(
         subject or email_subject, text_content, from_email, to, bcc=[bcc_email]
     )
     msg.attach_alternative(html_content, "text/html")
 
-    if attachment_path:
-        full_file_path = f"{settings.BASE_DIR}/{attachment_path}"
-        with open(full_file_path, mode="rb") as file:
-            content_file = ContentFile(
-                file.read(), name=os.path.basename(attachment_path)
-            )
-            attachement = Attachment.objects.create(file=content_file)
-            email.attachments.add(attachement)
-        msg.attach_file(full_file_path)
+    if parts:
+        for part in parts:
+            if "name" not in part or "data" not in part:
+                return "Please provide valid part data. It should include name and data fields"
+            memetype = mimetypes.guess_type(part["name"])
+            msg.attach(part["name"], part["data"], memetype[0])
 
     if attachments:
         for attachement_file in attachments:
             attachement = Attachment.objects.create(file=attachement_file)
             email.attachments.add(attachement)
-            msg.attach_file(f"{settings.BASE_DIR}/{attachement.file.url}")
+            memetype = mimetypes.guess_type(attachement_file.name)
+
+            msg.attach(
+                attachement_file.name,
+                open(
+                    os.path.join(settings.BASE_DIR, attachement.file.path), "rb"
+                ).read(),
+                memetype[0] if memetype else None,
+            )
 
     if enable_logo:
         msg.content_subtype = "html"
         msg.mixed_subtype = "related"
         image_path = os.path.join(
             settings.BASE_DIR, f"static/{settings.LOGO_IMAGE_NAME}"
         )
```

### Comparing `django-mails-1.0.0/setup.cfg` & `django-mails-1.0.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-mails
-version = 1.0.0
+version = 1.0.1
 description = A Django Library to Send Simple/HTML Emails
 readme = "README.md"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.example.com/
 author = Hashtrust Technologies Private Limited
 author_email = support@hashtrust.in
```

