# Comparing `tmp/dimjournal-1.0.6.tar.gz` & `tmp/dimjournal-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimjournal-1.0.6.tar", last modified: Wed Jul  5 02:02:51 2023, max compression
+gzip compressed data, was "dimjournal-1.0.7.tar", last modified: Wed Jul  5 02:26:01 2023, max compression
```

## Comparing `dimjournal-1.0.6.tar` & `dimjournal-1.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 02:02:37.000000 dimjournal-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 02:02:37.000000 dimjournal-1.0.6/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 02:02:37.000000 dimjournal-1.0.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:02:51.152285 dimjournal-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-05 02:02:37.000000 dimjournal-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 02:02:37.000000 dimjournal-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-05 02:02:51.156285 dimjournal-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 02:02:37.000000 dimjournal-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/dimjournal/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17122 2023-07-05 02:02:37.000000 dimjournal-1.0.6/src/dimjournal/dimjournal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/src/dimjournal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:02:50.000000 dimjournal-1.0.6/src/dimjournal.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 02:02:51.000000 dimjournal-1.0.6/src/dimjournal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:02:51.152285 dimjournal-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tests/test_dimjournal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 02:02:37.000000 dimjournal-1.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.609692 dimjournal-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 02:25:49.000000 dimjournal-1.0.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.601692 dimjournal-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.605692 dimjournal-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-05 02:25:49.000000 dimjournal-1.0.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-05 02:25:49.000000 dimjournal-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 02:25:49.000000 dimjournal-1.0.7/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-05 02:25:49.000000 dimjournal-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-05 02:25:49.000000 dimjournal-1.0.7/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-05 02:25:49.000000 dimjournal-1.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:26:01.609692 dimjournal-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-05 02:25:49.000000 dimjournal-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 02:25:49.000000 dimjournal-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-05 02:26:01.609692 dimjournal-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-05 02:25:49.000000 dimjournal-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.601692 dimjournal-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.605692 dimjournal-1.0.7/src/dimjournal/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 02:25:49.000000 dimjournal-1.0.7/src/dimjournal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-05 02:25:49.000000 dimjournal-1.0.7/src/dimjournal/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17404 2023-07-05 02:25:49.000000 dimjournal-1.0.7/src/dimjournal/dimjournal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.609692 dimjournal-1.0.7/src/dimjournal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 02:26:01.000000 dimjournal-1.0.7/src/dimjournal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 02:26:01.609692 dimjournal-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 02:25:49.000000 dimjournal-1.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-05 02:25:49.000000 dimjournal-1.0.7/tests/test_dimjournal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-05 02:25:49.000000 dimjournal-1.0.7/tox.ini
```

### Comparing `dimjournal-1.0.6/.coveragerc` & `dimjournal-1.0.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/.github/workflows/ci.yml` & `dimjournal-1.0.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/.gitignore` & `dimjournal-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/.pre-commit-config.yaml` & `dimjournal-1.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/LICENSE.txt` & `dimjournal-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/PKG-INFO` & `dimjournal-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.6
+Version: 1.0.7
 Summary: Archive utility for Midjourney
 Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
```

### Comparing `dimjournal-1.0.6/README.md` & `dimjournal-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/setup.cfg` & `dimjournal-1.0.7/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -24,28 +24,25 @@
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
-	importlib-metadata; python_version<"3.8"
 	beautifulsoup4>=4.12.2
 	fire>=0.5.0
 	numpy>=1.25.0
 	Pillow>=10.0.0
 	pymtpng>=1.0
 	pytest>=7.3.1
 	python-slugify>=8.0.1
-	Requests>=2.31.0
 	selenium>=4.10.0
 	setuptools>=67.6.1
 	tqdm>=4.65.0
 	undetected_chromedriver>=3.5.0
-	urwid>=2.1.2
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `dimjournal-1.0.6/setup.py` & `dimjournal-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/src/dimjournal/__init__.py` & `dimjournal-1.0.7/src/dimjournal/__init__.py`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/src/dimjournal/dimjournal.py` & `dimjournal-1.0.7/src/dimjournal/dimjournal.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,28 +38,28 @@
     job_details = ["id", "enqueue_time", "prompt"]
     user_json = Path("user.json")
     jobs_upscaled_json = Path("jobs_upscaled.json")
     cookies_pkl = Path("cookies.pkl")
     mj_download_image_js = """var callback=arguments[arguments.length-1];function getDataUri(e,n){var a=new XMLHttpRequest;a.onload=function(){var e=new FileReader;e.onloadend=function(){n(e.result)},e.readAsDataURL(a.response)},a.open("GET",e),a.responseType="blob",a.send()}getDataUri(document.querySelector("img").src,function(e){callback(e)});"""
 
 
-def prev_day(date_string: str) -> str:
+def get_date_ninety_days_prior(date_string: str) -> str:
     """
-    Calculate the date 90 days before the given date.
+    Get the date 90 days prior to the given date.
 
     Args:
         date_string (str): The date string in the format "%Y-%m-%d %H:%M:%S.%f".
 
     Returns:
-        str: The date string 90 days before the given date.
+        str: The date string 90 days prior to the given date.
     """
