# Comparing `tmp/minidevice-2.1.4.tar.gz` & `tmp/minidevice-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.1.4.tar", last modified: Sat Jun 24 15:13:22 2023, max compression
+gzip compressed data, was "minidevice-2.1.5.tar", last modified: Wed Jul  5 11:38:58 2023, max compression
```

## Comparing `minidevice-2.1.4.tar` & `minidevice-2.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 15:13:22.084527 minidevice-2.1.4/
--rw-rw-rw-   0        0        0      811 2023-06-24 15:13:22.083529 minidevice-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-06-24 12:06:18.000000 minidevice-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 15:13:22.079552 minidevice-2.1.4/minidevice/
--rw-rw-rw-   0        0        0     2980 2023-06-24 15:12:37.000000 minidevice-2.1.4/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.1.4/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      300 2023-06-24 12:06:51.000000 minidevice-2.1.4/minidevice/__init__.py
--rw-rw-rw-   0        0        0     5035 2023-06-24 09:21:19.000000 minidevice-2.1.4/minidevice/adb.py
--rw-rw-rw-   0        0        0      467 2023-06-24 09:21:26.000000 minidevice-2.1.4/minidevice/adbcap.py
--rw-rw-rw-   0        0        0      819 2023-06-24 09:18:16.000000 minidevice-2.1.4/minidevice/adbtouch.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.1.4/minidevice/logger.py
--rw-rw-rw-   0        0        0    13045 2023-06-24 09:46:11.000000 minidevice-2.1.4/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1498 2023-06-24 07:22:12.000000 minidevice-2.1.4/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      651 2023-06-24 09:39:45.000000 minidevice-2.1.4/minidevice/scrcpycap.py
--rw-rw-rw-   0        0        0     1049 2023-06-24 09:39:50.000000 minidevice-2.1.4/minidevice/scrcpytouch.py
--rw-rw-rw-   0        0        0      687 2023-06-21 07:24:32.000000 minidevice-2.1.4/minidevice/screencap.py
--rw-rw-rw-   0        0        0      620 2023-06-24 07:21:44.000000 minidevice-2.1.4/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-24 15:13:22.083529 minidevice-2.1.4/minidevice.egg-info/
--rw-rw-rw-   0        0        0      811 2023-06-24 15:13:22.000000 minidevice-2.1.4/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-24 15:13:22.000000 minidevice-2.1.4/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 15:13:22.000000 minidevice-2.1.4/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-06-24 15:13:22.000000 minidevice-2.1.4/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 15:13:22.000000 minidevice-2.1.4/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 15:13:22.084527 minidevice-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-24 15:06:27.000000 minidevice-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.517990 minidevice-2.1.5/
+-rw-rw-rw-   0        0        0      811 2023-07-05 11:38:58.517015 minidevice-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-07-05 10:51:23.000000 minidevice-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.505311 minidevice-2.1.5/minidevice/
+-rw-rw-rw-   0        0        0     2980 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-07-05 10:51:23.000000 minidevice-2.1.5/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      300 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     5061 2023-07-05 11:36:46.000000 minidevice-2.1.5/minidevice/adb.py
+-rw-rw-rw-   0        0        0      469 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/adbcap.py
+-rw-rw-rw-   0        0        0      823 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/adbtouch.py
+-rw-rw-rw-   0        0        0       39 2023-07-05 11:31:42.000000 minidevice-2.1.5/minidevice/logger.py
+-rw-rw-rw-   0        0        0    13512 2023-07-05 11:36:46.000000 minidevice-2.1.5/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1502 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      649 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/scrcpycap.py
+-rw-rw-rw-   0        0        0     1035 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/scrcpytouch.py
+-rw-rw-rw-   0        0        0      690 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      605 2023-07-05 11:03:04.000000 minidevice-2.1.5/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-07-05 11:38:58.516039 minidevice-2.1.5/minidevice.egg-info/
+-rw-rw-rw-   0        0        0      811 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-05 11:38:58.000000 minidevice-2.1.5/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-05 11:38:58.517990 minidevice-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-05 11:03:04.000000 minidevice-2.1.5/setup.py
```

### Comparing `minidevice-2.1.4/PKG-INFO` & `minidevice-2.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.4
+Version: 2.1.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.4/README.md` & `minidevice-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.4/minidevice/DroidCast.py` & `minidevice-2.1.5/minidevice/DroidCast.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 from minidevice.adb import ADB, ADB_PATH
 from minidevice.screencap import ScreenCap
 
 WORK_DIR = os.path.dirname(__file__)
 APK_PATH = "{}/bin/DroidCast-debug-1.1.0.apk".format(WORK_DIR)
 APK_ANDROID_PATH = "/data/local/tmp/DroidCast-debug-1.0.apk"
 
