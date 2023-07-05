# Comparing `tmp/pasco-0.3.62.tar.gz` & `tmp/pasco-0.3.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasco-0.3.62.tar", last modified: Tue Jun  6 16:57:10 2023, max compression
+gzip compressed data, was "pasco-0.3.63.tar", last modified: Wed Jul  5 15:56:01 2023, max compression
```

## Comparing `pasco-0.3.62.tar` & `pasco-0.3.63.tar`

### file list

```diff
@@ -1,29 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:57:10.320940 pasco-0.3.62/
--rw-rw-rw-   0        0        0     2355 2023-05-31 18:14:15.000000 pasco-0.3.62/LICENSE
--rw-rw-rw-   0        0        0       31 2023-05-31 18:14:15.000000 pasco-0.3.62/MANIFEST.in
--rw-rw-rw-   0        0        0    13805 2023-06-06 16:57:10.320940 pasco-0.3.62/PKG-INFO
--rw-rw-rw-   0        0        0    13277 2023-06-06 16:47:15.000000 pasco-0.3.62/README.md
--rw-rw-rw-   0        0        0      128 2023-05-31 18:14:15.000000 pasco-0.3.62/pyproject.toml
--rw-rw-rw-   0        0        0      737 2023-06-06 16:57:10.322938 pasco-0.3.62/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 16:57:10.259974 pasco-0.3.62/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 16:57:10.286959 pasco-0.3.62/src/pasco/
--rw-rw-rw-   0        0        0      245 2023-06-06 16:51:21.000000 pasco-0.3.62/src/pasco/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:57:10.318940 pasco-0.3.62/src/pasco/__pycache__/
--rw-rw-rw-   0        0        0      559 2023-06-05 22:21:36.000000 pasco-0.3.62/src/pasco/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     8096 2023-05-31 19:06:43.000000 pasco-0.3.62/src/pasco/__pycache__/character_library.cpython-311.pyc
--rw-rw-rw-   0        0        0     8736 2023-06-05 15:43:23.000000 pasco-0.3.62/src/pasco/__pycache__/code_node_device.cpython-311.pyc
--rw-rw-rw-   0        0        0    15115 2023-06-05 22:21:36.000000 pasco-0.3.62/src/pasco/__pycache__/control_node_device.cpython-311.pyc
--rw-rw-rw-   0        0        0    57154 2023-06-05 15:58:36.000000 pasco-0.3.62/src/pasco/__pycache__/pasco_ble_device.cpython-311.pyc
--rw-rw-rw-   0        0        0     1132 2023-06-05 23:55:13.000000 pasco-0.3.62/src/pasco/__pycache__/pasco_bot.cpython-311.pyc
--rw-rw-rw-   0        0        0     8816 2023-05-31 18:14:15.000000 pasco-0.3.62/src/pasco/character_library.py
--rw-rw-rw-   0        0        0     6119 2023-06-06 16:51:21.000000 pasco-0.3.62/src/pasco/code_node_device.py
--rw-rw-rw-   0        0        0    14200 2023-06-06 16:51:21.000000 pasco-0.3.62/src/pasco/control_node_device.py
--rw-rw-rw-   0        0        0   600774 2023-05-31 18:14:15.000000 pasco-0.3.62/src/pasco/datasheets.xml
--rw-rw-rw-   0        0        0    45810 2023-06-06 16:51:21.000000 pasco-0.3.62/src/pasco/pasco_ble_device.py
--rw-rw-rw-   0        0        0      572 2023-06-06 16:42:52.000000 pasco-0.3.62/src/pasco/pasco_bot.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:57:10.298952 pasco-0.3.62/src/pasco.egg-info/
--rw-rw-rw-   0        0        0    13805 2023-06-06 16:57:10.000000 pasco-0.3.62/src/pasco.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      731 2023-06-06 16:57:10.000000 pasco-0.3.62/src/pasco.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:57:10.000000 pasco-0.3.62/src/pasco.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-06 16:57:10.000000 pasco-0.3.62/src/pasco.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 16:57:10.000000 pasco-0.3.62/src/pasco.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 15:56:01.620617 pasco-0.3.63/
+-rw-rw-rw-   0        0        0     2355 2023-07-05 15:41:02.000000 pasco-0.3.63/LICENSE
+-rw-rw-rw-   0        0        0       31 2023-07-05 15:41:02.000000 pasco-0.3.63/MANIFEST.in
+-rw-rw-rw-   0        0        0    13769 2023-07-05 15:56:01.621614 pasco-0.3.63/PKG-INFO
+-rw-rw-rw-   0        0        0    13241 2023-07-05 15:42:02.000000 pasco-0.3.63/README.md
+-rw-rw-rw-   0        0        0      128 2023-07-05 15:41:02.000000 pasco-0.3.63/pyproject.toml
+-rw-rw-rw-   0        0        0      790 2023-07-05 15:56:01.622611 pasco-0.3.63/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 15:56:01.597680 pasco-0.3.63/src/
+drwxrwxrwx   0        0        0        0 2023-07-05 15:56:01.613636 pasco-0.3.63/src/pasco/
+-rw-rw-rw-   0        0        0      212 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/__init__.py
+-rw-rw-rw-   0        0        0     8816 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/character_library.py
+-rw-rw-rw-   0        0        0     5967 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/code_node_device.py
+-rw-rw-rw-   0        0        0     7950 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/control_node_device.py
+-rw-rw-rw-   0        0        0   600774 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/datasheets.xml
+-rw-rw-rw-   0        0        0    45806 2023-07-05 15:41:02.000000 pasco-0.3.63/src/pasco/pasco_ble_device.py
+drwxrwxrwx   0        0        0        0 2023-07-05 15:56:01.620617 pasco-0.3.63/src/pasco.egg-info/
+-rw-rw-rw-   0        0        0    13769 2023-07-05 15:56:01.000000 pasco-0.3.63/src/pasco.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-07-05 15:56:01.000000 pasco-0.3.63/src/pasco.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 15:56:01.000000 pasco-0.3.63/src/pasco.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-05 15:56:01.000000 pasco-0.3.63/src/pasco.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-05 15:56:01.000000 pasco-0.3.63/src/pasco.egg-info/top_level.txt
```

### Comparing `pasco-0.3.62/LICENSE` & `pasco-0.3.63/LICENSE`

 * *Files identical despite different names*

### Comparing `pasco-0.3.62/PKG-INFO` & `pasco-0.3.63/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pasco
-Version: 0.3.62
+Version: 0.3.63
 Summary: PASCO Python API for Wireless Sensors
 Author: Waqas Saeed
 Project-URL: Bug Tracker, https://github.com/PASCOscientific/pasco_python/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/pasco/)
