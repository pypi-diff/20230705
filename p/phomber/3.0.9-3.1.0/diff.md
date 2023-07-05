# Comparing `tmp/phomber-3.0.9.tar.gz` & `tmp/phomber-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phomber-3.0.9.tar", last modified: Tue Jun 27 15:48:02 2023, max compression
+gzip compressed data, was "phomber-3.1.0.tar", last modified: Wed Jul  5 18:41:47 2023, max compression
```

## Comparing `phomber-3.0.9.tar` & `phomber-3.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-06-27 15:48:02.680445 phomber-3.0.9/
--rw-r--r--   0 cyber     (1000) cyber     (1001)    35149 2023-06-27 14:15:54.000000 phomber-3.0.9/LICENSE
--rw-r--r--   0 cyber     (1000) cyber     (1001)    45210 2023-06-27 15:48:02.680445 phomber-3.0.9/PKG-INFO
--rw-r--r--   0 cyber     (1000) cyber     (1001)     4003 2023-06-27 14:29:58.000000 phomber-3.0.9/README.md
-drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-06-27 15:48:02.680445 phomber-3.0.9/phomber/
--rw-r--r--   0 cyber     (1000) cyber     (1001)        0 2023-05-21 11:32:11.000000 phomber-3.0.9/phomber/__init__.py
--rw-r--r--   0 cyber     (1000) cyber     (1001)    70448 2023-06-22 19:33:51.000000 phomber-3.0.9/phomber/phomber.py
-drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-06-27 15:48:02.680445 phomber-3.0.9/phomber.egg-info/
--rw-r--r--   0 cyber     (1000) cyber     (1001)    45210 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/PKG-INFO
--rw-r--r--   0 cyber     (1000) cyber     (1001)      259 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/SOURCES.txt
--rw-r--r--   0 cyber     (1000) cyber     (1001)        1 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/dependency_links.txt
--rw-r--r--   0 cyber     (1000) cyber     (1001)       91 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/entry_points.txt
--rw-r--r--   0 cyber     (1000) cyber     (1001)       90 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/requires.txt
--rw-r--r--   0 cyber     (1000) cyber     (1001)        8 2023-06-27 15:48:02.000000 phomber-3.0.9/phomber.egg-info/top_level.txt
--rw-r--r--   0 cyber     (1000) cyber     (1001)     1056 2023-06-27 15:47:25.000000 phomber-3.0.9/pyproject.toml
--rw-r--r--   0 cyber     (1000) cyber     (1001)       38 2023-06-27 15:48:02.680445 phomber-3.0.9/setup.cfg
+drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-07-05 18:41:47.779142 phomber-3.1.0/
+-rw-r--r--   0 cyber     (1000) cyber     (1001)    35149 2023-06-27 14:15:54.000000 phomber-3.1.0/LICENSE
+-rw-r--r--   0 cyber     (1000) cyber     (1001)    45489 2023-07-05 18:41:47.779142 phomber-3.1.0/PKG-INFO
+-rw-r--r--   0 cyber     (1000) cyber     (1001)     4191 2023-07-05 18:39:46.000000 phomber-3.1.0/README.md
+drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-07-05 18:41:47.779142 phomber-3.1.0/phomber/
+-rw-r--r--   0 cyber     (1000) cyber     (1001)        0 2023-05-21 11:32:11.000000 phomber-3.1.0/phomber/__init__.py
+-rw-r--r--   0 cyber     (1000) cyber     (1001)    69234 2023-07-05 18:32:58.000000 phomber-3.1.0/phomber/phomber.py
+drwxr-xr-x   0 cyber     (1000) cyber     (1001)        0 2023-07-05 18:41:47.779142 phomber-3.1.0/phomber.egg-info/
+-rw-r--r--   0 cyber     (1000) cyber     (1001)    45489 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/PKG-INFO
+-rw-r--r--   0 cyber     (1000) cyber     (1001)      259 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/SOURCES.txt
+-rw-r--r--   0 cyber     (1000) cyber     (1001)        1 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/dependency_links.txt
+-rw-r--r--   0 cyber     (1000) cyber     (1001)       91 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/entry_points.txt
+-rw-r--r--   0 cyber     (1000) cyber     (1001)       90 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/requires.txt
+-rw-r--r--   0 cyber     (1000) cyber     (1001)        8 2023-07-05 18:41:47.000000 phomber-3.1.0/phomber.egg-info/top_level.txt
+-rw-r--r--   0 cyber     (1000) cyber     (1001)     1136 2023-07-05 17:56:42.000000 phomber-3.1.0/pyproject.toml
+-rw-r--r--   0 cyber     (1000) cyber     (1001)       38 2023-07-05 18:41:47.779142 phomber-3.1.0/setup.cfg
```

### Comparing `phomber-3.0.9/LICENSE` & `phomber-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phomber-3.0.9/PKG-INFO` & `phomber-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomber
-Version: 3.0.9
+Version: 3.1.0
 Summary: `PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering
 Author: s41r4j
 Maintainer: s41r4j
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -681,14 +681,16 @@
         
 Project-URL: Homepage, https://github.com/s41r4j/phomber
 Project-URL: Bug Tracker, https://github.com/s41r4j/phomber/issues
 Keywords: python,hacking,pentesting,phomber,reverse,lookup,osint,framework,tool,s41r4j
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align=center>
          <img src='.images/phomber_logo.png'>
 </p>
@@ -696,39 +698,43 @@
 
 ```
 An open source infomation grathering & reconnaissance framework!
 ```
 
 <p align=center>
          <a href='https://www.w3schools.in/ethical-hacking/information-gathering-techniques/'><img src="https://img.shields.io/badge/Etical Hacking-OSINT-yellow.svg?logo=sharp"></a>
-         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks"></a>
+         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.1.0-orange.svg?logo=vectorworks"></a>
          <a href='https://www.python.org/'><img src="https://img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python"></a>
          <a href='LICENSE'><img src="https://img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg"></a>
          <a href=''><img src="https://img.shields.io/badge/Disclaimer-With great power comes great responsibility-red.svg?logo=hackaday"></a>
 </p>
       
 <br>
 
-<h1 align=center>PH0MBER: osint framework [3.0.9 (beta)]</h1>
+<h1 align=center>PH0MBER: osint framework</h1>
 
 
 
 <br>
 
 ## What is PH0MBER?
 
-- `PH0MBER` is a tool which is used to gather information about a target which is publicly available
-- Previously `PH0MBER` was a tool which was used to gather information about a phone number, but now it has been upgraded to a _framework_ with many _scanners_
+- `PH0MBER` is a one-stop tool for your information gathering and reconnaissance needs
+- It can help you gather multiple types of information (such as phone numbers, ip addr, whois, etc.) from various publicly available sources about the target
+> Previously, `PH0MBER` was a tool used to gather information about a phone number, but now it has been upgraded to a ___framework___ with many _scanners_ available!
 
 
 
 <br>
 <br>
 
-## Install & Usage: A Quick Guide
+## Quick Guide
+> Install, Update, Usage
+
+<br>
 
 ### Installation:
 - __git clone__
 ```
 git clone https://github.com/s41r4j/phomber
 cd phomber
 pip3 install -r requirements.txt
