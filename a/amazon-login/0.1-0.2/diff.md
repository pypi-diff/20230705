# Comparing `tmp/amazon_login-0.1.tar.gz` & `tmp/amazon_login-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_login-0.1.tar", last modified: Wed Jun 28 15:43:33 2023, max compression
+gzip compressed data, was "amazon_login-0.2.tar", last modified: Wed Jul  5 14:50:34 2023, max compression
```

## Comparing `amazon_login-0.1.tar` & `amazon_login-0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 15:43:33.204841 amazon_login-0.1/
--rw-rw-rw-   0        0        0     1093 2023-06-28 15:32:56.000000 amazon_login-0.1/LICENSE
--rw-rw-rw-   0        0        0       20 2023-06-28 15:34:47.000000 amazon_login-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      296 2023-06-28 15:43:33.203841 amazon_login-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-06-27 15:19:37.000000 amazon_login-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-28 15:43:33.192326 amazon_login-0.1/amazon_login.egg-info/
--rw-rw-rw-   0        0        0      296 2023-06-28 15:43:33.000000 amazon_login-0.1/amazon_login.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-06-28 15:43:33.000000 amazon_login-0.1/amazon_login.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 15:43:33.000000 amazon_login-0.1/amazon_login.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      830 2023-06-28 15:43:33.000000 amazon_login-0.1/amazon_login.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-28 15:43:33.000000 amazon_login-0.1/amazon_login.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-28 15:43:33.204841 amazon_login-0.1/setup.cfg
--rw-rw-rw-   0        0        0     2042 2023-06-28 15:43:29.000000 amazon_login-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:43:33.197834 amazon_login-0.1/utils/
--rw-rw-rw-   0        0        0        0 2023-06-21 17:52:16.000000 amazon_login-0.1/utils/__init__.py
--rw-rw-rw-   0        0        0     2124 2023-06-22 15:12:49.000000 amazon_login-0.1/utils/driver.py
--rw-rw-rw-   0        0        0     4784 2023-06-28 15:04:36.000000 amazon_login-0.1/utils/gmail_helper.py
--rw-rw-rw-   0        0        0     1007 2023-06-27 17:04:49.000000 amazon_login-0.1/utils/webdriver_actions.py
-drwxrwxrwx   0        0        0        0 2023-06-28 15:43:33.202843 amazon_login-0.1/vendor_central/
--rw-rw-rw-   0        0        0        0 2023-06-21 16:32:46.000000 amazon_login-0.1/vendor_central/__init__.py
--rw-rw-rw-   0        0        0      879 2023-06-27 16:58:20.000000 amazon_login-0.1/vendor_central/vendor_central.py
--rw-rw-rw-   0        0        0     2936 2023-06-27 16:57:35.000000 amazon_login-0.1/vendor_central/vendor_login.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:50:34.946569 amazon_login-0.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-28 15:32:56.000000 amazon_login-0.2/LICENSE
+-rw-rw-rw-   0        0        0       20 2023-06-28 15:34:47.000000 amazon_login-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      296 2023-07-05 14:50:34.945569 amazon_login-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-06-27 15:19:37.000000 amazon_login-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-05 14:50:34.897112 amazon_login-0.2/amazon_login.egg-info/
+-rw-rw-rw-   0        0        0      296 2023-07-05 14:50:34.000000 amazon_login-0.2/amazon_login.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-07-05 14:50:34.000000 amazon_login-0.2/amazon_login.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 14:50:34.000000 amazon_login-0.2/amazon_login.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      830 2023-07-05 14:50:34.000000 amazon_login-0.2/amazon_login.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-05 14:50:34.000000 amazon_login-0.2/amazon_login.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 14:50:34.912923 amazon_login-0.2/amazon_services/
+-rw-rw-rw-   0        0        0        0 2023-06-21 16:32:46.000000 amazon_login-0.2/amazon_services/__init__.py
+-rw-rw-rw-   0        0        0      955 2023-06-29 16:31:31.000000 amazon_login-0.2/amazon_services/amazon_manager.py
+-rw-rw-rw-   0        0        0     4754 2023-07-05 12:58:59.000000 amazon_login-0.2/amazon_services/login.py
+-rw-rw-rw-   0        0        0       42 2023-07-05 14:50:34.946569 amazon_login-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2042 2023-07-03 14:29:50.000000 amazon_login-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-05 14:50:34.942569 amazon_login-0.2/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-21 17:52:16.000000 amazon_login-0.2/utils/__init__.py
+-rw-rw-rw-   0        0        0     2481 2023-06-29 16:31:46.000000 amazon_login-0.2/utils/driver.py
+-rw-rw-rw-   0        0        0     4784 2023-06-28 15:04:36.000000 amazon_login-0.2/utils/gmail_helper.py
+-rw-rw-rw-   0        0        0     1942 2023-06-29 18:54:19.000000 amazon_login-0.2/utils/webdriver_actions.py
```

### Comparing `amazon_login-0.1/LICENSE` & `amazon_login-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_login-0.1/amazon_login.egg-info/requires.txt` & `amazon_login-0.2/amazon_login.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `amazon_login-0.1/setup.py` & `amazon_login-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="amazon_login",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     include_package_data=True,
     url="http://danielguardado.com",
     python_requires=">=3.9",
     license="MIT",
     author="Daniel Guardado",
     author_email="danguardado217@gmail.com",
```

