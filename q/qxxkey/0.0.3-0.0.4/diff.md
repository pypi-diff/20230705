# Comparing `tmp/qxxkey-0.0.3.tar.gz` & `tmp/qxxkey-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qxxkey-0.0.3.tar", max compression
+gzip compressed data, was "qxxkey-0.0.4.tar", max compression
```

## Comparing `qxxkey-0.0.3.tar` & `qxxkey-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0      249 2023-07-03 09:44:15.848388 qxxkey-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       24 2023-07-03 09:18:09.435120 qxxkey-0.0.3/qxxkey/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-03 09:43:49.124341 qxxkey-0.0.3/qxxkey/vault.py
--rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.3/README.md
--rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-07-05 05:04:56.649692 qxxkey-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-07-04 01:34:31.441629 qxxkey-0.0.4/qxxkey/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-04 04:05:12.830382 qxxkey-0.0.4/qxxkey/auth.py
+-rw-r--r--   0        0        0     1348 2023-07-04 04:01:29.825277 qxxkey-0.0.4/qxxkey/remote/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-04 02:13:03.180323 qxxkey-0.0.4/qxxkey/remote/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-07-05 05:02:36.409679 qxxkey-0.0.4/qxxkey/vault.py
+-rw-r--r--   0        0        0        0 2023-07-03 08:39:08.911479 qxxkey-0.0.4/README.md
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 qxxkey-0.0.4/PKG-INFO
```

### Comparing `qxxkey-0.0.3/qxxkey/vault.py` & `qxxkey-0.0.4/qxxkey/vault.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,20 +36,26 @@
     def save(self):
         import json
 
         with open(self.vault_path, "w") as f:
             json.dump(self.vault, f)
 
     def get(self, key):
-        return self.vault[key]
+        try:
+            return self.vault[key]
+        except KeyError:
+            return None
     
     def set(self, key, value):
         self.vault[key] = value
         self.save()
     
     def delete(self, key):
-        del self.vault[key]
-        self.save()
+        try:
+            del self.vault[key]
+            self.save()
+        except KeyError:
+            pass
 
     def list(self):
         return self.vault.keys()
```

