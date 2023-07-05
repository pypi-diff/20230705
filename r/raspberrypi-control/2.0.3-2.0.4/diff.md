# Comparing `tmp/raspberrypi_control-2.0.3.tar.gz` & `tmp/raspberrypi_control-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspberrypi_control-2.0.3.tar", last modified: Tue Jul  4 22:59:25 2023, max compression
+gzip compressed data, was "raspberrypi_control-2.0.4.tar", last modified: Wed Jul  5 18:08:00 2023, max compression
```

## Comparing `raspberrypi_control-2.0.3.tar` & `raspberrypi_control-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/raspberrypi_control/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/raspberrypi_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58549 2023-07-04 22:59:15.000000 raspberrypi_control-2.0.3/raspberrypi_control/raspberrypi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-04 22:59:25.000000 raspberrypi_control-2.0.3/raspberrypi_control.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 22:59:25.394819 raspberrypi_control-2.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:00.276537 raspberrypi_control-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-05 18:07:48.000000 raspberrypi_control-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-05 18:08:00.276537 raspberrypi_control-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-05 18:07:48.000000 raspberrypi_control-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 18:07:48.000000 raspberrypi_control-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:00.276537 raspberrypi_control-2.0.4/raspberrypi_control/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 18:07:48.000000 raspberrypi_control-2.0.4/raspberrypi_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58760 2023-07-05 18:07:48.000000 raspberrypi_control-2.0.4/raspberrypi_control/raspberrypi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 18:08:00.276537 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-05 18:08:00.000000 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-05 18:08:00.000000 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 18:08:00.000000 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 18:08:00.000000 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-05 18:08:00.000000 raspberrypi_control-2.0.4/raspberrypi_control.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 18:08:00.276537 raspberrypi_control-2.0.4/setup.cfg
```

### Comparing `raspberrypi_control-2.0.3/LICENSE` & `raspberrypi_control-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raspberrypi_control-2.0.3/PKG-INFO` & `raspberrypi_control-2.0.4/raspberrypi_control.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raspberrypi_control
-Version: 2.0.3
+Name: raspberrypi-control
+Version: 2.0.4
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -51,17 +51,19 @@
             if th == 30:  
                 time.sleep(0.1)  
                 break  
         return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
+        rp.raspberrypi().set_raspberry_info("username here", "password here") # set login info here
         rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
         rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
         rp.config("main") # file name if this file (no .py)  
+        rp.run_command("Hello World",True) # true is for if console ouput is print or no
         print(test())  
         print(other()) # you can get the output after
 
 ## How to install the package
 Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

### Comparing `raspberrypi_control-2.0.3/README.md` & `raspberrypi_control-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,19 @@
             if th == 30:  
                 time.sleep(0.1)  
                 break  
         return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
+        rp.raspberrypi().set_raspberry_info("username here", "password here") # set login info here
         rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
         rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
         rp.config("main") # file name if this file (no .py)  
+        rp.run_command("Hello World",True) # true is for if console ouput is print or no
         print(test())  
         print(other()) # you can get the output after
 
 ## How to install the package
 Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

