# Comparing `tmp/smdb_web_interface-0.1.0.tar.gz` & `tmp/smdb_web_interface-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smdb_web_interface-0.1.0.tar", last modified: Tue Jul  4 09:21:20 2023, max compression
+gzip compressed data, was "smdb_web_interface-0.1.1.tar", last modified: Wed Jul  5 08:47:32 2023, max compression
```

## Comparing `smdb_web_interface-0.1.0.tar` & `smdb_web_interface-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 09:21:20.570308 smdb_web_interface-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-06-18 19:13:59.000000 smdb_web_interface-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2423 2023-07-04 09:21:20.570308 smdb_web_interface-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1850 2023-07-04 06:34:38.000000 smdb_web_interface-0.1.0/README.md
--rw-rw-rw-   0        0        0      128 2023-07-04 05:55:03.000000 smdb_web_interface-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      635 2023-07-04 09:21:20.571833 smdb_web_interface-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 09:21:20.547419 smdb_web_interface-0.1.0/smdb_web_interface/
--rw-rw-rw-   0        0        0     2169 2023-07-04 06:21:50.000000 smdb_web_interface-0.1.0/smdb_web_interface/__init__.py
--rw-rw-rw-   0        0        0     1036 2023-06-29 06:24:03.000000 smdb_web_interface-0.1.0/smdb_web_interface/helpers.py
--rw-rw-rw-   0        0        0     8333 2023-07-04 09:00:28.000000 smdb_web_interface-0.1.0/smdb_web_interface/server.py
--rw-rw-rw-   0        0        0   405942 2023-07-04 08:59:53.000000 smdb_web_interface-0.1.0/smdb_web_interface/static.py
--rw-rw-rw-   0        0        0      875 2023-07-04 08:03:00.000000 smdb_web_interface-0.1.0/smdb_web_interface/templates.py
-drwxrwxrwx   0        0        0        0 2023-07-04 09:21:20.563173 smdb_web_interface-0.1.0/smdb_web_interface.egg-info/
--rw-rw-rw-   0        0        0     2423 2023-07-04 09:21:20.000000 smdb_web_interface-0.1.0/smdb_web_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-07-04 09:21:20.000000 smdb_web_interface-0.1.0/smdb_web_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 09:21:20.000000 smdb_web_interface-0.1.0/smdb_web_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-04 09:21:20.000000 smdb_web_interface-0.1.0/smdb_web_interface.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-04 09:21:20.569285 smdb_web_interface-0.1.0/tests/
--rw-rw-rw-   0        0        0     1305 2023-07-04 09:21:17.000000 smdb_web_interface-0.1.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:47:32.039703 smdb_web_interface-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-06-18 19:13:59.000000 smdb_web_interface-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2423 2023-07-05 08:47:32.039703 smdb_web_interface-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1850 2023-07-04 06:34:38.000000 smdb_web_interface-0.1.1/README.md
+-rw-rw-rw-   0        0        0      128 2023-07-04 05:55:03.000000 smdb_web_interface-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      635 2023-07-05 08:47:32.041232 smdb_web_interface-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-05 08:47:32.022351 smdb_web_interface-0.1.1/smdb_web_interface/
+-rw-rw-rw-   0        0        0     2267 2023-07-05 08:34:54.000000 smdb_web_interface-0.1.1/smdb_web_interface/__init__.py
+-rw-rw-rw-   0        0        0     1036 2023-06-29 06:24:03.000000 smdb_web_interface-0.1.1/smdb_web_interface/helpers.py
+-rw-rw-rw-   0        0        0     8333 2023-07-04 09:00:28.000000 smdb_web_interface-0.1.1/smdb_web_interface/server.py
+-rw-rw-rw-   0        0        0   406025 2023-07-05 08:37:40.000000 smdb_web_interface-0.1.1/smdb_web_interface/static.py
+-rw-rw-rw-   0        0        0      875 2023-07-04 08:03:00.000000 smdb_web_interface-0.1.1/smdb_web_interface/templates.py
+drwxrwxrwx   0        0        0        0 2023-07-05 08:47:32.038183 smdb_web_interface-0.1.1/smdb_web_interface.egg-info/
+-rw-rw-rw-   0        0        0     2423 2023-07-05 08:47:31.000000 smdb_web_interface-0.1.1/smdb_web_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-07-05 08:47:32.000000 smdb_web_interface-0.1.1/smdb_web_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-05 08:47:31.000000 smdb_web_interface-0.1.1/smdb_web_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-05 08:47:31.000000 smdb_web_interface-0.1.1/smdb_web_interface.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-05 08:47:32.039195 smdb_web_interface-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1343 2023-07-05 08:40:01.000000 smdb_web_interface-0.1.1/tests/test.py
```

### Comparing `smdb_web_interface-0.1.0/LICENSE` & `smdb_web_interface-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smdb_web_interface-0.1.0/PKG-INFO` & `smdb_web_interface-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb_web_interface
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to use Web interface for python application.
 Home-page: https://github.com/NightKey/web-cli
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/web-cli/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_web_interface-0.1.0/README.md` & `smdb_web_interface-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `smdb_web_interface-0.1.0/setup.cfg` & `smdb_web_interface-0.1.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6d64 625f 7765 625f 696e 7465   = smdb_web_inte
 00000020: 7266 6163 650d 0a76 6572 7369 6f6e 203d  rface..version =
-00000030: 2030 2e31 2e30 0d0a 6175 7468 6f72 203d   0.1.0..author =
+00000030: 2030 2e31 2e31 0d0a 6175 7468 6f72 203d   0.1.1..author =
 00000040: 204a 616e 7468 c3b3 2044 c3a1 7669 640d   Janth.. D..vid.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6461 7669 646a 616e 7468 6f40 676d 6169  davidjantho@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2041 6e20 6561 7379 2074 6f20  on = An easy to 
 00000090: 7573 6520 5765 6220 696e 7465 7266 6163  use Web interfac
 000000a0: 6520 666f 7220 7079 7468 6f6e 2061 7070  e for python app
```

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface/__init__.py` & `smdb_web_interface-0.1.1/smdb_web_interface/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
     def __get_history(self, args: Dict[str, str]):
         index = int(args["index"])
         return list(self.history.keys())[index].command
 
     def push_data(self, response: Union[str, List[str]], command: Optional[UserCommand] = None) -> None:
         if (command is None):
