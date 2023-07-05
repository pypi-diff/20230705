# Comparing `tmp/chromedriver-autoinstaller-0.4.0.tar.gz` & `tmp/chromedriver-autoinstaller-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromedriver-autoinstaller-0.4.0.tar", last modified: Wed Aug  3 10:17:50 2022, max compression
+gzip compressed data, was "chromedriver-autoinstaller-0.4.1.tar", last modified: Wed Jul  5 02:45:25 2023, max compression
```

## Comparing `chromedriver-autoinstaller-0.4.0.tar` & `chromedriver-autoinstaller-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yeongbinjo   (501) staff       (20)        0 2022-08-03 10:17:50.062966 chromedriver-autoinstaller-0.4.0/
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     1068 2022-08-03 01:16:31.000000 chromedriver-autoinstaller-0.4.0/LICENSE
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     2100 2022-08-03 10:17:50.063145 chromedriver-autoinstaller-0.4.0/PKG-INFO
--rw-r--r--   0 yeongbinjo   (501) staff       (20)      847 2022-08-03 01:16:31.000000 chromedriver-autoinstaller-0.4.0/README.md
-drwxr-xr-x   0 yeongbinjo   (501) staff       (20)        0 2022-08-03 10:17:50.060758 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller/
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     1398 2022-08-03 10:09:04.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller/__init__.py
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     8635 2022-08-03 10:12:21.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller/utils.py
-drwxr-xr-x   0 yeongbinjo   (501) staff       (20)        0 2022-08-03 10:17:50.062707 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     2100 2022-08-03 10:17:50.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/PKG-INFO
--rw-r--r--   0 yeongbinjo   (501) staff       (20)      364 2022-08-03 10:17:50.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/SOURCES.txt
--rw-r--r--   0 yeongbinjo   (501) staff       (20)        1 2022-08-03 10:17:50.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/dependency_links.txt
--rw-r--r--   0 yeongbinjo   (501) staff       (20)       96 2022-08-03 10:17:50.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/entry_points.txt
--rw-r--r--   0 yeongbinjo   (501) staff       (20)       27 2022-08-03 10:17:50.000000 chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/top_level.txt
--rw-r--r--   0 yeongbinjo   (501) staff       (20)       79 2022-08-03 10:17:50.063597 chromedriver-autoinstaller-0.4.0/setup.cfg
--rw-r--r--   0 yeongbinjo   (501) staff       (20)     1962 2022-08-03 10:13:42.000000 chromedriver-autoinstaller-0.4.0/setup.py
+drwxr-xr-x   0 chida      (501) staff       (20)        0 2023-07-05 02:45:25.971937 chromedriver-autoinstaller-0.4.1/
+-rw-r--r--   0 chida      (501) staff       (20)     1068 2023-07-05 02:41:57.000000 chromedriver-autoinstaller-0.4.1/LICENSE
+-rw-r--r--   0 chida      (501) staff       (20)     1883 2023-07-05 02:45:25.971986 chromedriver-autoinstaller-0.4.1/PKG-INFO
+-rw-r--r--   0 chida      (501) staff       (20)      847 2023-07-05 02:41:57.000000 chromedriver-autoinstaller-0.4.1/README.md
+drwxr-xr-x   0 chida      (501) staff       (20)        0 2023-07-05 02:45:25.971347 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller/
+-rw-r--r--   0 chida      (501) staff       (20)     1422 2023-07-05 02:41:57.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller/__init__.py
+-rw-r--r--   0 chida      (501) staff       (20)     9129 2023-07-05 02:41:57.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller/utils.py
+drwxr-xr-x   0 chida      (501) staff       (20)        0 2023-07-05 02:45:25.971846 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/
+-rw-r--r--   0 chida      (501) staff       (20)     1883 2023-07-05 02:45:25.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/PKG-INFO
+-rw-r--r--   0 chida      (501) staff       (20)      364 2023-07-05 02:45:25.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/SOURCES.txt
+-rw-r--r--   0 chida      (501) staff       (20)        1 2023-07-05 02:45:25.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/dependency_links.txt
+-rw-r--r--   0 chida      (501) staff       (20)       95 2023-07-05 02:45:25.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/entry_points.txt
+-rw-r--r--   0 chida      (501) staff       (20)       27 2023-07-05 02:45:25.000000 chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/top_level.txt
+-rw-r--r--   0 chida      (501) staff       (20)       79 2023-07-05 02:45:25.972156 chromedriver-autoinstaller-0.4.1/setup.cfg
+-rw-r--r--   0 chida      (501) staff       (20)     1984 2023-07-05 02:44:44.000000 chromedriver-autoinstaller-0.4.1/setup.py
```

### Comparing `chromedriver-autoinstaller-0.4.0/LICENSE` & `chromedriver-autoinstaller-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.4.0/PKG-INFO` & `chromedriver-autoinstaller-0.4.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
-Description: # chromedriver-autoinstaller
-        Automatically download and install [chromedriver](https://chromedriver.chromium.org/) that supports the currently installed version of chrome. This installer supports Linux, MacOS and Windows operating systems.
-        
-        ## Installation
-        
-        ```bash
-        pip install chromedriver-autoinstaller
-        ```
-        
-        ## Usage
-        Just type `import chromedriver_autoinstaller` in the module you want to use chromedriver.
-        
-        ## Example
-        ```
-        from selenium import webdriver
-        import chromedriver_autoinstaller
-        
-        
-        chromedriver_autoinstaller.install()  # Check if the current version of chromedriver exists
-                                              # and if it doesn't exist, download it automatically,
-                                              # then add chromedriver to path
-        
-        driver = webdriver.Chrome()
-        driver.get("http://www.python.org")
-        assert "Python" in driver.title
-        ```
-        
 Keywords: chromedriver chrome chromium selenium
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# chromedriver-autoinstaller
+Automatically download and install [chromedriver](https://chromedriver.chromium.org/) that supports the currently installed version of chrome. This installer supports Linux, MacOS and Windows operating systems.
+
+## Installation
+
+```bash
+pip install chromedriver-autoinstaller
+```
+
+## Usage
+Just type `import chromedriver_autoinstaller` in the module you want to use chromedriver.
+
+## Example
+```
+from selenium import webdriver
+import chromedriver_autoinstaller
+
+
+chromedriver_autoinstaller.install()  # Check if the current version of chromedriver exists
+                                      # and if it doesn't exist, download it automatically,
+                                      # then add chromedriver to path
+
+driver = webdriver.Chrome()
+driver.get("http://www.python.org")
+assert "Python" in driver.title
+```
```

### Comparing `chromedriver-autoinstaller-0.4.0/README.md` & `chromedriver-autoinstaller-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller/__init__.py` & `chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
-import os
 import logging
-from typing import Optional, AnyStr
+import os
+from typing import AnyStr, Optional
 
 from . import utils
 
 
 def install(cwd: bool = False, path: Optional[AnyStr] = None, no_ssl: bool = False):
     """
     Appends the directory of the chromedriver binary file to PATH.
@@ -16,21 +16,23 @@
     :param no_ssl: Determines whether or not to use the encryption protocol when downloading the chrome driver.
     :return: The file path of chromedriver
     """
     if cwd:
         path = os.getcwd()
     chromedriver_filepath = utils.download_chromedriver(path, no_ssl)
     if not chromedriver_filepath:
-        logging.debug('Can not download chromedriver.')
+        logging.debug("Can not download chromedriver.")
         return
     chromedriver_dir = os.path.dirname(chromedriver_filepath)
-    if 'PATH' not in os.environ:
-        os.environ['PATH'] = chromedriver_dir
-    elif chromedriver_dir not in os.environ['PATH']:
-        os.environ['PATH'] = chromedriver_dir + utils.get_variable_separator() + os.environ['PATH']
+    if "PATH" not in os.environ:
+        os.environ["PATH"] = chromedriver_dir
+    elif chromedriver_dir not in os.environ["PATH"]:
+        os.environ["PATH"] = (
+            chromedriver_dir + utils.get_variable_separator() + os.environ["PATH"]
+        )
     return chromedriver_filepath
 
 
 def get_chrome_version():
     """
     Get installed version of chrome on client
```

### Comparing `chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller/utils.py` & `chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,135 +1,156 @@
 # coding: utf-8
 """
 Helper functions for filename and URL generation.
 """
 
-import sys
+import logging
 import os
+import re
+import shutil
 import subprocess
-import urllib.request
+import sys
 import urllib.error
-import zipfile
+import urllib.request
 import xml.etree.ElementTree as elemTree
-import logging
-import re
-import shutil
-
+import zipfile
 from io import BytesIO
+import platform as pf
 
+__author__ = "Yeongbin Jo <iam.yeongbin.jo@gmail.com>"
 
-__author__ = 'Yeongbin Jo <iam.yeongbin.jo@gmail.com>'
-
-from typing import Optional, AnyStr
+from typing import AnyStr, Optional
 
 
 def get_chromedriver_filename():
     """
     Returns the filename of the binary for the current platform.
     :return: Binary filename
     """
-    if sys.platform.startswith('win'):
-        return 'chromedriver.exe'
-    return 'chromedriver'
+    if sys.platform.startswith("win"):
+        return "chromedriver.exe"
+    return "chromedriver"
 
 
 def get_variable_separator():
     """
     Returns the environment variable separator for the current platform.
     :return: Environment variable separator
     """
-    if sys.platform.startswith('win'):
-        return ';'
-    return ':'
-
-
-def get_platform_architecture():
-    if sys.platform.startswith('linux') and sys.maxsize > 2 ** 32:
-        platform = 'linux'
-        architecture = '64'
-    elif sys.platform == 'darwin':
-        platform = 'mac'
-        architecture = '64'
-    elif sys.platform.startswith('win'):
-        platform = 'win'
-        architecture = '32'
+    if sys.platform.startswith("win"):
+        return ";"
+    return ":"
+
+
+def get_platform_architecture(chrome_version=None):
+    if sys.platform.startswith("linux") and sys.maxsize > 2**32:
+        platform = "linux"
+        architecture = "64"
+    elif sys.platform == "darwin":
+        platform = "mac"
+        if pf.processor() == "arm":
+        # At some point, the release naming for Apple arm changed;
+        # Looking in http://chromedriver.storage.googleapis.com/, the changeover happened across these releases:
+        # 106.0.5249.61/chromedriver_mac_arm64.zip
+        # 106.0.5249.21/chromedriver_mac64_m1.zip
+            if chrome_version is not None and chrome_version <= "106.0.5249.21":
+                print("CHROME <= 106.0.5249.21, using mac64_m1")
+                architecture = "64_m1"
+            else:
+                print("CHROME > 106.0.5249.21, using mac_arm64")
+                architecture = "_arm64"
+        elif pf.processor() == "i386":
+            architecture = "64"
+        else:
+            raise RuntimeError("Could not determine Mac processor architecture.")
+    elif sys.platform.startswith("win"):
+        platform = "win"
+        architecture = "32"
     else:
-        raise RuntimeError('Could not determine chromedriver download URL for this platform.')
+        raise RuntimeError(
+            "Could not determine chromedriver download URL for this platform."
+        )
     return platform, architecture
 
 
 def get_chromedriver_url(version, no_ssl=False):
     """
     Generates the download URL for current platform , architecture and the given version.
     Supports Linux, MacOS and Windows.
     :param version: chromedriver version string
     :param no_ssl: Determines whether or not to use the encryption protocol when downloading the chrome driver.
     :return: Download URL for chromedriver
     """
     if no_ssl:
-        base_url = 'http://chromedriver.storage.googleapis.com/'
+        base_url = "http://chromedriver.storage.googleapis.com/"
     else:
-        base_url = 'https://chromedriver.storage.googleapis.com/'
-    platform, architecture = get_platform_architecture()
-    return base_url + version + '/chromedriver_' + platform + architecture + '.zip'
+        base_url = "https://chromedriver.storage.googleapis.com/"
+    platform, architecture = get_platform_architecture(version)
+    return base_url + version + "/chromedriver_" + platform + architecture + ".zip"
 
 
 def find_binary_in_path(filename):
     """
     Searches for a binary named `filename` in the current PATH. If an executable is found, its absolute path is returned
     else None.
     :param filename: Filename of the binary
     :return: Absolute path or None
     """
-    if 'PATH' not in os.environ:
+    if "PATH" not in os.environ:
         return None
-    for directory in os.environ['PATH'].split(get_variable_separator()):
+    for directory in os.environ["PATH"].split(get_variable_separator()):
         binary = os.path.abspath(os.path.join(directory, filename))
         if os.path.isfile(binary) and os.access(binary, os.X_OK):
             return binary
     return None
 
 
 def check_version(binary, required_version):
     try:
-        version = subprocess.check_output([binary, '-v'])
-        version = re.match(r'.*?([\d.]+).*?', version.decode('utf-8'))[1]
+        version = subprocess.check_output([binary, "-v"])
+        version = re.match(r".*?([\d.]+).*?", version.decode("utf-8"))[1]
         if version == required_version:
             return True
     except Exception:
         return False
     return False
 
 
 def get_chrome_version():
     """
     :return: the version of chrome installed on client
     """
     platform, _ = get_platform_architecture()
-    if platform == 'linux':
+    if platform == "linux":
         path = get_linux_executable_path()
-        with subprocess.Popen([path, '--version'], stdout=subprocess.PIPE) as proc:
-            version = proc.stdout.read().decode('utf-8').replace('Chromium', '').replace('Google Chrome', '').strip()
-    elif platform == 'mac':
-        process = subprocess.Popen(['/Applications/Google Chrome.app/Contents/MacOS/Google Chrome', '--version'], stdout=subprocess.PIPE)
-        version = process.communicate()[0].decode('UTF-8').replace('Google Chrome', '').strip()
-    elif platform == 'win':
+        with subprocess.Popen([path, "--version"], stdout=subprocess.PIPE) as proc:
+            version = (
+                proc.stdout.read()
+                .decode("utf-8")
+                .replace("Chromium", "")
+                .replace("Google Chrome", "")
+                .strip()
+            )
+    elif platform == "mac":
         process = subprocess.Popen(
-            ['reg', 'query', 'HKEY_CURRENT_USER\\Software\\Google\\Chrome\\BLBeacon', '/v', 'version'],
-            stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, stdin=subprocess.DEVNULL
+            [
+                "/Applications/Google Chrome.app/Contents/MacOS/Google Chrome",
+                "--version",
+            ],
+            stdout=subprocess.PIPE,
         )
-        output = process.communicate()
-        if output and output[0] and len(output[0]) > 0:
-            version = output[0].decode('UTF-8').strip().split()[-1]
-        else:
-            process = subprocess.Popen(
-                ['powershell', '-command', '$(Get-ItemProperty -Path Registry::HKEY_CURRENT_USER\\Software\\Google\\chrome\\BLBeacon).version'],
-                stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE
-            )
-            version = process.communicate()[0].decode('UTF-8').strip()
+        version = (
+            process.communicate()[0]
+            .decode("UTF-8")
+            .replace("Google Chrome", "")
+            .strip()
+        )
+    elif platform == "win":
+        dirs = [f.name for f in os.scandir("C:\\Program Files\\Google\\Chrome\\Application") if f.is_dir() and re.match("^[0-9.]+$", f.name)]
+        version = max(dirs)
     else:
         return
     return version
 
 
 def get_linux_executable_path():
     """
@@ -154,30 +175,34 @@
 
 
 def get_major_version(version):
     """
     :param version: the version of chrome
     :return: the major version of chrome
     """
-    return version.split('.')[0]
+    return version.split(".")[0]
 
 
 def get_matched_chromedriver_version(version, no_ssl=False):
     """
     :param version: the version of chrome
     :return: the version of chromedriver
     """
     if no_ssl:
-        doc = urllib.request.urlopen('http://chromedriver.storage.googleapis.com').read()
+        doc = urllib.request.urlopen(
+            "http://chromedriver.storage.googleapis.com"
+        ).read()
     else:
-        doc = urllib.request.urlopen('https://chromedriver.storage.googleapis.com').read()
+        doc = urllib.request.urlopen(
+            "https://chromedriver.storage.googleapis.com"
+        ).read()
     root = elemTree.fromstring(doc)
-    for k in root.iter('{http://doc.s3.amazonaws.com/2006-03-01}Key'):
-        if k.text.find(get_major_version(version) + '.') == 0:
-            return k.text.split('/')[0]
+    for k in root.iter("{http://doc.s3.amazonaws.com/2006-03-01}Key"):
+        if k.text.find(get_major_version(version) + ".") == 0:
+            return k.text.split("/")[0]
     return
 
 
 def get_chromedriver_path():
     """
     :return: path of the chromedriver binary
     """
@@ -198,54 +223,53 @@
 
     :param str path: Path of the directory where to save the downloaded chromedriver to.
     :param bool no_ssl: Determines whether or not to use the encryption protocol when downloading the chrome driver.
     :return: The file path of chromedriver
     """
     chrome_version = get_chrome_version()
     if not chrome_version:
-        logging.debug('Chrome is not installed.')
+        logging.debug("Chrome is not installed.")
         return
     chromedriver_version = get_matched_chromedriver_version(chrome_version, no_ssl)
     if not chromedriver_version:
-        logging.warning('Can not find chromedriver for currently installed chrome version.')
+        logging.warning(
+            "Can not find chromedriver for currently installed chrome version."
+        )
         return
     major_version = get_major_version(chromedriver_version)
 
     if path:
         if not os.path.isdir(path):
-            raise ValueError(f'Invalid path: {path}')
-        chromedriver_dir = os.path.join(
-            os.path.abspath(path),
-            major_version
-        )
+            raise ValueError(f"Invalid path: {path}")
+        chromedriver_dir = os.path.join(os.path.abspath(path), major_version)
     else:
         chromedriver_dir = os.path.join(
-            os.path.abspath(os.path.dirname(__file__)),
-            major_version
+            os.path.abspath(os.path.dirname(__file__)), major_version
         )
     chromedriver_filename = get_chromedriver_filename()
     chromedriver_filepath = os.path.join(chromedriver_dir, chromedriver_filename)
-    if not os.path.isfile(chromedriver_filepath) or \
-            not check_version(chromedriver_filepath, chromedriver_version):
-        logging.info(f'Downloading chromedriver ({chromedriver_version})...')
+    if not os.path.isfile(chromedriver_filepath) or not check_version(
+        chromedriver_filepath, chromedriver_version
+    ):
+        logging.info(f"Downloading chromedriver ({chromedriver_version})...")
         if not os.path.isdir(chromedriver_dir):
             os.makedirs(chromedriver_dir)
         url = get_chromedriver_url(version=chromedriver_version, no_ssl=no_ssl)
         try:
             response = urllib.request.urlopen(url)
             if response.getcode() != 200:
-                raise urllib.error.URLError('Not Found')
+                raise urllib.error.URLError("Not Found")
         except urllib.error.URLError:
-            raise RuntimeError(f'Failed to download chromedriver archive: {url}')
+            raise RuntimeError(f"Failed to download chromedriver archive: {url}")
         archive = BytesIO(response.read())
         with zipfile.ZipFile(archive) as zip_file:
             zip_file.extract(chromedriver_filename, chromedriver_dir)
     else:
-        logging.info('Chromedriver is already installed.')
+        logging.info("Chromedriver is already installed.")
     if not os.access(chromedriver_filepath, os.X_OK):
         os.chmod(chromedriver_filepath, 0o744)
     return chromedriver_filepath
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     print(get_chrome_version())
     print(download_chromedriver(no_ssl=False))
```

### Comparing `chromedriver-autoinstaller-0.4.0/chromedriver_autoinstaller.egg-info/PKG-INFO` & `chromedriver-autoinstaller-0.4.1/chromedriver_autoinstaller.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: chromedriver-autoinstaller
-Version: 0.4.0
+Version: 0.4.1
 Summary: Automatically install chromedriver that supports the currently installed version of chrome.
 Home-page: https://github.com/yeongbin-jo/python-chromedriver-autoinstaller
 Author: Yeongbin Jo
 Author-email: iam.yeongbin.jo@gmail.com
 License: MIT
-Description: # chromedriver-autoinstaller
-        Automatically download and install [chromedriver](https://chromedriver.chromium.org/) that supports the currently installed version of chrome. This installer supports Linux, MacOS and Windows operating systems.
-        
-        ## Installation
-        
-        ```bash
-        pip install chromedriver-autoinstaller
-        ```
-        
-        ## Usage
-        Just type `import chromedriver_autoinstaller` in the module you want to use chromedriver.
-        
-        ## Example
-        ```
-        from selenium import webdriver
-        import chromedriver_autoinstaller
-        
-        
-        chromedriver_autoinstaller.install()  # Check if the current version of chromedriver exists
-                                              # and if it doesn't exist, download it automatically,
-                                              # then add chromedriver to path
-        
-        driver = webdriver.Chrome()
-        driver.get("http://www.python.org")
-        assert "Python" in driver.title
-        ```
-        
 Keywords: chromedriver chrome chromium selenium
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# chromedriver-autoinstaller
+Automatically download and install [chromedriver](https://chromedriver.chromium.org/) that supports the currently installed version of chrome. This installer supports Linux, MacOS and Windows operating systems.
+
+## Installation
+
+```bash
+pip install chromedriver-autoinstaller
+```
+
+## Usage
+Just type `import chromedriver_autoinstaller` in the module you want to use chromedriver.
+
+## Example
+```
+from selenium import webdriver
+import chromedriver_autoinstaller
+
+
+chromedriver_autoinstaller.install()  # Check if the current version of chromedriver exists
+                                      # and if it doesn't exist, download it automatically,
+                                      # then add chromedriver to path
+
+driver = webdriver.Chrome()
+driver.get("http://www.python.org")
+assert "Python" in driver.title
+```
```

### Comparing `chromedriver-autoinstaller-0.4.0/setup.py` & `chromedriver-autoinstaller-0.4.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,61 @@
 # coding: utf-8
 import os
 import sys
 
 from setuptools import setup
 
+__author__ = "Yeongbin Jo <iam.yeongbin.jo@gmail.com>"
 
-__author__ = 'Yeongbin Jo <iam.yeongbin.jo@gmail.com>'
 
-
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 
 # 'setup.py publish' shortcut.
-if sys.argv[-1] == 'publish':
-    os.system('python3 setup.py sdist bdist_wheel')
-    os.system('twine upload dist/*')
+if sys.argv[-1] == "publish":
+    os.system("python3 setup.py sdist bdist_wheel")
+    os.system("twine upload dist/*")
     sys.exit()
-elif sys.argv[-1] == 'clean':
+elif sys.argv[-1] == "clean":
     import shutil
-    if os.path.isdir('build'):
-        shutil.rmtree('build')
-    if os.path.isdir('dist'):
-        shutil.rmtree('dist')
-    if os.path.isdir('chromedriver_autoinstaller.egg-info'):
-        shutil.rmtree('chromedriver_autoinstaller.egg-info')
+
+    if os.path.isdir("build"):
+        shutil.rmtree("build")
+    if os.path.isdir("dist"):
+        shutil.rmtree("dist")
+    if os.path.isdir("chromedriver_autoinstaller.egg-info"):
+        shutil.rmtree("chromedriver_autoinstaller.egg-info")
 
 
 setup(
     name="chromedriver-autoinstaller",
-    version="0.4.0",
+    version="0.4.1",
     author="Yeongbin Jo",
     author_email="iam.yeongbin.jo@gmail.com",
     description="Automatically install chromedriver that supports the currently installed version of chrome.",
     license="MIT",
     keywords="chromedriver chrome chromium selenium",
     url="https://github.com/yeongbin-jo/python-chromedriver-autoinstaller",
-    packages=['chromedriver_autoinstaller'],
+    packages=["chromedriver_autoinstaller"],
     entry_points={
-        'console_scripts': ['chromedriver-path=chromedriver_autoinstaller.utils:print_chromedriver_path'],
+        "console_scripts": [
+            "chromedriver-path=chromedriver_autoinstaller.utils:print_chromedriver_path"
+        ],
     },
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     long_description=long_description,
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Topic :: Software Development :: Testing',
-        'Topic :: System :: Installation/Setup',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "Development Status :: 5 - Production/Stable",
+        "Topic :: Software Development :: Testing",
+        "Topic :: System :: Installation/Setup",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
 )
```

