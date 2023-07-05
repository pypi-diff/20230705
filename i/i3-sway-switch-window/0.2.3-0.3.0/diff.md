# Comparing `tmp/i3_sway_switch_window-0.2.3.tar.gz` & `tmp/i3_sway_switch_window-0.3.0.tar.gz`

## Comparing `i3_sway_switch_window-0.2.3.tar` & `i3_sway_switch_window-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/requirements.txt
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/setup.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/docs/construction.org
--rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/elisp/emacs-with-nyxt.el
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__init__.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__main__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/__version__.py
--rwxr-xr-x   0        0        0     2450 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/browser_tab_list.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/config.py
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/display_error_message.py
--rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_buffer_lists.py
--rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_recentf_list.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/get_nyxt_title_url.py
--rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_add.py
--rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_switch.py
--rwxr-xr-x   0        0        0    15806 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/main.py
--rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/i3_sway_switch_window/wm_window_list.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/LICENSE
--rw-r--r--   0        0        0    10749 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    11825 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/requirements.txt
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/setup.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/docs/construction.org
+-rw-r--r--   0        0        0    21361 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/elisp/emacs-with-nyxt.el
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/__init__.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/__main__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/__version__.py
+-rwxr-xr-x   0        0        0     2777 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/browser_tab_list.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/config.py
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/display_error_message.py
+-rwxr-xr-x   0        0        0     2411 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/emacs_buffer_lists.py
+-rwxr-xr-x   0        0        0     1905 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/emacs_recentf_list.py
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/get_nyxt_title_url.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/get_qutebrowser_title_url.py
+-rwxr-xr-x   0        0        0     1139 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/i3_do_add.py
+-rwxr-xr-x   0        0        0     1482 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/i3_do_switch.py
+-rwxr-xr-x   0        0        0    16196 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/main.py
+-rwxr-xr-x   0        0        0     1329 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/i3_sway_switch_window/wm_window_list.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11083 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/README.md
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12181 2020-02-02 00:00:00.000000 i3_sway_switch_window-0.3.0/PKG-INFO
```

### Comparing `i3_sway_switch_window-0.2.3/setup.py` & `i3_sway_switch_window-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         ],
     project_urls = {
         "Bug Tracker": "https://github.com/johanwiden/i3-sway-switch-window/issues"
     },
     license='MIT License',
     packages=setuptools.find_packages(),
     # packages=['i3-switch-window'],