+            if len(self.history.keys()) < 1:
+                self.history[UserCommand("")] = []
             command = list(self.history.keys())[-1]
         if (isinstance(response, str)):
             self.history[command].append(response)
         else:
             self.history[command].extend(response)
 
     def __send(self, data: bytes):
```

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface/helpers.py` & `smdb_web_interface-0.1.1/smdb_web_interface/helpers.py`

 * *Files identical despite different names*

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface/server.py` & `smdb_web_interface-0.1.1/smdb_web_interface/server.py`

 * *Files identical despite different names*

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface/static.py` & `smdb_web_interface-0.1.1/smdb_web_interface/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,18 @@
                 if (content.find('#FIX_input')[0] !== undefined) {
                     userValue = content.find('#FIX_input')[0].value;
                 }
                 let blocks = "";
                 console.log(data);
                 for (let index in data) {
                     let block = data[index];
-                    blocks += "<div id=\"" + block["hash"] + "\">\n";
-                    blocks += "<div class=\"user\">" + consolName + "> <input type=\"text\" id=\"" + block["hash"] + "_input\" value=\"" + block["command"] + "\" readonly></div>";
+                    if (block["command"] === "") {
+                        blocks += "<div id=\"" + block["hash"] + "\">\n";
+                        blocks += "<div class=\"user\">" + consolName + "> <input type=\"text\" id=\"" + block["hash"] + "_input\" value=\"" + block["command"] + "\" readonly></div>";
+                    }
                     blocks += "<div class=\"response\">";
                     for (let index in block["response"]) {
                         let line = block["response"][index];
                         blocks += "<div>" + line + "</div>";
                     }
                     blocks += "</div></div>\n";
                 }
```

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface/templates.py` & `smdb_web_interface-0.1.1/smdb_web_interface/templates.py`

 * *Files identical despite different names*

### Comparing `smdb_web_interface-0.1.0/smdb_web_interface.egg-info/PKG-INFO` & `smdb_web_interface-0.1.1/smdb_web_interface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smdb-web-interface
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy to use Web interface for python application.
 Home-page: https://github.com/NightKey/web-cli
 Author: Janthó Dávid
 Author-email: davidjantho@gmail.com
 Project-URL: Bug Tracker, https://github.com/NightKey/web-cli/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smdb_web_interface-0.1.0/tests/test.py` & `smdb_web_interface-0.1.1/tests/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         self.cli.start()
 
     def stop_cli(self):
         self.cli.stop()
 
     def logger(self):
         sleep(30)
-        self.cli.push_data(None, [
-            "Multi line command\nTesting line formatting", "And is a list"])
+        self.cli.push_data(["Multi line command\nTesting line formatting", "And is a list"])
 
     def mock_backend(self, input: UserCommand) -> None:
         if (input.command == "start"):
             threading.Thread(target=self.logger).start()
         sleep(1)
         self.cli.push_data("Answer 1", input)
         sleep(1)
@@ -39,9 +38,11 @@
         sleep(1)
         self.cli.push_data("Answer 3", input)
 
 
 if __name__ == "__main__":
     mock = MockClass()
     mock.start_cli()
-    input("Server running")
+    print("Server started")
+    mock.logger()    
+    input("press return to exit")
     mock.stop_cli()
```