+
 class DroidCast(ScreenCap):
     def __init__(self, device, DroidCastServerPort=53516) -> None:
         """
         __init__ DroidCast截图方法
 
         Args:
             device (str): 设备id
             DroidCastServerPort (int, optional): DroidCastServerPort服务端端口号. Defaults to 53516.
         """
         self.droidcast_adb = ADB(device)
         self.DroidCastServerPort = DroidCastServerPort
-        self.class_path = APK_ANDROID_PATH 
+        self.class_path = APK_ANDROID_PATH
         self.DroidCastSession = requests.Session()
         self.__install()
         self.__start()
 
     def __install(self):
         self.droidcast_adb.push_file(APK_PATH, self.class_path)
         self.droidcast_adb.install_apk(APK_PATH)
@@ -38,15 +39,15 @@
         )
         prefix = "package:"
         postfix = ".apk"
         beg = out.index(prefix, 0)
         end = out.rfind(postfix)
 
         self.class_path = (
-            "CLASSPATH=" + out[beg + len(prefix) : (end + len(postfix))].strip()
+                "CLASSPATH=" + out[beg + len(prefix): (end + len(postfix))].strip()
         )
         print(self.class_path)
         start_droidcast_cmd = (
             "exec app_process / com.rayworks.droidcast.Main --port={}".format(
                 self.DroidCastServerPort
             )
         )
@@ -87,8 +88,7 @@
         if self.droidcast_popen.poll() is not None:
             self.__stop()
             self.__start()
         return self.DroidCastSession.get(self.droidcast_url, timeout=3).content
 
     def __del__(self):
         self.__stop()
-
```

### Comparing `minidevice-2.1.4/minidevice/QueueUtils.py` & `minidevice-2.1.5/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.1.4/minidevice/adb.py` & `minidevice-2.1.5/minidevice/adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+import random
 import shutil
 import subprocess
-import random
-from minidevice.logger import logger
 
-
-from minidevice.screencap import ScreenCap
-from minidevice.touch import Touch
+from minidevice.logger import logger
 
 ADB_PATH = "adb"
 if shutil.which("adb.exe") is None:
     import os
 
     WORK_DIR = os.path.dirname(__file__)
     ADB_PATH = shutil.which("adb.exe", path="{}/bin".format(WORK_DIR))
 
 
 class ADB:
     def __init__(self, device=None):
+        if device is not None and device not in self.list_devices():
+            raise Exception("设备不存在")
         self.device = device
 
     def adb_command(self, command: list):
         """执行shell脚本语句,获取返回的源数据"""
         adb_command = [ADB_PATH]
         if self.device:
             adb_command.extend(["-s", self.device])
@@ -130,12 +129,7 @@
     dict_info = {}
     lines = str.splitlines()
     for line in lines:
         if ":" in line:
             key, value = line.split(":", 1)
             dict_info[key.strip()] = value.strip()
     return dict_info
-
-
-
-
-
```

### Comparing `minidevice-2.1.4/minidevice/adbtouch.py` & `minidevice-2.1.5/minidevice/adbtouch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from minidevice.logger import logger
 from minidevice.adb import ADB
+from minidevice.logger import logger
 from minidevice.touch import Touch
 
