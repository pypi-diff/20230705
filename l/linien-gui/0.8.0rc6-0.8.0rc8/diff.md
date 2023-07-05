# Comparing `tmp/linien-gui-0.8.0rc6.tar.gz` & `tmp/linien-gui-0.8.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-gui-0.8.0rc6.tar", last modified: Mon Jul  3 14:23:31 2023, max compression
+gzip compressed data, was "linien-gui-0.8.0rc8.tar", last modified: Wed Jul  5 09:24:24 2023, max compression
```

## Comparing `linien-gui-0.8.0rc6.tar` & `linien-gui-0.8.0rc8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:31.738295 linien-gui-0.8.0rc6/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 14:23:31.738295 linien-gui-0.8.0rc6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:31.730295 linien-gui-0.8.0rc6/linien_gui/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/icon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:31.738295 linien-gui-0.8.0rc6/linien_gui/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/device_manager.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/general_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/general_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/lock_status_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/locking_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/locking_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/logging_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/logging_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/modulation_sweep_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/modulation_sweep_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/new_device_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/new_device_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/optimization_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/optimization_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/psd_plot_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/psd_table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/psd_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/psd_window.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/right_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/spectroscopy_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/spectroscopy_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/spin_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/sweep_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/version_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/view_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/ui/view_panel.ui
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/linien_gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:23:31.734295 linien-gui-0.8.0rc6/linien_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 14:23:31.000000 linien-gui-0.8.0rc6/linien_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:23:31.738295 linien-gui-0.8.0rc6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-03 14:22:35.000000 linien-gui-0.8.0rc6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:24.066430 linien-gui-0.8.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 09:24:24.066430 linien-gui-0.8.0rc8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:24.062430 linien-gui-0.8.0rc8/linien_gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   410598 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:24.066430 linien-gui-0.8.0rc8/linien_gui/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/device_manager.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/general_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26265 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/general_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/lock_status_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/locking_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39174 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/locking_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/logging_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/logging_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42356 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/modulation_sweep_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/modulation_sweep_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/new_device_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/new_device_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/optimization_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/optimization_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/psd_plot_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/psd_table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/psd_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/psd_window.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/right_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/spectroscopy_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/spectroscopy_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/spin_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/sweep_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/version_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/view_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/ui/view_panel.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/linien_gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:24:24.062430 linien-gui-0.8.0rc8/linien_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 09:24:24.000000 linien-gui-0.8.0rc8/linien_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:24:24.066430 linien-gui-0.8.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-05 09:23:25.000000 linien-gui-0.8.0rc8/setup.py
```

### Comparing `linien-gui-0.8.0rc6/PKG-INFO` & `linien-gui-0.8.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/app.py` & `linien-gui-0.8.0rc8/linien_gui/app.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/config.py` & `linien-gui-0.8.0rc8/linien_gui/config.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/dialogs.py` & `linien-gui-0.8.0rc8/linien_gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/icon.ico` & `linien-gui-0.8.0rc8/linien_gui/icon.ico`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/threads.py` & `linien-gui-0.8.0rc8/linien_gui/threads.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import traceback
 
 from linien_client.connection import LinienClient
 from linien_client.deploy import install_remote_server
 from linien_client.exceptions import (
-    GeneralConnectionErrorException,
+    GeneralConnectionError,
     InvalidServerVersionException,
     RPYCAuthenticationException,
     ServerNotInstalledException,
 )
 from linien_common.config import DEFAULT_SERVER_PORT
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 
@@ -111,15 +111,15 @@
             self.invalid_server_version_exception_raised.emit(
                 e.remote_version, e.client_version
             )
 
         except RPYCAuthenticationException:
             self.authentication_exception_raised.emit()
 
-        except GeneralConnectionErrorException:
+        except GeneralConnectionError:
             self.general_connection_exception_raised.emit()
 
         except Exception:
             traceback.print_exc()
             self.other_exception_raised.emit(traceback.format_exc())
 
     def on_connection_lost(self):
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/device_manager.py` & `linien-gui-0.8.0rc8/linien_gui/ui/device_manager.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/device_manager.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/device_manager.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/general_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/general_panel.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from linien_common.common import (
-    ANALOG_OUT0,
     ANALOG_OUT_V,
-    FAST_OUT1,
-    FAST_OUT2,
+    OutputChannel,
     convert_channel_mixing_value,
 )
 from linien_gui.utils import get_linien_app_instance, param2ui
 from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
@@ -194,10 +192,16 @@
             self.parameters.sweep_channel.value,
         }
 
         if self.parameters.pid_on_slow_enabled.value:
             used_channels.add(self.parameters.slow_control_channel.value)
 
         self.polaritySelectorGroupBox.setVisible(len(used_channels) > 1)
-        self.polarityContainerFastOut1.setVisible(FAST_OUT1 in used_channels)
-        self.polarityContainerFastOut2.setVisible(FAST_OUT2 in used_channels)
-        self.polarityContainerAnalogOut0.setVisible(ANALOG_OUT0 in used_channels)
+        self.polarityContainerFastOut1.setVisible(
+            OutputChannel.FAST_OUT1 in used_channels
+        )
+        self.polarityContainerFastOut2.setVisible(
+            OutputChannel.FAST_OUT2 in used_channels
+        )
+        self.polarityContainerAnalogOut0.setVisible(
+            OutputChannel.ANALOG_OUT0 in used_channels
+        )
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/general_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/general_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/lock_status_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/lock_status_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/locking_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/locking_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
-from linien_common.common import FAST_AUTOLOCK
+from linien_common.common import AutolockMode
 from linien_gui.utils import get_linien_app_instance, param2ui
 from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class LockingPanel(QtWidgets.QWidget):
     def __init__(self, *args, **kwargs):
@@ -130,15 +130,15 @@
 
     def autolock_mode_preference_changed(self, idx):
         self.parameters.autolock_mode_preference.value = idx
 
     def start_manual_lock(self):
         self.parameters.target_slope_rising.value = self.button_slope_rising.isChecked()
         self.parameters.fetch_additional_signals.value = False
-        self.parameters.autolock_mode.value = FAST_AUTOLOCK
+        self.parameters.autolock_mode.value = AutolockMode.FAST
         self.parameters.autolock_target_position.value = 0
         self.control.write_registers()
         self.control.start_lock()
 
     def auto_offset_changed(self):
         self.parameters.autolock_determine_offset.value = int(
             self.autoOffsetCheckbox.checkState()
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/locking_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/locking_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/logging_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/logging_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/logging_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/logging_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/main_window.py` & `linien-gui-0.8.0rc8/linien_gui/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/main_window.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/main_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/modulation_sweep_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/modulation_sweep_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/modulation_sweep_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/modulation_sweep_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/new_device_dialog.py` & `linien-gui-0.8.0rc8/linien_gui/ui/new_device_dialog.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/new_device_dialog.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/new_device_dialog.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/optimization_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/optimization_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/optimization_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/optimization_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/plot_widget.py` & `linien-gui-0.8.0rc8/linien_gui/ui/plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/psd_plot_widget.py` & `linien-gui-0.8.0rc8/linien_gui/ui/psd_plot_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/psd_table_widget.py` & `linien-gui-0.8.0rc8/linien_gui/ui/psd_table_widget.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/psd_window.py` & `linien-gui-0.8.0rc8/linien_gui/ui/psd_window.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 from time import time
 
 import linien_gui
-from linien_common.common import PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH
+from linien_common.common import PSDAlgorithm
 from linien_gui.dialogs import error_dialog
 from linien_gui.utils import (
     RandomColorChoser,
     get_linien_app_instance,
     param2ui,
     set_window_icon,
 )
@@ -77,15 +77,15 @@
             self.parameters.psd_acquisition_max_decimation,
             self.maximum_measurement_time,
             lambda max_decimation: max_decimation - 12,
         )
         param2ui(
             self.parameters.psd_algorithm,
             self.psd_algorithm,
-            lambda algo: {PSD_ALGORITHM_LPSD: 0, PSD_ALGORITHM_WELCH: 1}[algo],
+            lambda algo: {PSDAlgorithm.LPSD: 0, PSDAlgorithm.WELCH: 1}[algo],
         )
 
         def update_status(_):
             psd_running = self.parameters.psd_acquisition_running.value
             if psd_running:
                 self.container_psd_running.show()
                 self.container_psd_not_running.hide()
@@ -101,15 +101,15 @@
         event.ignore()
         self.hide()
 
     def change_maximum_measurement_time(self, index):
         self.parameters.psd_acquisition_max_decimation.value = 12 + index
 
     def change_psd_algorithm(self, index):
-        self.parameters.psd_algorithm.value = [PSD_ALGORITHM_LPSD, PSD_ALGORITHM_WELCH][
+        self.parameters.psd_algorithm.value = [PSDAlgorithm.LPSD, PSDAlgorithm.WELCH][
             index
         ]
 
     def psd_data_received(self, data_pickled):
         if data_pickled is None:
             return
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/psd_window.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/psd_window.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/right_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/right_panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,21 +62,25 @@
         self.app.open_psd_window()
 
     def open_device_manager(self):
         self.app.open_device_manager()
 
     def autolock_status_changed(self, value):
         if value:
-            self.main_window.settings_toolbox.setCurrentWidget(self.lockingPanel)
+            self.main_window.settings_toolbox.setCurrentWidget(
+                self.main_window.lockingPanel
+            )
 
         self.enable_or_disable_panels()
 
     def optimization_status_changed(self, value):
         if value:
-            self.main_window.settings_toolbox.setCurrentWidget(self.optimizationPanel)
+            self.main_window.settings_toolbox.setCurrentWidget(
+                self.main_window.optimizationPanel
+            )
 
         self.enable_or_disable_panels()
 
     def enable_or_disable_panels(self, *args):
         lock = self.parameters.lock.value
         autolock = self.parameters.autolock_running.value
         optimization = self.parameters.optimization_running.value
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/spectroscopy_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/spectroscopy_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from typing import Union
 
 from linien_client.remote_parameters import RemoteParameter
-from linien_common.common import HIGH_PASS_FILTER, LOW_PASS_FILTER
+from linien_common.common import FilterType
 from linien_gui.utils import get_linien_app_instance, param2ui
 from linien_gui.widgets import UI_PATH
 from PyQt5 import QtWidgets, uic
 
 
 class SpectroscopyPanel(QtWidgets.QWidget):
     CHANNEL = Union[str, None]
@@ -45,15 +45,15 @@
             )
             self.get_param(f"filter_{filter_i}_enabled").value = filter_enabled
             self.control.exposed_write_registers()
 
         def change_filter_type(filter_i):
             param = self.get_param(f"filter_{filter_i}_type")
             current_idx = getattr(self, f"filter_{filter_i}_type").currentIndex()
-            param.value = (LOW_PASS_FILTER, HIGH_PASS_FILTER)[current_idx]
+            param.value = (FilterType.LOW_PASS, FilterType.HIGH_PASS)[current_idx]
             self.control.exposed_write_registers()
 
         for filter_i in [1, 2]:
             for key, fct in {
                 f"change_filter_{filter_i}_frequency": change_filter_frequency,
                 f"change_filter_{filter_i}_enabled": change_filter_enabled,
                 f"change_filter_{filter_i}_type": change_filter_type,
@@ -128,15 +128,15 @@
             param2ui(
                 self.get_param(f"filter_{filter_i}_frequency"),
                 getattr(self, f"filter_{filter_i}_frequency"),
             )
             param2ui(
                 self.get_param(f"filter_{filter_i}_type"),
                 getattr(self, f"filter_{filter_i}_type"),
-                lambda type_: {LOW_PASS_FILTER: 0, HIGH_PASS_FILTER: 1}[type_],
+                lambda type_: {FilterType.LOW_PASS: 0, FilterType.HIGH_PASS: 1}[type_],
             )
 
     def get_param(self, name: str) -> RemoteParameter:
         return getattr(self.parameters, f"{name}_{self.CHANNEL}")
 
     def change_signal_offset(self):
         self.get_param("offset").value = self.signalOffsetSpinBox.value() * 8191
```

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/spectroscopy_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/spectroscopy_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/spin_box.py` & `linien-gui-0.8.0rc8/linien_gui/ui/spin_box.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/sweep_control.py` & `linien-gui-0.8.0rc8/linien_gui/ui/sweep_control.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/version_checker.py` & `linien-gui-0.8.0rc8/linien_gui/ui/version_checker.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/view_panel.py` & `linien-gui-0.8.0rc8/linien_gui/ui/view_panel.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/ui/view_panel.ui` & `linien-gui-0.8.0rc8/linien_gui/ui/view_panel.ui`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/utils.py` & `linien-gui-0.8.0rc8/linien_gui/utils.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui/widgets.py` & `linien-gui-0.8.0rc8/linien_gui/widgets.py`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/linien_gui.egg-info/PKG-INFO` & `linien-gui-0.8.0rc8/linien_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-gui
-Version: 0.8.0rc6
+Version: 0.8.0rc8
 Summary: Graphical user interface of the Linien spectroscopy lock application.
 Home-page: https://github.com/linien-org/linien
 Author: Benjamin Wiegand
 Author-email: highwaychile@posteo.de
 Maintainer: Bastian Leykauf
 Maintainer-email: leykauf@physik.hu-berlin.de
 Classifier: Programming Language :: Python :: 3
```

### Comparing `linien-gui-0.8.0rc6/linien_gui.egg-info/SOURCES.txt` & `linien-gui-0.8.0rc8/linien_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linien-gui-0.8.0rc6/setup.py` & `linien-gui-0.8.0rc8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Linien.  If not, see <http://www.gnu.org/licenses/>.
 
 from setuptools import find_packages, setup
 
-version = "0.8.0rc6"
+version = "0.8.0rc8"
 
 setup(
     name="linien-gui",
     version=version,
     author="Benjamin Wiegand",
     author_email="highwaychile@posteo.de",
     maintainer="Bastian Leykauf",
```