-    install_requires=['i3ipc','psutil','stat','subprocess','tempfile'],
+    install_requires=['i3ipc','psutil','pyyaml','stat','subprocess','tempfile'],
     entry_points = {
         'console_scripts': [
             'emacs_buffers = i3_sway_switch_window.main:cli_emacs_buffers',
             'emacs_recentf = i3_sway_switch_window.main:cli_emacs_recentf',
             'browser_tab = i3_sway_switch_window.main:cli_browser_tab',
             'wm_window_switch = i3_sway_switch_window.main:cli_wm_window_switch',
         ]
```

### Comparing `i3_sway_switch_window-0.2.3/docs/construction.org` & `i3_sway_switch_window-0.3.0/docs/construction.org`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/elisp/emacs-with-nyxt.el` & `i3_sway_switch_window-0.3.0/elisp/emacs-with-nyxt.el`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/browser_tab_list.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/browser_tab_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 # The list is sorted case insensitive.
 
 # Note to developer: All error messages are to be presented to the user in one (well known) place.
 
 import re
 import subprocess
 import i3_sway_switch_window.get_nyxt_title_url
+import i3_sway_switch_window.get_qutebrowser_title_url
 import i3_sway_switch_window.display_error_message
 
-def _browser_tab_list(get_urls_from_nyxt):
+def _browser_tab_list(get_urls_from_nyxt, get_urls_from_qutebrowser):
     """Return list of web browser tab titles and URLs.
 
     If get_urls_from_nyxt is True then also try to get titles and URLs from nyxt browser.
+    If get_urls_from_qutebrowser is True then also try to get titles and URLs from qutebrowser.
     The first column (tab ID), of each list item, is removed. The list is sorted case insensitive.
     """
     success = 1
     try:
         subprocess_result = subprocess.run(['bt','list'],
                                            capture_output=True, encoding="utf-8", check=True, timeout=5)
     except FileNotFoundError as exc:
@@ -39,13 +41,15 @@
         all_tabs = [re.sub(r'^\S+\s', '', token) for token in all_tabs] # Remove tab ID column
         # Filter out internal URIs
         web_tabs = [token for token in all_tabs if 'https://' in token]
         # Standardise number of spaces before https://
         web_tabs = [re.sub(r'\s+https://', r'  https://', token) for token in web_tabs]
         if get_urls_from_nyxt:
             web_tabs = web_tabs + i3_sway_switch_window.get_nyxt_title_url._get_nyxt_title_url()
+        if get_urls_from_qutebrowser:
+            web_tabs = web_tabs + i3_sway_switch_window.get_qutebrowser_title_url._get_qutebrowser_title_url()
         # Make a sorted list, without duplicates
         set_res = set(web_tabs)
         web_tabs = sorted(list(set_res), key=str.casefold)
         return web_tabs
     else:
         return []
```

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/config.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/config.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/display_error_message.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/display_error_message.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_buffer_lists.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/emacs_buffer_lists.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/emacs_recentf_list.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/emacs_recentf_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/get_nyxt_title_url.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/get_nyxt_title_url.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_add.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/i3_do_add.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/i3_do_switch.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/i3_do_switch.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/main.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 roficommand = 'rofi -dmenu'
 
 webbrowser = 'vivaldi' # Default value
 webbrowser_commandlineoptions = '--new-window'
 webbrowser_urlprefix = ''
 webbrowser_urlsuffix = ''
 get_urls_from_nyxt = False
+get_urls_from_qutebrowser = False
 
 swap_workspace = '2'
 
 def _select_item_and_switch(add_or_swap_window, focused_window_id, window_name_list):
     """Call 'rofi' to select an item from 'window_name_list'. Swap in or move window at focused window.
 
     Parameters:
@@ -169,15 +170,15 @@
     """Get browser tab titles and URLs. Select one, display it in desktop window.
 
     Use rofi to select URL. Display with web browser. Parameter 'add_or_swap_window':
     - add: Show the window next to the currently focused window.
     - swap: The window is displayed instead of the currently focused window.
             The currently focused window is moved to a different workspace.
     """
-    tab_list = i3_sway_switch_window.browser_tab_list._browser_tab_list(get_urls_from_nyxt)
+    tab_list = i3_sway_switch_window.browser_tab_list._browser_tab_list(get_urls_from_nyxt, get_urls_from_qutebrowser)
     command_prefix = webbrowser + " " + webbrowser_commandlineoptions + " " + webbrowser_urlprefix
     command_suffix = webbrowser_urlsuffix + "\n"
     if len(webbrowser_urlprefix) > 0 and webbrowser_urlprefix[-1] == '"':
         _select_item_execute_and_switch(add_or_swap_window, tab_list,
                                         command_prefix, command_suffix,
                                         r'.*h(ttps://\S+)\s*$', r"h\1")
     else:
@@ -224,21 +225,23 @@
         exit(1)
     config_roficommand = i3_sway_switch_window.config._get_value('roficommand', 'roficommand')
     config_webbrowser = i3_sway_switch_window.config._get_value('webbrowser', 'webbrowser')
     config_webbrowser_commandlineoptions = i3_sway_switch_window.config._get_value('webbrowser', 'commandlineoptions')
     config_webbrowser_urlprefix = i3_sway_switch_window.config._get_value('webbrowser', 'urlprefix')
     config_webbrowser_urlsuffix = i3_sway_switch_window.config._get_value('webbrowser', 'urlsuffix')
     config_webbrowser_get_urls_from_nyxt = i3_sway_switch_window.config._get_value('webbrowser', 'get_urls_from_nyxt')
+    config_webbrowser_get_urls_from_qutebrowser = i3_sway_switch_window.config._get_value('webbrowser', 'get_urls_from_qutebrowser')
     config_swap_workspace = i3_sway_switch_window.config._get_value('workspace', 'swap_workspace')
     global roficommand
     global webbrowser
     global webbrowser_commandlineoptions
     global webbrowser_urlprefix
     global webbrowser_urlsuffix
     global get_urls_from_nyxt
+    global get_urls_from_qutebrowser
     global swap_workspace
     if len(config_roficommand) > 0:
         roficommand = config_roficommand
     if args.browser:
         webbrowser = args.browser
     elif len(config_webbrowser) > 0:
         webbrowser = config_webbrowser
@@ -246,14 +249,16 @@
         webbrowser_commandlineoptions = config_webbrowser_commandlineoptions
     if len(config_webbrowser_urlprefix) > 0:
         webbrowser_urlprefix = config_webbrowser_urlprefix
     if len(config_webbrowser_urlsuffix) > 0:
         webbrowser_urlsuffix = config_webbrowser_urlsuffix
     if len(config_webbrowser_get_urls_from_nyxt) > 0 and config_webbrowser_get_urls_from_nyxt == 'yes':
         get_urls_from_nyxt = True
+    if len(config_webbrowser_get_urls_from_qutebrowser) > 0 and config_webbrowser_get_urls_from_qutebrowser == 'yes':
+        get_urls_from_qutebrowser = True
     if len(config_swap_workspace) > 0:
         swap_workspace = config_swap_workspace
     return args.action
 
 def cli_emacs_buffers():
     """Use rofi to select an emacs buffer. Open emacsclient with selected buffer.
```

### Comparing `i3_sway_switch_window-0.2.3/i3_sway_switch_window/wm_window_list.py` & `i3_sway_switch_window-0.3.0/i3_sway_switch_window/wm_window_list.py`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/.gitignore` & `i3_sway_switch_window-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/LICENSE` & `i3_sway_switch_window-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `i3_sway_switch_window-0.2.3/README.md` & `i3_sway_switch_window-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,23 @@
 #    (remote-execution-p t)))
 
 # Should we try to get a list of titles and URLs from nyxt webbrowser.
 # There are some requirements: See the project README.
 # default is no
 get_urls_from_nyxt = yes
 
+# Config for displaying in qutebrowser:
+# webbrowser = qutebrowser
+# commandlineoptions = --target window
+
+# Should we try to get a list of titles and URLs from qutebrowser.
+# There are some requirements: See the project README.
+# default is no
+get_urls_from_qutebrowser = yes
+
 [workspace]
 # i3, or sway, workspace to which focused window will be swapped
 # Default is "2"
 swap_workspace = 9
 ```
 
 ## How to use
@@ -160,14 +169,16 @@
   - conda create --name i3env
   - conda activate i3env
   - conda install -c anaconda pip
   - pip install i3ipc
     This is a package dependency
   - pip install psutil
     This is a package dependency
+  - pip install pyyaml
+    This is a package dependency
   - pip install build
     This is the tool to build the package.
 - Change directory to the downloaded repo
 - python3 -m build
     This should build the package, the result is stored in subdirectory 'dist'
 
 ### Running the applications
```

### Comparing `i3_sway_switch_window-0.2.3/pyproject.toml` & `i3_sway_switch_window-0.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "i3_sway_switch_window"
-version = "0.2.3"
+version = "0.3.0"
 authors = [
   { name="Johan Widén", email="j.e.widen@gmail.com" },
 ]
 description = "In i3wm, or sway, replace current window with emacs buffer, browser tab or other window"
 readme = "README.md"
 requires-python = ">=3.8"
-dependencies = ["i3ipc", "psutil"]
+dependencies = ["i3ipc", "psutil", "pyyaml"]
 classifiers = [
     # complete classifier list:
     # http://pypi.python.org/pypi?%3Aaction=list_classifiers
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: MIT License',
     'Environment :: X11 Applications',
     'Intended Audience :: End Users/Desktop',
```

### Comparing `i3_sway_switch_window-0.2.3/PKG-INFO` & `i3_sway_switch_window-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i3_sway_switch_window
-Version: 0.2.3
+Version: 0.3.0
 Summary: In i3wm, or sway, replace current window with emacs buffer, browser tab or other window
 Project-URL: Homepage, https://github.com/johanwiden/i3-sway-switch-window
 Project-URL: Bug Tracker, https://github.com/johanwiden/i3-sway-switch-window/issues
 Author-email: Johan Widén <j.e.widen@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: Desktop Environment :: Window Managers
 Requires-Python: >=3.8
 Requires-Dist: i3ipc
 Requires-Dist: psutil
+Requires-Dist: pyyaml
 Description-Content-Type: text/markdown
 
 # i3-sway-switch-window
 
 <div align="center">
 
 [![Python Version](https://img.shields.io/pypi/pyversions/i3-sway-switch-window.svg)](https://pypi.org/project/i3-sway-switch-window/)
@@ -109,14 +110,23 @@
 #    (remote-execution-p t)))
 
 # Should we try to get a list of titles and URLs from nyxt webbrowser.
 # There are some requirements: See the project README.
 # default is no
 get_urls_from_nyxt = yes
 
+# Config for displaying in qutebrowser:
+# webbrowser = qutebrowser
+# commandlineoptions = --target window
+
+# Should we try to get a list of titles and URLs from qutebrowser.
+# There are some requirements: See the project README.
+# default is no
+get_urls_from_qutebrowser = yes
+
 [workspace]
 # i3, or sway, workspace to which focused window will be swapped
 # Default is "2"
 swap_workspace = 9
 ```
 
 ## How to use
@@ -185,14 +195,16 @@
   - conda create --name i3env
   - conda activate i3env
   - conda install -c anaconda pip
   - pip install i3ipc
     This is a package dependency
   - pip install psutil
     This is a package dependency
+  - pip install pyyaml
+    This is a package dependency
   - pip install build
     This is the tool to build the package.
 - Change directory to the downloaded repo
 - python3 -m build
     This should build the package, the result is stored in subdirectory 'dist'
 
 ### Running the applications
```