+    DAYS_PRIOR = 90
     date_obj = dt.datetime.strptime(date_string, Constants.date_format)
-    prev_day_obj = date_obj - dt.timedelta(days=90)
+    prev_day_obj = date_obj - dt.timedelta(days=DAYS_PRIOR)
     prev_day_string = prev_day_obj.strftime(Constants.date_format)
-
     return prev_day_string
 
 
 class MidjourneyAPI:
     """
     A class to interact with the Midjourney API.
 
@@ -84,69 +84,85 @@
     def log_in(self) -> bool:
         """
         Log in to the Midjourney API.
 
         Returns:
             bool: True if login is successful, False otherwise.
         """
+
+    def load_cookies(self):
         self.cookies_path = Path(self.archive_folder, Constants.cookies_pkl)
         if self.cookies_path.is_file():
             cookies = pickle.load(open(self.cookies_path, "rb"))
             for cookie in cookies:
                 try:
                     self.driver.add_cookie(cookie)
                 except InvalidCookieDomainException:
                     pass
+
+    def save_cookies(self):
+        pickle.dump(self.driver.get_cookies(), open(self.cookies_path, "wb"))
+
+    def log_in(self) -> bool:
+        """
+        Log in to the Midjourney API.
+
+        Returns:
+            bool: True if login is successful, False otherwise.
+        """
+        self.load_cookies()
         try:
             self.driver.get(Constants.home_url)
             WebDriverWait(self.driver, 60 * 10).until(EC.url_to_be(Constants.app_url))
             WebDriverWait(self.driver, 60 * 10).until(
                 EC.presence_of_element_located((By.ID, Constants.app_element_id))
             )
             cookie = self.driver.get_cookie(Constants.session_token_cookie)
             if cookie is not None:
-                pickle.dump(self.driver.get_cookies(), open(self.cookies_path, "wb"))
+                self.save_cookies()
                 self.session_token = cookie["value"]
                 return True
             else:
                 return False
         except Exception as e:
             _log.error(f"Failed to get session token: {str(e)}")
             return False
 
-    def get_user_info(self) -> bool:
-        """
-        Get the user information from the Midjourney API.
-
-        Returns:
-            bool: True if the user information is successfully retrieved, False otherwise.
-        """
+    def load_user_info(self):
         self.user_info = {}
         self.user_json = Path(self.archive_folder, Constants.user_json)
         if self.user_json.is_file():
             self.user_info = json.loads(self.user_json.read_text())
         else:
-            try:
-                self.driver.get(Constants.account_url)
-                WebDriverWait(self.driver, 60 * 10).until(
-                    EC.presence_of_element_located(
-                        (By.ID, Constants.account_element_id)
-                    )
-                )
-                soup = BeautifulSoup(self.driver.page_source, "html.parser")
-                script_tag_contents = soup.find(
-                    "script", id=Constants.account_element_id
-                ).text
-                self.user_info = json.loads(script_tag_contents)
+            self.user_info = self.fetch_user_info()
+            if self.user_info:
                 self.user_json.write_text(json.dumps(self.user_info))
-            except Exception as e:
-                _log.error(f"Failed to get user info: {str(e)}")
-                return False
-        self.user_id = self.user_info["props"]["pageProps"]["user"]["id"]
-        return True
+
+    def fetch_user_info(self):
+        try:
+            self.driver.get(Constants.account_url)
+            WebDriverWait(self.driver, 60 * 10).until(
+                EC.presence_of_element_located((By.ID, Constants.account_element_id))
+            )
+            soup = BeautifulSoup(self.driver.page_source, "html.parser")
+            script_tag_contents = soup.find(
+                "script", id=Constants.account_element_id
+            ).text
+            return json.loads(script_tag_contents)
+        except Exception as e:
+            _log.error(f"Failed to get user info: {str(e)}")
+            return None
+
+    def get_user_info(self) -> bool:
+        self.load_user_info()
+        if self.user_info:
+            self.user_id = self.user_info["props"]["pageProps"]["user"]["id"]
+            return True
+        else:
+            return False
 
     def request_recent_jobs(
         self,
         from_date: str | None = None,
         page: int | None = None,
         job_type: str | None = None,
         amount: int = 50,
```

### Comparing `dimjournal-1.0.6/src/dimjournal.egg-info/PKG-INFO` & `dimjournal-1.0.7/src/dimjournal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimjournal
-Version: 1.0.6
+Version: 1.0.7
 Summary: Archive utility for Midjourney
 Home-page: https://pypi.org/project/dimjournal/
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: Apache-2.0
 Project-URL: Documentation, https://twardoch.github.io/dimjournal/
 Project-URL: Source, https://github.com/twardoch/dimjournal
```

### Comparing `dimjournal-1.0.6/src/dimjournal.egg-info/SOURCES.txt` & `dimjournal-1.0.7/src/dimjournal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dimjournal-1.0.6/tox.ini` & `dimjournal-1.0.7/tox.ini`

 * *Files identical despite different names*

