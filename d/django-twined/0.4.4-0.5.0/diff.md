# Comparing `tmp/django_twined-0.4.4.tar.gz` & `tmp/django_twined-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.4.4.tar", max compression
+gzip compressed data, was "django_twined-0.5.0.tar", max compression
```

## Comparing `django_twined-0.4.4.tar` & `django_twined-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,55 @@
--rw-r--r--   0        0        0     1088 2023-06-21 17:04:03.628860 django_twined-0.4.4/LICENSE
--rw-r--r--   0        0        0     1463 2023-06-21 17:04:03.628860 django_twined-0.4.4/README.md
--rw-r--r--   0        0        0       64 2023-06-21 17:04:03.628860 django_twined-0.4.4/django_twined/__init__.py
--rw-r--r--   0        0        0      257 2023-06-21 17:04:03.628860 django_twined-0.4.4/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     6781 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/admin.py
--rw-r--r--   0        0        0      402 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/apps.py
--rw-r--r--   0        0        0      104 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/__init__.py
--rw-r--r--   0        0        0     3765 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/analysis.py
--rw-r--r--   0        0        0     1001 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/analysis_log.py
--rw-r--r--   0        0        0     5822 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/consumers/service.py
--rw-r--r--   0        0        0      130 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/exceptions.py
--rw-r--r--   0        0        0     2357 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/fields.py
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2299 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2990 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/messages.py
--rw-r--r--   0        0        0     2345 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4710 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      698 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11440 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9794 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     6623 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/questions.py
--rw-r--r--   0        0        0     7824 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     2514 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      290 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/routing.py
--rw-r--r--   0        0        0      479 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3079 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/static/.gitignore
--rw-r--r--   0        0        0     2666 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/tasks.py
--rw-r--r--   0        0        0     1149 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2023-06-21 17:04:03.632860 django_twined-0.4.4/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0     1532 2023-06-21 17:04:03.632860 django_twined-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_twined-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-07-05 16:34:11.450003 django_twined-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1463 2023-07-05 16:34:11.450003 django_twined-0.5.0/README.md
+-rw-r--r--   0        0        0       64 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/__init__.py
+-rw-r--r--   0        0        0      257 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     6781 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/admin/admin.py
+-rw-r--r--   0        0        0      402 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/apps.py
+-rw-r--r--   0        0        0      104 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/consumers/__init__.py
+-rw-r--r--   0        0        0     3766 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/consumers/analysis.py
+-rw-r--r--   0        0        0     1002 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/consumers/analysis_log.py
+-rw-r--r--   0        0        0     5823 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/consumers/service.py
+-rw-r--r--   0        0        0      130 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2358 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2300 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2991 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/messages.py
+-rw-r--r--   0        0        0     2346 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4711 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      698 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11441 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9795 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     6624 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/questions.py
+-rw-r--r--   0        0        0     8628 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     2515 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      290 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/routing.py
+-rw-r--r--   0        0        0      479 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3080 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     2667 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/tasks.py
+-rw-r--r--   0        0        0     1149 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0      175 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/urls.py
+-rw-r--r--   0        0        0     2419 2023-07-05 16:34:11.450003 django_twined-0.5.0/django_twined/views.py
+-rw-r--r--   0        0        0     1552 2023-07-05 16:34:11.454003 django_twined-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 django_twined-0.5.0/PKG-INFO
```

### Comparing `django_twined-0.4.4/LICENSE` & `django_twined-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/README.md` & `django_twined-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/admin/admin.py` & `django_twined-0.5.0/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/admin/mixins.py` & `django_twined-0.5.0/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/admin/proxy.py` & `django_twined-0.5.0/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/consumers/analysis.py` & `django_twined-0.5.0/django_twined/consumers/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 from uuid import uuid4
+
 from asgiref.sync import async_to_sync
 from channels.generic.websocket import WebsocketConsumer
 from django.core.cache import cache
 from django_twined.messages import ReelMessage
 from django_twined.tasks import ask
```

### Comparing `django_twined-0.4.4/django_twined/consumers/analysis_log.py` & `django_twined-0.5.0/django_twined/consumers/analysis_log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from channels.generic.websocket import WebsocketConsumer
 from django_twined.messages import ReelMessage
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/consumers/service.py` & `django_twined-0.5.0/django_twined/consumers/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+
 from asgiref.sync import async_to_sync
 from channels.generic.websocket import WebsocketConsumer
 from django.conf import settings
 from django_twined.messages import ReelMessage
 from django_twined.tasks import ask
```

### Comparing `django_twined-0.4.4/django_twined/fields.py` & `django_twined-0.5.0/django_twined/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from django.conf import settings
 from django.db import models
 from django.utils.module_loading import import_string
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.5.0/django_twined/management/commands/sync_data_stores.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from django.apps import apps
 from django.conf import settings
 from django.core.management.base import BaseCommand
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/messages.py` & `django_twined-0.5.0/django_twined/messages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 from time import time
 from uuid import uuid4
+
 import django.dispatch
 from asgiref.sync import async_to_sync
 from channels.layers import get_channel_layer
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/migrations/0001_initial.py` & `django_twined-0.5.0/django_twined/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Disable for migrations:
 # pylint: disable=missing-docstring
 
 import uuid