@@ -736,14 +742,28 @@
 - __pip__
 ```
 pip install phomber
 ```
 
 <br>
 
+### Update:
+- __git clone__ (assuming you are in the `phomber` directory)
+```
+git pull
+```
+
+- __pip__
+```
+pip install --upgrade phomber
+```
+
+
+<br>
+
 ### Usage:
 - __git clone__ (assuming you are in the `phomber` directory)
 ```
 python3 phomber.py
 ```
 
 - __pip__
@@ -752,38 +772,36 @@
 ```
 
 - Help menu
 ```
     ┌────────────────────────────────────────────────────┐
     | COMMANDS      | DESCRIPTION                        |
     |----------------------------------------------------|
-    |                <Basic Commands>                    |
+    |                 <(Basic Commands)>                 |
     |----------------------------------------------------|
     | help          | Display this help menu             | 
     | exit/quit     | Exit the framework                 |
     | dork          | Show a random google dork query *  |  
     | exp           | Show info about all available      |       
     |               | expressions                        |
     | check         | Check internet connection          |
     | clear         | Clear screen                       |
     | save          | Save output of previous scanner    |
     |               | command in a file                  |
     | shell <cmd>   | Execute native shell/cmd commands  |
     | info          | Show info about framework & system |
     | change        | Change user command input color    |
     |----------------------------------------------------|
-    |                 <Scanner Commands>                 |
+    |                <(Scanner Commands)>                |
     |----------------------------------------------------|
     | number        | Reverse phone number lookup *      |
     | ip            | Reverse ip address lookup *        |
     | mac           | Reverse mac address lookup         |
     | whois         | Reverse whois lookup *             |
