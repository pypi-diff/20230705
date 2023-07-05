# Comparing `tmp/fh_fablib-1.0.20230630.tar.gz` & `tmp/fh_fablib-1.0.20230705.tar.gz`

## Comparing `fh_fablib-1.0.20230630.tar` & `fh_fablib-1.0.20230705.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.editorconfig
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.pre-commit-config.yaml
--rw-r--r--   0        0        0    19912 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/CHANGELOG.rst
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/bumpversion.sh
--rw-r--r--   0        0        0    26697 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/__init__.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/extract_js_gettext_strings.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.editorconfig
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.eslintrc.js
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/pyproject.toml
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/fh_fablib/dotfiles/webpack.library.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/LICENSE
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/README.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/pyproject.toml
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230630/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.editorconfig
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20073 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/CHANGELOG.rst
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/bumpversion.sh
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0    26750 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/__init__.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/extract_js_gettext_strings.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.editorconfig
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.eslintrc.js
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/pyproject.toml
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/fh_fablib/dotfiles/webpack.library.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/LICENSE
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/README.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/pyproject.toml
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 fh_fablib-1.0.20230705/PKG-INFO
```

### Comparing `fh_fablib-1.0.20230630/.pre-commit-config.yaml` & `fh_fablib-1.0.20230705/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.274"
+    rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `fh_fablib-1.0.20230630/CHANGELOG.rst` & `fh_fablib-1.0.20230705/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 ==========
 Change log
 ==========
 
 Next version
 ~~~~~~~~~~~~
 
+1.0.20230705
+~~~~~~~~~~~~
+
+- Removed the unused ``config.app``.
+- Exposed all configuration values as ``FL_*`` environment values, for example
+  ``FL_DOMAIN``.
+
 1.0.20230630
 ~~~~~~~~~~~~
 
 - Fixed the ``find`` command which deletes old ``static`` files.
 - Updated the example Webpack configuration to work with the newest version of
   ``postcss-custom-media``.
```

### Comparing `fh_fablib-1.0.20230630/fh_fablib/__init__.py` & `fh_fablib-1.0.20230705/fh_fablib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fabric import Connection, task
 from invoke import Collection  # noqa, re-export
 from speckenv_django import django_database_url
 
 from fh_fablib.extract_js_gettext_strings import generate_strings
 
 
-__version__ = "1.0.20230630"
+__version__ = "1.0.20230705"
 
 
 # I don't care, in this context.
 warnings.simplefilter("ignore", category=ResourceWarning)
 
 
 def ansi(code):
@@ -112,37 +112,38 @@
     kw.setdefault("replace_env", False)
     if not kw.get("hide"):
         progress(" ".join(str(part) for part in a))
     return c.run(*a, **kw)
 
 
 class Config:
-    app = "app"
-    base = _find_base()
-    environment = "default"
-    environments = {}
-    force = False
-
     def update(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
+            os.environ[f"FL_{key.upper()}"] = str(value)
 
     def __getattr__(self, key):
         environments = getattr(self, "environments", None)
         if environments:
             environments = f" [{', '.join(environments)}]"
         terminate(
             f"Configuration key '{key}' not set. "
             f"Maybe you forgot to set an environment with which to interact?"
             f"{environments}"
         )
 
 
 #: Defaults
 config = Config()
+config.update(
+    base=_find_base(),
+    environment="default",
+    environments={},
+    force=False,
+)
 os.chdir(config.base)
 
 
 def environment(name, cfg, **kwargs):
     config.environments[name] = cfg
 
     if name in kwargs.get("aliases", ()):
```

### Comparing `fh_fablib-1.0.20230630/fh_fablib/extract_js_gettext_strings.py` & `fh_fablib-1.0.20230705/fh_fablib/extract_js_gettext_strings.py`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230630/fh_fablib/dotfiles/.pre-commit-config.yaml` & `fh_fablib-1.0.20230705/fh_fablib/dotfiles/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,23 @@
       - id: django-upgrade
         args: [--target-version, "4.0"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.274"
+    rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.43.0
+    rev: v8.44.0
     hooks:
       - id: eslint
         args: [--fix]
         types_or: [css, scss, javascript]
         verbose: true
         additional_dependencies:
           - eslint
@@ -66,14 +66,14 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.9-for-vscode
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$|.*\\.json$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.12.1
+    rev: 0.13.0
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
     rev: v0.13
     hooks:
       - id: validate-pyproject
```

### Comparing `fh_fablib-1.0.20230630/fh_fablib/dotfiles/pyproject.toml` & `fh_fablib-1.0.20230705/fh_fablib/dotfiles/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230630/fh_fablib/dotfiles/webpack.library.js` & `fh_fablib-1.0.20230705/fh_fablib/dotfiles/webpack.library.js`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230630/LICENSE` & `fh_fablib-1.0.20230705/LICENSE`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230630/README.rst` & `fh_fablib-1.0.20230705/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230630")
+       fl.require("1.0.20230705")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -90,15 +90,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230630")
+    fl.require("1.0.20230705")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

### Comparing `fh_fablib-1.0.20230630/pyproject.toml` & `fh_fablib-1.0.20230705/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fh_fablib-1.0.20230630/PKG-INFO` & `fh_fablib-1.0.20230705/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fh-fablib
-Version: 1.0.20230630
+Version: 1.0.20230705
 Summary: fh-fablib
 Project-URL: Homepage, https://github.com/feinheit/fh-fablib/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.9
@@ -28,15 +28,15 @@
 
 3. Add a ``fabfile.py`` to your project. A minimal example follows:
 
    .. code-block:: python
 
        import fh_fablib as fl
 
-       fl.require("1.0.20230630")
+       fl.require("1.0.20230705")
        fl.config.update(host="www-data@feinheit06.nine.ch")
 
        environments = [
            fl.environment(
                "production",
                {
                    "domain": "example.com",
@@ -104,15 +104,15 @@
 
 If you need multiple environments, add environment tasks as follows:
 
 .. code-block:: python
 
     import fh_fablib as fl
 
-    fl.require("1.0.20230630")
+    fl.require("1.0.20230705")
     fl.config.update(host="www-data@feinheit06.nine.ch")
 
     environments = [
         fl.environment(
             "production",
             {
                 "domain": "example.com",
```