### Comparing `amazon_login-0.1/utils/driver.py` & `amazon_login-0.2/utils/driver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,66 @@
 import os
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.chrome.options import Options
 from datetime import datetime
 
 
-def find_chromedriver(directory):
-    for root, dirs, files in os.walk(directory):
-        for file in files:
-            if file == "chromedriver.exe" or file == "chromedriver":
-                return os.path.join(root, file)
-    return None
-
+class ChromeDriver:
+    def __init__(
+        self,
+        type,
+        download_path=None,
+    ):
+        if not download_path:
+            current_date_time = datetime.now().strftime("%Y-%m-%d_%H.%M.%S")
+            self.download_path = os.path.join(os.getcwd(), "tmp", current_date_time)
+        else:
+            self.download_path = download_path
+
+        self.chrome_profile_path = os.path.join(os.getcwd(), f"chrome_profile_{type}")
+        self.driver = self.init_driver(self.chrome_profile_path, self.download_path)
+
+    @staticmethod
+    def find_chromedriver(directory):
+        for root, dirs, files in os.walk(directory):
+            for file in files:
+                if file == "chromedriver.exe" or file == "chromedriver":
+                    return os.path.join(root, file)
+        return None
+
+    def init_driver(self, chrome_profile_path, download_path):
+        options = Options()
+
+        # Create a new Chrome profile if the specified directory does not exist
+        if not os.path.exists(chrome_profile_path):
+            os.makedirs(chrome_profile_path)
+            options.add_argument(
+                "--no-first-run"
+            )  # Skip the first-run dialog for new profiles
 
-def init_driver(chrome_profile_path, download_path=os.getcwd()):
-    options = Options()
-
-    # Create a new Chrome profile if the specified directory does not exist
-    if not os.path.exists(chrome_profile_path):
-        os.makedirs(chrome_profile_path)
+        options.add_argument(f"user-data-dir={chrome_profile_path}")
         options.add_argument(
-            "--no-first-run"
-        )  # Skip the first-run dialog for new profiles
+            "profile-directory=Default"
+        )  # Use the same profile directory
 
-    options.add_argument(f"user-data-dir={chrome_profile_path}")
-    options.add_argument("profile-directory=Default")  # Use the same profile directory
+        # Create download directory if it doesn't exist
+        os.makedirs(download_path, exist_ok=True)
 
-    # Create download directory if it doesn't exist
-    os.makedirs(download_path, exist_ok=True)
+        # Add download directory to Chrome preferences
+        prefs = {"download.default_directory": download_path}
+        options.add_experimental_option("prefs", prefs)
+
+        # Find and initialize the Chrome driver
+        chromedriver_path = self.find_chromedriver(os.getcwd())
+        if chromedriver_path:
+            driver = webdriver.Chrome(
+                service=Service(chromedriver_path), options=options
+            )
+        else:
+            chromedriver_path = ChromeDriverManager(path=os.getcwd()).install()
+            driver = webdriver.Chrome(
+                service=Service(chromedriver_path), options=options
+            )
 
-    # Add download directory to Chrome preferences
-    prefs = {"download.default_directory": download_path}
-    options.add_experimental_option("prefs", prefs)
-
-    # Find and initialize the Chrome driver
-    chromedriver_path = find_chromedriver(os.getcwd())
-    if chromedriver_path:
-        driver = webdriver.Chrome(service=Service(chromedriver_path), options=options)
-        return driver
-    else:
-        chromedriver_path = ChromeDriverManager(path=os.getcwd()).install()
-        driver = webdriver.Chrome(service=Service(chromedriver_path), options=options)
         return driver
-
-
-def get_default_driver():
-    chrome_profile_path = os.path.join(os.getcwd(), "chrome_profile")
-    current_date_time = datetime.now().strftime("%Y-%m-%d_%H.%M.%S")
-    download_path = os.path.join(os.getcwd(), "tmp", current_date_time)
-    driver = init_driver(chrome_profile_path, download_path)
-    return driver
```

### Comparing `amazon_login-0.1/utils/gmail_helper.py` & `amazon_login-0.2/utils/gmail_helper.py`

 * *Files identical despite different names*

### Comparing `amazon_login-0.1/vendor_central/vendor_central.py` & `amazon_login-0.2/amazon_services/amazon_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-from vendor_central.vendor_login import VendorLogin
+# from vendor_central.vendor_login import VendorLogin
 from utils.webdriver_actions import WebDriverActions
-from utils.driver import get_default_driver
+from utils.driver import ChromeDriver
+from amazon_services.login import Login
 
 
-class VendorCentral:
+class AmazonManager:
     def __init__(
         self,
         username,
         password,
         login_link,
         logged_in_element,
         sender_email,
         recipient_emails,
-        driver=None,
+        type,
+        chrome_driver=None,
+        download_path=None,
     ):
-        if driver is None:
-            self.driver = get_default_driver()
-        else:
-            self.driver = driver
-        self.driver_actions = WebDriverActions(self.driver)
-        self.login_module = VendorLogin(
+        if chrome_driver is None:
+            chrome_driver = ChromeDriver(type, download_path)
+        self.driver_actions = WebDriverActions(chrome_driver)
+        self.login_module = Login(
             self.driver_actions,
             username,
             password,
             login_link,
             logged_in_element,
             sender_email,
             recipient_emails,
+            type,
         )
 
     def login(self):
         return self.login_module.login()
```