+
 import django.db.models.deletion
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
```

### Comparing `django_twined-0.4.4/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.5.0/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.5.0/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.5.0/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.5.0/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Disable for migrations:
 # pylint: disable=missing-docstring
 
 import uuid
+
 import django.db.models.deletion
 import django_twined.models.service_revisions
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
```

### Comparing `django_twined-0.4.4/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.5.0/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.5.0/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.5.0/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.5.0/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.5.0/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.5.0/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/models/__init__.py` & `django_twined-0.5.0/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/django_twined/models/datastores.py` & `django_twined-0.5.0/django_twined/models/datastores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import uuid
 import warnings
+
 from django.db import models
 from octue.resources import Datafile
 from octue.utils.encoders import OctueJSONEncoder
 
 from .querysets import DatastoreQueryset
```

### Comparing `django_twined-0.4.4/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.5.0/django_twined/models/querysets/datastore_queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from django.db import transaction
 from django.db.models.query import QuerySet
 from django.db.utils import IntegrityError
 from octue.resources import Datafile, Dataset
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/models/questions.py` & `django_twined-0.5.0/django_twined/models/questions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import uuid
 from datetime import datetime, timezone
+
 from django.db import models
 from model_utils.managers import InheritanceManager
 
 from ..fields import ManifestField, ValuesField
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/models/service_revisions.py` & `django_twined-0.5.0/django_twined/models/service_revisions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 import logging
+
+import packaging.version
 from django.conf import settings
 from django.db import models, transaction
 from django_gcp.events.utils import get_event_url
 from octue.cloud.pub_sub.service import Service
 from octue.resources.service_backends import get_backend
 
 from .service_usage_events import QUESTION_RESPONSE_UPDATED
 
 
 logger = logging.getLogger(__name__)
 
 QUESTION_ASK_TIMEOUT_SECONDS = 60
 
 
+def service_revision_is_latest_semantic_version(service_revision):
+    """Determine if a service revision is the latest semantic version based on its revision tag.
+
+    :param django_twined.models.service_revision.ServiceRevision service_revision: the service revision to check
+    :return bool: `True` if the service revision is the latest semantic version according to its revision tag
+    """
+    sorted_service_revisions = sorted(
+        [
+            *ServiceRevision.objects.filter(namespace=service_revision.namespace, name=service_revision.name),
+            service_revision,
+        ],
+        key=lambda revision: packaging.version.parse(revision.tag),
+    )
+
+    return sorted_service_revisions[-1] == service_revision
+
+
 def get_default_namespace():
     """Return the default namespace for service revisions"""
     return settings.TWINED_DEFAULT_NAMESPACE
 
 
 def get_default_project_name():
     """Return the default project name for service revisions"""
@@ -179,23 +198,27 @@
     def __str__(self):
         return self.sruid
 
     def __repr__(self):
         return f"Service Revision ({self.sruid})"
 
     def save(self, *args, **kwargs):
-        """Override save method to ensure that there can be only one default service revision"""
+        """Override save method to ensure that there can be only one default service revision."""
         with transaction.atomic():
             if self.is_default:
                 previous_default = ServiceRevision.objects.filter(
-                    namespace=self.namespace, name=self.name, is_default=True
+                    namespace=self.namespace,
+                    name=self.name,
+                    is_default=True,
                 ).first()
+
                 if previous_default is not None:
                     previous_default.is_default = False
                     previous_default.save()
+
             super().save(*args, **kwargs)
 
 
 class ServiceRevision(AbstractServiceRevision):
     """Concrete model to register available service revisions in the system"""
```

### Comparing `django_twined-0.4.4/django_twined/models/service_usage_events.py` & `django_twined-0.5.0/django_twined/models/service_usage_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from django.db import models
 
 
 logger = logging.getLogger(__name__)
 
 
 QUESTION_ASKED = "q-asked"
```

### Comparing `django_twined-0.4.4/django_twined/signals/receivers.py` & `django_twined-0.5.0/django_twined/signals/receivers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from django.dispatch import receiver
 from django_gcp.events.signals import event_received
 from django_gcp.events.utils import decode_pubsub_message
 from django_twined.models import QUESTION_ASKED, QUESTION_RESPONSE_UPDATED, ServiceUsageEvent
 from django_twined.signals.senders import (
     delivery_acknowledgement_received,
     exception_received,
```

### Comparing `django_twined-0.4.4/django_twined/tasks.py` & `django_twined-0.5.0/django_twined/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+
 import dramatiq
 from django.conf import settings
 from django_twined.messages import ReelMessage
 from octue import Runner
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `django_twined-0.4.4/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.5.0/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.4.4/pyproject.toml` & `django_twined-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.4.4"
+version = "0.5.0"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -45,11 +45,12 @@
 pytest-sugar = "^0.9.4"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-tabs = "^3.2.0"
 Sphinx = "^4.4.0"
 tox = "^3.24.5"
 tox-gh-actions = "^2.9.1"
 tox-poetry = "^0.4.1"
+icecream = "^2.1.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_twined-0.4.4/PKG-INFO` & `django_twined-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.4.4
+Version: 0.5.0
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<3.11
```