+
 class ADBtouch(Touch, ADB):
     def __init__(self, device) -> None:
         """
         __init__ ADB 操作方式
 
         Args:
             device (str): 设备id
@@ -18,8 +19,8 @@
 
     def swipe(self, points: list, duration: int = 300):
         start_x, start_y = points[0]
         end_x, end_y = points[-1]
         ADB.swipe(self, start_x, start_y, end_x, end_y, duration)
         logger.debug(
             f"ADB swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
-        )
+        )
```

### Comparing `minidevice-2.1.4/minidevice/minicap.py` & `minidevice-2.1.5/minidevice/minicap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import socket
 import struct
 import subprocess
 import threading
 import time
 
+from minidevice.QueueUtils import PipeQueue
 from minidevice.adb import ADB, ADB_PATH
 from minidevice.logger import logger
-from minidevice.QueueUtils import PipeQueue
 from minidevice.screencap import ScreenCap
 
 WORK_DIR = os.path.dirname(__file__)
 MINICAP_PATH = "{}/bin/minicap/libs".format(WORK_DIR)
 MINICAPSO_PATH = "{}/bin/minicap/jni".format(WORK_DIR)
 
 
@@ -33,33 +33,33 @@
         self.VirtualWidth = 0  # 设备的虚拟宽度
         self.VirtualHeight = 0  # 设备的虚拟高度
         self.Orientation = 0  # 设备方向
         self.Quirks = 0  # 设备信息获取策略
 
     def __str__(self):
         message = (
-            "Banner [Version="
-            + str(self.Version)
-            + ", length="
-            + str(self.Length)
-            + ", Pid="
-            + str(self.Pid)
-            + ", realWidth="
-            + str(self.RealWidth)
-            + ", realHeight="
-            + str(self.RealHeight)
-            + ", virtualWidth="
-            + str(self.VirtualWidth)
-            + ", virtualHeight="
-            + str(self.VirtualHeight)
-            + ", orientation="
-            + str(self.Orientation)
-            + ", quirks="
-            + str(self.Quirks)
-            + "]"
+                "Banner [Version="
+                + str(self.Version)
+                + ", length="
+                + str(self.Length)
+                + ", Pid="
+                + str(self.Pid)
+                + ", realWidth="
+                + str(self.RealWidth)
+                + ", realHeight="
+                + str(self.RealHeight)
+                + ", virtualWidth="
+                + str(self.VirtualWidth)
+                + ", virtualHeight="
+                + str(self.VirtualHeight)
+                + ", orientation="
+                + str(self.Orientation)
+                + ", quirks="
+                + str(self.Quirks)
+                + "]"
         )
         return message
 
     def set_of_bytes(self, data):
         (
             self.Version,
             self.Length,
@@ -132,51 +132,51 @@
                     if readBannerBytes == 0:
                         self.banner.Version = chunk[cursor]
                     elif readBannerBytes == 1:
                         bannerLength = chunk[cursor]
                         self.banner.Length = bannerLength
                     elif readBannerBytes in [2, 3, 4, 5]:
                         self.banner.Pid += (
-                            chunk[cursor] << ((readBannerBytes - 2) * 8)
-                        ) >> 0
+                                                   chunk[cursor] << ((readBannerBytes - 2) * 8)
+                                           ) >> 0
                     elif readBannerBytes in [6, 7, 8, 9]:
                         self.banner.RealWidth += (
-                            chunk[cursor] << ((readBannerBytes - 6) * 8)
-                        ) >> 0
+                                                         chunk[cursor] << ((readBannerBytes - 6) * 8)
+                                                 ) >> 0
                     elif readBannerBytes in [10, 11, 12, 13]:
                         self.banner.RealHeight += (
-                            chunk[cursor] << ((readBannerBytes - 10) * 8)
-                        ) >> 0
+                                                          chunk[cursor] << ((readBannerBytes - 10) * 8)
+                                                  ) >> 0
                     elif readBannerBytes in [14, 15, 16, 17]:
                         self.banner.VirtualWidth += (
-                            chunk[cursor] << ((readBannerBytes - 14) * 8)
-                        ) >> 0
+                                                            chunk[cursor] << ((readBannerBytes - 14) * 8)
+                                                    ) >> 0
                     elif readBannerBytes in [18, 19, 20, 21]:
                         self.banner.VirtualHeight += (
-                            chunk[cursor] << ((readBannerBytes - 18) * 8)
-                        ) >> 0
+                                                             chunk[cursor] << ((readBannerBytes - 18) * 8)
+                                                     ) >> 0
                     elif readBannerBytes == 22:
                         self.banner.Orientation = chunk[cursor] * 90
                     elif readBannerBytes == 23:
                         self.banner.Quirks = chunk[cursor]
                     cursor += 1
                     readBannerBytes += 1
                     if readBannerBytes == bannerLength:
                         print(self.banner)
                 # 读取图片大小数据
                 elif readFrameBytes < 4:
                     frameBodyLength = frameBodyLength + (
-                        (chunk[cursor] << (readFrameBytes * 8)) >> 0
+                            (chunk[cursor] << (readFrameBytes * 8)) >> 0
                     )
                     cursor += 1
                     readFrameBytes += 1
                 # 读取图片内容
                 else:
                     if length - cursor >= frameBodyLength:
-                        dataBody = dataBody + chunk[cursor : (cursor + frameBodyLength)]
+                        dataBody = dataBody + chunk[cursor: (cursor + frameBodyLength)]
                         if dataBody[0] != 0xFF or dataBody[1] != 0xD8:
                             return
                         self.queue.put(dataBody)
                         cursor += frameBodyLength
                         frameBodyLength = 0
                         readFrameBytes = 0
                         dataBody = b""
@@ -192,19 +192,19 @@
             self.ReadImageStreamTask.join()  # 等待读取图像流的线程结束
         if self.minicapSocket:
             self.minicapSocket.close()  # 关闭 minicap 的 socket 连接
 
 
 class Minicap(ScreenCap):
     def __init__(
-        self,
-        device,
-        rate=15,
-        quality=100,
-        use_stream=True,
+            self,
+            device,
+            rate=15,
+            quality=100,
+            use_stream=True,
     ) -> None:
         """
         __init__ minicap截图方式
 
         Args:
             device (str): 设备id
             rate (int, optional): 截图帧率. Defaults to 15.