-    | dns           | Reverse or normal DNS lookup       |
-    |----------------------------------------------------|
-    | MORE SCANNERS COMING SOON, THIS IS A BETA VER      |
+    | dns           | Reverse or normal DNS lookup *     |
     └────────────────────────────────────────────────────┘
 ```
 
 #### Pro tips:
 - Type `help` to get a list of commands
 - Type `help <command>` to see more info about a command
 - Use `Tab` key to auto-complete commands
@@ -796,9 +814,9 @@
 <br>
 
 
 ### NOTES:
 ```
 - `PH0MBER` is back with all new features and user interface
 - `v3` has osint tools with no _api key_ requirement
-- Currently this `v3.0-beta` is for testing, try using & report bugs
+- ADD: custom-scanner feature; create, distribute and deploy your own scanner
 ```
```

### Comparing `phomber-3.0.9/README.md` & `phomber-3.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 
 ```
 An open source infomation grathering & reconnaissance framework!
 ```
 
 <p align=center>
          <a href='https://www.w3schools.in/ethical-hacking/information-gathering-techniques/'><img src="https://img.shields.io/badge/Etical Hacking-OSINT-yellow.svg?logo=sharp"></a>
-         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks"></a>
+         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.1.0-orange.svg?logo=vectorworks"></a>
          <a href='https://www.python.org/'><img src="https://img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python"></a>
          <a href='LICENSE'><img src="https://img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg"></a>
          <a href=''><img src="https://img.shields.io/badge/Disclaimer-With great power comes great responsibility-red.svg?logo=hackaday"></a>
 </p>
       
 <br>
 
-<h1 align=center>PH0MBER: osint framework [3.0.9 (beta)]</h1>
+<h1 align=center>PH0MBER: osint framework</h1>
 
 
 
 <br>
 
 ## What is PH0MBER?
 
-- `PH0MBER` is a tool which is used to gather information about a target which is publicly available
-- Previously `PH0MBER` was a tool which was used to gather information about a phone number, but now it has been upgraded to a _framework_ with many _scanners_
+- `PH0MBER` is a one-stop tool for your information gathering and reconnaissance needs
+- It can help you gather multiple types of information (such as phone numbers, ip addr, whois, etc.) from various publicly available sources about the target
+> Previously, `PH0MBER` was a tool used to gather information about a phone number, but now it has been upgraded to a ___framework___ with many _scanners_ available!
 
 
 
 <br>
 <br>
 
-## Install & Usage: A Quick Guide
+## Quick Guide
+> Install, Update, Usage
+
+<br>
 
 ### Installation:
 - __git clone__
 ```
 git clone https://github.com/s41r4j/phomber
 cd phomber
 pip3 install -r requirements.txt
@@ -45,14 +49,28 @@
 - __pip__
 ```
 pip install phomber
 ```
 
 <br>
 
+### Update:
+- __git clone__ (assuming you are in the `phomber` directory)
+```
+git pull
+```
+
+- __pip__
+```
+pip install --upgrade phomber
+```
+
+
+<br>
+
 ### Usage:
 - __git clone__ (assuming you are in the `phomber` directory)
 ```
 python3 phomber.py
 ```
 
 - __pip__
@@ -61,38 +79,36 @@
 ```
 
 - Help menu
 ```
     ┌────────────────────────────────────────────────────┐
     | COMMANDS      | DESCRIPTION                        |
     |----------------------------------------------------|
-    |                <Basic Commands>                    |
+    |                 <(Basic Commands)>                 |
     |----------------------------------------------------|
     | help          | Display this help menu             | 
     | exit/quit     | Exit the framework                 |
     | dork          | Show a random google dork query *  |  
     | exp           | Show info about all available      |       
     |               | expressions                        |
     | check         | Check internet connection          |
     | clear         | Clear screen                       |
     | save          | Save output of previous scanner    |
     |               | command in a file                  |
     | shell <cmd>   | Execute native shell/cmd commands  |
     | info          | Show info about framework & system |
     | change        | Change user command input color    |
     |----------------------------------------------------|
-    |                 <Scanner Commands>                 |
+    |                <(Scanner Commands)>                |
     |----------------------------------------------------|
     | number        | Reverse phone number lookup *      |
     | ip            | Reverse ip address lookup *        |
     | mac           | Reverse mac address lookup         |
     | whois         | Reverse whois lookup *             |
-    | dns           | Reverse or normal DNS lookup       |
-    |----------------------------------------------------|
-    | MORE SCANNERS COMING SOON, THIS IS A BETA VER      |
+    | dns           | Reverse or normal DNS lookup *     |
     └────────────────────────────────────────────────────┘
 ```
 
 #### Pro tips:
 - Type `help` to get a list of commands
 - Type `help <command>` to see more info about a command
 - Use `Tab` key to auto-complete commands