### Comparing `raspberrypi_control-2.0.3/pyproject.toml` & `raspberrypi_control-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raspberrypi_control"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Geoloup Team", email="franckiebbb@gmail.com"},
 ]
 description = "Control Raspberrypi board with ssh and python"
 readme = "README.md"
 dependencies = [
     "requests",
```

### Comparing `raspberrypi_control-2.0.3/raspberrypi_control/raspberrypi.py` & `raspberrypi_control-2.0.4/raspberrypi_control/raspberrypi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1162,19 +1162,17 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
             try:
                 global raspberrypi_prep
                 global raspberrypi_info
                 global imported
                 global function_to_add
-                HOST_IP = raspberrypi().local(raspberrypi_prep)
-                SSH_PWD = raspberrypi_info[0]
                 ssh_controller = ssh.SSHController(
-                    host=HOST_IP,
-                    user="geoloup",
+                    host=raspberrypi().local(raspberrypi_prep),
+                    user=raspberrypi_info[0],
                     ssh_password=raspberrypi_info[1]
                 )
                 ssh_controller.connect()
                 import inspect
                 func_content = inspect.getsource(func)
                 func_content = func_content.splitlines(True)
                 func_contentl = list()
@@ -1257,16 +1255,17 @@
                 ssh_controller.remove(file_name)
                 # send the return value
                 re = "raspberrypi_code.raspberrypi.package.python.glt.org.py return "
                 if output[-1].find(re) != -1:
                     return output[-1].replace(re, "")
                 else:
                     return None
+                ssh_controller.disconnect()
             except Exception as f:  # if raspberrypi not find it's will be run in local on the computer
-                print("raspberrypi was not find or a erro have appedned. The error is : " + str(f))
+                print("raspberrypi was not find or a error have appened. The error is : " + str(f))
                 return func(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 def raspberry_command_add():
@@ -1409,15 +1408,16 @@
         raspberrypi_prep = start
         raspberrypi_prep_max = max_loop
         raspberrypi_prep_timeout = timeout_time
 
     def local(self, start_ip):
         global raspberrypi_ip
         global raspberrypi_prep_max
-        if raspberrypi_ip == 0:
+        global raspberrypi_prep
+        if raspberrypi_ip == 0 and raspberrypi_prep == start_ip:
             gh = 0
             gj = []
             while True:
                 gj.append(start_ip + str(gh))
                 gh = gh + 1
                 if gh == int(raspberrypi_prep_max):
                     break
@@ -1425,16 +1425,19 @@
                 hoip = host
                 if raspberrypi().check(hoip):
                     raspberrypi_ip = hoip
                     break
                 else:
                     continue
         res = raspberrypi_ip
-        return res
-    
+        if res != 0:
+            return res
+        else:
+            quit("password or username are not good or raspberry is on the internet")
+
     def set_raspberry_info(self,user_name,password):
         global raspberrypi_info
         raspberrypi_info = list()
         raspberrypi_info.append(user_name)
         raspberrypi_info.append(password)
 
 def run_command(command=None,display=False):
@@ -1451,14 +1454,15 @@
         try:
             ssh_controller.connect()
             exit_code, output = ssh_controller.run(
                 command=command,
                 display=display,
                 capture=True
             )
+            ssh_controller.disconnect()
             return output[-1]
-        except:
+        except Exception:
             import os
             return  os.system(command)
     else:
         quit("You need to have a command... At run_command")
-        return None
+        return None
```

### Comparing `raspberrypi_control-2.0.3/raspberrypi_control.egg-info/PKG-INFO` & `raspberrypi_control-2.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: raspberrypi-control
-Version: 2.0.3
+Name: raspberrypi_control
+Version: 2.0.4
 Summary: Control Raspberrypi board with ssh and python
 Author-email: Geoloup Team <franckiebbb@gmail.com>
 Project-URL: Homepage, https://github.com/Geoloup/raspberry_control/
 Project-URL: Bug Tracker, https://github.com/Geoloup/raspberry_control/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -51,17 +51,19 @@
             if th == 30:  
                 time.sleep(0.1)  
                 break  
         return th  
       
       
     if __name__ == "__main__": # put all you're code to run at start here. Because if not the code will be run 2 time  
+        rp.raspberrypi().set_raspberry_info("username here", "password here") # set login info here
         rp.raspberrypi().set_preparation("192.168.0.10", 8, 1) # config locator for the raspberrypi  
         rp.raspberrypi().local("192.168.0.10") # set the start ip set in the line in the top  
         rp.config("main") # file name if this file (no .py)  
+        rp.run_command("Hello World",True) # true is for if console ouput is print or no
         print(test())  
         print(other()) # you can get the output after
 
 ## How to install the package
 Do `pip install raspberry-control`
 Supported for python 3.10 and higher*
 *note not tested for lower version
```

