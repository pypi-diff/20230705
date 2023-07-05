# Comparing `tmp/django-magnet-data-1.1.8.tar.gz` & `tmp/django-magnet-data-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magnet-data-1.1.8.tar", max compression
+gzip compressed data, was "django-magnet-data-1.1.9.tar", max compression
```

## Comparing `django-magnet-data-1.1.8.tar` & `django-magnet-data-1.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.8/LICENSE
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/__init__.py
--rw-r--r--   0        0        0      241 2023-06-08 18:49:27.912079 django-magnet-data-1.1.8/magnet_data/apps.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/__init__.py
--rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/client.py
--rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.8/magnet_data/currencies/currency_pair.py
--rw-r--r--   0        0        0      290 2023-06-08 18:50:18.368530 django-magnet-data-1.1.8/magnet_data/currencies/enums.py
--rw-r--r--   0        0        0      801 2023-06-08 18:50:34.816675 django-magnet-data-1.1.8/magnet_data/currencies/exceptions.py
--rw-r--r--   0        0        0     1313 2023-06-08 18:50:41.364732 django-magnet-data-1.1.8/magnet_data/currencies/models.py
--rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/urls.py
--rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.8/magnet_data/holidays/__init__.py
--rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/holidays/admin.py
--rw-r--r--   0        0        0    11688 2023-06-08 18:48:25.403508 django-magnet-data-1.1.8/magnet_data/holidays/enums.py
--rw-r--r--   0        0        0     2331 2023-06-23 15:11:37.081168 django-magnet-data-1.1.8/magnet_data/holidays/models.py
--rw-r--r--   0        0        0     3839 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/magnet_data_client.py
--rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/migrations/0001_initial.py
--rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/migrations/0002_holiday.py
--rw-r--r--   0        0        0      354 2023-06-23 16:46:05.694654 django-magnet-data-1.1.8/magnet_data/migrations/0003_alter_holiday_unique_together.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/migrations/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.8/magnet_data/models.py
--rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/utils.py
--rw-r--r--   0        0        0      862 2023-06-23 16:46:03.146652 django-magnet-data-1.1.8/pyproject.toml
--rw-r--r--   0        0        0      748 2023-06-23 16:46:09.588324 django-magnet-data-1.1.8/setup.py
--rw-r--r--   0        0        0      861 2023-06-23 16:46:09.588504 django-magnet-data-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.9/magnet_data/__init__.py
+-rw-r--r--   0        0        0      241 2023-06-08 18:49:27.912079 django-magnet-data-1.1.9/magnet_data/apps.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.9/magnet_data/currencies/__init__.py
+-rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.9/magnet_data/currencies/client.py
+-rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.9/magnet_data/currencies/currency_pair.py
+-rw-r--r--   0        0        0      290 2023-06-08 18:50:18.368530 django-magnet-data-1.1.9/magnet_data/currencies/enums.py
+-rw-r--r--   0        0        0      801 2023-06-08 18:50:34.816675 django-magnet-data-1.1.9/magnet_data/currencies/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-06-08 18:50:41.364732 django-magnet-data-1.1.9/magnet_data/currencies/models.py
+-rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.9/magnet_data/currencies/urls.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.9/magnet_data/holidays/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.9/magnet_data/holidays/admin.py
+-rw-r--r--   0        0        0    11688 2023-06-08 18:48:25.403508 django-magnet-data-1.1.9/magnet_data/holidays/enums.py
+-rw-r--r--   0        0        0     2331 2023-06-23 15:11:37.081168 django-magnet-data-1.1.9/magnet_data/holidays/models.py
+-rw-r--r--   0        0        0     4484 2023-07-05 10:38:29.328243 django-magnet-data-1.1.9/magnet_data/magnet_data_client.py
+-rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.9/magnet_data/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.9/magnet_data/migrations/0002_holiday.py
+-rw-r--r--   0        0        0      354 2023-06-23 16:46:05.694654 django-magnet-data-1.1.9/magnet_data/migrations/0003_alter_holiday_unique_together.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.9/magnet_data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.9/magnet_data/models.py
+-rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.9/magnet_data/utils.py
+-rw-r--r--   0        0        0      862 2023-06-30 17:47:59.311164 django-magnet-data-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      748 2023-07-05 10:39:57.495687 django-magnet-data-1.1.9/setup.py
+-rw-r--r--   0        0        0      861 2023-07-05 10:39:57.495857 django-magnet-data-1.1.9/PKG-INFO
```

### Comparing `django-magnet-data-1.1.8/LICENSE` & `django-magnet-data-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/currencies/client.py` & `django-magnet-data-1.1.9/magnet_data/currencies/client.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/currencies/currency_pair.py` & `django-magnet-data-1.1.9/magnet_data/currencies/currency_pair.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/currencies/exceptions.py` & `django-magnet-data-1.1.9/magnet_data/currencies/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/currencies/models.py` & `django-magnet-data-1.1.9/magnet_data/currencies/models.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/holidays/enums.py` & `django-magnet-data-1.1.9/magnet_data/holidays/enums.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/holidays/models.py` & `django-magnet-data-1.1.9/magnet_data/holidays/models.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/magnet_data_client.py` & `django-magnet-data-1.1.9/magnet_data/magnet_data_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,20 @@
         threshold = now - datetime.timedelta(1)
         if self.last_updated is None or self.last_updated < threshold:
             self.last_updated = now
             self.cls.update_holidays(country_code=country_code.upper())
 
     def is_workday(self, date, country_code: str):
         """
+        Alias for Holidays.get_next_business_day for backwards compatibility
+        """
+        return self.is_workday(date, country_code)
+
+    def is_business_day(self, date, country_code: str):
+        """
         Returns True if the given date is not Saturday, Sunday, or
         Holiday
         Keyword arguments:
             from_date -- date to check
             country-code -- ISO 3166 country code
         """
         self.update(country_code)