@@ -266,15 +266,18 @@
                 adb_command = [
                     "shell",
                     "LD_LIBRARY_PATH=/data/local/tmp",
                     "/data/local/tmp/minicap",
                 ]
                 adb_command.extend(["-P", f"{self.vm_size}@{self.vm_size}/0"])
                 adb_command.extend(["-t"])
-                result = self.minicap_adb.adb_command(adb_command).strip()
+                try:
+                    result = self.minicap_adb.adb_command(adb_command).strip()
+                except AttributeError:
+                    return False
                 if "OK" in result.decode("utf-8"):
                     return func(self, *args, **kwargs)
                 return False
             except subprocess.CalledProcessError:
                 return False
 
         return wrapper
@@ -335,15 +338,16 @@
         self.minicap_stream.stop()  # 停止stream
         # self.minicap_adb.remove_forward(self.minicap_port)  # 清理端口
         if self.minicap_popen.poll() is None:  # 清理管道
             self.minicap_popen.kill()
 
     def __del__(self):
         self.__stop_minicap_by_stream()
-        
+
+
 if __name__ == "__main__":
     a = Minicap("127.0.0.1:16384")
     time.sleep(5)
     import cv2
 
     cv2.imshow("", a.screencap_opencv())
     cv2.waitKey()
```

### Comparing `minidevice-2.1.4/minidevice/minitouch.py` & `minidevice-2.1.5/minidevice/minitouch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
-from minidevice.adb import ADB
 from pyminitouch import MNTDevice
+
+from minidevice.adb import ADB
 from minidevice.logger import logger
 from minidevice.touch import Touch
 
 WORK_DIR = os.path.dirname(__file__)
 MINITOUCH_PATH = "{}/bin/minitouch/libs".format(WORK_DIR)
 
 
