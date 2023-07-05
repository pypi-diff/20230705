# Comparing `tmp/pysomneo-2.5.2.tar.gz` & `tmp/pysomneo-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysomneo-2.5.2.tar", last modified: Sat Mar 25 10:35:31 2023, max compression
+gzip compressed data, was "pysomneo-2.6.0.tar", last modified: Wed Jul  5 10:03:49 2023, max compression
```

## Comparing `pysomneo-2.5.2.tar` & `pysomneo-2.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 10:35:31.542456 pysomneo-2.5.2/
--rw-rw-rw-   0        0        0    35802 2022-07-24 08:01:01.000000 pysomneo-2.5.2/LICENSE
--rw-rw-rw-   0        0        0    41811 2023-03-25 10:35:31.541454 pysomneo-2.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2021-08-16 14:58:00.000000 pysomneo-2.5.2/README.md
--rw-rw-rw-   0        0        0      769 2023-03-25 10:34:47.000000 pysomneo-2.5.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-03-25 10:35:31.498673 pysomneo-2.5.2/pysomneo/
--rw-rw-rw-   0        0        0    20855 2023-03-25 10:34:23.000000 pysomneo-2.5.2/pysomneo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 10:35:31.540453 pysomneo-2.5.2/pysomneo.egg-info/
--rw-rw-rw-   0        0        0    41811 2023-03-25 10:35:31.000000 pysomneo-2.5.2/pysomneo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      181 2023-03-25 10:35:31.000000 pysomneo-2.5.2/pysomneo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 10:35:31.000000 pysomneo-2.5.2/pysomneo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-03-25 10:35:31.000000 pysomneo-2.5.2/pysomneo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 10:35:31.542456 pysomneo-2.5.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 10:03:49.263850 pysomneo-2.6.0/
+-rw-rw-rw-   0        0        0    35802 2023-07-05 09:34:08.000000 pysomneo-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0    41811 2023-07-05 10:03:49.262683 pysomneo-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-07-05 09:34:08.000000 pysomneo-2.6.0/README.md
+-rw-rw-rw-   0        0        0      769 2023-07-05 10:01:51.000000 pysomneo-2.6.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-05 10:03:49.247181 pysomneo-2.6.0/pysomneo/
+-rw-rw-rw-   0        0        0    21637 2023-07-05 10:01:16.000000 pysomneo-2.6.0/pysomneo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-05 10:03:49.261683 pysomneo-2.6.0/pysomneo.egg-info/
+-rw-rw-rw-   0        0        0    41811 2023-07-05 10:03:49.000000 pysomneo-2.6.0/pysomneo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      181 2023-07-05 10:03:49.000000 pysomneo-2.6.0/pysomneo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 10:03:49.000000 pysomneo-2.6.0/pysomneo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-05 10:03:49.000000 pysomneo-2.6.0/pysomneo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 10:03:49.263850 pysomneo-2.6.0/setup.cfg
```

### Comparing `pysomneo-2.5.2/LICENSE` & `pysomneo-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysomneo-2.5.2/PKG-INFO` & `pysomneo-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 2.5.2
+Version: 2.6.0
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pysomneo-2.5.2/pyproject.toml` & `pysomneo-2.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.24.0",
     "urllib3>=1.26.5"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysomneo"
-version = "2.5.2"
+version = "2.6.0"
 authors = [
   { name="Ruud van der Horst", email="pypi@mail.ruudvdhorst.nl" },
 ]
 description = "A library to communicate with the API of Philips Somneo."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `pysomneo-2.5.2/pysomneo/__init__.py` & `pysomneo-2.6.0/pysomneo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,22 @@
 
         # Some Wake-ups lights don't work with wucrv, remove key if exists
         if 'wucrv' in payload:
             payload.pop('wucrv')
 
         self._put('wulgt', payload = payload)
 
+    def dismiss_alarm(self):
+        """ Dismiss a running alarm. """
+        self._put('wualm/alctr', payload={'disms':True})
+
+    def snooze_alarm(self):
+        """ Snooze a running alarm. """
+        self._put('wualm/alctr', payload={'tapsz':True})
+
     def get_alarm_settings(self, alarm):
         """ Get the alarm settings. """
         # Get alarm position
         alarm_pos = self.alarm_data[alarm]['position']
 
         # Get current alarm settings
         return self._put('wualm',payload={'prfnr':alarm_pos})
@@ -294,14 +302,27 @@
             payload.pop('wucrv')
 
         self._put('wulgt', payload=payload)
 
     def update(self):
         """Get the latest update from Somneo."""
 
+        # Get alarm status
+        alarm_status = self._get('wusts')
+        if alarm_status['wusts'] == 1:
+            self.alarm_status = 'off'
+        elif alarm_status['wusts'] == 2321:
+            self.alarm_status = 'snooze'
+        elif alarm_status['wusts'] == 2309:
+            self.alarm_status = 'wake-up'
+        elif alarm_status['wusts'] == 2817:
+            self.alarm_status = 'on'
+        else:
+            self.alarm_status = 'unknown'
+
         # Get light information
         self.light_data = self._get('wulgt')
 
         # Get sensor data
         self.sensor_data = self._get('wusrd')
         
         # Get sunset data
@@ -339,14 +360,16 @@
 
         # Store info in data structure compatible with home assistant coordinator.
         data = dict()
         data['light_is_on'], data['light_brightness'] = self.light_status()
         data['nightlight_is_on'] = self.night_light_status()
         data['alarms'] = self.alarms()
 
+        data['alarm_status'] = self.alarm_status
+
         data['alarms_hour'] = dict()
         data['alarms_minute'] = dict()
         data['alarms_day'] = dict()
         data['powerwake'] = dict()
         data['powerwake_delta'] = dict()
         for alarm in data['alarms']:
             alarm_datetime = datetime.datetime.strptime(self.alarm_data[alarm]['time'].isoformat(),'%H:%M:%S')
```

### Comparing `pysomneo-2.5.2/pysomneo.egg-info/PKG-INFO` & `pysomneo-2.6.0/pysomneo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysomneo
-Version: 2.5.2
+Version: 2.6.0
 Summary: A library to communicate with the API of Philips Somneo.
 Author-email: Ruud van der Horst <pypi@mail.ruudvdhorst.nl>
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

