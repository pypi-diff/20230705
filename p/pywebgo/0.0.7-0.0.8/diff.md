# Comparing `tmp/pywebgo-0.0.7.tar.gz` & `tmp/pywebgo-0.0.8.tar.gz`

## Comparing `pywebgo-0.0.7.tar` & `pywebgo-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/__init__.py
--rw-r--r--   0        0        0    15042 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/controller.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/data.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/elements.py
--rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.7/src/pywebgo/utils.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.7/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.7/LICENSE
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.7/README.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pywebgo-0.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/__init__.py
+-rw-r--r--   0        0        0    15060 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/controller.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/data.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/elements.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 pywebgo-0.0.8/src/pywebgo/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pywebgo-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 pywebgo-0.0.8/LICENSE
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pywebgo-0.0.8/README.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pywebgo-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pywebgo-0.0.8/PKG-INFO
```

### Comparing `pywebgo-0.0.7/.github/workflows/python-publish.yml` & `pywebgo-0.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/src/pywebgo/controller.py` & `pywebgo-0.0.8/src/pywebgo/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             index = self.elem_handler.elements.index(element)
             # Switch window if the element is located in a different window
             self.switch_window(element)
             # Call the custom function if it exists
             if callable(element['custom']):
                 element['custom'](self, element)
                 continue
-            web_element = self.get_element(element, timeout)
+            web_element = self.get_element(element, self.retry_attempts, timeout)
             self.elem_handler.store_web_element(web_element)
             self.retrieve_data(web_element, element)
             self.execute_actions(web_element, element)
             self.load_next_page(index)
             # Handle alert if appears after any action
             self.handle_alert(element, web_element)
 
@@ -150,41 +150,41 @@
         :param timeout: time before throwing exception if the element is not found
         :return: active web element
         """
         active_element = self.switch_to.active_element
         self.wait_for_element_visibility(active_element, timeout)
         return active_element
 
-    def get_element(self, element: dict, timeout: float) -> WebElement:
+    def get_element(self, element: dict, retry: int, timeout: float) -> WebElement:
         """
         Get the WebElement from the given element dict using the 'loc' and 'value' keys
 
-        :param timeout: time before throwing exception if the element is not found
         :param element: a dictionary containing WebElement specifications
+        :param retry: the number of retry attempts to get an element
+        :param timeout: time before throwing exception if the element is not found
         :return: a WebElement corresponding to the given element dict
         """
 
         # If locator is active, get the active element
         if element['loc'] == 'active':
             return self.get_active_element(timeout)
 
         # Get element identifiers
         identifiers = utils.get_element_identifiers(element)
         strategy, locator, index = identifiers.values()
-        retry_count = 0
-        while retry_count <= self.retry_attempts:
+
+        for i in range(retry + 1):
             try:
                 self.wait_for_element_load(element, timeout)
                 if index:
                     return self.find_elements(strategy, locator)[int(index)]
                 return self.find_element(strategy, locator)
             except NoSuchElementException:
-                retry_count += 1
                 time.sleep(1)  # Wait for a second before retrying
-        raise NoSuchElementException(f"Element not found after {self.retry_attempts} attempts.")
+        raise NoSuchElementException(f"Element not found after {retry} attempts.")
 
     def get_page_html(self, url: str = None) -> str:
         """
         Retrieve and return the HTML of the current page or from a given url.
 
         :param url: URL of a web page
         :return: requested HTML of a web page
@@ -343,30 +343,28 @@
         if isinstance(element, WebElement):
             wait.until(expected_conditions.visibility_of(element))
         else:
             identifiers = utils.get_element_identifiers(element)
             (strategy, locator) = (identifiers['strategy'], identifiers['locator'])
             wait.until(expected_conditions.visibility_of_element_located((strategy, locator)))
 
-    def element_exists(self, element, wait=0) -> bool:
+    def element_exists(self, element, retry=0, timeout=0) -> bool:
         """
         Check if an element exists.
 
         :param element: dictionary containing element specifications
-        :param wait:
-        :return:
+        :param retry: the number of retry attempts to find an element
+        :param timeout: wait time before throwing an exception
+        :return: bool flag to assert the existence of an element
         """
         try:
-            identifiers = utils.get_element_identifiers(element)
-            (strategy, locator) = (identifiers['strategy'], identifiers['locator'])
-            time.sleep(wait)
-            self.find_element(strategy, locator)
+            self.get_element(element, retry, timeout)
+            return True
         except NoSuchElementException:
             return False
-        return True
 
     def run_controller(self, elements: list, timeout: float = 20) -> None:
         """
         Runs the controller to initiate the execution of the operations.
 
         :param timeout:
         :param elements: elements to interact with
```

### Comparing `pywebgo-0.0.7/src/pywebgo/data.py` & `pywebgo-0.0.8/src/pywebgo/data.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/src/pywebgo/elements.py` & `pywebgo-0.0.8/src/pywebgo/elements.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/src/pywebgo/utils.py` & `pywebgo-0.0.8/src/pywebgo/utils.py`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/.gitignore` & `pywebgo-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/LICENSE` & `pywebgo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebgo-0.0.7/pyproject.toml` & `pywebgo-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pywebgo"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Adil Zafar Khan", email="adilzafar66@gmail.com" },
 ]
 description = "A selenium client that automates web surfing with simple commands."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pywebgo-0.0.7/PKG-INFO` & `pywebgo-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebgo
-Version: 0.0.7
+Version: 0.0.8
 Summary: A selenium client that automates web surfing with simple commands.
 Project-URL: Homepage, https://github.com/adilzafar66/pywebgo
 Project-URL: Bug Tracker, https://github.com/adilzafar66/pywebgo/issues
 Author-email: Adil Zafar Khan <adilzafar66@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