@@ -58,14 +64,24 @@
 
     def get_next_working_day(self,
                              country_code: str,
                              working_days: int = 1,
                              from_date: datetime.date = None,
                              step: int = 1):
         """
+        Alias for Holidays.get_next_business_day for backwards compatibility
+        """
+        return self.get_next_business_day(country_code, working_days, from_date, step)
+
+    def get_next_business_day(self,
+                              country_code: str,
+                              working_days: int = 1,
+                              from_date: datetime.date = None,
+                              step: int = 1):
+        """
         Returns the next date that is a working day.
         Keyword arguments:
             country-code -- ISO 3166 country code
             working_days -- number of working days to count (default 1)
             from_date -- date to start counting from (default today)
             step -- the amount by which the index increases. (default 1)
         """
```

### Comparing `django-magnet-data-1.1.8/magnet_data/migrations/0001_initial.py` & `django-magnet-data-1.1.9/magnet_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/magnet_data/migrations/0002_holiday.py` & `django-magnet-data-1.1.9/magnet_data/migrations/0002_holiday.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.8/pyproject.toml` & `django-magnet-data-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-magnet-data"
-version = "1.1.8"
+version = "1.1.9"
 description = "An API client for data.magnet.cl"
 authors = ["Ignacio Munizaga <muni@magnet.cl>"]
 license = "MIT"
 repository = "https://github.com/magnet-cl/django-magnet-data"
 homepage = "https://github.com/magnet-cl/django-magnet-data"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django-magnet-data-1.1.8/setup.py` & `django-magnet-data-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['django>=2.2']
 
 setup_kwargs = {
     'name': 'django-magnet-data',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'An API client for data.magnet.cl',
     'long_description': None,
     'author': 'Ignacio Munizaga',
     'author_email': 'muni@magnet.cl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/magnet-cl/django-magnet-data',
```

### Comparing `django-magnet-data-1.1.8/PKG-INFO` & `django-magnet-data-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magnet-data
-Version: 1.1.8
+Version: 1.1.9
 Summary: An API client for data.magnet.cl
 Home-page: https://github.com/magnet-cl/django-magnet-data
 License: MIT
 Author: Ignacio Munizaga
 Author-email: muni@magnet.cl
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Framework :: Django
```