@@ -105,9 +121,9 @@
 <br>
 
 
 ### NOTES:
 ```
 - `PH0MBER` is back with all new features and user interface
 - `v3` has osint tools with no _api key_ requirement
-- Currently this `v3.0-beta` is for testing, try using & report bugs
+- ADD: custom-scanner feature; create, distribute and deploy your own scanner
 ```
```

#### html2text {}

```diff
@@ -1,44 +1,48 @@
                           [.images/phomber_logo.png]
 ``` An open source infomation grathering & reconnaissance framework! ```
   [https://img.shields.io/badge/Etical_Hacking-OSINT-yellow.svg?logo=sharp]
-[https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks] [https:
-  //img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python] [https://
-      img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg] [https://
+  [https://img.shields.io/badge/Version-v3.1.0-orange.svg?logo=vectorworks]
+[https://img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python] [https:
+     //img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg] [https://
  img.shields.io/badge/Disclaimer-With great power comes great responsibility-
                             red.svg?logo=hackaday]
 
-             ****** PH0MBER: osint framework [3.0.9 (beta)] ******
+                    ****** PH0MBER: osint framework ******
 
-## What is PH0MBER? - `PH0MBER` is a tool which is used to gather information
-about a target which is publicly available - Previously `PH0MBER` was a tool
-which was used to gather information about a phone number, but now it has been
-upgraded to a _framework_ with many _scanners_
+## What is PH0MBER? - `PH0MBER` is a one-stop tool for your information
+gathering and reconnaissance needs - It can help you gather multiple types of
+information (such as phone numbers, ip addr, whois, etc.) from various publicly
+available sources about the target > Previously, `PH0MBER` was a tool used to
+gather information about a phone number, but now it has been upgraded to a
+___framework___ with many _scanners_ available!
 
-## Install & Usage: A Quick Guide ### Installation: - __git clone__ ``` git
-clone https://github.com/s41r4j/phomber cd phomber pip3 install -
-r requirements.txt ``` - __pip__ ``` pip install phomber ```
+## Quick Guide > Install, Update, Usage
+### Installation: - __git clone__ ``` git clone https://github.com/s41r4j/
+phomber cd phomber pip3 install -r requirements.txt ``` - __pip__ ``` pip
+install phomber ```
+### Update: - __git clone__ (assuming you are in the `phomber` directory) ```
+git pull ``` - __pip__ ``` pip install --upgrade phomber ```
 ### Usage: - __git clone__ (assuming you are in the `phomber` directory) ```
 python3 phomber.py ``` - __pip__ ``` phomber ``` - Help menu ```
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 | COMMANDS | DESCRIPTION | |---------------------------------------------------
--| |  | |----------------------------------------------------| | help | Display
-this help menu | | exit/quit | Exit the framework | | dork | Show a random
-google dork query * | | exp | Show info about all available | | | expressions |
-| check | Check internet connection | | clear | Clear screen | | save | Save
-output of previous scanner | | | command in a file | | shell  | Execute native
-shell/cmd commands | | info | Show info about framework & system | | change |
-Change user command input color | |--------------------------------------------
---------| |  | |----------------------------------------------------| | number
-| Reverse phone number lookup * | | ip | Reverse ip address lookup * | | mac |
-Reverse mac address lookup | | whois | Reverse whois lookup * | | dns | Reverse
-or normal DNS lookup | |----------------------------------------------------| |
-MORE SCANNERS COMING SOON, THIS IS A BETA VER |
+-| | <(Basic Commands)> | |----------------------------------------------------
+| | help | Display this help menu | | exit/quit | Exit the framework | | dork |
+Show a random google dork query * | | exp | Show info about all available | | |
+expressions | | check | Check internet connection | | clear | Clear screen | |
+save | Save output of previous scanner | | | command in a file | | shell  |
+Execute native shell/cmd commands | | info | Show info about framework & system
+| | change | Change user command input color | |-------------------------------
+---------------------| | <(Scanner Commands)> | |------------------------------
+----------------------| | number | Reverse phone number lookup * | | ip |
+Reverse ip address lookup * | | mac | Reverse mac address lookup | | whois |
+Reverse whois lookup * | | dns | Reverse or normal DNS lookup * |
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââ
 ``` #### Pro tips: - Type `help` to get a list of commands - Type `help ` to
 see more info about a command - Use `Tab` key to auto-complete commands - Try
 silent mode by using `-s`/`--silent` flag - You can also use `Ctrl+C` to exit -
 Descriptions ending with `*` needs internet connection
 
 ### NOTES: ``` - `PH0MBER` is back with all new features and user interface -
-`v3` has osint tools with no _api key_ requirement - Currently this `v3.0-beta`
-is for testing, try using & report bugs ```
+`v3` has osint tools with no _api key_ requirement - ADD: custom-scanner
+feature; create, distribute and deploy your own scanner ```
```

### Comparing `phomber-3.0.9/phomber/phomber.py` & `phomber-3.1.0/phomber/phomber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 
 #==============================================================================#
 #                                                                              #
 # [prog]   : PH0MBER                                                           #
-# [ver]    : 3.0.8 beta                                                        #
+# [ver]    : 3.1.0                                                        #
 # [desc]   : An open source infomation grathering & reconnaissance framework!  #
 # [dev]    : @s41r4j                                                           #
 # [license]: GNU GPLv3                                                         #
 # [github] : https://github.com/s41r4j/phomber                                 #
 # [pypi]   : https://pypi.org/project/phomber/                                 #
 #                                                                              #
 #==============================================================================#
@@ -34,23 +34,24 @@
 import sys           # Default
 import random        # Default
 import time          # Default
 import readline      # Default
 import re            # Default
 import uuid          # Default
 import socket        # Default
+import platform      # Default
 import psutil        # pip install psutil
 import bs4           # pip install beautifulsoup4
 import phonenumbers  # pip install phonenumbers
 from mac_vendor_lookup import MacLookup # pip install mac-vendor-lookup
 import whois         # pip install python-whois
 import dns.resolver  # pip install dnspython
 
 
-# ------------------------ Global variables ------------------------ #
+# ------------------------- Global variables ------------------------ #
 avaliable_commands = ['change', 'check', 'clear', 'dork', 'dns', 'exit', 'exp', 'help', 'info', 'ip', 'mac', 'number', 'quit', 'save', 'shell', 'whois']
 prv_op = ''
 full_cmd = ''
 silent_mode = False
 
 # ------------------------ Scanner functions ------------------------ #
 
@@ -731,39 +732,34 @@
     '''
 
     print('\n    ┌──────────────────────────────────────────────────────┐\n'+final_output_scanned+final_output_remaining)
     prv_op += '\n    ┌──────────────────────────────────────────────────────┐'+'\n'+final_output_scanned+final_output_remaining
 
     return True
 
-# Reverse email lookup
-def email_lookup():
-    pass
-
 # --------------------------- Basic functions ------------------------ #
 
 def printit(text, center='', line_up=False, line_down=False, space_up=False, space_down=False, coledt=[0, 0, 0], normaltxt_start='', normaltxt_end='', hide=False, verbose_mode=False, input_mode=False):
     if not hide or verbose_mode:
         # get terminal width
         width = os.get_terminal_size().columns
 
         # printing text
         if space_up: print()
         if line_up: print('⸺'*width)
 
         print(normaltxt_start, end='')
 
-        if len(text) < width:
-            new_width = int((width - len(text))/2)
-            print(center*new_width, end='')
-            print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
-            if input_mode: input_var = input(text)
-            else: print(str(text), end='')
-            print('\033[0m', end='')
-            print(center*new_width)
+        new_width = int((width - len(text))/2)
+        print(center*new_width, end='')
+        print(f'\33[{coledt[0]};{coledt[1]};{coledt[2]}m', end='')
+        if input_mode: input_var = input(text)
+        else: print(str(text), end='')
+        print('\033[0m', end='')
+        print(center*new_width)
 
         print(normaltxt_end, end='')
 
         if line_down: print('⸺'*width)
         if space_down: print()
 
         if input_mode: return input_var
@@ -894,23 +890,24 @@
     | \33[1;49;93m:|\033[0m            | It's a warning (remember)          |
     | \33[1;49;91m:(\033[0m            | Something went wrong               |
     | \33[1;49;97m:o\033[0m            | Scan results available             |
     └────────────────────────────────────────────────────┘'''
 
     # Variables
     user = '\33[1;49;96m'+str(os.getlogin())+'\033[0m'+ ' '*int(34-len(str(os.getlogin())))
-    hostname = '\33[1;49;96m'+str(os.uname().nodename)+'\033[0m'+' '*int(34-len(str(os.uname().nodename)))
-    os_name = '\33[1;49;96m'+str(os.uname().sysname)+'\033[0m'+' '*int(34-len(str(os.uname().sysname)))
+    hostname = '\33[1;49;96m'+str(platform.node())+'\033[0m'+' '*int(34-len(str(platform.node())))
+    os_name = '\33[1;49;96m'+str(platform.system())+'\033[0m'+' '*int(34-len(str(platform.system())))
     ram = '\33[1;49;96m'+str(psutil.virtual_memory().percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.virtual_memory().percent)))
     cpu = '\33[1;49;96m'+str(psutil.cpu_percent())+"%"+'\033[0m'+' '*int(32-len(str(psutil.cpu_percent())))
     disk = '\33[1;49;96m'+str(psutil.disk_usage('/').percent)+"%"+'\033[0m'+' '*int(33-len(str(psutil.disk_usage('/').percent)))
     sys_mac = '\33[1;49;96m'+str(':'.join(re.findall('..', '%012x' % uuid.getnode())))+'\033[0m'+' '*int(34-len(str(':'.join(re.findall('..', '%012x' % uuid.getnode())))))
-    arch = '\33[1;49;96m'+str(os.uname().machine)+'\033[0m'+' '*int(34-len(str(os.uname().machine)))
-
-    ver = '\33[1;49;96m3.0.8 (beta)\033[0m'+' '*int(34-len(str(3.0)))
+    arch = '\33[1;49;96m'+str(platform.machine())+'\033[0m'+' '*int(34-len(str(platform.machine())))
+    
+    v = '3.1.0'
+    ver = '\33[1;49;96m'+str(v)+'\033[0m'+' '*int(34-len(str(v)))
 
     sysinfo = f'''
     ┌────────────────────────────────────────────────────┐
     | SYSTEM INFO   | DESCRIPTION                        |
     |----------------------------------------------------|
     | \33[1;49;97mUser\033[0m          | {user} |
     | \33[1;49;97mHostname\033[0m      | {hostname} |
@@ -955,18 +952,15 @@
     |----------------------------------------------------|
     |                <(Scanner Commands)>                |
     |----------------------------------------------------|
     | \33[1;49;97mnumber\033[0m        | Reverse phone number lookup \33[1;49;91m*\033[0m      |
     | \33[1;49;97mip\033[0m            | Reverse ip address lookup \33[1;49;91m*\033[0m        |
     | \33[1;49;97mmac\033[0m           | Reverse mac address lookup         |
     | \33[1;49;97mwhois\033[0m         | Reverse whois lookup \33[1;49;91m*\033[0m             |
-    | \33[1;49;97mdns\033[0m           | Reverse or normal DNS lookup       |
-    |----------------------------------------------------|
-    | \33[1;49;91mMORE SCANNERS COMING SOON, THIS IS A BETA VER\033[0m      |
-    | \33[1;49;91mReport bugs at: github.com/s41r4j/phomber/issues\033[0m   |
+    | \33[1;49;97mdns\033[0m           | Reverse or normal DNS lookup \33[1;49;91m*\033[0m     |
     └────────────────────────────────────────────────────┘
     '''
 
     tips = ['Type `\33[7;49;93mhelp <command>\033[0m\33[1;49;93m` to see more info about a command',
             'Use `\33[7;49;93mTab\033[0m\33[1;49;93m` key to auto-complete commands',
             'Try silent mode by using `\33[7;49;93m-s\033[0m\33[1;49;93m`/`\33[7;49;93m--silent\033[0m\33[1;49;93m` flag',
             'You can also use `\33[7;49;93mCtrl+C\033[0m\33[1;49;93m` to exit',
@@ -1081,22 +1075,14 @@
                     crt_exp = exp[1]
                     number_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mnumber\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `number`, it will reverse lookup phone number over internet and show public info associated with it
     \33[1;49;92m> SYNTAX: \33[1;49;97mnumber <phone_number>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mnumber +1234567890
     \033[0m'''
                     print(number_help)
-                elif cmd == 'email':
-                    crt_exp = exp[1]
-                    email_help = f'''  \33[1;49;93m[+] Command Info: \33[1;49;93memail\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `email`, it will perform reverse email lookup
-    \33[1;49;92m> SYNTAX: \33[1;49;97memail <email_address>
-    \33[1;49;92m> EXAMPLE: \33[1;49;97memail {user.strip()}\33[1;49;96m@gmail.com
-    \033[0m'''
-                    print(email_help)
                 elif cmd == 'whois':
                     crt_exp = exp[1]
                     whois_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mwhois\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `whois`, it will perform reverse whois lookup
     \33[1;49;92m> SYNTAX: \33[1;49;97mwhois <domain_name>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mwhois example.com
     \033[0m'''
@@ -1113,30 +1099,14 @@
                     crt_exp = exp[1]
                     ip_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mip\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `ip`, it will perform an ip address lookup over internet and show info about given ip address
     \33[1;49;92m> SYNTAX: \33[1;49;97mip <ip_address>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mip 8.8.8.8
     \033[0m'''
                     print(ip_help)
-                elif cmd == 'username':
-                    crt_exp = exp[1]
-                    username_help = f'''  \33[1;49;93m[+] Command Info: \33[1;49;93musername\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `username`, it will perform reverse username lookup over various social media platforms and check if username is associated with any account
-    \33[1;49;92m> SYNTAX: \33[1;49;97musername <username>
-    \33[1;49;92m> EXAMPLE: \33[1;49;97musername {user.strip()}
-    \033[0m'''
-                    print(username_help)
-                elif cmd == 'hash':
-                    crt_exp = exp[1]
-                    hash_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mhash\n
-    \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `hash`, it will perform reverse hash lookup
-    \33[1;49;92m> SYNTAX: \33[1;49;97mhash <hash>
-    \33[1;49;92m> EXAMPLE: \33[1;49;97mhash 098f6bcd4621d373cade4e832627b4f6
-    \033[0m'''
-                    print(hash_help)
                 elif cmd == 'mac':
                     crt_exp = exp[1]
                     mac_help = '''  \33[1;49;93m[+] Command Info: \33[1;49;93mmac\n
     \33[1;49;92m> DESCRIPTION: \33[1;49;97mWhen you type `mac`, it will lookup probable vendor/manufacture of given mac address
     \33[1;49;92m> SYNTAX: \33[1;49;97mmac <mac_address>
     \33[1;49;92m> EXAMPLE: \33[1;49;97mmac ff:ff:ff:ff:ff:ff
     \033[0m'''
@@ -1358,10 +1328,18 @@
         control_center()
     except KeyboardInterrupt:
         print()
         if not silent_mode:
             printit('[#] Terminating `PH0MBER` framework...', coledt=[1, 49, random.choice([91, 93])], space_down=True, line_down=True, line_up=True, space_up=True)
             exit()
         else: print()
+    except Exception as e:
+        print()
+        if not silent_mode:
+            printit(f'[!] An error occured: {e}', coledt=[1, 49, 91], space_up=True)
+            printit(f'[i] Please report this error/bug/issue at: https://github.com/s41r4j/phomber/issues', coledt=[1, 49, 93], space_down=True)
+            printit('[#] Terminating `PH0MBER` framework...', coledt=[1, 49, random.choice([91, 93])], space_down=True, line_down=True, line_up=True, space_up=True)
+            exit()
+        else: print()
 
 if __name__ == '__main__':
     main()
```

### Comparing `phomber-3.0.9/phomber.egg-info/PKG-INFO` & `phomber-3.1.0/phomber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phomber
-Version: 3.0.9
+Version: 3.1.0
 Summary: `PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering
 Author: s41r4j
 Maintainer: s41r4j
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -681,14 +681,16 @@
         
 Project-URL: Homepage, https://github.com/s41r4j/phomber
 Project-URL: Bug Tracker, https://github.com/s41r4j/phomber/issues
 Keywords: python,hacking,pentesting,phomber,reverse,lookup,osint,framework,tool,s41r4j
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Environment :: Console
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align=center>
          <img src='.images/phomber_logo.png'>
 </p>
@@ -696,39 +698,43 @@
 
 ```
 An open source infomation grathering & reconnaissance framework!
 ```
 
 <p align=center>
          <a href='https://www.w3schools.in/ethical-hacking/information-gathering-techniques/'><img src="https://img.shields.io/badge/Etical Hacking-OSINT-yellow.svg?logo=sharp"></a>
-         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.0-orange.svg?logo=vectorworks"></a>
+         <a href='https://github.com/s41r4j/phomber/releases/'><img src="https://img.shields.io/badge/Version-v3.1.0-orange.svg?logo=vectorworks"></a>
          <a href='https://www.python.org/'><img src="https://img.shields.io/badge/Python-3-blue.svg?style=flat&logo=python"></a>
          <a href='LICENSE'><img src="https://img.shields.io/badge/License-GPL%20v3.0-brightgreen.svg"></a>
          <a href=''><img src="https://img.shields.io/badge/Disclaimer-With great power comes great responsibility-red.svg?logo=hackaday"></a>
 </p>
       
 <br>
 
-<h1 align=center>PH0MBER: osint framework [3.0.9 (beta)]</h1>
+<h1 align=center>PH0MBER: osint framework</h1>
 
 
 
 <br>
 
 ## What is PH0MBER?
 
-- `PH0MBER` is a tool which is used to gather information about a target which is publicly available
-- Previously `PH0MBER` was a tool which was used to gather information about a phone number, but now it has been upgraded to a _framework_ with many _scanners_
+- `PH0MBER` is a one-stop tool for your information gathering and reconnaissance needs
+- It can help you gather multiple types of information (such as phone numbers, ip addr, whois, etc.) from various publicly available sources about the target
+> Previously, `PH0MBER` was a tool used to gather information about a phone number, but now it has been upgraded to a ___framework___ with many _scanners_ available!
 
 
 
 <br>
 <br>
 
-## Install & Usage: A Quick Guide
+## Quick Guide
+> Install, Update, Usage
+
+<br>
 
 ### Installation:
 - __git clone__
 ```
 git clone https://github.com/s41r4j/phomber
 cd phomber
 pip3 install -r requirements.txt
@@ -736,14 +742,28 @@
 - __pip__
 ```
 pip install phomber
 ```
 
 <br>
 
+### Update:
+- __git clone__ (assuming you are in the `phomber` directory)
+```
+git pull
+```
+
+- __pip__
+```
+pip install --upgrade phomber
+```
+
+
+<br>
+
 ### Usage:
 - __git clone__ (assuming you are in the `phomber` directory)
 ```
 python3 phomber.py
 ```
 
 - __pip__
@@ -752,38 +772,36 @@
 ```
 
 - Help menu
 ```
     ┌────────────────────────────────────────────────────┐
     | COMMANDS      | DESCRIPTION                        |
     |----------------------------------------------------|
-    |                <Basic Commands>                    |
+    |                 <(Basic Commands)>                 |
     |----------------------------------------------------|
     | help          | Display this help menu             | 
     | exit/quit     | Exit the framework                 |
     | dork          | Show a random google dork query *  |  
     | exp           | Show info about all available      |       
     |               | expressions                        |
     | check         | Check internet connection          |
     | clear         | Clear screen                       |
     | save          | Save output of previous scanner    |
     |               | command in a file                  |
     | shell <cmd>   | Execute native shell/cmd commands  |
     | info          | Show info about framework & system |
     | change        | Change user command input color    |
     |----------------------------------------------------|
-    |                 <Scanner Commands>                 |
+    |                <(Scanner Commands)>                |
     |----------------------------------------------------|
     | number        | Reverse phone number lookup *      |
     | ip            | Reverse ip address lookup *        |
     | mac           | Reverse mac address lookup         |
     | whois         | Reverse whois lookup *             |
-    | dns           | Reverse or normal DNS lookup       |
-    |----------------------------------------------------|
-    | MORE SCANNERS COMING SOON, THIS IS A BETA VER      |
+    | dns           | Reverse or normal DNS lookup *     |
     └────────────────────────────────────────────────────┘
 ```
 
 #### Pro tips:
 - Type `help` to get a list of commands
 - Type `help <command>` to see more info about a command
 - Use `Tab` key to auto-complete commands
@@ -796,9 +814,9 @@
 <br>
 
 
 ### NOTES:
 ```
 - `PH0MBER` is back with all new features and user interface
 - `v3` has osint tools with no _api key_ requirement
-- Currently this `v3.0-beta` is for testing, try using & report bugs
+- ADD: custom-scanner feature; create, distribute and deploy your own scanner
 ```
```

### Comparing `phomber-3.0.9/pyproject.toml` & `phomber-3.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "phomber"
-version = "3.0.9"
+version = "3.1.0"
 description = "`PH0MBER` a simple yet powerful osint framework for reconnaissance and information gathering"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 authors = [
   {name = "s41r4j"}
 ]
@@ -17,14 +17,16 @@
   {name = "s41r4j"}
 ]
 keywords=['python', 'hacking', 'pentesting', 'phomber', 'reverse', 'lookup', 'osint', 'framework', 'tool', 's41r4j']
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
+    "Environment :: Console",
+    "Development Status :: 5 - Production/Stable"
 ]
 dependencies = ['requests', 'uuid', 'psutil', 'beautifulsoup4', 'phonenumbers', 'mac-vendor-lookup', 'python-whois', 'dnspython']
 
 
 [project.urls]
 "Homepage" = "https://github.com/s41r4j/phomber"
 "Bug Tracker" = "https://github.com/s41r4j/phomber/issues"
```