+[![Python](https://img.shields.io/badge/python-3.11-blue)](https://pypi.org/project/pasco/)
 
 ![Platform](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)
 
 # README
 
 This PASCO Python library allows users to connect to PASCO Wireless sensors using Python. Create your own data collection application, use sensors to interact with other hardware devices, or come up with your own unique solution!
```

### Comparing `pasco-0.3.62/README.md` & `pasco-0.3.63/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/pasco/)
+[![Python](https://img.shields.io/badge/python-3.11-blue)](https://pypi.org/project/pasco/)
 
 ![Platform](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)
 
 # README
 
 This PASCO Python library allows users to connect to PASCO Wireless sensors using Python. Create your own data collection application, use sensors to interact with other hardware devices, or come up with your own unique solution!
```

### Comparing `pasco-0.3.62/setup.cfg` & `pasco-0.3.63/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6173 636f 0d0a 7665 7273 696f   = pasco..versio
-00000020: 6e20 3d20 302e 332e 3632 0d0a 6175 7468  n = 0.3.62..auth
+00000020: 6e20 3d20 302e 332e 3633 0d0a 6175 7468  n = 0.3.63..auth
 00000030: 6f72 203d 2057 6171 6173 2053 6165 6564  or = Waqas Saeed
 00000040: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000050: 5041 5343 4f20 5079 7468 6f6e 2041 5049  PASCO Python API
 00000060: 2066 6f72 2057 6972 656c 6573 7320 5365   for Wireless Se
 00000070: 6e73 6f72 730d 0a6c 6f6e 675f 6465 7363  nsors..long_desc
 00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
 00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
@@ -37,11 +37,14 @@
 00000240: 7569 7265 7320 3d20 0d0a 0962 6c65 616b  uires = ...bleak
 00000250: 3d3d 302e 3230 2e32 0d0a 096e 6573 745f  ==0.20.2...nest_
 00000260: 6173 796e 6369 6f3d 3d31 2e35 2e36 0d0a  asyncio==1.5.6..
 00000270: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
 00000280: 6461 7461 203d 2054 7275 650d 0a0d 0a5b  data = True....[
 00000290: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
 000002a0: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
-000002b0: 7372 630d 0a0d 0a5b 6567 675f 696e 666f  src....[egg_info
-000002c0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000002d0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000002e0: 0a                                       .
+000002b0: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
+000002c0: 7061 636b 6167 655f 6461 7461 5d0d 0a70  package_data]..p
+000002d0: 6173 636f 203d 200d 0a09 6461 7461 7368  asco = ...datash
+000002e0: 6565 7473 2e78 6d6c 0d0a 0d0a 5b65 6767  eets.xml....[egg
+000002f0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000300: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000310: 2030 0d0a 0d0a                            0....
```

### Comparing `pasco-0.3.62/src/pasco/character_library.py` & `pasco-0.3.63/src/pasco/character_library.py`

 * *Files identical despite different names*

### Comparing `pasco-0.3.62/src/pasco/code_node_device.py` & `pasco-0.3.63/src/pasco/code_node_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         if intensity and type(intensity) not in (int, float):
             raise self.InvalidParameter
 
         led_index = 20 - (y * 5) + x # Converts xy position to LED index
         led_intensity = self._limit(intensity, 0, 255)
 
         cmd = [ self.GCMD_CODENODE_CMD, self.CODENODE_CMD_SET_LED, led_index, led_intensity ]
-        self._loop.run_until_complete(self.write_await_callback(self.SENSOR_SERVICE_ID, cmd))
+        self._send_command(self.SENSOR_SERVICE_ID, cmd)
 
 
     def set_leds_in_array(self, xy_list=[], intensity=128):
         """
         Set multiple LEDs on the 5x5 Matrix
 
         Args:
@@ -67,15 +67,15 @@
             led_activate += 2 ** led_index
 
         led_intensity = self._limit(intensity, 0, 255)
 
         cmd = [ self.GCMD_CODENODE_CMD, self.CODENODE_CMD_SET_LEDS,
                 led_activate & 0xFF, led_activate>>8 & 0XFF, led_activate>>16 & 0XFF, led_activate>>24 & 0XFF,
                 led_intensity ]
-        self._loop.run_until_complete(self.write_await_callback(self.SENSOR_SERVICE_ID, cmd))
+        self._send_command(self.SENSOR_SERVICE_ID, cmd)
 
 
     def set_rgb_led(self, red, green, blue):
         """
         Set the //code.Node's RGB LED
         
         Args:
@@ -92,15 +92,15 @@
             raise self.InvalidParameter
 
         led_r = int(self._limit(red, 0, 255))
         led_g = int(self._limit(green, 0, 255))
         led_b = int(self._limit(blue, 0, 255))
 
         cmd = [ self.GCMD_CODENODE_CMD, self.CODENODE_CMD_SET_LEDS, led_r, led_g, led_b, 0X80, 0X00 ]
-        self._loop.run_until_complete(self.write_await_callback(self.SENSOR_SERVICE_ID, cmd))
+        self._send_command(self.SENSOR_SERVICE_ID, cmd)
 
 
     def set_sound_frequency(self, frequency):
         """
         Control the code node's built in speaker output frequency
 
         Args:
@@ -111,15 +111,15 @@
 
         if frequency and type(frequency) not in (int, float):
             raise self.InvalidParameter
 
         frequency = self._limit(frequency, 0, 20000)
 
         cmd = [ self.GCMD_CODENODE_CMD, self.CODENODE_CMD_SET_SOUND_FREQ, frequency & 0xFF, frequency>>8 & 0XFF ]
-        self._loop.run_until_complete(self.write_await_callback(self.SENSOR_SERVICE_ID, cmd))
+        self._send_command(self.SENSOR_SERVICE_ID, cmd)
 
 
     def scroll_text_in_array(self, text):
         """
         Scroll text/numbers on the 5x5 LED Array
 
         Args:
```

### Comparing `pasco-0.3.62/src/pasco/datasheets.xml` & `pasco-0.3.63/src/pasco/datasheets.xml`

 * *Files identical despite different names*

### Comparing `pasco-0.3.62/src/pasco/pasco_ble_device.py` & `pasco-0.3.63/src/pasco/pasco_ble_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,19 +347,19 @@
                 for c in interface.findall("./Channel")
             ]
 
             for sensor in self._setup_sensors:
                 if sensor['type'] == 'Pasport' and sensor['sensor_id'] == "" and sensor['plug_detect'] == 1:
                     do_plug_detect = True
 
-            # if do_plug_detect:
-            #     print("detecting")
-            #     self.detect_controlnode_devices()
-            # else:
-            self.get_sensor_datasheet_info()
+            if do_plug_detect:
+                print("detecting")
+                self.detect_controlnode_devices()
+            else:
+                self.get_sensor_datasheet_info()
         
         except:
             raise self.SensorSetupError
 
 
     def get_sensor_datasheet_info(self):
         try:
```

### Comparing `pasco-0.3.62/src/pasco.egg-info/PKG-INFO` & `pasco-0.3.63/src/pasco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pasco
-Version: 0.3.62
+Version: 0.3.63
 Summary: PASCO Python API for Wireless Sensors
 Author: Waqas Saeed
 Project-URL: Bug Tracker, https://github.com/PASCOscientific/pasco_python/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-blue)](https://pypi.org/project/pasco/)
+[![Python](https://img.shields.io/badge/python-3.11-blue)](https://pypi.org/project/pasco/)
 
 ![Platform](https://img.shields.io/badge/platform-windows%20%7C%20macos%20%7C%20linux-lightgrey)
 
 # README
 
 This PASCO Python library allows users to connect to PASCO Wireless sensors using Python. Create your own data collection application, use sensors to interact with other hardware devices, or come up with your own unique solution!
```