@@ -39,10 +40,11 @@
         logger.debug(
             f"minitouch swipe from ({points[0]}) to ({points[-1]}) consume:{duration}ms"
         )
 
     def __del__(self):
         MNTDevice.stop(self)
 
+
 if __name__ == "__main__":
     a = Minitouch("127.0.0.1:16384")
     a.stop()
```

### Comparing `minidevice-2.1.4/minidevice/scrcpycap.py` & `minidevice-2.1.5/minidevice/scrcpycap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import time
+
 import cv2
 import scrcpy
+
 from minidevice.screencap import ScreenCap
 
 
 class ScrcpyCap(ScreenCap):
     def __init__(self, device: scrcpy.Client) -> None:
         """
         __init__ ScrcpyCap
@@ -20,8 +22,7 @@
 
     def screencap_raw(self) -> bytes:
         _, img_data = cv2.imencode(".png", self.screencap_opencv())
         return img_data.tobytes()
 
     def screencap_opencv(self):
         return self.client.last_frame
-
```

### Comparing `minidevice-2.1.4/minidevice/scrcpytouch.py` & `minidevice-2.1.5/minidevice/scrcpytouch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import time
+
 import scrcpy
+
 from minidevice.touch import Touch
 
 
 class ScrcpyTouch(Touch):
     def __init__(self, device: scrcpy.Client) -> None:
         """
         __init__ ScrcpyCap
@@ -12,20 +14,19 @@
             device: scrcpy.Client
             
         """
         self.client = device
         if not self.client.alive:
             self.client.start(daemon_threaded=True)
             time.sleep(2)
-            
+
     def click(self, x: int, y: int, duration: int = 100):
         self.client.control.touch(x, y, scrcpy.ACTION_DOWN)
         time.sleep(duration / 1000)
         self.client.control.touch(x, y, scrcpy.ACTION_UP)
 
     def swipe(self, points: list, duration: int = 300):
         self.client.control.touch(points[0][0], points[0][1], scrcpy.ACTION_DOWN)
         for point in points[1:-1]:
             time.sleep(duration / (len(points) * 1000))
             self.client.control.touch(point[0], point[1], scrcpy.ACTION_MOVE)
         self.client.control.touch(points[-1][0], points[-1][1], scrcpy.ACTION_UP)
-
```

### Comparing `minidevice-2.1.4/minidevice/screencap.py` & `minidevice-2.1.5/minidevice/screencap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+
 import cv2
 import numpy as np
 
 
 class ScreenCap(ABC):
     @abstractmethod
     def screencap_raw(self) -> bytes:
@@ -16,9 +17,9 @@
     def save_screencap(self, filename="screencap.png"):
         """
         save_screencap 保存截图
 
         Args:
             filename (str, optional): 截图保存路径. Defaults to "screencap.png".
         """
-        with open(filename,"wb") as fp:
+        with open(filename, "wb") as fp:
             fp.write(self.screencap_raw())
```

### Comparing `minidevice-2.1.4/minidevice/touch.py` & `minidevice-2.1.5/minidevice/touch.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from abc import ABC, abstractclassmethod
+from abc import ABC, abstractmethod
 
 
 class Touch(ABC):
-    @abstractclassmethod
+    @abstractmethod
     def click(self, x: int, y: int, duration: int = 100):
         """
         click 点击
 
         Args:
             x (int): 横坐标
             y (int): 纵坐标
             duration (int, optional): 持续时间. Defaults to 100.
         """
 
-    @abstractclassmethod
+    @abstractmethod
     def swipe(self, points: list, duration: int = 300):
         """
         swipe 滑动
 
         Args:
             points (list): [(x,y),(x,y),(x,y)] 坐标列表
             duration (int): 持续时间. Defaults to 300.
```

### Comparing `minidevice-2.1.4/minidevice.egg-info/PKG-INFO` & `minidevice-2.1.5/minidevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.1.4
+Version: 2.1.5
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.1.4/setup.py` & `minidevice-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.1.4',
+      version='2.1.5',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

