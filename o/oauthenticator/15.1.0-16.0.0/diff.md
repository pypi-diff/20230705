# Comparing `tmp/oauthenticator-15.1.0.tar.gz` & `tmp/oauthenticator-16.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthenticator-15.1.0.tar", last modified: Thu Sep  8 08:54:57 2022, max compression
+gzip compressed data, was "oauthenticator-16.0.0.tar", last modified: Wed Jul  5 09:29:59 2023, max compression
```

## Comparing `oauthenticator-15.1.0.tar` & `oauthenticator-16.0.0.tar`

### file list

```diff
@@ -1,58 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3728 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:57.237628 oauthenticator-15.1.0/oauthenticator/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4835 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/auth0.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/awscognito.py
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/azuread.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/azureadb2c.py
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (121)    14903 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/cilogon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1432 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     7649 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)    13330 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/github.py
--rw-r--r--   0 runner    (1001) docker     (121)     8985 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (121)    13730 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/globus.py
--rw-r--r--   0 runner    (1001) docker     (121)    11656 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/google.py
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (121)    15847 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/okpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5319 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/openshift.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/oauthenticator/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)      940 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/schemas/cilogon-schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/oauthenticator/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8869 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_auth0.py
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_azuread.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_bitbucket.py
--rw-r--r--   0 runner    (1001) docker     (121)    13157 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_cilogon.py
--rw-r--r--   0 runner    (1001) docker     (121)     6373 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (121)     7619 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (121)     9677 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (121)    16372 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_google.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_mediawiki.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_okpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3750 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/tests/test_openshift.py
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/traitlets.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/oauthenticator/yandex.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/oauthenticator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-09-08 08:54:57.000000 oauthenticator-15.1.0/oauthenticator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-08 08:54:57.241628 oauthenticator-15.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4336 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-09-08 08:54:45.000000 oauthenticator-15.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.980432 oauthenticator-16.0.0/oauthenticator/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10979 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36900 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/schemas/cilogon-schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_auth0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_bitbucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14935 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_cilogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_mediawiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_okpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/oauthenticator/tests/test_openshift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/oauthenticator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-05 09:29:59.000000 oauthenticator-16.0.0/oauthenticator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 09:29:59.984432 oauthenticator-16.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-05 09:29:47.000000 oauthenticator-16.0.0/setup.py
```

### Comparing `oauthenticator-15.1.0/CONTRIBUTING.md` & `oauthenticator-16.0.0/CONTRIBUTING.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,30 +11,25 @@
    git clone https://github.com/jupyterhub/oauthenticator
    ```
 
 2. Do a development install with pip:
 
    ```
    cd oauthenticator
-   pip install -e .
+   pip install -e ".[test]"
    ```
 
-3. Install test dependencies
+3. Install pre-commit hooks that checks formatting before commits are made.
 
    ```
-   pip install -r test-requirements.txt
+   pip install pre-commit
+   pre-commit install --install-hooks
    ```
 
-4. Install pre-commit hooks that checks formatting before commits are made.
-
-   ```
-   pre-commit install
-   ```
-
-5. Run tests
+4. Run tests
 
    ```
    pytest
    ```
 
 Note: OAuthenticator _is not_ accepting pull requests adding new OAuth providers.
 See the documentation for how to use GenericOAuthenticator with your provider
```

### Comparing `oauthenticator-15.1.0/LICENSE` & `oauthenticator-16.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oauthenticator-15.1.0/PKG-INFO` & `oauthenticator-16.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 15.1.0
+Version: 16.0.0
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
 Platform: Mac OS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: azuread
 Provides-Extra: googlegroups
+Provides-Extra: mediawiki
+Provides-Extra: test
 License-File: LICENSE
 
 # OAuth + JupyterHub Authenticator = OAuthenticator :heart:
 
 [![Documentation build status](https://img.shields.io/readthedocs/oauthenticator?logo=read-the-docs)](https://oauthenticator.readthedocs.org/en/latest)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jupyterhub/oauthenticator/Tests?logo=github)](https://github.com/jupyterhub/oauthenticator/actions)
+[![GitHub Workflow Status - Test](https://img.shields.io/github/actions/workflow/status/jupyterhub/oauthenticator/test.yml?logo=github&label=tests)](https://github.com/jupyterhub/oauthenticator/actions)
 [![Latest PyPI version](https://img.shields.io/pypi/v/oauthenticator?logo=pypi)](https://pypi.python.org/pypi/oauthenticator)
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/oauthenticator?logo=conda-forge)](https://anaconda.org/conda-forge/oauthenticator)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/jupyterhub/oauthenticator/issues)
 [![Discourse](https://img.shields.io/badge/help_forum-discourse-blue?logo=discourse)](https://discourse.jupyter.org/c/jupyterhub)
 [![Gitter](https://img.shields.io/badge/social_chat-gitter-blue?logo=gitter)](https://gitter.im/jupyterhub/jupyterhub)
 
 [OAuth](https://en.wikipedia.org/wiki/OAuth) is a token based login mechanism that doesn't rely on a username and password mapping.
@@ -43,40 +46,27 @@
 
 There is also a [GenericAuthenticator](oauthenticator/generic.py)
 that can be configured with any OAuth 2.0 identity provider or can be used
 to create a new authenticator class when additional customization is needed.
 
 ## Installation
 
-The installation guide can be found in the [docs](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#installation).
+The installation guide can be found in the [docs](https://oauthenticator.readthedocs.io/en/latest/tutorials/install.html).
 
-The docs also provide example setups for different OAuth2 identity providers:
-
-- [General Setup](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#general-setup)
-- [Azure AD](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#azure-ad-setup)
-- [FeiShu](https://github.com/tezignlab/jupyterhub_feishu_authenticator)
-- [GitHub](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#github-setup)
-- [GitLab](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#gitlab-setup)
-- [Google](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#google-setup)
-- [OpenShift](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#openshift-setup)
-- [Okpy](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#okpyauthenticator)
-- [Globus](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#globus-setup)
-- [Moodle](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#moodle-setup)
-- [Yandex](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#yandex-setup)
+The [docs](https://oauthenticator.readthedocs.io/en/latest/tutorials/provider-specific-setup/index.html) also provide example setups for different OAuth2 identity providers.
 
 ## Running tests
 
-To run the tests locally:
+To run the tests locally, first setup a development environment as described in
+[CONTRIBUTING.md], and then do:
 
 ```
-$ pip install --upgrade --pre -r test-requirements.txt
-```
-
-```
-$ pytest -v ./oauthenticator/tests/
+pytest -v ./oauthenticator/tests/
 ```
 
 Or you run a specific test file with:
 
 ```
-$ pytest -v ./oauthenticator/tests/<test-file-name>
+pytest -v ./oauthenticator/tests/<test-file-name>
 ```
+
+[contributing.md]: https://github.com/jupyterhub/oauthenticator/blob/main/CONTRIBUTING.md
```

### Comparing `oauthenticator-15.1.0/oauthenticator/auth0.py` & `oauthenticator-16.0.0/oauthenticator/tests/test_auth0.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,149 +1,160 @@
-"""
-Custom Authenticator to use Auth0 OAuth with JupyterHub
+import logging
+from unittest.mock import Mock
 
-Derived using the Github and Google OAuthenticator implementations as examples.
-
-The following environment variables may be used for configuration:
-
-* AUTH0_DOMAIN - The domain for your Auth0 account
-* AUTH0_SUBDOMAIN - Alternative to AUTH0_DOMAIN if your domain ends with .auth0.com
-* OAUTH_CLIENT_ID - Your client id
-* OAUTH_CLIENT_SECRET - Your client secret
-* OAUTH_CALLBACK_URL - Your callback handler URL
-
-You must provide either AUTH0_DOMAIN or AUTH0_SUBDOMAIN. If both are provided,
-AUTH0_DOMAIN will take precedence.
-
-Additionally, if you are concerned about your secrets being exposed by
-an env dump(I know I am!) you can set the client_secret, client_id and
-oauth_callback_url directly on the config for Auth0OAuthenticator.
-
-One instance of this could be adding the following to your jupyterhub_config.py::
-
-  c.Auth0OAuthenticator.auth0_domain = 'auth.example.com'
-  c.Auth0OAuthenticator.client_id = 'YOUR_CLIENT_ID'
-  c.Auth0OAuthenticator.client_secret = 'YOUR_CLIENT_SECRET'
-  c.Auth0OAuthenticator.oauth_callback_url = 'YOUR_CALLBACK_URL'
-  c.Auth0OAuthenticator.scope = ['openid','profile','email']
-
-If you are using the environment variable config, all you should need to
-do is define them in the environment then add the following line to 
-jupyterhub_config.py :
-
-  c.JupyterHub.authenticator_class = 'oauthenticator.auth0.Auth0OAuthenticator'
-
-"""
-import json
-import os
-
-from jupyterhub.auth import LocalAuthenticator
-from tornado.httpclient import HTTPRequest
-from traitlets import Unicode, default
-
-from .oauth2 import OAuthenticator
-
-
-class Auth0OAuthenticator(OAuthenticator):
-
-    login_service = "Auth0"
-
-    auth0_subdomain = Unicode(config=True)
-    auth0_domain = Unicode(config=True)
-
-    @default("auth0_subdomain")
-    def _auth0_subdomain_default(self):
-        # This is allowed to be empty unless auth0_domain is not supplied either
-        return os.getenv("AUTH0_SUBDOMAIN", "")
-
-    @default("auth0_domain")
-    def _auth0_domain_default(self):
-        domain = os.getenv("AUTH0_DOMAIN", "")
-        if domain:
-            return domain
-        if self.auth0_subdomain:
-            return '%s.auth0.com' % self.auth0_subdomain
-        raise ValueError(
-            "Please specify $AUTH0_DOMAIN env, $AUTH0_SUBDOMAIN env, %s.auth0_domain config, or %s.auth0_subdomain config"
-            % (self.__class__.__name__, self.__class__.__name__)
-        )
-
-    username_key = Unicode(
-        os.environ.get("OAUTH2_USERNAME_KEY", "email"),
-        config=True,
-        help="Userdata username key from returned json with user data login information",
+from pytest import fixture, mark, raises
+from tornado import web
+from traitlets.config import Config
+
+from ..auth0 import Auth0OAuthenticator
+from ..oauth2 import OAuthLogoutHandler
+from .mocks import mock_handler, setup_oauth_mock
+
+AUTH0_DOMAIN = "jupyterhub-test.auth0.com"
+
+
+@fixture
+def auth0_client(client):
+    setup_oauth_mock(
+        client,
+        host=AUTH0_DOMAIN,
+        access_token_path='/oauth/token',
+        user_path='/userinfo',
     )
-
-    @default("logout_redirect_url")
-    def _logout_redirect_url_default(self):
-        return 'https://%s/v2/logout' % self.auth0_domain
-
-    @default("authorize_url")
-    def _authorize_url_default(self):
-        return "https://%s/authorize" % self.auth0_domain
-
-    @default("token_url")
-    def _token_url_default(self):
-        return "https://%s/oauth/token" % self.auth0_domain
-
-    async def authenticate(self, handler, data=None):
-        code = handler.get_argument("code")
-
-        params = {
-            'grant_type': 'authorization_code',
-            'client_id': self.client_id,
-            'client_secret': self.client_secret,
-            'code': code,
-            'redirect_uri': self.get_callback_url(handler),
-        }
-        url = self.token_url
-
-        req = HTTPRequest(
-            url,
-            method="POST",
-            headers={"Content-Type": "application/json"},
-            body=json.dumps(params),
-        )
-
-        resp_json = await self.fetch(req)
-
-        access_token = resp_json['access_token']
-
-        refresh_token = resp_json.get('refresh_token')
-        id_token = resp_json.get('id_token')
-
-        # Determine who the logged in user is
-        headers = {
-            "Accept": "application/json",
-            "User-Agent": "JupyterHub",
-            "Authorization": "Bearer {}".format(access_token),
-        }
-        req = HTTPRequest(
-            "https://%s/userinfo" % self.auth0_domain,
-            method="GET",
-            headers=headers,
-        )
-        resp_json = await self.fetch(req)
-
-        name = resp_json.get(self.username_key)
-        if not name:
-            self.log.error(
-                "Auth0 user contains no key %s: %s", self.username_key, resp_json
-            )
-            return
-
-        return {
-            'name': name,
-            'auth_state': {
-                'access_token': access_token,
-                'refresh_token': refresh_token,
-                'id_token': id_token,
-                'auth0_user': resp_json,
-            },
-        }
+    return client
 
 
-class LocalAuth0OAuthenticator(LocalAuthenticator, Auth0OAuthenticator):
+def user_model():
+    """Return a user model"""
+    return {
+        "email": "user1@example.com",
+        "name": "user1",
+    }
+
+
+@mark.parametrize(
+    "test_variation_id,class_config,expect_allowed,expect_admin",
+    [
+        # no allow config tested
+        ("00", {}, False, None),
+        # allow config, individually tested
+        ("01", {"allow_all": True}, True, None),
+        ("02", {"allowed_users": {"user1"}}, True, None),
+        ("03", {"allowed_users": {"not-test-user"}}, False, None),
+        ("04", {"admin_users": {"user1"}}, True, True),
+        ("05", {"admin_users": {"not-test-user"}}, False, None),
+        # allow config, some combinations of two tested
+        (
+            "10",
+            {
+                "allow_all": False,
+                "allowed_users": {"not-test-user"},
+            },
+            False,
+            None,
+        ),
+        (
+            "11",
+            {
+                "admin_users": {"user1"},
+                "allowed_users": {"not-test-user"},
+            },
+            True,
+            True,
+        ),
+    ],
+)
+async def test_auth0(
+    auth0_client,
+    test_variation_id,
+    class_config,
+    expect_allowed,
+    expect_admin,
+):
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.Auth0OAuthenticator = Config(class_config)
+    c.Auth0OAuthenticator.auth0_domain = AUTH0_DOMAIN
+    c.Auth0OAuthenticator.username_claim = "name"
+    authenticator = Auth0OAuthenticator(config=c)
+
+    handled_user_model = user_model()
+    handler = auth0_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+
+    if expect_allowed:
+        assert auth_model
+        assert set(auth_model) == {"name", "admin", "auth_state"}
+        assert auth_model["admin"] == expect_admin
+        auth_state = auth_model["auth_state"]
+        assert "access_token" in auth_state
+        user_info = auth_state[authenticator.user_auth_state_key]
+        assert user_info == handled_user_model
+        assert auth_model["name"] == user_info[authenticator.username_claim]
+    else:
+        assert auth_model == None
+
+
+async def test_custom_logout(monkeypatch):
+    authenticator = Auth0OAuthenticator()
+    logout_handler = mock_handler(OAuthLogoutHandler, authenticator=authenticator)
+    monkeypatch.setattr(web.RequestHandler, 'redirect', Mock())
+
+    logout_handler.clear_login_cookie = Mock()
+    logout_handler.clear_cookie = Mock()
+    logout_handler._jupyterhub_user = Mock()
+    monkeypatch.setitem(logout_handler.settings, 'statsd', Mock())
+
+    # Sanity check: Ensure the logout handler and url are set on the hub
+    handlers = [handler for _, handler in authenticator.get_handlers(None)]
+    assert any([h == OAuthLogoutHandler for h in handlers])
+    assert authenticator.logout_url('http://myhost') == 'http://myhost/logout'
+
+    # Check redirection to the custom logout url
+    authenticator.auth0_domain = AUTH0_DOMAIN
+    await logout_handler.get()
+    custom_logout_url = f'https://{AUTH0_DOMAIN}/v2/logout'
+    logout_handler.redirect.assert_called_with(custom_logout_url)
+
+
+@mark.parametrize(
+    "test_variation_id,class_config,expect_config,expect_loglevel,expect_message",
+    [
+        (
+            "username_key",
+            {"username_key": "dummy"},
+            {"username_claim": "dummy"},
+            logging.WARNING,
+            "Auth0OAuthenticator.username_key is deprecated in Auth0OAuthenticator 16.0.0, use Auth0OAuthenticator.username_claim instead",
+        ),
+    ],
+)
+async def test_deprecated_config(
+    caplog,
+    test_variation_id,
+    class_config,
+    expect_config,
+    expect_loglevel,
+    expect_message,
+):
+    """
+    Tests that a warning is emitted when using a deprecated config and that
+    configuring the old config ends up configuring the new config.
+    """
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.Auth0OAuthenticator = Config(class_config)
+
+    test_logger = logging.getLogger('testlog')
+    if expect_loglevel == logging.ERROR:
+        with raises(ValueError, match=expect_message):
+            Auth0OAuthenticator(config=c, log=test_logger)
+    else:
+        authenticator = Auth0OAuthenticator(config=c, log=test_logger)
+        for key, value in expect_config.items():
+            assert getattr(authenticator, key) == value
 
-    """A version that mixes in local system user creation"""
+    captured_log_tuples = caplog.record_tuples
+    print(captured_log_tuples)
 
-    pass
+    expected_log_tuple = (test_logger.name, expect_loglevel, expect_message)
+    assert expected_log_tuple in captured_log_tuples
```

### Comparing `oauthenticator-15.1.0/oauthenticator/azuread.py` & `oauthenticator-16.0.0/oauthenticator/bitbucket.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,92 +1,102 @@
 """
-Custom Authenticator to use Azure AD with JupyterHub
+A JupyterHub authenticator class for use with Bitbucket as an identity provider.
 """
 import os
-import urllib
 
-import jwt
 from jupyterhub.auth import LocalAuthenticator
-from tornado.httpclient import HTTPRequest
-from traitlets import Unicode, default
+from tornado.httputil import url_concat
+from traitlets import Set, default
 
 from .oauth2 import OAuthenticator
 
 
-class AzureAdOAuthenticator(OAuthenticator):
-    login_service = Unicode(
-        os.environ.get('LOGIN_SERVICE', 'Azure AD'),
-        config=True,
-        help="""Azure AD domain name string, e.g. My College""",
-    )
-
-    tenant_id = Unicode(config=True, help="The Azure Active Directory Tenant ID")
-
-    @default('tenant_id')
-    def _tenant_id_default(self):
-        return os.environ.get('AAD_TENANT_ID', '')
-
-    username_claim = Unicode(config=True)
-
-    @default('username_claim')
-    def _username_claim_default(self):
-        return 'name'
+class BitbucketOAuthenticator(OAuthenticator):
+    client_id_env = "BITBUCKET_CLIENT_ID"
+    client_secret_env = "BITBUCKET_CLIENT_SECRET"
+    user_auth_state_key = "bitbucket_user"
+
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "Bitbucket")
 
     @default("authorize_url")
     def _authorize_url_default(self):
-        return 'https://login.microsoftonline.com/{0}/oauth2/authorize'.format(
-            self.tenant_id
-        )
+        return "https://bitbucket.org/site/oauth2/authorize"
 
     @default("token_url")
     def _token_url_default(self):
-        return 'https://login.microsoftonline.com/{0}/oauth2/token'.format(
-            self.tenant_id
-        )
-
-    async def authenticate(self, handler, data=None):
-        code = handler.get_argument("code")
+        return "https://bitbucket.org/site/oauth2/access_token"
 
-        params = dict(
-            client_id=self.client_id,
-            client_secret=self.client_secret,
-            grant_type='authorization_code',
-            code=code,
-            redirect_uri=self.get_callback_url(handler),
-        )
-
-        data = urllib.parse.urlencode(params, doseq=True, encoding='utf-8', safe='=')
-
-        url = self.token_url
+    @default("userdata_url")
+    def _userdata_url_default(self):
+        return "https://api.bitbucket.org/2.0/user"
 
-        headers = {'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'}
-        req = HTTPRequest(
-            url,
-            method="POST",
-            headers=headers,
-            body=data,  # Body is required for a POST...
-        )
+    allowed_teams = Set(
+        config=True,
+        help="""
+        Allow members of selected Bitbucket teams to sign in.
+        """,
+    )
 
-        resp_json = await self.fetch(req)
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "team_whitelist": ("allowed_teams", "0.12.0"),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    team_whitelist = Set(
+        config=True,
+        help="""
+        .. deprecated:: 0.12
 
-        access_token = resp_json['access_token']
-        id_token = resp_json['id_token']
+           Use :attr:`allowed_teams`.
+        """,
+    )
 
-        decoded = jwt.decode(
-            id_token,
-            options={"verify_signature": False},
-            audience=self.client_id,
+    async def _fetch_user_teams(self, access_token, token_type):
+        """
+        Get user's team memberships via bitbucket's API.
+        """
+        headers = self.build_userdata_request_headers(access_token, token_type)
+        next_page = url_concat(
+            "https://api.bitbucket.org/2.0/workspaces", {'role': 'member'}
         )
 
-        userdict = {"name": decoded[self.username_claim]}
-        userdict["auth_state"] = auth_state = {}
-        auth_state['access_token'] = access_token
-        # results in a decoded JWT for the user data
-        auth_state['user'] = decoded
+        user_teams = set()
+        while next_page:
+            resp_json = await self.httpfetch(next_page, method="GET", headers=headers)
+            next_page = resp_json.get('next', None)
+            user_teams |= {entry["name"] for entry in resp_json["values"]}
+        return user_teams
+
+    async def update_auth_model(self, auth_model):
+        """
+        Fetch and store `user_teams` in auth state if `allowed_teams` is
+        configured.
+        """
+        if self.allowed_teams:
+            access_token = auth_model["auth_state"]["token_response"]["access_token"]
+            token_type = auth_model["auth_state"]["token_response"]["token_type"]
+            user_teams = await self._fetch_user_teams(access_token, token_type)
+            auth_model["auth_state"]["user_teams"] = user_teams
+
+        return auth_model
+
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        `allowed_teams`.
+        """
+        if await super().check_allowed(username, auth_model):
+            return True
+
+        if self.allowed_teams:
+            user_teams = auth_model["auth_state"]["user_teams"]
+            if any(user_teams & self.allowed_teams):
+                return True
 
-        return userdict
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
 
-class LocalAzureAdOAuthenticator(LocalAuthenticator, AzureAdOAuthenticator):
+class LocalBitbucketOAuthenticator(LocalAuthenticator, BitbucketOAuthenticator):
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/cilogon.py` & `oauthenticator-16.0.0/oauthenticator/cilogon.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,379 +1,363 @@
-"""CILogon OAuthAuthenticator for JupyterHub
-
-Uses OAuth 2.0 with cilogon.org (override with CILOGON_HOST)
-
-Caveats:
-
-- For allowed user list /admin purposes, username will be the ePPN by default.
-  This is typically an email address and may not work as a Unix userid.
-  Normalization may be required to turn the JupyterHub username into a Unix username.
-- Default username_claim of ePPN does not work for all providers,
-  e.g. generic OAuth such as Google.
-  Use `c.CILogonOAuthenticator.username_claim = 'email'` to use
-  email instead of ePPN as the JupyterHub username.
+"""
+A JupyterHub authenticator class for use with CILogon as an identity provider.
 """
 import os
 from urllib.parse import urlparse
 
 import jsonschema
 from jupyterhub.auth import LocalAuthenticator
 from ruamel.yaml import YAML
 from tornado import web
-from tornado.httpclient import HTTPRequest
-from tornado.httputil import url_concat
 from traitlets import Bool, Dict, List, Unicode, default, validate
 
 from .oauth2 import OAuthenticator, OAuthLoginHandler
 
 yaml = YAML(typ="safe", pure=True)
 
 
 class CILogonLoginHandler(OAuthLoginHandler):
     """See https://www.cilogon.org/oidc for general information."""
 
     def authorize_redirect(self, *args, **kwargs):
-        """Add idp, skin to redirect params"""
+        """
+        Optionally add "skin" to redirect params, and always add "selected_idp"
+        (aka. "idphint") based on allowed_idps config.
+
+        Related documentation at https://www.cilogon.org/oidc#h.p_IWGvXH0okDI_.
+        """
+        # kwargs is updated to include extra_params if it doesn't already
+        # include it, we then modify kwargs' extra_params dictionary
         extra_params = kwargs.setdefault('extra_params', {})
-        if self.authenticator.shown_idps:
-            # selected_idp must be a string where idps are separated by commas, with no space between, otherwise it will get escaped
-            # example: https://accounts.google.com/o/oauth2/auth,https://github.com/login/oauth/authorize
-            idps = ",".join(self.authenticator.shown_idps)
-            extra_params["selected_idp"] = idps
+
+        # selected_idp should be a comma separated string
+        allowed_idps = ",".join(self.authenticator.allowed_idps.keys())
+        extra_params["selected_idp"] = allowed_idps
+
         if self.authenticator.skin:
             extra_params["skin"] = self.authenticator.skin
 
         return super().authorize_redirect(*args, **kwargs)
 
 
 class CILogonOAuthenticator(OAuthenticator):
-    _deprecated_oauth_aliases = {
-        # <deprecated-config>:
-        #   (
-        #    <new-config>,
-        #    <deprecation-version>,
-        #    <deprecated-config-and-new-config-have-same-type>
-        #   )
-        "idp_whitelist": ("allowed_idps", "0.12.0", False),
-        "idp": ("shown_idps", "15.0.0", False),
-        "strip_idp_domain": ("allowed_idps", "15.0.0", False),
-        **OAuthenticator._deprecated_oauth_aliases,
-    }
-
-    login_service = "CILogon"
+    login_handler = CILogonLoginHandler
 
+    user_auth_state_key = "cilogon_user"
     client_id_env = 'CILOGON_CLIENT_ID'
     client_secret_env = 'CILOGON_CLIENT_SECRET'
-    login_handler = CILogonLoginHandler
 
-    cilogon_host = Unicode(os.environ.get("CILOGON_HOST") or "cilogon.org", config=True)
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "CILogon")
+
+    cilogon_host = Unicode(
+        os.environ.get("CILOGON_HOST") or "cilogon.org",
+        config=True,
+        help="""
+        Used to determine the default values for `authorize_url`, `token_url`,
+        and `userdata_url`.
+        """,
+    )
 
     @default("authorize_url")
     def _authorize_url_default(self):
-        return "https://%s/authorize" % self.cilogon_host
+        return f"https://{self.cilogon_host}/authorize"
 
     @default("token_url")
     def _token_url(self):
-        return "https://%s/oauth2/token" % self.cilogon_host
+        return f"https://{self.cilogon_host}/oauth2/token"
+
+    @default("userdata_url")
+    def _userdata_url_default(self):
+        return f"https://{self.cilogon_host}/oauth2/userinfo"
 
     scope = List(
         Unicode(),
-        default_value=['openid', 'email', 'org.cilogon.userinfo'],
+        default_value=['openid', 'email', 'org.cilogon.userinfo', 'profile'],
         config=True,
-        help="""The OAuth scopes to request.
+        help="""
+        OAuth scopes to request.
+
+        `openid` and `org.cilogon.userinfo` is required.
 
-        See cilogon_scope.md for details.
-        At least 'openid' is required.
+        Read more about CILogon scopes in https://www.cilogon.org/oidc.
         """,
     )
 
     @validate('scope')
     def _validate_scope(self, proposal):
-        """Ensure `openid` is always requested and `org.cilogon.userinfo`
-        is requested when allowed_idps is specified.
+        """
+        Ensure `openid` and `org.cilogon.userinfo` is requested.
+
+        - The `idp` claim is required, and its documented to associate with
+          requesting the `org.cilogon.userinfo` scope.
+
+        ref: https://www.cilogon.org/oidc#h.p_PEQXL8QUjsQm
         """
         scopes = proposal.value
 
         if 'openid' not in proposal.value:
             scopes += ['openid']
 
-        if self.allowed_idps and 'org.cilogon.userinfo' not in proposal.value:
+        if 'org.cilogon.userinfo' not in proposal.value:
             scopes += ['org.cilogon.userinfo']
 
         return scopes
 
-    idp_whitelist = List(
-        help="Deprecated, use `CIlogonOAuthenticator.allowed_idps`",
-        config=True,
-    )
-
     allowed_idps = Dict(
         config=True,
-        default_value={},
-        help="""A dictionary of the only entity IDs that will be allowed to be used as login options.
-        See https://cilogon.org/idplist for the list of `EntityIDs` of each IdP.
+        help="""
+        A dictionary of the only entity IDs that will be allowed to be used as
+        login options. See https://cilogon.org/idplist for the list of
+        `EntityIDs` of each IdP.
 
-        It can be used to enable domain stripping, adding prefixes to the usernames and to specify an identity provider specific username claim.
+        It can be used to enable domain stripping, adding prefixes to the
+        usernames and to specify an identity provider specific username claim.
 
         For example::
 
-            allowed_idps = {
+            c.CILogonOAuthenticator.allowed_idps = {
                 "https://idpz.utorauth.utoronto.ca/shibboleth": {
                     "username_derivation": {
                         "username_claim": "email",
                         "action": "strip_idp_domain",
                         "domain": "utoronto.ca",
-                    }
+                    },
                 },
                 "https://github.com/login/oauth/authorize": {
                     "username_derivation": {
                         "username_claim": "username",
                         "action": "prefix",
-                        "prefix": "gh"
-                    }
-                }
+                        "prefix": "github",
+                    },
+                },
                 "http://google.com/accounts/o8/id": {
                     "username_derivation": {
                         "username_claim": "username",
-                    }
-                    "allowed_domains": ["uni.edu", "something.org"]
-                }
+                        "action": "prefix",
+                        "prefix": "google",
+                    },
+                    "allowed_domains": ["uni.edu", "something.org"],
+                },
             }
 
         Where `username_derivation` defines:
-            * :attr:`username_claim`: string
-                The claim in the `userinfo` response from which to get the JupyterHub username.
-                Examples include: `eppn`, `email`. What keys are available will depend on the scopes requested.
-                It will overwrite any value set through CILogonOAuthenticator.username_claim for this identity provider.
-            * :attr:`action`: string
-                What action to perform on the username. Available options are "strip_idp_domain", which will strip the domain from the username if specified and "prefix", which will prefix the hub username with "prefix:".
-            * :attr:`domain:` string
-                The domain after "@" which will be stripped from the username if it exists and if the action is "strip_idp_domain".
-            * :attr:`prefix`: string
-                The prefix which will be added at the beginning of the username followed by a semi-column ":", if the action is "prefix".
-            * :attr:`allowed_domains`: string
-                It defines which domains will be allowed to login using the specific identity provider.
-
-        Requirements:
-            * if `username_derivation.action` is `strip_idp_domain`, then `username_derivation.domain` must also be specified
-            * if `username_derivation.action` is `prefix`, then `username_derivation.prefix` must also be specified.
-            * `username_claim` must be provided for each idp in `allowed_idps`
 
-        .. versionchanged:: 15.0.0
-            `CILogonOAuthenticaor.allowed_idps` changed type from list to dict
+            * `username_claim`: string (required)
+                The claim in the `userinfo` response from which to get the
+                JupyterHub username. Examples include: `eppn`, `email`. What
+                keys are available will depend on the scopes requested.
+            * `action`: string
+                What action to perform on the username. Available options are
+                "strip_idp_domain", which will strip the domain from the
+                username if specified and "prefix", which will prefix the hub
+                username with "prefix:".
+            * `domain:` string (required if action is strip_idp_domain)
+                The domain after "@" which will be stripped from the username if
+                it exists and if the action is "strip_idp_domain".
+            * `prefix`: string (required if action is prefix)
+                The prefix which will be added at the beginning of the username
+                followed by a semi-column ":", if the action is "prefix".
+            * `allowed_domains`: string
+                It defines which domains will be allowed to login using the
+                specific identity provider.
+
+        .. versionchanged:: 15.0
+
+           Changed format from a list to a dictionary.
         """,
     )
 
     @validate("allowed_idps")
     def _validate_allowed_idps(self, proposal):
         idps = proposal.value
 
-        for entity_id, username_derivation in idps.items():
-            # Validate `username_derivation` config using the schema
+        if not idps:
+            raise ValueError("One or more allowed_idps must be configured")
+
+        for entity_id, idp_config in idps.items():
+            # Validate `idp_config` config using the schema
             root_dir = os.path.dirname(os.path.abspath(__file__))
             schema_file = os.path.join(root_dir, "schemas", "cilogon-schema.yaml")
             with open(schema_file) as schema_fd:
                 schema = yaml.load(schema_fd)
                 # Raises useful exception if validation fails
-                jsonschema.validate(username_derivation, schema)
+                jsonschema.validate(idp_config, schema)
 
-            # Make sure allowed_idps containes EntityIDs and not domain names.
+            # Make sure allowed_idps contains EntityIDs and not domain names.
             accepted_entity_id_scheme = ["urn", "https", "http"]
             entity_id_scheme = urlparse(entity_id).scheme
             if entity_id_scheme not in accepted_entity_id_scheme:
                 # Validate entity ids are the form of: `https://github.com/login/oauth/authorize`
                 self.log.error(
                     f"Trying to allow an auth provider: {entity_id}, that doesn't look like a valid CILogon EntityID.",
                 )
                 raise ValueError(
-                    """The keys of `allowed_idps` **must** be CILogon permitted EntityIDs.
-                    See https://cilogon.org/idplist for the list of EntityIDs of each IDP.
-                    """
+                    "The keys of `allowed_idps` **must** be CILogon permitted EntityIDs. "
+                    "See https://cilogon.org/idplist for the list of EntityIDs of each IDP."
                 )
 
         return idps
 
-    strip_idp_domain = Bool(
-        False,
+    skin = Unicode(
         config=True,
-        help="""Deprecated, use `CILogonOAuthenticator.allowed_idps["username_derivation"]["action"] = "strip_idp_domain"`
-        to enable it and `CIlogonOAuthenticator.allowed_idps["username_derivation"]["domain"]` to list the domain
-        which will be stripped
+        help="""
+        The `skin` attribute is the name of the custom CILogon interface skin
+        for your application.
+
+        Contact help@cilogon.org to request a custom skin.
         """,
     )
 
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "idp_whitelist": ("allowed_idps", "0.12.0", False),
+        "idp": ("shown_idps", "15.0.0", False),
+        "strip_idp_domain": ("allowed_idps", "15.0.0", False),
+        "shown_idps": ("allowed_idps", "16.0.0", False),
+        "additional_username_claims": ("allowed_idps", "16.0.0", False),
+        "username_claim": ("allowed_idps", "16.0.0", False),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    idp_whitelist = List(
+        config=True,
+        help="""
+        .. versionremoved:: 0.12
+
+           Use :attr:`allowed_idps`.
+        """,
+    )
     idp = Unicode(
-        config=True, help="Deprecated, use `CILogonOAuthenticator.shown_idps`."
+        config=True,
+        help="""
+        .. versionremoved:: 15.0
+
+           Use :attr:`allowed_idps`.
+        """,
     )
+    strip_idp_domain = Bool(
+        config=True,
+        help="""
+        .. versionremoved:: 15.0
 
+           Use :attr:`allowed_idps`.
+        """,
+    )
     shown_idps = List(
-        Unicode(),
         config=True,
-        help="""A list of identity providers to be shown as login options.
-        The `idp` attribute is the SAML Entity ID of the user's selected
-        identity provider.
+        help="""
+        .. versionremoved:: 16.0
 
-        See https://cilogon.org/include/idplist.xml for the list of identity
-        providers supported by CILogon.
+           Use :attr:`allowed_idps`.
         """,
     )
-
-    skin = Unicode(
+    additional_username_claims = List(
         config=True,
-        help="""The `skin` attribute is the name of the custom CILogon interface skin
-        for your application.
+        help="""
+        .. versionremoved:: 16.0
 
-        Contact help@cilogon.org to request a custom skin.
+           Use :attr:`allowed_idps`.
         """,
     )
-
     username_claim = Unicode(
-        "eppn",
         config=True,
-        help="""The claim in the userinfo response from which to get the JupyterHub username
-        Examples include: eppn, email
+        help="""
+        .. versionremoved:: 16.0
 
-        What keys are available will depend on the scopes requested.
-
-        See https://www.cilogon.org/oidc for details.
-
-        Note that this option can be overridden for specific identity providers via `allowed_idps[<identity provider>]["username_derivation"]["username_claim"]`.
+           Use :attr:`allowed_idps`.
         """,
     )
 
-    additional_username_claims = List(
-        config=True,
-        help="""Additional claims to check if the username_claim fails.
+    def user_info_to_username(self, user_info):
+        """
+        Overrides OAuthenticator.user_info_to_username that relies on
+        username_claim to instead consider idp specific config in under
+        allowed_idps[user_info["idp"]]["username_derivation"].
 
-        This is useful for linked identities where not all of them return
-        the primary username_claim.
-        """,
-    )
+        Returns a username based on user_info and configuration in allowed_idps
+        under the associated idp's username_derivation config.
+        """
+        # NOTE: The first time we have received user_info is when
+        #       user_info_to_username is called by OAuthenticator.authenticate,
+        #       so we make a check here that the "idp" claim is received and
+        #       that we allowed_idps is configured to handle that idp.
+        #
+        user_idp = user_info.get("idp")
+        if not user_idp:
+            message = "'idp' claim was not part of the response to the userdata_url"
+            self.log.error(message)
+            raise web.HTTPError(500, message)
+        if not self.allowed_idps.get(user_idp):
+            message = f"Login with identity provider {user_idp} is not pre-configured"
+            self.log.error(message)
+            raise web.HTTPError(403, message)
+
+        unprocessed_username = self._user_info_to_unprocessed_username(user_info)
+        username = self._get_processed_username(unprocessed_username, user_info)
 
-    def check_username_claim(self, claimlist, resp_json):
-        for claim in claimlist:
-            username = resp_json.get(claim)
-            if username:
-                return username
+        return username
+
+    def _user_info_to_unprocessed_username(self, user_info):
+        """
+        Returns a username from user_info without also applying the "action"
+        specified under "username_derivation" for the associated idp.
+        """
+        user_idp = user_info["idp"]
+        username_derivation = self.allowed_idps[user_idp]["username_derivation"]
+        username_claim = username_derivation["username_claim"]
 
+        username = user_info.get(username_claim)
         if not username:
-            if len(claimlist) < 2:
-                self.log.error(
-                    "Username claim %s not found in response: %s",
-                    self.username_claim,
-                    sorted(resp_json.keys()),
-                )
-            else:
-                self.log.error(
-                    "No username claim from %r in response: %s",
-                    claimlist,
-                    sorted(resp_json.keys()),
-                )
-            raise web.HTTPError(500, "Failed to get username from CILogon")
+            message = f"Configured username_claim {username_claim} for {user_idp} was not found in the response {user_info.keys()}"
+            self.log.error(message)
+            raise web.HTTPError(500, message)
 
-    async def authenticate(self, handler, data=None):
-        """We set up auth_state based on additional CILogon info if we
-        receive it.
-        """
-        code = handler.get_argument("code")
-
-        # Exchange the OAuth code for a CILogon Access Token
-        # See: https://www.cilogon.org/oidc
-        headers = {"Accept": "application/json", "User-Agent": "JupyterHub"}
-
-        params = dict(
-            client_id=self.client_id,
-            client_secret=self.client_secret,
-            redirect_uri=self.get_callback_url(handler),
-            code=code,
-            grant_type='authorization_code',
-        )
-
-        url = url_concat(self.token_url, params)
-
-        req = HTTPRequest(url, headers=headers, method="POST", body='')
-
-        token_response = await self.fetch(req)
-        access_token = token_response['access_token']
-        # Determine who the logged in user is
-        params = dict(access_token=access_token)
-        req = HTTPRequest(
-            url_concat("https://%s/oauth2/userinfo" % self.cilogon_host, params),
-            headers=headers,
-        )
-        resp_json = await self.fetch(req)
-
-        claimlist = [self.username_claim]
-        if self.additional_username_claims:
-            claimlist.extend(self.additional_username_claims)
-
-        selected_idp = resp_json.get("idp")
-        # Check if selected idp was marked as allowed
-        if self.allowed_idps:
-            # Faild hard if idp wasn't allowed
-            if selected_idp not in self.allowed_idps.keys():
-                self.log.error(
-                    f"Trying to login from an identity provider that was not allowed {selected_idp}",
-                )
-                raise web.HTTPError(
-                    500,
-                    "Trying to login using an identity provider that was not allowed",
-                )
+        return username
 
-            # The username_claim which should be used for this idp
-            claimlist = [
-                self.allowed_idps[selected_idp]["username_derivation"]["username_claim"]
-            ]
-
-        # Check if the requested username_claim exists in the response from the provider
-        username = self.check_username_claim(claimlist, resp_json)
-
-        # Check if we need to strip/prefix username
-        if self.allowed_idps:
-            username_derivation_config = self.allowed_idps[selected_idp][
-                "username_derivation"
-            ]
-            action = username_derivation_config.get("action", None)
-            allowed_domains = self.allowed_idps[selected_idp].get(
-                "allowed_domains", None
-            )
-
-            if allowed_domains:
-                gotten_name, gotten_domain = username.split('@')
-                if gotten_domain not in allowed_domains:
-                    raise web.HTTPError(
-                        500,
-                        "Trying to login using a domain that was not allowed",
-                    )
-
-            if action == "strip_idp_domain":
-                gotten_name, gotten_domain = username.split('@')
-                if gotten_domain != username_derivation_config["domain"]:
-                    self.log.warning(
-                        "Trying to strip from the username a domain that doesn't exist."
-                        "Username will be left unchanged."
-                    )
-                else:
-                    username = gotten_name
-            elif action == "prefix":
-                prefix = username_derivation_config["prefix"]
-                username = f"{prefix}:{username}"
-
-        userdict = {"name": username}
-        # Now we set up auth_state
-        userdict["auth_state"] = auth_state = {}
-        # Save the token response and full CILogon reply in auth state
-        # These can be used for user provisioning
-        #  in the Lab/Notebook environment.
-        auth_state['token_response'] = token_response
-        # store the whole user model in auth_state.cilogon_user
-        # keep access_token as well, in case anyone was relying on it
-        auth_state['access_token'] = access_token
-        auth_state['cilogon_user'] = resp_json
-        return userdict
+    def _get_processed_username(self, username, user_info):
+        """
+        Optionally adjusts a username from user_info based on the "action"
+        specified under "username_derivation" for the associated idp.
+        """
+        user_idp = user_info["idp"]
+        username_derivation = self.allowed_idps[user_idp]["username_derivation"]
 
+        # Optionally execute action "strip_idp_domain" or "prefix"
+        action = username_derivation.get("action")
+        if action == "strip_idp_domain":
+            domain_suffix = "@" + username_derivation["domain"]
+            if username.lower().endswith(domain_suffix.lower()):
+                username = username[: -len(domain_suffix)]
+        elif action == "prefix":
+            prefix = username_derivation["prefix"]
+            username = f"{prefix}:{username}"
 
-class LocalCILogonOAuthenticator(LocalAuthenticator, CILogonOAuthenticator):
+        return username
 
-    """A version that mixes in local system user creation"""
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        an `allowed_domains` as configured under `allowed_idps`.
+        """
+        if await super().check_allowed(username, auth_model):
+            return True
+
+        user_info = auth_model["auth_state"][self.user_auth_state_key]
+        user_idp = user_info["idp"]
+        idp_allowed_domains = self.allowed_idps[user_idp].get("allowed_domains")
+        if idp_allowed_domains:
+            unprocessed_username = self._user_info_to_unprocessed_username(user_info)
+            user_domain = unprocessed_username.split("@", 1)[1].lower()
+            if user_domain in idp_allowed_domains:
+                return True
+
+            message = f"Login with domain @{user_domain} is not allowed"
+            self.log.warning(message)
+            raise web.HTTPError(403, message)
+
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
-    pass
+
+class LocalCILogonOAuthenticator(LocalAuthenticator, CILogonOAuthenticator):
+    """A version that mixes in local system user creation"""
```

### Comparing `oauthenticator-15.1.0/oauthenticator/generic.py` & `oauthenticator-16.0.0/oauthenticator/gitlab.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,227 +1,254 @@
 """
-Custom Authenticator to use generic OAuth2 with JupyterHub
+A JupyterHub authenticator class for use with GitLab as an identity provider.
 """
-import base64
 import os
-from functools import reduce
-from urllib.parse import urlencode
+import warnings
+from urllib.parse import quote
 
 from jupyterhub.auth import LocalAuthenticator
-from tornado.httpclient import AsyncHTTPClient, HTTPRequest
-from tornado.httputil import url_concat
-from traitlets import Bool, Dict, List, Unicode, Union, default
+from tornado.escape import url_escape
+from traitlets import CUnicode, Set, Unicode, default
 
 from .oauth2 import OAuthenticator
-from .traitlets import Callable
 
 
-class GenericOAuthenticator(OAuthenticator):
-    login_service = Unicode("OAuth 2.0", config=True)
+def _api_headers(access_token):
+    return {
+        "Accept": "application/json",
+        "User-Agent": "JupyterHub",
+        "Authorization": f"Bearer {access_token}",
+    }
+
+
+class GitLabOAuthenticator(OAuthenticator):
+    user_auth_state_key = "gitlab_user"
+    client_id_env = 'GITLAB_CLIENT_ID'
+    client_secret_env = 'GITLAB_CLIENT_SECRET'
+
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "GitLab")
 
-    extra_params = Dict(help="Extra parameters for first POST request").tag(config=True)
-
-    claim_groups_key = Union(
-        [Unicode(os.environ.get('OAUTH2_GROUPS_KEY', 'groups')), Callable()],
+    gitlab_url = Unicode(
         config=True,
         help="""
-        Userdata groups claim key from returned json for USERDATA_URL.
-
-        Can be a string key name (use periods for nested keys), or a callable
-        that accepts the returned json (as a dict) and returns the groups list.
+        Used to determine the default values for `gitlab_api`, `authorize_url`,
+        `token_url`.
         """,
     )
 
-    allowed_groups = List(
-        Unicode(),
-        config=True,
-        help="Automatically allow members of selected groups",
-    )
+    @default("gitlab_url")
+    def _default_gitlab_url(self):
+        """get default gitlab url from env"""
+        gitlab_url = os.getenv('GITLAB_URL')
+        gitlab_host = os.getenv('GITLAB_HOST')
+
+        if not gitlab_url and gitlab_host:
+            warnings.warn(
+                'Use of GITLAB_HOST might be deprecated in the future. '
+                'Rename GITLAB_HOST environment variable to GITLAB_URL.',
+                PendingDeprecationWarning,
+            )
+            if gitlab_host.startswith(('https:', 'http:')):
+                gitlab_url = gitlab_host
+            else:
+                # Hides common mistake of users which set the GITLAB_HOST
+                # without a protocol specification.
+                gitlab_url = f'https://{gitlab_host}'
+                warnings.warn(
+                    "The https:// prefix has been added to GITLAB_HOST. "
+                    f'Set GITLAB_URL="{gitlab_host}" instead.'
+                )
 
-    admin_groups = List(
-        Unicode(),
-        config=True,
-        help="Groups whose members should have Jupyterhub admin privileges",
-    )
+        # default to gitlab.com
+        if not gitlab_url:
+            gitlab_url = 'https://gitlab.com'
+
+        return gitlab_url
 
-    username_key = Union(
-        [Unicode(os.environ.get('OAUTH2_USERNAME_KEY', 'username')), Callable()],
+    @default("authorize_url")
+    def _authorize_url_default(self):
+        return f"{self.gitlab_url}/oauth/authorize"
+
+    @default("token_url")
+    def _token_url_default(self):
+        return f"{self.gitlab_url}/oauth/token"
+
+    gitlab_api_version = CUnicode(
         config=True,
         help="""
-        Userdata username key from returned json for USERDATA_URL.
+        Used to determine the default values for `gitlab_api`.
 
-        Can be a string key name or a callable that accepts the returned
-        json (as a dict) and returns the username.  The callable is useful
-        e.g. for extracting the username from a nested object in the
-        response.
+        For details, see https://docs.gitlab.com/ee/api/rest/.
         """,
     )
 
-    userdata_params = Dict(
-        help="Userdata params to get user data login information"
-    ).tag(config=True)
+    @default("gitlab_api_version")
+    def _gitlab_api_version_default(self):
+        return os.environ.get("GITLAB_API_VERSION") or "4"
 
-    userdata_token_method = Unicode(
-        os.environ.get('OAUTH2_USERDATA_REQUEST_TYPE', 'header'),
+    gitlab_api = Unicode(
         config=True,
-        help="Method for sending access token in userdata request. Supported methods: header, url. Default: header",
+        help="""
+        Used to determine the default value for `userdata_url`.
+        """,
     )
 
-    tls_verify = Bool(
-        os.environ.get('OAUTH2_TLS_VERIFY', 'True').lower() in {'true', '1'},
-        config=True,
-        help="Disable TLS verification on http request",
-    )
+    @default("gitlab_api")
+    def _default_gitlab_api(self):
+        return f"{self.gitlab_url}/api/v{self.gitlab_api_version}"
+
+    @default("userdata_url")
+    def _userdata_url_default(self):
+        return f"{self.gitlab_api}/user"
 
-    basic_auth = Bool(
-        os.environ.get('OAUTH2_BASIC_AUTH', 'True').lower() in {'true', '1'},
+    allowed_gitlab_groups = Set(
         config=True,
-        help="Disable basic authentication for access token request",
-    )
-
-    @default("http_client")
-    def _default_http_client(self):
-        return AsyncHTTPClient(
-            force_instance=True, defaults=dict(validate_cert=self.tls_verify)
-        )
+        help="""
+        Allow members of selected GitLab groups to sign in.
 
-    def _get_headers(self):
-        headers = {"Accept": "application/json", "User-Agent": "JupyterHub"}
+        Note that for each group allowed, an additional REST API call needs to
+        be made when a user is signing in. To reduce the risk of JupyterHub
+        being rate limited, don't specify too many.
+        """,
+    )
 
-        if self.basic_auth:
-            b64key = base64.b64encode(
-                bytes("{}:{}".format(self.client_id, self.client_secret), "utf8")
-            )
-            headers.update({"Authorization": "Basic {}".format(b64key.decode("utf8"))})
-        return headers
-
-    def _get_token(self, headers, params):
-        if self.token_url:
-            url = self.token_url
-        else:
-            raise ValueError("Please set the $OAUTH2_TOKEN_URL environment variable")
+    allowed_project_ids = Set(
+        config=True,
+        help="""
+        Allow members with Developer access or higher in selected project ids to
+        sign in.
 
-        req = HTTPRequest(
-            url,
-            method="POST",
-            headers=headers,
-            body=urlencode(params),
-        )
-        return self.fetch(req, "fetching access token")
+        Note that for each project allowed, an additional REST API call needs to
+        be made when a user is signing in. To reduce the risk of JupyterHub
+        being rate limited, don't specify too many.
+        """,
+    )
 
-    def _get_user_data(self, token_response):
-        access_token = token_response['access_token']
-        token_type = token_response['token_type']
-
-        # Determine who the logged in user is
-        headers = {
-            "Accept": "application/json",
-            "User-Agent": "JupyterHub",
-            "Authorization": "{} {}".format(token_type, access_token),
-        }
-        if self.userdata_url:
-            url = url_concat(self.userdata_url, self.userdata_params)
-        else:
-            raise ValueError("Please set the OAUTH2_USERDATA_URL environment variable")
-
-        if self.userdata_token_method == "url":
-            url = url_concat(self.userdata_url, dict(access_token=access_token))
-
-        req = HTTPRequest(url, headers=headers)
-        return self.fetch(req, "fetching user data")
-
-    @staticmethod
-    def _create_auth_state(token_response, user_data_response):
-        access_token = token_response['access_token']
-        refresh_token = token_response.get('refresh_token', None)
-        scope = token_response.get('scope', '')
-        if isinstance(scope, str):
-            scope = scope.split(' ')
-
-        return {
-            'access_token': access_token,
-            'refresh_token': refresh_token,
-            'oauth_user': user_data_response,
-            'scope': scope,
-        }
-
-    @staticmethod
-    def check_user_in_groups(member_groups, allowed_groups):
-        return bool(set(member_groups) & set(allowed_groups))
-
-    async def authenticate(self, handler, data=None):
-        code = handler.get_argument("code")
-
-        params = dict(
-            redirect_uri=self.get_callback_url(handler),
-            code=code,
-            grant_type='authorization_code',
-        )
-        params.update(self.extra_params)
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "gitlab_group_whitelist": ("allowed_gitlab_groups", "0.12.0"),
+        "gitlab_project_id_whitelist": ("allowed_project_ids", "0.12.0"),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    gitlab_group_whitelist = Set(
+        config=True,
+        help="""
+        .. deprecated:: 0.12
 
-        headers = self._get_headers()
+           Use :attr:`allowed_gitlab_groups`.
+        """,
+    )
+    gitlab_project_id_whitelist = Set(
+        config=True,
+        help="""
+        .. deprecated:: 0.12
 
-        token_resp_json = await self._get_token(headers, params)
+           Use :attr:`allowed_project_ids`.
+        """,
+    )
 
-        user_data_resp_json = await self._get_user_data(token_resp_json)
+    gitlab_version = None
+    member_api_variant = None
 
-        if callable(self.username_key):
-            name = self.username_key(user_data_resp_json)
-        else:
-            name = user_data_resp_json.get(self.username_key)
-            if not name:
-                self.log.error(
-                    "OAuth user contains no key %s: %s",
-                    self.username_key,
-                    user_data_resp_json,
-                )
-                return
+    async def _set_gitlab_version(self, access_token):
+        # memoize gitlab version for class lifetime
+        if self.gitlab_version is None:
+            self.gitlab_version = await self._get_gitlab_version(access_token)
+            self.member_api_variant = 'all/' if self.gitlab_version >= [12, 4] else ''
+
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        `allowed_google_groups` or `allowed_project_ids`.
+        """
+        if await super().check_allowed(username, auth_model):
+            return True
+
+        access_token = auth_model["auth_state"]["token_response"]["access_token"]
+        user_id = auth_model["auth_state"][self.user_auth_state_key]["id"]
+
+        if self.allowed_gitlab_groups:
+            user_in_group = await self._check_membership_allowed_groups(
+                user_id, access_token
+            )
+            if user_in_group:
+                return True
 
-        user_info = {
-            'name': name,
-            'auth_state': self._create_auth_state(token_resp_json, user_data_resp_json),
-        }
-
-        if self.allowed_groups:
-            self.log.info(
-                'Validating if user claim groups match any of {}'.format(
-                    self.allowed_groups
-                )
+        if self.allowed_project_ids:
+            user_in_project = await self._check_membership_allowed_project_ids(
+                user_id, access_token
             )
+            if user_in_project:
+                return True
 
-            if callable(self.claim_groups_key):
-                groups = self.claim_groups_key(user_data_resp_json)
-            else:
-                try:
-                    groups = reduce(
-                        dict.get, self.claim_groups_key.split("."), user_data_resp_json
-                    )
-                except TypeError:
-                    # This happens if a nested key does not exist (reduce trying to call None.get)
-                    self.log.error(
-                        "The key {} does not exist in the user token, or it is set to null".format(
-                            self.claim_groups_key
-                        )
-                    )
-                    groups = None
-            if not groups:
-                self.log.error(
-                    "No claim groups found for user! Something wrong with the `claim_groups_key` {}? {}".format(
-                        self.claim_groups_key, user_data_resp_json
-                    )
-                )
-                groups = []
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
-            if self.check_user_in_groups(groups, self.allowed_groups):
-                user_info['admin'] = self.check_user_in_groups(
-                    groups, self.admin_groups
-                )
-            else:
-                user_info = None
+    async def _get_gitlab_version(self, access_token):
+        url = f"{self.gitlab_api}/version"
+        resp_json = await self.httpfetch(
+            url,
+            method="GET",
+            headers=_api_headers(access_token),
+            validate_cert=self.validate_server_cert,
+        )
+        version_strings = resp_json['version'].split('-')[0].split('.')[:3]
+        version_ints = list(map(int, version_strings))
+        return version_ints
+
+    async def _check_membership_allowed_groups(self, user_id, access_token):
+        headers = _api_headers(access_token)
+        await self._set_gitlab_version(access_token)
+
+        # Check if user is a member of any group in the allowed list
+        for group in map(url_escape, self.allowed_gitlab_groups):
+            url = "%s/groups/%s/members/%s%d" % (
+                self.gitlab_api,
+                quote(group, safe=''),
+                self.member_api_variant,
+                user_id,
+            )
+            resp = await self.httpfetch(
+                url,
+                parse_json=False,
+                raise_error=False,
+                method="GET",
+                headers=headers,
+                validate_cert=self.validate_server_cert,
+            )
+            if resp.code == 200:
+                return True  # user _is_ in group
+        return False
+
+    async def _check_membership_allowed_project_ids(self, user_id, access_token):
+        headers = _api_headers(access_token)
+        await self._set_gitlab_version(access_token)
+
+        # Check if user has developer access to any project in the allowed list
+        for project in self.allowed_project_ids:
+            url = "%s/projects/%s/members/%s%d" % (
+                self.gitlab_api,
+                project,
+                self.member_api_variant,
+                user_id,
+            )
+            resp_json = await self.httpfetch(
+                url,
+                raise_error=False,
+                method="GET",
+                headers=headers,
+                validate_cert=self.validate_server_cert,
+            )
+            if resp_json:
+                access_level = resp_json.get('access_level', 0)
 
-        return user_info
+                # We only allow access level Developer and above
+                # Reference: https://docs.gitlab.com/ee/api/members.html
+                if access_level >= 30:
+                    return True
+        return False
 
 
-class LocalGenericOAuthenticator(LocalAuthenticator, GenericOAuthenticator):
+class LocalGitLabOAuthenticator(LocalAuthenticator, GitLabOAuthenticator):
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/github.py` & `oauthenticator-16.0.0/oauthenticator/github.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,278 +1,265 @@
 """
-Authenticator to use GitHub OAuth with JupyterHub
+A JupyterHub authenticator class for use with GitHub as an identity provider.
 """
 import json
 import os
 import warnings
 
 from jupyterhub.auth import LocalAuthenticator
 from requests.utils import parse_header_links
-from tornado import web
-from tornado.httpclient import HTTPRequest
-from tornado.httputil import url_concat
 from traitlets import Bool, Set, Unicode, default
 
 from .oauth2 import OAuthenticator
 
 
-def _api_headers(access_token):
-    return {
-        "Accept": "application/json",
-        "User-Agent": "JupyterHub",
-        "Authorization": "token {}".format(access_token),
-    }
-
-
 class GitHubOAuthenticator(OAuthenticator):
+    user_auth_state_key = "github_user"
 
-    # see github_scopes.md for details about scope config
-    # set scopes via config, e.g.
-    # c.GitHubOAuthenticator.scope = ['read:org']
-
-    _deprecated_oauth_aliases = {
-        "github_organization_whitelist": ("allowed_organizations", "0.12.0"),
-        **OAuthenticator._deprecated_oauth_aliases,
-    }
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "GitHub")
 
-    login_service = "GitHub"
+    @default("username_claim")
+    def _username_claim_default(self):
+        return "login"
 
-    github_url = Unicode("https://github.com", config=True)
+    github_url = Unicode(
+        config=True,
+        help="""
+        Used to determine the default values for `github_api`, `authorize_url`,
+        `token_url`, and `userdata_url`.
+        """,
+    )
 
     @default("github_url")
     def _github_url_default(self):
         github_url = os.environ.get("GITHUB_URL")
         if not github_url:
             # fallback on older GITHUB_HOST config,
             # treated the same as GITHUB_URL
             host = os.environ.get("GITHUB_HOST")
             if host:
                 if os.environ.get("GITHUB_HTTP"):
                     protocol = "http"
                     warnings.warn(
-                        'Use of GITHUB_HOST with GITHUB_HTTP might be deprecated in the future. '
-                        'Use GITHUB_URL=http://{} to set host and protocol together.'.format(
-                            host
-                        ),
+                        "Use of GITHUB_HOST with GITHUB_HTTP might be deprecated in the future. "
+                        f"Use GITHUB_URL=http://{host} to set host and protocol together.",
                         PendingDeprecationWarning,
                     )
                 else:
                     protocol = "https"
-                github_url = "{}://{}".format(protocol, host)
+                github_url = f"{protocol}://{host}"
 
         if github_url:
             if '://' not in github_url:
                 # ensure protocol is included, assume https if missing
                 github_url = 'https://' + github_url
 
             return github_url
         else:
             # nothing specified, this is the true default
             github_url = "https://github.com"
 
         # ensure no trailing slash
         return github_url.rstrip("/")
 
-    github_api = Unicode("https://api.github.com", config=True)
+    github_api = Unicode(
+        config=True,
+        help="""
+        URL to the GitHub REST API to use.
+
+        Determined based on `github_url` by default and may never need to be
+        explicitly set.
+        """,
+    )
 
     @default("github_api")
     def _github_api_default(self):
         if self.github_url == "https://github.com":
             return "https://api.github.com"
         else:
+            # Only github.com has its api at api.github.com, enterprise server
+            # deployments has it in the same domain path under /api/v3
             return self.github_url + "/api/v3"
 
     @default("authorize_url")
     def _authorize_url_default(self):
-        return "%s/login/oauth/authorize" % (self.github_url)
+        return f"{self.github_url}/login/oauth/authorize"
 
     @default("token_url")
     def _token_url_default(self):
-        return "%s/login/oauth/access_token" % (self.github_url)
-
-    # deprecated names
-    github_client_id = Unicode(config=True, help="DEPRECATED")
-
-    def _github_client_id_changed(self, name, old, new):
-        self.log.warning("github_client_id is deprecated, use client_id")
-        self.client_id = new
-
-    github_client_secret = Unicode(config=True, help="DEPRECATED")
+        return f"{self.github_url}/login/oauth/access_token"
 
-    def _github_client_secret_changed(self, name, old, new):
-        self.log.warning("github_client_secret is deprecated, use client_secret")
-        self.client_secret = new
+    @default("userdata_url")
+    def _userdata_url_default(self):
+        return f"{self.github_api}/user"
 
     client_id_env = 'GITHUB_CLIENT_ID'
     client_secret_env = 'GITHUB_CLIENT_SECRET'
 
-    github_organization_whitelist = Set(
-        help="Deprecated, use `GitHubOAuthenticator.allowed_organizations`",
+    allowed_organizations = Set(
         config=True,
-    )
+        help="""
+        Allow members of organizations or organizations' teams by specifying
+        organization names like `org-a` and/or an organizations' team names like
+        `org-b:team-1`.
+
+        The names can have a human friendly variant with spaces etc, but you
+        should specify the name as seen in a URL. As an example, it should be
+        `jupyterhub:mybinder-org-operators` for the team
+        https://github.com/orgs/jupyterhub/teams/mybinder-org-operators.
 
-    allowed_organizations = Set(
-        config=True, help="Automatically allow members of selected organizations"
+        Requires `read:org` to be set in `scope` to not just allow based on
+        public membership.
+        """,
     )
 
     populate_teams_in_auth_state = Bool(
         False,
+        config=True,
         help="""
         Populates the authentication state dictionary `auth_state` with a key
         `teams` assigned the list of teams the current user is a member of at
         the time of authentication. The list of teams is structured like the
         response of the GitHub API documented in
         https://docs.github.com/en/rest/reference/teams#list-teams-for-the-authenticated-user.
 
         Requires `read:org` to be set in `scope`.
         
         Note that authentication state is only be available to a
         `post_auth_hook` before being discarded unless configured to be
         persisted via `enable_auth_state`. For more information, see
         https://jupyterhub.readthedocs.io/en/stable/reference/authenticators.html#authentication-state.
         """,
-        config=True,
     )
 
-    async def authenticate(self, handler, data=None):
-        """We set up auth_state based on additional GitHub info if we
-        receive it.
-        """
-        code = handler.get_argument("code")
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "github_client_id": ("client_id", "0.1.0"),
+        "github_client_secret": ("client_secret", "0.1.0"),
+        "github_organization_whitelist": ("allowed_organizations", "0.12.0"),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    github_client_id = Unicode(
+        config=True,
+        help="""
+        .. deprecated:: 0.1
 
-        # Exchange the OAuth code for a GitHub Access Token
-        #
-        # See: https://docs.github.com/en/developers/apps/building-oauth-apps/authorizing-oauth-apps
+           Use :attr:`client_id`.
+        """,
+    )
+    github_client_secret = Unicode(
+        config=True,
+        help="""
+        .. deprecated:: 0.1
 
-        # GitHub specifies a POST request yet requires URL parameters
-        params = dict(
-            client_id=self.client_id, client_secret=self.client_secret, code=code
-        )
+           Use :attr:`client_secret`.
+        """,
+    )
+    github_organization_whitelist = Set(
+        config=True,
+        help="""
+        .. deprecated:: 0.12
 
-        url = url_concat(self.token_url, params)
+           Use :attr:`allowed_organizations`.
+        """,
+    )
 
-        req = HTTPRequest(
-            url,
-            method="POST",
-            headers={"Accept": "application/json"},
-            body='',  # Body is required for a POST...
-            validate_cert=self.validate_server_cert,
-        )
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        `allowed_organizations`.
+        """
+        if await super().check_allowed(username, auth_model):
+            return True
 
-        resp_json = await self.fetch(req)
+        if self.allowed_organizations:
+            access_token = auth_model["auth_state"]["token_response"]["access_token"]
+            token_type = auth_model["auth_state"]["token_response"]["token_type"]
+            for org_team in self.allowed_organizations:
+                if await self._check_membership_allowed_organizations(
+                    org_team, username, access_token, token_type
+                ):
+                    return True
+            message = f"User {username} is not part of allowed_organizations"
+            self.log.warning(message)
 
-        if 'access_token' in resp_json:
-            access_token = resp_json['access_token']
-        elif 'error_description' in resp_json:
-            raise web.HTTPError(
-                403,
-                "An access token was not returned: {}".format(
-                    resp_json['error_description']
-                ),
-            )
-        else:
-            raise web.HTTPError(500, "Bad response: {}".format(resp_json))
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
-        granted_scopes = []
-        if resp_json.get("scope"):
-            granted_scopes = resp_json["scope"].split(",")
-
-        # Determine who the logged-in user is
-        req = HTTPRequest(
-            self.github_api + "/user",
-            method="GET",
-            headers=_api_headers(access_token),
-            validate_cert=self.validate_server_cert,
-        )
-        resp_json = await self.fetch(req, "fetching user info")
+    async def update_auth_model(self, auth_model):
+        """
+        Fetch and store `email` in auth state if the user's only was: private,
+        not part of the initial response, and we was granted a scope to fetch
+        the private email.
+
+        Also fetch and store `teams` in auth state if
+        `populate_teams_in_auth_state` is configured.
+        """
+        user_info = auth_model["auth_state"][self.user_auth_state_key]
 
-        username = resp_json["login"]
-        # username is now the GitHub userid.
-        if not username:
-            return None
-        # Check if user is a member of any allowed organizations.
-        # This check is performed here, as it requires `access_token`.
-        if self.allowed_organizations:
-            for org in self.allowed_organizations:
-                user_in_org = await self._check_membership_allowed_organizations(
-                    org, username, access_token
-                )
-                if user_in_org:
-                    break
-            else:  # User not found in member list for any organisation
-                self.log.warning("User %s is not in allowed org list", username)
-                return None
-        userdict = {"name": username}
-        # Now we set up auth_state
-        userdict["auth_state"] = auth_state = {}
-        # Save the access token and full GitHub reply (name, id, email) in auth state
-        # These can be used for user provisioning in the Lab/Notebook environment.
-        # e.g.
-        #  1) stash the access token
-        #  2) use the GitHub ID as the id
-        #  3) set up name/email for .gitconfig
-        auth_state['access_token'] = access_token
-        # store the whole user model in auth_state.github_user
-        auth_state['github_user'] = resp_json
         # If a public email is not available, an extra API call has to be made
         # to a /user/emails using the access token to retrieve emails. The
         # scopes relevant for this are checked based on this documentation:
         # - about scopes: https://docs.github.com/en/developers/apps/building-oauth-apps/scopes-for-oauth-apps#available-scopes
         # - about /user/emails: https://docs.github.com/en/rest/reference/users#list-email-addresses-for-the-authenticated-user
         #
         # Note that the read:user scope does not imply the user:emails scope!
-        if not auth_state['github_user']['email'] and (
-            'user' in granted_scopes or 'user:email' in granted_scopes
+        access_token = auth_model["auth_state"]["token_response"]["access_token"]
+        token_type = auth_model["auth_state"]["token_response"]["token_type"]
+        granted_scopes = auth_model["auth_state"].get("scope", [])
+        if not user_info["email"] and (
+            "user" in granted_scopes or "user:email" in granted_scopes
         ):
-            req = HTTPRequest(
-                self.github_api + "/user/emails",
+            resp_json = await self.httpfetch(
+                f"{self.github_api}/user/emails",
+                "fetching user emails",
                 method="GET",
-                headers=_api_headers(access_token),
+                headers=self.build_userdata_request_headers(access_token, token_type),
                 validate_cert=self.validate_server_cert,
             )
-            resp_json = await self.fetch(req, "fetching user emails")
             for val in resp_json:
                 if val["primary"]:
-                    auth_state['github_user']['email'] = val['email']
+                    user_info["email"] = val["email"]
                     break
 
         if self.populate_teams_in_auth_state:
-            if 'read:org' not in self.scope:
-                # This means the 'read:org' scope was not set, and we can't fetch teams
+            if "read:org" not in self.scope:
+                # This means the "read:org" scope was not set, and we can't
+                # fetch teams
                 self.log.error(
-                    'read:org scope is required for populate_teams_in_auth_state functionality to work'
+                    "read:org scope is required for populate_teams_in_auth_state functionality to work"
                 )
             else:
-                # Number of teams to request per page
-                per_page = 100
-
-                #  https://docs.github.com/en/rest/reference/teams#list-teams-for-the-authenticated-user
-                url = self.github_api + f"/user/teams?per_page={per_page}"
-
-                auth_state['teams'] = await self._paginated_fetch(url, access_token)
+                # https://docs.github.com/en/rest/teams/teams?apiVersion=2022-11-28#list-teams-for-the-authenticated-user
+                url = f"{self.github_api}/user/teams?per_page=100"
+                user_teams = await self._paginated_fetch(url, access_token, token_type)
+                auth_model["auth_state"]["teams"] = user_teams
 
-        return userdict
+        return auth_model
 
-    async def _paginated_fetch(self, api_url, access_token):
+    async def _paginated_fetch(self, api_url, access_token, token_type):
         """
         Fetch all items via a paginated GitHub API call
 
         Makes a request to api_url, and if pagination information is returned,
         keep paginating until all the items are retrieved.
         """
         url = api_url
         content = []
         while True:
-            req = HTTPRequest(
+            resp = await self.httpfetch(
                 url,
+                "fetching user teams",
+                parse_json=False,
                 method="GET",
-                headers=_api_headers(access_token),
+                headers=self.build_userdata_request_headers(access_token, token_type),
                 validate_cert=self.validate_server_cert,
             )
-            resp = await self.fetch(req, "fetching user teams", parse_json=False)
 
             resp_json = json.loads(resp.body.decode())
             content += resp_json
 
             # Check if a Link header is present, with a collection of pagination links
             links_header = resp.headers.get('Link')
             if not links_header:
@@ -294,60 +281,57 @@
             if next_url is not None:
                 url = next_url
             else:
                 break
         return content
 
     async def _check_membership_allowed_organizations(
-        self, org, username, access_token
+        self, org_team, username, access_token, token_type
     ):
-        headers = _api_headers(access_token)
-        # Check membership of user `username` for organization `org` via api [check-membership](https://docs.github.com/en/rest/orgs/members#check-membership)
-        # With empty scope (even if authenticated by an org member), this
-        # will only await public org members.  You want 'read:org' in order
-        # to be able to iterate through all members. If you would only like to
-        # allow certain teams within an organisation, specify
-        # allowed_organisations = {org_name:team_name}
-
-        check_membership_url = self._build_check_membership_url(org, username)
+        """
+        Checks if a user is part of an organization or organization's team via
+        GitHub's REST API. The `read:org` scope is required to not only check
+        for public org/team membership.
+
+        The `org_team` parameter accepts values like `org-a` or `org-b:team-1`,
+        and will adjust to use a the relevant REST API to check either org or
+        team membership.
+        """
+        headers = self.build_userdata_request_headers(access_token, token_type)
 
-        req = HTTPRequest(
-            check_membership_url,
+        if ":" in org_team:
+            # check if user is part of an organization's team
+            # https://docs.github.com/en/rest/teams/members?apiVersion=2022-11-28#get-team-member-legacy
+            org, team = org_team.split(":")
+            api_url = f"{self.github_api}/orgs/{org}/teams/{team}/members/{username}"
+        else:
+            # check if user is part of an organization
+            # https://docs.github.com/en/rest/orgs/members?apiVersion=2022-11-28#check-organization-membership-for-a-user
+            org = org_team
+            api_url = f"{self.github_api}/orgs/{org}/members/{username}"
+
+        self.log.debug(f"Checking GitHub organization membership: {username} in {org}?")
+        resp = await self.httpfetch(
+            api_url,
+            parse_json=False,
+            raise_error=False,
             method="GET",
             headers=headers,
             validate_cert=self.validate_server_cert,
         )
-        self.log.debug(
-            "Checking GitHub organization membership: %s in %s?", username, org
-        )
-        resp = await self.fetch(req, raise_error=False, parse_json=False)
         if resp.code == 204:
-            self.log.info("Allowing %s as member of %s", username, org)
+            self.log.debug(f"Allowing {username} as member of {org_team}")
             return True
         else:
             try:
                 resp_json = json.loads((resp.body or b'').decode('utf8', 'replace'))
                 message = resp_json.get('message', '')
             except ValueError:
                 message = ''
             self.log.debug(
-                "%s does not appear to be a member of %s (status=%s): %s",
-                username,
-                org,
-                resp.code,
-                message,
+                f"{username} does not appear to be a member of {org_team} (status={resp.code}): {message}",
             )
         return False
 
-    def _build_check_membership_url(self, org: str, username: str) -> str:
-        if ":" in org:
-            org, team = org.split(":")
-            return f"{self.github_api}/orgs/{org}/teams/{team}/members/{username}"
-        else:
-            return f"{self.github_api}/orgs/{org}/members/{username}"
-
 
 class LocalGitHubOAuthenticator(LocalAuthenticator, GitHubOAuthenticator):
-
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/globus.py` & `oauthenticator-16.0.0/oauthenticator/globus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
-Custom Authenticator to use Globus OAuth2 with JupyterHub
+A JupyterHub authenticator class for use with Globus as an identity provider.
 """
 import base64
 import os
 import pickle
 import urllib
 
 from jupyterhub.auth import LocalAuthenticator
-from tornado.httpclient import HTTPRequest
-from tornado.web import HTTPError
+from tornado import web
 from traitlets import Bool, List, Set, Unicode, default
 
 from .oauth2 import OAuthenticator, OAuthLogoutHandler
 
 
 class GlobusLogoutHandler(OAuthLogoutHandler):
     """
@@ -34,15 +33,16 @@
             # return after the redirect to avoid exceptions.
             self.redirect(self.authenticator.logout_redirect_url)
             return
         await super().get()
 
     async def handle_logout(self):
         """Overridden method for custom logout functionality. Should be called by
-        Jupyterhub on logout just before destroying the users session to log them out."""
+        Jupyterhub on logout just before destroying the users session to log them out.
+        """
         await super().handle_logout()
 
         if self.current_user and self.authenticator.revoke_tokens_on_logout:
             await self.clear_tokens(self.current_user)
 
     async def clear_tokens(self, user):
         """Revoke and clear user tokens from the database"""
@@ -55,70 +55,95 @@
                 )
             )
             state['tokens'] = {}
             await user.save_auth_state(state)
 
 
 class GlobusOAuthenticator(OAuthenticator):
-    """The Globus OAuthenticator handles both authorization and passing
-    transfer tokens to the spawner."""
+    """
+    The Globus OAuthenticator handles authentication, authorization, and sets
+    transfer tokens on the spawner environment variables via a pre_spawn_start
+    hook.
+    """
 
-    login_service = 'Globus'
     logout_handler = GlobusLogoutHandler
 
+    user_auth_state_key = "globus_user"
+
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "Globus")
+
     @default("userdata_url")
     def _userdata_url_default(self):
         return "https://auth.globus.org/v2/oauth2/userinfo"
 
     @default("authorize_url")
     def _authorize_url_default(self):
         return "https://auth.globus.org/v2/oauth2/authorize"
 
-    @default("revocation_url")
-    def _revocation_url_default(self):
-        return "https://auth.globus.org/v2/oauth2/token/revoke"
-
-    revocation_url = Unicode(help="Globus URL to revoke live tokens.").tag(config=True)
-
     @default("token_url")
     def _token_url_default(self):
         return "https://auth.globus.org/v2/oauth2/token"
 
-    globus_groups_url = Unicode(help="Globus URL to get list of user's Groups.").tag(
-        config=True
+    revocation_url = Unicode(
+        "https://auth.globus.org/v2/oauth2/token/revoke",
+        config=True,
+        help="""
+        Globus URL to revoke live tokens.
+        """,
     )
 
-    @default("globus_groups_url")
-    def _globus_groups_url_default(self):
-        return "https://groups.api.globus.org/v2/groups/my_groups"
+    globus_groups_url = Unicode(
+        "https://groups.api.globus.org/v2/groups/my_groups",
+        config=True,
+        help="""
+        Globus URL to get list of user's Groups.
+        """,
+    )
 
     identity_provider = Unicode(
-        help="""Restrict which institution a user
-    can use to login (GlobusID, University of Hogwarts, etc.). This should
-    be set in the app at developers.globus.org, but this acts as an additional
-    check to prevent unnecessary account creation."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        Restrict which institution (domain) a user can use to login (GlobusID,
+        University of Hogwarts, etc.). This should be set in the app at
+        developers.globus.org, but this acts as an additional check to prevent
+        unnecessary account creation.
+
+        Note that users with an associated email domains must still be allowed
+        via another config, such as `allow_all`.
+        """,
+    )
 
     def _identity_provider_default(self):
         return os.getenv('IDENTITY_PROVIDER', '')
 
     username_from_email = Bool(
-        help="""Create username from email address, not preferred username. If
-        an identity provider is specified, email address must be from the same
-        domain. Email scope will be set automatically."""
-    ).tag(config=True)
+        False,
+        config=True,
+        help="""
+        Create username from email address, not preferred username. If an
+        identity provider is specified, email address must be from the same
+        domain. Email scope will be set automatically.
+        """,
+    )
 
-    @default("username_from_email")
-    def _username_from_email_default(self):
-        return False
+    @default("username_claim")
+    def _username_claim_default(self):
+        if self.username_from_email:
+            return "email"
+        return "preferred_username"
 
     exclude_tokens = List(
-        help="""Exclude tokens from being passed into user environments
-        when they start notebooks, Terminals, etc."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        Exclude tokens from being passed into user environments when they start
+        notebooks, Terminals, etc.
+        """,
+    )
 
     def _exclude_tokens_default(self):
         return ['auth.globus.org', 'groups.api.globus.org']
 
     def _scope_default(self):
         scopes = [
             'openid',
@@ -130,80 +155,75 @@
                 'urn:globus:auth:scope:groups.api.globus.org:view_my_groups_and_memberships'
             )
         if self.username_from_email:
             scopes.append('email')
         return scopes
 
     globus_local_endpoint = Unicode(
-        help="""If Jupyterhub is also a Globus
-    endpoint, its endpoint id can be specified here."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        If JupyterHub is also a Globus endpoint, its endpoint id can be
+        specified here.
+        """,
+    )
 
     def _globus_local_endpoint_default(self):
         return os.getenv('GLOBUS_LOCAL_ENDPOINT', '')
 
     revoke_tokens_on_logout = Bool(
-        help="""Revoke tokens so they cannot be used again. Single-user servers
-        MUST be restarted after logout in order to get a fresh working set of
-        tokens."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        Revoke tokens so they cannot be used again. Single-user servers MUST be
+        restarted after logout in order to get a fresh working set of tokens.
+        """,
+    )
 
     def _revoke_tokens_on_logout_default(self):
         return False
 
     allowed_globus_groups = Set(
-        help="""Allow members of defined Globus Groups to access JupyterHub. Users in an
-        admin Globus Group are also automatically allowed. Groups are specified with their UUIDs. Setting this will
-        add the Globus Groups scope."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        Allow members of selected Globus groups to sign in. Globus groups should
+        be specified using their UUIDs.
+
+        If this is configured, the default value of the scope configuration is
+        appended with the scope
+        `urn:globus:auth:scope:groups.api.globus.org:view_my_groups_and_memberships`.
+        """,
+    )
 
     admin_globus_groups = Set(
-        help="""Set members of defined Globus Groups as JupyterHub admin users.
-        These users are automatically allowed to login to JupyterHub. Groups are specified with
-        their UUIDs. Setting this will add the Globus Groups scope."""
-    ).tag(config=True)
+        config=True,
+        help="""
+        Allow members of selected Globus groups to sign in and consider them as
+        JupyterHub admins. Globus groups should be specified using their UUIDs.
+
+        If this is set and a user isn't part of one of these groups or listed in
+        `admin_users`, a user signing in will have their admin status revoked.
+
+        If this is configured, the default value of the scope configuration is
+        appended with the scope
+        `urn:globus:auth:scope:groups.api.globus.org:view_my_groups_and_memberships`.
+        """,
+    )
 
     async def pre_spawn_start(self, user, spawner):
-        """Add tokens to the spawner whenever the spawner starts a notebook.
+        """
+        Add tokens to the spawner whenever the spawner starts a notebook.
         This will allow users to create a transfer client:
         globus-sdk-python.readthedocs.io/en/stable/tutorial/#tutorial-step4
         """
         spawner.environment['GLOBUS_LOCAL_ENDPOINT'] = self.globus_local_endpoint
         state = await user.get_auth_state()
         if state:
             globus_data = base64.b64encode(pickle.dumps(state))
             spawner.environment['GLOBUS_DATA'] = globus_data.decode('utf-8')
 
-    async def authenticate(self, handler, data=None):
-        """
-        Authenticate with globus.org. Usernames (and therefore Jupyterhub
-        accounts) will correspond to a Globus User ID, so foouser@globusid.org
-        will have the 'foouser' account in Jupyterhub.
-        """
-        # Complete login and exchange the code for tokens.
-        params = dict(
-            redirect_uri=self.get_callback_url(handler),
-            code=handler.get_argument("code"),
-            grant_type='authorization_code',
-        )
-        req = HTTPRequest(
-            self.token_url,
-            method="POST",
-            headers=self.get_client_credential_headers(),
-            body=urllib.parse.urlencode(params),
-        )
-        token_json = await self.fetch(req)
-
-        # Fetch user info at Globus's oauth2/userinfo/ HTTP endpoint to get the username
-        user_headers = self.get_default_headers()
-        user_headers['Authorization'] = 'Bearer {}'.format(token_json['access_token'])
-        req = HTTPRequest(self.userdata_url, method='GET', headers=user_headers)
-        user_resp = await self.fetch(req)
-        username = self.get_username(user_resp)
-
+    def get_globus_tokens(self, token_info):
         # Each token should have these attributes. Resource server is optional,
         # and likely won't be present.
         token_attrs = [
             'expires_in',
             'resource_server',
             'scope',
             'token_type',
@@ -211,128 +231,166 @@
             'access_token',
         ]
         # The Auth Token is a bit special, it comes back at the top level with the
         # id token. The id token has some useful information in it, but nothing that
         # can't be retrieved with an Auth token.
         # Repackage the Auth token into a dict that looks like the other tokens
         auth_token_dict = {
-            attr_name: token_json.get(attr_name) for attr_name in token_attrs
+            attr_name: token_info.get(attr_name) for attr_name in token_attrs
         }
         # Make sure only the essentials make it into tokens. Other items, such as 'state' are
         # not needed after authentication and can be discarded.
         other_tokens = [
             {attr_name: token_dict.get(attr_name) for attr_name in token_attrs}
-            for token_dict in token_json['other_tokens']
+            for token_dict in token_info['other_tokens']
         ]
-        tokens = other_tokens + [auth_token_dict]
+        return other_tokens + [auth_token_dict]
+
+    def build_auth_state_dict(self, token_info, user_info):
+        """
+        Usernames (and therefore Jupyterhub
+        accounts) will correspond to a Globus User ID, so foouser@globusid.org
+        will have the 'foouser' account in Jupyterhub.
+        """
+        tokens = self.get_globus_tokens(token_info)
         # historically, tokens have been organized by resource server for convenience.
         # If multiple scopes are requested from the same resource server, they will be
         # combined into a single token from Globus Auth.
         by_resource_server = {
             token_dict['resource_server']: token_dict
             for token_dict in tokens
             if token_dict['resource_server'] not in self.exclude_tokens
         }
 
-        user_info = {
-            'name': username,
-            'auth_state': {
-                'client_id': self.client_id,
-                'tokens': by_resource_server,
-            },
+        return {
+            'client_id': self.client_id,
+            'tokens': by_resource_server,
+            'token_response': token_info,
+            self.user_auth_state_key: user_info,
         }
-        use_globus_groups = False
-        user_allowed = False
+
+    async def _fetch_users_groups(self, tokens):
+        user_groups = set()
+        # Get Groups access token, may not be in dict headed to auth state
+        for token_dict in tokens:
+            if token_dict['resource_server'] == 'groups.api.globus.org':
+                groups_token = token_dict['access_token']
+        # Get list of user's Groups
+        groups_headers = self.get_default_headers()
+        groups_headers['Authorization'] = f'Bearer {groups_token}'
+        groups_resp = await self.httpfetch(
+            self.globus_groups_url, method='GET', headers=groups_headers
+        )
+        # Build set of Group IDs
+        for group in groups_resp:
+            user_groups.add(group['id'])
+
+        return user_groups
+
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        `allowed_globus_groups`.
+        """
+        # before considering allowing a username by being recognized in a list
+        # of usernames or similar, we must ensure that the authenticated user is
+        # from an allowed identity provider domain.
+        if self.identity_provider:
+            # It's possible for identity provider domains to be namespaced
+            # https://docs.globus.org/api/auth/specification/#identity_provider_namespaces
+            user_info = auth_model["auth_state"][self.user_auth_state_key]
+            user_domain = user_info.get(self.username_claim).split('@', 1)[-1]
+            if user_domain != self.identity_provider:
+                message = f"This site is restricted to {self.identity_provider} accounts. Link your account at app.globus.org/account."
+                self.log.warning(message)
+                raise web.HTTPError(403, message)
+
+        if await super().check_allowed(username, auth_model):
+            return True
+
+        if self.allowed_globus_groups:
+            user_groups = auth_model["auth_state"]["globus_groups"]
+            if any(user_groups & self.allowed_globus_groups):
+                return True
+            self.log.warning(f"{username} not in an allowed Globus Group")
+
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
+
+    async def update_auth_model(self, auth_model):
+        """
+        Fetch and store `globus_groups` in auth state if `allowed_globus_groups`
+        or `admin_globus_groups` is configured.
+
+        Sets admin status to True or False if `admin_globus_groups` is
+        configured and the user isn't part of `admin_users`. Note that leaving
+        it at None makes users able to retain an admin status while setting it
+        to False makes it be revoked.
+        """
+        user_groups = set()
         if self.allowed_globus_groups or self.admin_globus_groups:
-            # If any of these configurations are set, user must be in the allowed or admin Globus Group
-            use_globus_groups = True
-            user_group_ids = set()
-            # Get Groups access token, may not be in dict headed to auth state
-            for token_dict in tokens:
-                if token_dict['resource_server'] == 'groups.api.globus.org':
-                    groups_token = token_dict['access_token']
-            # Get list of user's Groups
-            groups_headers = self.get_default_headers()
-            groups_headers['Authorization'] = 'Bearer {}'.format(groups_token)
-            req = HTTPRequest(
-                self.globus_groups_url, method='GET', headers=groups_headers
-            )
-            groups_resp = await self.fetch(req)
-            # Build set of Group IDs
-            for group in groups_resp:
-                user_group_ids.add(group['id'])
-            if user_group_ids & self.allowed_globus_groups:
-                user_allowed = True
-            if self.admin_globus_groups:
-                # Admin users are being managed via Globus Groups
-                # Default to False
-                user_info['admin'] = False
-                if user_group_ids & self.admin_globus_groups:
-                    # User is an admin, admins allowed by default
-                    user_allowed = user_info['admin'] = True
-
-        if user_allowed or not use_globus_groups:
-            return user_info
-        else:
-            self.log.warning('{} not in an allowed Globus Group'.format(username))
-            return None
-
-    def get_username(self, user_data):
-        # It's possible for identity provider domains to be namespaced
-        # https://docs.globus.org/api/auth/specification/#identity_provider_namespaces # noqa
-        username_field = 'preferred_username'
-        if self.username_from_email:
-            username_field = 'email'
-        username, domain = user_data.get(username_field).split('@', 1)
-        if self.identity_provider and domain != self.identity_provider:
-            raise HTTPError(
-                403,
-                'This site is restricted to {} accounts. Please link your {}'
-                ' account at {}.'.format(
-                    self.identity_provider,
-                    self.identity_provider,
-                    'globus.org/app/account',
-                ),
-            )
-        return username
+            tokens = self.get_globus_tokens(auth_model["auth_state"]["token_response"])
+            user_groups = await self._fetch_users_groups(tokens)
+        auth_model["auth_state"]["globus_groups"] = user_groups
+
+        if auth_model["admin"]:
+            # auth_model["admin"] being True means the user was in admin_users
+            return auth_model
+
+        if self.admin_globus_groups:
+            # admin status should in this case be True or False, not None
+            auth_model["admin"] = any(user_groups & self.admin_globus_groups)
+
+        return auth_model
+
+    def user_info_to_username(self, user_info):
+        """
+        Usernames (and therefore Jupyterhub
+        accounts) will correspond to a Globus User ID, so foouser@globusid.org
+        will have the 'foouser' account in Jupyterhub.
+        """
+        return user_info.get(self.username_claim).split('@')[0]
 
     def get_default_headers(self):
         return {"Accept": "application/json", "User-Agent": "JupyterHub"}
 
     def get_client_credential_headers(self):
         headers = self.get_default_headers()
         b64key = base64.b64encode(
-            bytes("{}:{}".format(self.client_id, self.client_secret), "utf8")
+            bytes(f"{self.client_id}:{self.client_secret}", "utf8")
         )
         headers["Authorization"] = "Basic {}".format(b64key.decode("utf8"))
         return headers
 
     async def revoke_service_tokens(self, services):
-        """Revoke live Globus access and refresh tokens. Revoking inert or
-        non-existent tokens does nothing. Services are defined by dicts
-        returned by tokens.by_resource_server, for example:
-        services = { 'transfer.api.globus.org': {'access_token': 'token'}, ...
-            <Additional services>...
-        }
+        """
+        Revoke live Globus access and refresh tokens.
+
+        Revoking inert or non-existent tokens does nothing.
+        Services are defined by dicts returned by `tokens.by_resource_server`.
+
+        For example::
+
+            services = {
+                'transfer.api.globus.org': {'access_token': 'token'},
+                <Additional services>...
+            }
         """
         access_tokens = [
             token_dict.get('access_token') for token_dict in services.values()
         ]
         refresh_tokens = [
             token_dict.get('refresh_token') for token_dict in services.values()
         ]
         all_tokens = [tok for tok in access_tokens + refresh_tokens if tok is not None]
 
         for token in all_tokens:
-            req = HTTPRequest(
+            await self.httpfetch(
                 self.revocation_url,
                 method="POST",
                 headers=self.get_client_credential_headers(),
                 body=urllib.parse.urlencode({'token': token}),
             )
-            await self.fetch(req)
 
 
 class LocalGlobusOAuthenticator(LocalAuthenticator, GlobusOAuthenticator):
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/google.py` & `oauthenticator-16.0.0/oauthenticator/google.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,97 +1,124 @@
 """
-Custom Authenticator to use Google OAuth with JupyterHub.
-
-Derived from the GitHub OAuth authenticator.
+A JupyterHub authenticator class for use with Google as an identity provider.
 """
 import os
-import urllib.parse
 
 from jupyterhub.auth import LocalAuthenticator
-from jupyterhub.crypto import EncryptionUnavailable, InvalidToken, decrypt
 from tornado.auth import GoogleOAuth2Mixin
-from tornado.httpclient import HTTPRequest
-from tornado.httputil import url_concat
 from tornado.web import HTTPError
-from traitlets import Dict, List, Unicode, default, validate
+from traitlets import Dict, List, Set, Unicode, default, validate
 
 from .oauth2 import OAuthenticator
 
 
-def check_user_in_groups(member_groups, allowed_groups):
-    # Check if user is a member of any group in the allowed groups
-    if any(g in member_groups for g in allowed_groups):
-        return True  # user _is_ in group
-    else:
-        return False
+class GoogleOAuthenticator(OAuthenticator, GoogleOAuth2Mixin):
+    user_auth_state_key = "google_user"
 
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "Google")
 
-class GoogleOAuthenticator(OAuthenticator, GoogleOAuth2Mixin):
-    _deprecated_oauth_aliases = {
-        "google_group_whitelist": ("allowed_google_groups", "0.12.0"),
-        **OAuthenticator._deprecated_oauth_aliases,
-    }
+    @default("scope")
+    def _scope_default(self):
+        return ["openid", "email"]
 
-    google_api_url = Unicode("https://www.googleapis.com", config=True)
+    @default("username_claim")
+    def _username_claim_default(self):
+        return "email"
 
-    @default('google_api_url')
+    @default("authorize_url")
+    def _authorize_url_default(self):
+        return "https://accounts.google.com/o/oauth2/v2/auth"
+
+    google_api_url = Unicode(
+        config=True,
+        help="""
+        Used to determine the default values for `token_url` and `userdata_url`.
+        """,
+    )
+
+    @default("google_api_url")
     def _google_api_url(self):
         """get default google apis url from env"""
         google_api_url = os.getenv('GOOGLE_API_URL')
 
         # default to googleapis.com
         if not google_api_url:
             google_api_url = 'https://www.googleapis.com'
 
         return google_api_url
 
-    @default('scope')
-    def _scope_default(self):
-        return ['openid', 'email']
-
-    @default("authorize_url")
-    def _authorize_url_default(self):
-        return "https://accounts.google.com/o/oauth2/v2/auth"
-
     @default("token_url")
     def _token_url_default(self):
-        return "%s/oauth2/v4/token" % (self.google_api_url)
+        return f"{self.google_api_url}/oauth2/v4/token"
+
+    @default("userdata_url")
+    def _userdata_url_default(self):
+        return f"{self.google_api_url}/oauth2/v1/userinfo"
 
     google_service_account_keys = Dict(
         Unicode(),
-        help="Service account keys to use with each domain, see https://developers.google.com/admin-sdk/directory/v1/guides/delegation",
-    ).tag(config=True)
+        config=True,
+        help="""
+        Service account keys to use with each domain, see https://developers.google.com/admin-sdk/directory/v1/guides/delegation
+
+        Required if and only if `allowed_google_groups` or `admin_google_groups`
+        is configured.
+        """,
+    )
 
     gsuite_administrator = Dict(
         Unicode(),
-        help="Username of a G Suite Administrator for the service account to act as",
-    ).tag(config=True)
-
-    google_group_whitelist = Dict(
-        help="Deprecated, use `GoogleOAuthenticator.allowed_google_groups`",
         config=True,
+        help="""
+        Username of a G Suite Administrator for the service account to act as.
+
+        Required if and only if `allowed_google_groups` or `admin_google_groups`
+        is configured.
+        """,
     )
 
     allowed_google_groups = Dict(
-        List(Unicode()), help="Automatically allow members of selected groups"
-    ).tag(config=True)
+        Set(Unicode()),
+        config=True,
+        help="""
+        Allow members of selected Google groups to sign in.
+
+        Use of this requires configuration of `gsuite_administrator` and
+        `google_service_account_keys`.
+        """,
+    )
 
     admin_google_groups = Dict(
-        List(Unicode()),
-        help="Groups whose members should have Jupyterhub admin privileges",
-    ).tag(config=True)
+        Set(Unicode()),
+        config=True,
+        help="""
+        Allow members of selected Google groups to sign in and consider them as
+        JupyterHub admins.
 
-    user_info_url = Unicode(
-        "https://www.googleapis.com/oauth2/v1/userinfo", config=True
+        If this is set and a user isn't part of one of these groups or listed in
+        `admin_users`, a user signing in will have their admin status revoked.
+
+        Use of this requires configuration of `gsuite_administrator` and
+        `google_service_account_keys`.
+        """,
     )
 
     hosted_domain = List(
         Unicode(),
         config=True,
-        help="""List of domains used to restrict sign-in, e.g. mycollege.edu""",
+        help="""
+        Restrict sign-in to a list of email domain names, such as
+        `["mycollege.edu"]`.
+
+        Note that users with email domains in this list must still be allowed
+        via another config, such as `allow_all`, `allowed_users`, or
+        `allowed_google_groups`.
+        """,
     )
 
     @default('hosted_domain')
     def _hosted_domain_from_env(self):
         domains = []
         for domain in os.environ.get('HOSTED_DOMAIN', '').split(';'):
             if domain:
@@ -105,142 +132,121 @@
         """handle backward-compatibility with hosted_domain is a single domain as a string"""
         if isinstance(proposal.value, str):
             # pre-0.9 hosted_domain was a string
             # set it to a single item list
             # (or if it's empty, an empty list)
             if proposal.value == '':
                 return []
-            return [proposal.value]
-        return proposal.value
+            return [proposal.value.lower()]
+        return [hd.lower() for hd in proposal.value]
 
-    login_service = Unicode(
-        os.environ.get('LOGIN_SERVICE', 'Google'),
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "google_group_whitelist": ("allowed_google_groups", "0.12.0"),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    google_group_whitelist = Dict(
         config=True,
-        help="""Google Apps hosted domain string, e.g. My College""",
-    )
-
-    username_claim = Unicode(
-        "email",
-        help="""Field in userinfo reply to use for username
+        help="""
+        .. deprecated:: 0.12
 
-        Default: 'email'
-        Also reasonable: 'sub' for the opaque unique id
+           Use :attr:`allowed_google_groups`.
         """,
-        config=True,
     )
 
-    @default('username_claim')
-    def _username_claim_default(self):
-        return 'email'
+    async def update_auth_model(self, auth_model):
+        """
+        Fetch and store `google_groups` in auth state if `allowed_google_groups`
+        or `admin_google_groups` is configured.
 
-    async def authenticate(self, handler, data=None, google_groups=None):
-        code = handler.get_argument("code")
-        body = urllib.parse.urlencode(
-            dict(
-                code=code,
-                redirect_uri=self.get_callback_url(handler),
-                client_id=self.client_id,
-                client_secret=self.client_secret,
-                grant_type="authorization_code",
+        Sets admin status to True or False if `admin_google_groups` is
+        configured and the user isn't part of `admin_users`. Note that leaving
+        it at None makes users able to retain an admin status while setting it
+        to False makes it be revoked.
+        """
+        user_info = auth_model["auth_state"][self.user_auth_state_key]
+        user_email = user_info["email"]
+        user_domain = user_info["domain"] = user_email.split("@")[1].lower()
+
+        user_groups = set()
+        if self.allowed_google_groups or self.admin_google_groups:
+            user_groups = user_info["google_groups"] = self._fetch_user_groups(
+                user_email, user_domain
             )
-        )
+        user_info["google_groups"] = user_groups
 
-        req = HTTPRequest(
-            self.token_url,
-            method="POST",
-            headers={"Content-Type": "application/x-www-form-urlencoded"},
-            body=body,
-        )
-        user = await self.fetch(req, "completing oauth")
-        access_token = str(user['access_token'])
-        refresh_token = user.get('refresh_token', None)
-
-        req = HTTPRequest(
-            url_concat(
-                self.user_info_url,
-                {'access_token': access_token},
-            )
-        )
-        bodyjs = await self.fetch(req, "fetching user info")
-        user_email = bodyjs['email']
-        user_email_domain = user_email.split('@')[1]
-        username = bodyjs[self.username_claim]
-
-        if not bodyjs['verified_email']:
-            self.log.warning("Google OAuth unverified email attempt: %s", user_email)
-            raise HTTPError(403, "Google email {} not verified".format(user_email))
+        if auth_model["admin"]:
+            # auth_model["admin"] being True means the user was in admin_users
+            return auth_model
 
-        if self.hosted_domain:
-            if user_email_domain not in self.hosted_domain:
-                self.log.warning(
-                    "Google OAuth unauthorized domain attempt: %s", user_email
-                )
-                raise HTTPError(
-                    403,
-                    "Google account domain @{} not authorized.".format(
-                        user_email_domain
-                    ),
-                )
-            if len(self.hosted_domain) == 1 and user_email == username:
-                # unambiguous domain, use only base name
-                username = user_email.split('@')[0]
-
-        if refresh_token is None:
-            self.log.debug(
-                "Refresh token was empty, will try to pull refresh_token from previous auth_state"
-            )
-            user = handler.find_user(username)
+        if self.admin_google_groups:
+            # admin status should in this case be True or False, not None
+            admin_groups = self.admin_google_groups.get(user_domain, set())
+            auth_model["admin"] = any(user_groups & admin_groups)
 
-            if user and user.encrypted_auth_state:
-                self.log.debug(
-                    "encrypted_auth_state was found, will try to decrypt and pull refresh_token from it"
-                )
-                try:
-                    encrypted = user.encrypted_auth_state
-                    auth_state = await decrypt(encrypted)
-                    refresh_token = auth_state.get('refresh_token')
-                except (ValueError, InvalidToken, EncryptionUnavailable) as e:
-                    self.log.warning(
-                        "Failed to retrieve encrypted auth_state for %s because %s",
-                        username,
-                        e,
-                    )
-
-        user_info = {
-            'name': username,
-            'auth_state': {
-                'access_token': access_token,
-                'refresh_token': refresh_token,
-                'google_user': bodyjs,
-            },
-        }
+        return auth_model
 
-        if self.admin_google_groups or self.allowed_google_groups:
-            user_info = await self._add_google_groups_info(user_info, google_groups)
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides the OAuthenticator.check_allowed to also allow users part of
+        `allowed_google_groups`.
+        """
+        # before considering allowing a username by being recognized in a list
+        # of usernames or similar, we must ensure that the authenticated user
+        # has a verified email and is part of hosted_domain if configured.
+        user_info = auth_model["auth_state"][self.user_auth_state_key]
+        user_email = user_info["email"]
+        user_domain = user_info["domain"]
+
+        if not user_info["verified_email"]:
+            message = f"Login with unverified email {user_email} is not allowed"
+            self.log.warning(message)
+            raise HTTPError(403, message)
+
+        # NOTE: If hosted_domain is configured as ["a.com", "b.com"], and
+        #       allowed_google_groups is declared as {"a.com": {"a-group"}}, a
+        #       "b.com" user won't be authorized unless allowed in another way.
+        #
+        #       This means that its not possible to allow all users of a given
+        #       domain if one wants to restrict another.
+        #
+        if self.hosted_domain:
+            if user_domain not in self.hosted_domain:
+                message = f"Login with domain @{user_domain} is not allowed"
+                self.log.warning(message)
+                raise HTTPError(403, message)
+
+        if await super().check_allowed(username, auth_model):
+            return True
+
+        if self.allowed_google_groups:
+            user_groups = user_info["google_groups"]
+            allowed_groups = self.allowed_google_groups.get(user_domain, set())
+            if any(user_groups & allowed_groups):
+                return True
 
-        return user_info
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
     def _service_client_credentials(self, scopes, user_email_domain):
         """
         Return a configured service client credentials for the API.
         """
         try:
             from google.oauth2 import service_account
         except:
             raise ImportError(
                 "Could not import google.oauth2's service_account,"
-                "you may need to run pip install oauthenticator[googlegroups] or not declare google groups"
+                "you may need to run 'pip install oauthenticator[googlegroups]' or not declare google groups"
             )
 
         gsuite_administrator_email = "{}@{}".format(
             self.gsuite_administrator[user_email_domain], user_email_domain
         )
-        self.log.debug(
-            "scopes are %s, user_email_domain is %s", scopes, user_email_domain
-        )
+        self.log.debug(f"scopes are {scopes}, user_email_domain is {user_email_domain}")
         credentials = service_account.Credentials.from_service_account_file(
             self.google_service_account_keys[user_email_domain], scopes=scopes
         )
 
         credentials = credentials.with_subject(gsuite_administrator_email)
 
         return credentials
@@ -250,87 +256,52 @@
         Return a configured service client for the API.
         """
         try:
             from googleapiclient.discovery import build
         except:
             raise ImportError(
                 "Could not import googleapiclient.discovery's build,"
-                "you may need to run pip install oauthenticator[googlegroups] or not declare google groups"
+                "you may need to run 'pip install oauthenticator[googlegroups]' or not declare google groups"
             )
 
         self.log.debug(
-            "service_name is %s, service_version is %s", service_name, service_version
+            f"service_name is {service_name}, service_version is {service_version}"
         )
 
         return build(
             serviceName=service_name,
             version=service_version,
             credentials=credentials,
             cache_discovery=False,
             http=http,
         )
 
-    async def _google_groups_for_user(self, user_email, credentials, http=None):
+    def _fetch_user_groups(self, user_email, user_email_domain, http=None):
         """
-        Return google groups a given user is a member of
+        Return a set with the google groups a given user is a member of
         """
+        # FIXME: When this function is used and waiting for web request
+        #        responses, JupyterHub gets blocked from doing other things.
+        #        Ideally the web requests should be made using an async client
+        #        that can be awaited while JupyterHub handles other things.
+        #
+        credentials = self._service_client_credentials(
+            scopes=[f"{self.google_api_url}/auth/admin.directory.group.readonly"],
+            user_email_domain=user_email_domain,
+        )
         service = self._service_client(
             service_name='admin',
             service_version='directory_v1',
             credentials=credentials,
             http=http,
         )
 
-        results = service.groups().list(userKey=user_email).execute()
-        results = [
-            g['email'].split('@')[0] for g in results.get('groups', [{'email': None}])
-        ]
-        self.log.debug("user_email %s is a member of %s", user_email, results)
-        return results
-
-    async def _add_google_groups_info(self, user_info, google_groups=None):
-        user_email_domain = user_info['auth_state']['google_user']['hd']
-        user_email = user_info['auth_state']['google_user']['email']
-        if google_groups is None:
-            credentials = self._service_client_credentials(
-                scopes=[
-                    '%s/auth/admin.directory.group.readonly' % (self.google_api_url)
-                ],
-                user_email_domain=user_email_domain,
-            )
-            google_groups = await self._google_groups_for_user(
-                user_email=user_email, credentials=credentials
-            )
-        user_info['auth_state']['google_user']['google_groups'] = google_groups
-
-        # Check if user is a member of any admin groups.
-        if self.admin_google_groups:
-            is_admin = check_user_in_groups(
-                google_groups, self.admin_google_groups[user_email_domain]
-            )
-
-        # Check if user is a member of any allowed groups.
-        allowed_groups = self.allowed_google_groups
-
-        if allowed_groups:
-            if user_email_domain in allowed_groups:
-                user_in_group = check_user_in_groups(
-                    google_groups, allowed_groups[user_email_domain]
-                )
-            else:
-                return None
-        else:
-            user_in_group = True
-
-        if self.admin_google_groups and (is_admin or user_in_group):
-            user_info['admin'] = is_admin
-            return user_info
-        elif user_in_group:
-            return user_info
-        else:
-            return None
+        resp = service.groups().list(userKey=user_email).execute()
+        user_groups = {
+            g['email'].split('@')[0] for g in resp.get('groups', [{'email': None}])
+        }
+        self.log.debug(f"user_email {user_email} is a member of {user_groups}")
+        return user_groups
 
 
 class LocalGoogleOAuthenticator(LocalAuthenticator, GoogleOAuthenticator):
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/mediawiki.py` & `oauthenticator-16.0.0/oauthenticator/mediawiki.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
-Custom Authenticator to use MediaWiki OAuth with JupyterHub
-
-Requires `mwoauth` package.
+A JupyterHub authenticator class for use with MediaWiki as an identity provider.
 """
 import json
 import os
 from asyncio import wrap_future
 from concurrent.futures import ThreadPoolExecutor
 
 from jupyterhub.handlers import BaseHandler
 from jupyterhub.utils import url_path_join
 from mwoauth import ConsumerToken, Handshaker
 from mwoauth.tokens import RequestToken
-from traitlets import Any, Integer, Unicode
+from traitlets import Any, Integer, Unicode, default
 
 from oauthenticator import OAuthCallbackHandler, OAuthenticator
 
 # Name of cookie used to pass auth token between the oauth
 # login and authentication phase
 AUTH_REQUEST_COOKIE_NAME = 'mw_oauth_request_token_v2'
 
+
 # Helpers to jsonify/de-jsonify request_token
 # It is a named tuple with bytestrings, json.dumps balks
 def jsonify(request_token):
     return json.dumps(
         [
             request_token.key,
             request_token.secret,
@@ -72,68 +71,87 @@
         pass
 
     def get_state_url(self):
         return None
 
 
 class MWOAuthenticator(OAuthenticator):
-    login_service = 'MediaWiki'
     login_handler = MWLoginHandler
     callback_handler = MWCallbackHandler
 
+    user_auth_state_key = "MEDIAWIKI_USER_IDENTITY"
+
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "MediaWiki")
+
     mw_index_url = Unicode(
         os.environ.get('MW_INDEX_URL', 'https://meta.wikimedia.org/w/index.php'),
         config=True,
-        help='Full path to index.php of the MW instance to use to log in',
+        help="""
+        Full path to index.php of the MW instance to use to log in
+        """,
     )
 
     executor_threads = Integer(
         12,
-        help="""Number of executor threads.
+        config=True,
+        help="""
+        Number of executor threads.
 
         MediaWiki OAuth requests happen in this thread,
         so it is mostly waiting for network replies.
         """,
-        config=True,
     )
+
     executor = Any()
 
+    def _executor_default(self):
+        return ThreadPoolExecutor(self.executor_threads)
+
     def normalize_username(self, username):
         """
-        Override normalize_username to avoid lowercasing usernames
+        Override normalize_username to avoid lowercasing usernames.
         """
+        username = username.replace(' ', '_')
         return username
 
-    def _executor_default(self):
-        return ThreadPoolExecutor(self.executor_threads)
+    def build_access_tokens_request_params(self, handler, data=None):
+        """
+        We're overriding this method because mediawiki needs a Handshaker object
+        to send the tokes request. So, we're building the params directly in the
+        `get_token_info`.
+        """
+        return None
 
-    async def authenticate(self, handler, data=None):
+    async def get_token_info(self, handler, params):
+        # Exchange the OAuth code for an Access Token
         consumer_token = ConsumerToken(
             self.client_id,
             self.client_secret,
         )
 
         handshaker = Handshaker(self.mw_index_url, consumer_token)
         request_token = dejsonify(handler.get_secure_cookie(AUTH_REQUEST_COOKIE_NAME))
         handler.clear_cookie(AUTH_REQUEST_COOKIE_NAME)
         access_token = await wrap_future(
             self.executor.submit(
                 handshaker.complete, request_token, handler.request.query
             )
         )
+        return {"access_token": access_token, "consumer_token": consumer_token}
 
-        identity = await wrap_future(
-            self.executor.submit(handshaker.identify, access_token)
+    async def token_to_user(self, token_info):
+        handshaker = Handshaker(self.mw_index_url, token_info["consumer_token"])
+
+        return await wrap_future(
+            self.executor.submit(handshaker.identify, token_info["access_token"])
         )
-        if identity and 'username' in identity:
-            # this shouldn't be necessary anymore,
-            # but keep for backward-compatibility
-            return {
-                'name': identity['username'].replace(' ', '_'),
-                'auth_state': {
-                    'ACCESS_TOKEN_KEY': access_token.key,
-                    'ACCESS_TOKEN_SECRET': access_token.secret,
-                    'MEDIAWIKI_USER_IDENTITY': identity,
-                },
-            }
-        else:
-            self.log.error("No username found in %s", identity)
+
+    def build_auth_state_dict(self, token_info, user_info):
+        # this shouldn't be necessary anymore,
+        # but keep for backward-compatibility
+        return {
+            'ACCESS_TOKEN_KEY': token_info["access_token"].key,
+            'ACCESS_TOKEN_SECRET': token_info["access_token"].secret,
+            self.user_auth_state_key: user_info,
+        }
```

### Comparing `oauthenticator-15.1.0/oauthenticator/openshift.py` & `oauthenticator-16.0.0/oauthenticator/openshift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,175 +1,187 @@
 """
-Custom Authenticator to use OpenShift OAuth with JupyterHub.
-
-Derived from the GitHub OAuth authenticator.
+A JupyterHub authenticator class for use with OpenShift as an identity provider.
 """
+import json
 import os
 
-import requests
 from jupyterhub.auth import LocalAuthenticator
-from tornado.httpclient import HTTPRequest
-from tornado.httputil import url_concat
+from tornado.httpclient import HTTPClient, HTTPRequest
 from traitlets import Bool, Set, Unicode, default
 
 from oauthenticator.oauth2 import OAuthenticator
 
 
 class OpenShiftOAuthenticator(OAuthenticator):
+    user_auth_state_key = "openshift_user"
 
-    login_service = "OpenShift"
+    @default("scope")
+    def _scope_default(self):
+        return ["user:info"]
+
+    @default("login_service")
+    def _login_service_default(self):
+        return os.environ.get("LOGIN_SERVICE", "OpenShift")
+
+    @default("username_claim")
+    def _username_claim_default(self):
+        return "name"
 
-    scope = ['user:info']
+    @default("http_request_kwargs")
+    def _http_request_kwargs_default(self):
+        ca_cert_file = "/run/secrets/kubernetes.io/serviceaccount/ca.crt"
+        if self.validate_server_cert and os.path.exists(ca_cert_file):
+            return {"ca_certs": ca_cert_file}
+        return {}
 
     openshift_url = Unicode(
         os.environ.get('OPENSHIFT_URL')
         or 'https://openshift.default.svc.cluster.local',
         config=True,
+        help="""
+        Used to determine the default values for `openshift_auth_api_url` and
+        `openshift_rest_api_url`.
+        """,
     )
 
-    validate_cert = Bool(
-        True, config=True, help="Set to False to disable certificate validation"
-    )
-
-    ca_certs = Unicode(config=True)
-
     allowed_groups = Set(
         config=True,
-        help="Set of OpenShift groups that should be allowed to access the hub.",
+        help="""
+        Allow members of selected OpenShift groups to sign in.
+        """,
     )
 
     admin_groups = Set(
         config=True,
-        help="Set of OpenShift groups that should be given admin access to the hub.",
+        help="""
+        Allow members of selected OpenShift groups to sign in and consider them
+        as JupyterHub admins.
+
+        If this is set and a user isn't part of one of these groups or listed in
+        `admin_users`, a user signing in will have their admin status revoked.
+        """,
     )
 
-    @default("ca_certs")
-    def _ca_certs_default(self):
-        ca_cert_file = "/run/secrets/kubernetes.io/serviceaccount/ca.crt"
-        if self.validate_cert and os.path.exists(ca_cert_file):
-            return ca_cert_file
-
-        return ''
-
-    openshift_auth_api_url = Unicode(config=True)
+    openshift_auth_api_url = Unicode(
+        config=True,
+        help="""
+        Used to determine the default values for `authorize_url` and
+        `token_url`.
+
+        By default, this is determined on startup by a request to the
+        `openshift_url` appended with "/.well-known/oauth-authorization-server",
+        where "issuer" is extracted from the response.
+
+        For more context, see the `Obtaining Authorization Server Metadata
+        section <https://datatracker.ietf.org/doc/html/rfc8414#section-3>`_ in
+        an OAuth2 standard document.
+        """,
+    )
 
     @default("openshift_auth_api_url")
     def _openshift_auth_api_url_default(self):
-        auth_info_url = '%s/.well-known/oauth-authorization-server' % self.openshift_url
+        auth_info_url = f"{self.openshift_url}/.well-known/oauth-authorization-server"
 
-        resp = requests.get(auth_info_url, verify=self.ca_certs or self.validate_cert)
-        resp_json = resp.json()
+        # Makes a request like OAuthenticator.httpfetch would but non-async as
+        # this code run during startup when we can't yet use async
+        # functionality.
+        client = HTTPClient()
+        req = HTTPRequest(auth_info_url, **self.http_request_kwargs)
+        resp = client.fetch(req)
+        resp_json = json.loads(resp.body.decode("utf8", "replace"))
 
         return resp_json.get('issuer')
 
+    @default("authorize_url")
+    def _authorize_url_default(self):
+        return f"{self.openshift_auth_api_url}/oauth/authorize"
+
+    @default("token_url")
+    def _token_url_default(self):
+        return f"{self.openshift_auth_api_url}/oauth/token"
+
     openshift_rest_api_url = Unicode(
-        os.environ.get('OPENSHIFT_REST_API_URL')
-        or 'https://openshift.default.svc.cluster.local',
         config=True,
+        help="""
+        Used to determine the default value for `userdata_url`.
+
+        Defaults to the `openshift_url`.
+        """,
     )
 
     @default("openshift_rest_api_url")
     def _openshift_rest_api_url_default(self):
         return self.openshift_url
 
-    @default("authorize_url")
-    def _authorize_url_default(self):
-        return "%s/oauth/authorize" % self.openshift_auth_api_url
-
-    @default("token_url")
-    def _token_url_default(self):
-        return "%s/oauth/token" % self.openshift_auth_api_url
-
     @default("userdata_url")
     def _userdata_url_default(self):
-        return "%s/apis/user.openshift.io/v1/users/~" % self.openshift_rest_api_url
+        return f"{self.openshift_rest_api_url}/apis/user.openshift.io/v1/users/~"
+
+    # _deprecated_oauth_aliases is used by deprecation logic in OAuthenticator
+    _deprecated_oauth_aliases = {
+        "ca_certs": ("http_request_kwargs", "16.0.0", False),
+        "validate_cert": ("validate_server_cert", "16.0.0"),
+        **OAuthenticator._deprecated_oauth_aliases,
+    }
+    ca_certs = Unicode(
+        config=True,
+        help="""
+        .. versionremoved:: 16.0
+
+           Use :attr:`http_request_kwargs`.
+        """,
+    )
+    validate_cert = Bool(
+        config=True,
+        help="""
+        .. deprecated:: 16.0
 
-    @staticmethod
-    def user_in_groups(user_groups: set, allowed_groups: set):
-        return any(user_groups.intersection(allowed_groups))
-
-    async def authenticate(self, handler, data=None):
-        code = handler.get_argument("code")
-
-        # Exchange the OAuth code for a OpenShift Access Token
-        #
-        # See: https://docs.openshift.org/latest/architecture/additional_concepts/authentication.html#api-authentication
-
-        params = dict(
-            client_id=self.client_id,
-            client_secret=self.client_secret,
-            grant_type="authorization_code",
-            code=code,
-        )
-
-        url = url_concat(self.token_url, params)
-
-        req = HTTPRequest(
-            url,
-            method="POST",
-            validate_cert=self.validate_cert,
-            ca_certs=self.ca_certs,
-            headers={"Accept": "application/json"},
-            body='',  # Body is required for a POST...
-        )
-
-        resp_json = await self.fetch(req)
-        access_token = resp_json['access_token']
-
-        # Determine who the logged in user is
-        headers = {
-            "Accept": "application/json",
-            "User-Agent": "JupyterHub",
-            "Authorization": "Bearer {}".format(access_token),
-        }
-
-        req = HTTPRequest(
-            self.userdata_url,
-            method="GET",
-            validate_cert=self.validate_cert,
-            ca_certs=self.ca_certs,
-            headers=headers,
-        )
-
-        ocp_user = await self.fetch(req)
-
-        username = ocp_user['metadata']['name']
-
-        user_info = {
-            'name': username,
-            'auth_state': {'access_token': access_token, 'openshift_user': ocp_user},
-        }
-
-        if self.allowed_groups or self.admin_groups:
-            user_info = await self._add_openshift_group_info(user_info)
-
-        return user_info
+           Use :attr:`validate_server_cert`.
+        """,
+    )
 
-    async def _add_openshift_group_info(self, user_info: dict):
+    def user_info_to_username(self, user_info):
         """
-        Use the group info stored on the OpenShift User object to determine if a user
-        is authenticated based on groups, an admin, or both.
+        Overrides OAuthenticator.user_info_to_username instead of setting
+        username_claim as the username is nested inside another dictionary.
         """
-        user_groups = set(user_info['auth_state']['openshift_user']['groups'])
-        username = user_info['name']
+        return user_info['metadata']['name']
+
+    async def update_auth_model(self, auth_model):
+        """
+        Sets admin status to True or False if `admin_groups` is configured and
+        the user isn't part of `admin_users`. Note that leaving it at None makes
+        users able to retain an admin status while setting it to False makes it
+        be revoked.
+        """
+        if auth_model["admin"]:
+            # auth_model["admin"] being True means the user was in admin_users
+            return auth_model
 
         if self.admin_groups:
-            is_admin = self.user_in_groups(user_groups, self.admin_groups)
+            # admin status should in this case be True or False, not None
+            user_info = auth_model["auth_state"][self.user_auth_state_key]
+            user_groups = set(user_info["groups"])
+            auth_model["admin"] = any(user_groups & self.admin_groups)
+
+        return auth_model
 
-        user_in_allowed_group = self.user_in_groups(user_groups, self.allowed_groups)
+    async def check_allowed(self, username, auth_model):
+        """
+        Overrides OAuthenticator.check_allowed to also allow users part of
+        `allowed_groups`.
+        """
+        if await super().check_allowed(username, auth_model):
+            return True
 
-        if self.admin_groups and (is_admin or user_in_allowed_group):
-            user_info['admin'] = is_admin
-            return user_info
-        elif user_in_allowed_group:
-            return user_info
-        else:
-            msg = f"username:{username} User not in any of the allowed/admin groups"
-            self.log.warning(msg)
-            return None
+        if self.allowed_groups:
+            user_info = auth_model["auth_state"][self.user_auth_state_key]
+            user_groups = set(user_info["groups"])
+            if any(user_groups & self.allowed_groups):
+                return True
 
+        # users should be explicitly allowed via config, otherwise they aren't
+        return False
 
-class LocalOpenShiftOAuthenticator(LocalAuthenticator, OpenShiftOAuthenticator):
 
+class LocalOpenShiftOAuthenticator(LocalAuthenticator, OpenShiftOAuthenticator):
     """A version that mixes in local system user creation"""
-
-    pass
```

### Comparing `oauthenticator-15.1.0/oauthenticator/schemas/cilogon-schema.yaml` & `oauthenticator-16.0.0/oauthenticator/schemas/cilogon-schema.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+# This JSONSchema is used to validate the values in the
+# CILogonOAuthenticator.allowed_idps dictionary.
+#
 $schema: http://json-schema.org/draft-07/schema#
-title: username_derivation
 type: object
 additionalProperties: false
 required:
   - username_derivation
 properties:
   allowed_domains:
     type: array
     items:
       type: string
   username_derivation:
     type: object
     additionalProperties: false
+    required:
+      - username_claim
     properties:
       username_claim:
         type: string
       action:
         type: string
         enum:
           - strip_idp_domain
           - prefix
       domain:
         type: string
       prefix:
         type: string
-    required:
-      - username_claim
     allOf:
+      # if action is strip_idp_domain, then domain is required
       - if:
           properties:
             action:
               const: strip_idp_domain
           required:
             - action
         then:
           required:
             - domain
+      # if action is prefix, then prefix is required
       - if:
           properties:
             action:
               const: prefix
           required:
             - action
         then:
```

### Comparing `oauthenticator-15.1.0/oauthenticator/tests/mocks.py` & `oauthenticator-16.0.0/oauthenticator/tests/mocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,38 +29,38 @@
         self.hosts = {}
 
     def add_host(self, host, paths):
         """Add a host whose requests should be mocked.
 
         Args:
             host (str): the host to mock (e.g. 'api.github.com')
-            paths (list(str|regex, callable)): a list of paths (or regexps for paths)
+            paths (list[(str|regex, callable)]): a list of paths (or regexps for paths)
                 and callables to be called for those paths.
                 The mock handlers will receive the request as their only argument.
 
         Mock handlers can return:
             - None
             - int (empty response with this status code)
             - str, bytes for raw response content (status=200)
             - list, dict for JSON response (status=200)
             - HTTPResponse (passed unmodified)
 
         Example::
 
             client.add_host('api.github.com', [
-                ('/user': lambda request: {'login': 'name'})
+                ('/user', lambda request: {'login': 'name'})
             ])
         """
         self.hosts[host] = paths
 
     def fetch_impl(self, request, response_callback):
         urlinfo = urlparse(request.url)
         host = urlinfo.hostname
         if host not in self.hosts:
-            app_log.warning("Not mocking request to %s", request.url)
+            app_log.warning(f"Not mocking request to {request.url}")
             return super().fetch_impl(request, response_callback)
         paths = self.hosts[host]
         response = None
         for path_spec, handler in paths:
             if isinstance(path_spec, str):
                 if path_spec == urlinfo.path:
                     response = handler(request)
@@ -136,47 +136,28 @@
     def access_token(request):
         """Handler for access token endpoint
 
         Checks code and allocates a new token.
         Replies with JSON model for the token.
         """
         assert request.method == 'POST', request.method
-        if token_request_style == 'json':
-            body = request.body.decode('utf8')
-            try:
-                body = json.loads(body)
-            except ValueError:
-                return HTTPResponse(
-                    request=request,
-                    code=400,
-                    reason="Body not JSON: %r" % body,
-                )
-            else:
-                code = body['code']
-        else:
-            query = urlparse(request.url).query
-            if not query:
-                query = request.body.decode('utf8')
-            query = parse_qs(query)
-            if 'code' not in query:
-                return HTTPResponse(
-                    request=request,
-                    code=400,
-                    reason="No code in access token request: url=%s, body=%s"
-                    % (
-                        request.url,
-                        request.body,
-                    ),
-                )
-            code = query['code'][0]
-        if code not in oauth_codes:
+        query = urlparse(request.url).query
+        if not query:
+            query = request.body.decode('utf8')
+        query = parse_qs(query)
+        if 'code' not in query:
             return HTTPResponse(
                 request=request,
-                code=403,
-                reason="No such code: %s" % code,
+                code=400,
+                reason=f"No code in access token request: url={request.url}, body={request.body}",
+            )
+        code = query['code'][0]
+        if code not in oauth_codes:
+            return HTTPResponse(
+                request=request, code=403, reason=f"No such code: {code}"
             )
 
         # consume code, allocate token
         token = uuid.uuid4().hex
         user = oauth_codes.pop(code)
         access_tokens[token] = user
         model = {
@@ -231,15 +212,15 @@
         """
         code = uuid.uuid4().hex
         oauth_codes[code] = user
         handler = Mock(spec=web.RequestHandler)
         handler.find_user = Mock(return_value=None)
         handler.get_argument = Mock(return_value=code)
         handler.request = HTTPServerRequest(
-            method='GET', uri='https://hub.example.com?code=%s' % code
+            method="GET", uri=f"https://hub.example.com?code={code}"
         )
         handler.hub = Mock(server=Mock(base_url='/hub/'), base_url='/hub/')
         return handler
 
     client.handler_for_user = handler_for_user
 
 
@@ -248,15 +229,15 @@
     application = web.Application(
         hub=Mock(
             base_url='/hub/',
             server=Mock(base_url='/hub/'),
         ),
         cookie_secret=os.urandom(32),
         db=Mock(rollback=Mock(return_value=None)),
-        **settings
+        **settings,
     )
     request = HTTPServerRequest(
         method=method,
         uri=uri,
         connection=Mock(),
     )
     handler = Handler(
@@ -268,9 +249,9 @@
 
 
 async def no_code_test(authenticator):
     """Run a test to exercise no code in the request"""
     handler = Mock(spec=web.RequestHandler)
     handler.get_argument = Mock(return_value=None)
     with pytest.raises(web.HTTPError) as exc:
-        name = await authenticator.authenticate(handler)
+        await authenticator.get_authenticated_user(handler, None)
     assert exc.value.status_code == 400
```

### Comparing `oauthenticator-15.1.0/oauthenticator/tests/test_generic.py` & `oauthenticator-16.0.0/oauthenticator/tests/test_generic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,201 +1,240 @@
 from functools import partial
 
-from pytest import fixture
+from pytest import fixture, mark
+from traitlets.config import Config
 
 from ..generic import GenericOAuthenticator
 from .mocks import setup_oauth_mock
 
 
 def user_model(username, **kwargs):
     """Return a user model"""
-    user = {
-        'username': username,
-        'scope': 'basic',
+    return {
+        "username": username,
+        "scope": "basic",
+        "groups": ["group1"],
+        **kwargs,
     }
-    user.update(kwargs)
-    return user
-
-
-def _get_authenticator(**kwargs):
-    return GenericOAuthenticator(
-        token_url='https://generic.horse/oauth/access_token',
-        userdata_url='https://generic.horse/oauth/userinfo',
-        **kwargs
-    )
-
-
-def get_simple_handler(generic_client):
-    return generic_client.handler_for_user(user_model('wash'))
 
 
 @fixture
 def generic_client(client):
     setup_oauth_mock(
         client,
         host='generic.horse',
         access_token_path='/oauth/access_token',
         user_path='/oauth/userinfo',
     )
     return client
 
 
+def _get_authenticator(**kwargs):
+    return GenericOAuthenticator(
+        token_url='https://generic.horse/oauth/access_token',
+        userdata_url='https://generic.horse/oauth/userinfo',
+        **kwargs,
+    )
+
+
 @fixture
-def get_authenticator(generic_client, **kwargs):
+def get_authenticator(generic_client):
+    """
+    http_client can't be configured, only passed as argument to the constructor.
+    """
     return partial(_get_authenticator, http_client=generic_client)
 
 
-async def test_generic(get_authenticator, generic_client):
+@mark.parametrize(
+    "test_variation_id,class_config,expect_allowed,expect_admin",
+    [
+        # no allow config tested
+        ("00", {}, False, None),
+        # allow config, individually tested
+        ("01", {"allow_all": True}, True, None),
+        ("02", {"allowed_users": {"user1"}}, True, None),
+        ("03", {"allowed_users": {"not-test-user"}}, False, None),
+        ("04", {"admin_users": {"user1"}}, True, True),
+        ("05", {"admin_users": {"not-test-user"}}, False, None),
+        ("06", {"allowed_groups": {"group1"}}, True, None),
+        ("07", {"allowed_groups": {"test-user-not-in-group"}}, False, None),
+        ("08", {"admin_groups": {"group1"}}, True, True),
+        ("09", {"admin_groups": {"test-user-not-in-group"}}, False, False),
+        # allow config, some combinations of two tested
+        (
+            "10",
+            {
+                "allow_all": False,
+                "allowed_users": {"not-test-user"},
+            },
+            False,
+            None,
+        ),
+        (
+            "11",
+            {
+                "allowed_users": {"not-test-user"},
+                "admin_users": {"user1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "12",
+            {
+                "allowed_groups": {"group1"},
+                "admin_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "13",
+            {
+                "allowed_groups": {"group1"},
+                "admin_groups": {"test-user-not-in-group"},
+            },
+            True,
+            False,
+        ),
+        (
+            "14",
+            {
+                "allowed_groups": {"test-user-not-in-group"},
+                "admin_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "15",
+            {
+                "allowed_groups": {"test-user-not-in-group"},
+                "admin_groups": {"test-user-not-in-group"},
+            },
+            False,
+            False,
+        ),
+        (
+            "16",
+            {
+                "admin_users": {"user1"},
+                "admin_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "17",
+            {
+                "admin_users": {"user1"},
+                "admin_groups": {"test-user-not-in-group"},
+            },
+            True,
+            True,
+        ),
+        (
+            "18",
+            {
+                "admin_users": {"not-test-user"},
+                "admin_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "19",
+            {
+                "admin_users": {"not-test-user"},
+                "admin_groups": {"test-user-not-in-group"},
+            },
+            False,
+            False,
+        ),
+    ],
+)
+async def test_generic(
+    get_authenticator,
+    generic_client,
+    test_variation_id,
+    class_config,
+    expect_allowed,
+    expect_admin,
+):
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.GenericOAuthenticator = Config(class_config)
+    c.GenericOAuthenticator.username_claim = "username"
+    authenticator = get_authenticator(config=c)
+
+    handled_user_model = user_model("user1")
+    handler = generic_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+
+    if expect_allowed:
+        assert auth_model
+        assert set(auth_model) == {"name", "admin", "auth_state"}
+        assert auth_model["admin"] == expect_admin
+        auth_state = auth_model["auth_state"]
+        assert "access_token" in auth_state
+        assert "oauth_user" in auth_state
+        assert "refresh_token" in auth_state
+        assert "scope" in auth_state
+        user_info = auth_state[authenticator.user_auth_state_key]
+        assert auth_model["name"] == user_info[authenticator.username_claim]
+    else:
+        assert auth_model == None
+
+
+async def test_generic_data(get_authenticator, generic_client):
+    c = Config()
+    c.GenericOAuthenticator.allow_all = True
     authenticator = get_authenticator()
 
-    handler = get_simple_handler(generic_client)
-    user_info = await authenticator.authenticate(handler)
-    assert sorted(user_info) == ['auth_state', 'name']
-    name = user_info['name']
-    assert name == 'wash'
-    auth_state = user_info['auth_state']
-    assert 'access_token' in auth_state
-    assert 'oauth_user' in auth_state
-    assert 'refresh_token' in auth_state
-    assert 'scope' in auth_state
-
-
-async def test_generic_callable_username_key(get_authenticator, generic_client):
-    authenticator = get_authenticator(username_key=lambda r: r['alternate_username'])
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe')
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'zoe'
-
-
-async def test_generic_callable_groups_claim_key_with_allowed_groups(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key=lambda r: r.get('policies').get('roles'),
-        allowed_groups=['super_user'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe', policies={'roles': ['super_user']})
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'wash'
-
+    handled_user_model = user_model("user1")
+    handler = generic_client.handler_for_user(handled_user_model)
+    data = {"testing": "data"}
+    auth_model = await authenticator.authenticate(handler, data)
 
-async def test_generic_groups_claim_key_with_allowed_groups(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='groups',
-        allowed_groups=['super_user'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe', groups=['super_user'])
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'wash'
+    assert auth_model
 
 
-async def test_generic_groups_claim_key_nested_strings(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='permissions.groups',
-        allowed_groups=['super_user'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model(
-            'wash', alternate_username='zoe', permissions={"groups": ['super_user']}
-        )
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'wash'
+async def test_generic_callable_username_key(get_authenticator, generic_client):
+    c = Config()
+    c.GenericOAuthenticator.allow_all = True
+    c.GenericOAuthenticator.username_key = lambda r: r["alternate_username"]
+    authenticator = get_authenticator(config=c)
 
+    handled_user_model = user_model("user1", alternate_username="zoe")
+    handler = generic_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
 
-async def test_generic_groups_claim_key_nested_strings_nonexistant_key(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='permissions.groups',
-        allowed_groups=['super_user'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe')
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info is None
+    assert auth_model["name"] == "zoe"
 
 
-async def test_generic_groups_claim_key_with_allowed_groups_unauthorized(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='groups',
-        allowed_groups=['user'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe', groups=['public'])
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info is None
+async def test_generic_claim_groups_key_callable(get_authenticator, generic_client):
+    c = Config()
+    c.GenericOAuthenticator.claim_groups_key = lambda r: r["policies"]["roles"]
+    c.GenericOAuthenticator.allowed_groups = ["super_user"]
+    authenticator = get_authenticator(config=c)
 
+    handled_user_model = user_model("user1", policies={"roles": ["super_user"]})
+    handler = generic_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
 
-async def test_generic_groups_claim_key_with_allowed_groups_and_admin_groups(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='groups',
-        allowed_groups=['user'],
-        admin_groups=['administrator'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe', groups=['user', 'administrator'])
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'wash'
-    assert user_info['admin'] is True
+    assert auth_model
 
 
-async def test_generic_groups_claim_key_with_allowed_groups_and_admin_groups_not_admin(
+async def test_generic_claim_groups_key_nested_strings(
     get_authenticator, generic_client
 ):
-    authenticator = get_authenticator(
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key='groups',
-        allowed_groups=['user'],
-        admin_groups=['administrator'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model('wash', alternate_username='zoe', groups=['user'])
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'wash'
-    assert user_info['admin'] is False
+    c = Config()
+    c.GenericOAuthenticator.claim_groups_key = "permissions.groups"
+    c.GenericOAuthenticator.admin_groups = ["super_user"]
+    authenticator = get_authenticator(config=c)
 
+    handled_user_model = user_model("user1", permissions={"groups": ["super_user"]})
+    handler = generic_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
 
-async def test_generic_callable_groups_claim_key_with_allowed_groups_and_admin_groups(
-    get_authenticator, generic_client
-):
-    authenticator = get_authenticator(
-        username_key=lambda r: r['alternate_username'],
-        scope=['openid', 'profile', 'roles'],
-        claim_groups_key=lambda r: r.get('policies').get('roles'),
-        allowed_groups=['user', 'public'],
-        admin_groups=['administrator'],
-    )
-    handler = generic_client.handler_for_user(
-        user_model(
-            'wash',
-            alternate_username='zoe',
-            policies={'roles': ['user', 'administrator']},
-        )
-    )
-    user_info = await authenticator.authenticate(handler)
-    assert user_info['name'] == 'zoe'
-    assert user_info['admin'] is True
+    assert auth_model
+    assert auth_model["admin"]
```

### Comparing `oauthenticator-15.1.0/oauthenticator/tests/test_gitlab.py` & `oauthenticator-16.0.0/oauthenticator/tests/test_github.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,289 +1,275 @@
-import collections
 import functools
 import json
 import logging
 import re
 from io import BytesIO
 from urllib.parse import parse_qs, urlparse
 
-from pytest import fixture
+from pytest import fixture, mark, raises
 from tornado.httpclient import HTTPResponse
 from tornado.httputil import HTTPHeaders
 from traitlets.config import Config
 
-from ..gitlab import GitLabOAuthenticator
+from ..github import GitHubOAuthenticator
 from .mocks import setup_oauth_mock
 
-API_ENDPOINT = '/api/v%s' % (GitLabOAuthenticator().gitlab_api_version)
 
-
-def user_model(username, id=1, is_admin=False):
+def user_model(username):
     """Return a user model"""
-    user = {
-        'username': username,
-        'id': id,
+    return {
+        'email': 'dinosaurs@space',
+        'id': 5,
+        'login': username,
+        'name': 'Hoban Washburn',
     }
-    if is_admin:
-        # Some versions of the API do not return the is_admin property
-        # for non-admin users (See #115).
-        user['is_admin'] = True
-    return user
 
 
 @fixture
-def gitlab_client(client):
+def github_client(client):
     setup_oauth_mock(
         client,
-        host='gitlab.com',
-        access_token_path='/oauth/token',
-        user_path=API_ENDPOINT + '/user',
+        host=['github.com', 'api.github.com'],
+        access_token_path='/login/oauth/access_token',
+        user_path='/user',
+        token_type='token',
     )
     return client
 
 
-def mock_api_version(client, version):
-    def mock_version_response(request):
-        ret = {'version': version, 'revision': "f79c1794977"}
-        return HTTPResponse(
-            request,
-            200,
-            headers={'Content-Type': 'application/json'},
-            buffer=BytesIO(json.dumps(ret).encode('utf-8')),
-        )
-
-    regex = re.compile(API_ENDPOINT + '/version')
-    client.hosts['gitlab.com'].append((regex, mock_version_response))
-
-
-async def test_gitlab(gitlab_client):
-    authenticator = GitLabOAuthenticator()
-    mock_api_version(gitlab_client, '12.3.1-ee')
-    handler = gitlab_client.handler_for_user(user_model('wash'))
-    user_info = await authenticator.authenticate(handler)
-    assert sorted(user_info) == ['auth_state', 'name']
-    name = user_info['name']
-    assert name == 'wash'
-    auth_state = user_info['auth_state']
-    assert 'access_token' in auth_state
-    assert 'gitlab_user' in auth_state
+@mark.parametrize(
+    "test_variation_id,class_config,expect_allowed,expect_admin",
+    [
+        # no allow config tested
+        ("00", {}, False, None),
+        # allow config, individually tested
+        ("01", {"allow_all": True}, True, None),
+        ("02", {"allowed_users": {"user1"}}, True, None),
+        ("03", {"allowed_users": {"not-test-user"}}, False, None),
+        ("04", {"admin_users": {"user1"}}, True, True),
+        ("05", {"admin_users": {"not-test-user"}}, False, None),
+        # allow config, some combinations of two tested
+        (
+            "10",
+            {
+                "allow_all": False,
+                "allowed_users": {"not-test-user"},
+            },
+            False,
+            None,
+        ),
+        (
+            "11",
+            {
+                "admin_users": {"user1"},
+                "allowed_users": {"not-test-user"},
+            },
+            True,
+            True,
+        ),
+    ],
+)
+async def test_github(
+    github_client,
+    test_variation_id,
+    class_config,
+    expect_allowed,
+    expect_admin,
+):
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.GitHubOAuthenticator = Config(class_config)
+    c.GitHubOAuthenticator.username_claim = "login"
+    authenticator = GitHubOAuthenticator(config=c)
+
+    handled_user_model = user_model("user1")
+    handler = github_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+
+    if expect_allowed:
+        assert auth_model
+        assert set(auth_model) == {"name", "admin", "auth_state"}
+        assert auth_model["admin"] == expect_admin
+        auth_state = auth_model["auth_state"]
+        assert "access_token" in auth_state
+        user_info = auth_state[authenticator.user_auth_state_key]
+        assert user_info == handled_user_model
+        assert auth_model["name"] == user_info[authenticator.username_claim]
+    else:
+        assert auth_model == None
 
 
 def make_link_header(urlinfo, page):
     return {
-        'Link': '<{}://{}{}?page={}>;rel="next"'.format(
-            urlinfo.scheme, urlinfo.netloc, urlinfo.path, page
-        )
+        "Link": f'<{urlinfo.scheme}://{urlinfo.netloc}{urlinfo.path}?page={page}>;rel="next"'
     }
 
 
-async def test_allowed_groups(gitlab_client):
-    client = gitlab_client
-    authenticator = GitLabOAuthenticator()
-    mock_api_version(client, '12.4.0-ee')
-
-    ## set up fake Gitlab API
-
-    user_groups = collections.OrderedDict(
-        {
-            'grif': ['red', 'yellow'],
-            'simmons': ['red', 'yellow'],
-            'caboose': ['blue', 'yellow'],
-            'burns': ['blue', 'yellow'],
-        }
-    )
+async def test_allowed_org_membership(github_client):
+    authenticator = GitHubOAuthenticator()
 
-    def group_user_model(username, is_admin=False):
-        return user_model(
-            username, list(user_groups.keys()).index(username) + 1, is_admin
-        )
+    ## Mock Github API
 
-    member_regex = re.compile(API_ENDPOINT + r'/groups/(.*)/members/all/(.*)')
+    allowed_org_members = {
+        "org1": ["user1"],
+    }
+    allowed_org_team_members = {
+        "org1": {
+            "team1": ["user1"],
+        },
+    }
 
-    def is_member(request):
+    member_regex = re.compile(r'/orgs/(.*)/members')
+
+    def org_members(paginate, request):
         urlinfo = urlparse(request.url)
-        group, uid = member_regex.match(urlinfo.path).group(1, 2)
-        uname = list(user_groups.keys())[int(uid) - 1]
-        if group in user_groups[uname]:
-            return HTTPResponse(request, 200)
-        else:
+        org = member_regex.match(urlinfo.path).group(1)
+
+        if org not in allowed_org_members:
             return HTTPResponse(request, 404)
 
-    def groups(paginate, request):
-        urlinfo = urlparse(request.url)
-        _, token = request._headers.get('Authorization').split()
-        user = client.access_tokens[token]['username']
         if not paginate:
-            return [{'path': group} for group in user_groups[user]]
+            return [user_model(m) for m in allowed_org_members[org]]
         else:
             page = parse_qs(urlinfo.query).get('page', ['1'])
             page = int(page[0])
-            return groups_paginated(
-                user, page, urlinfo, functools.partial(HTTPResponse, request)
+            return org_members_paginated(
+                org, page, urlinfo, functools.partial(HTTPResponse, request)
             )
 
-    def groups_paginated(user, page, urlinfo, response):
-        if page < len(user_groups[user]):
+    def org_members_paginated(org, page, urlinfo, response):
+        if page < len(allowed_org_members[org]):
             headers = make_link_header(urlinfo, page + 1)
-        elif page == len(user_groups[user]):
+        elif page == len(allowed_org_members[org]):
             headers = {}
         else:
             return response(400)
 
         headers.update({'Content-Type': 'application/json'})
 
-        ret = [{'path': user_groups[user][page - 1]}]
+        ret = [user_model(allowed_org_members[org][page - 1])]
 
         return response(
             200,
             headers=HTTPHeaders(headers),
             buffer=BytesIO(json.dumps(ret).encode('utf-8')),
         )
 
-    client.hosts['gitlab.com'].append((member_regex, is_member))
+    org_membership_regex = re.compile(r'/orgs/(.*)/members/(.*)')
 
-    ## actual tests
-
-    for paginate in (False, True):
-        client.hosts['gitlab.com'].append(
-            (API_ENDPOINT + '/groups', functools.partial(groups, paginate))
-        )
+    def org_membership(request):
+        urlinfo = urlparse(request.url)
+        urlmatch = org_membership_regex.match(urlinfo.path)
+        org = urlmatch.group(1)
+        username = urlmatch.group(2)
+        print(f"Request org = {org}, username = {username}")
+        if org not in allowed_org_members:
+            print(f"Org not found: org = {org}")
+            return HTTPResponse(request, 404)
+        if username not in allowed_org_members[org]:
+            print(f"Member not found: org = {org}, username = {username}")
+            return HTTPResponse(request, 404)
+        return HTTPResponse(request, 204)
 
-        authenticator.allowed_gitlab_groups = ['blue']
+    team_membership_regex = re.compile(r'/orgs/(.*)/teams/(.*)/members/(.*)')
 
-        handler = client.handler_for_user(group_user_model('caboose'))
-        user_info = await authenticator.authenticate(handler)
-        name = user_info['name']
-        assert name == 'caboose'
-
-        handler = client.handler_for_user(group_user_model('burns', is_admin=True))
-        user_info = await authenticator.authenticate(handler)
-        name = user_info['name']
-        assert name == 'burns'
-
-        handler = client.handler_for_user(group_user_model('grif'))
-        name = await authenticator.authenticate(handler)
-        assert name is None
-
-        handler = client.handler_for_user(group_user_model('simmons', is_admin=True))
-        name = await authenticator.authenticate(handler)
-        assert name is None
-
-        # reverse it, just to be safe
-        authenticator.allowed_gitlab_groups = ['red']
-
-        handler = client.handler_for_user(group_user_model('caboose'))
-        name = await authenticator.authenticate(handler)
-        assert name is None
-
-        handler = client.handler_for_user(group_user_model('grif'))
-        user_info = await authenticator.authenticate(handler)
-        name = user_info['name']
-        assert name == 'grif'
-
-        client.hosts['gitlab.com'].pop()
-
-
-async def test_allowed_project_ids(gitlab_client):
-    client = gitlab_client
-    authenticator = GitLabOAuthenticator()
-    mock_api_version(client, '12.4.0-pre')
-
-    user_projects = {
-        '1231231': {
-            '3588673': {
-                'id': 3588674,
-                'name': 'john',
-                'username': 'john',
-                'state': 'active',
-                'avatar_url': 'https://secure.gravatar.com/avatar/382a6b306679b2d97b547bfff3d73242?s=80&d=identicon',
-                'web_url': 'https://gitlab.com/john',
-                'access_level': 10,  # Guest
-                'expires_at': '2030-02-23',
-            },
-            '3588674': {
-                'id': 3588674,
-                'name': 'harry',
-                'username': 'harry',
-                'state': 'active',
-                'avatar_url': 'https://secure.gravatar.com/avatar/382a6b306679b2d97b547bfff3d73242?s=80&d=identicon',
-                'web_url': 'https://gitlab.com/harry',
-                'access_level': 30,  # Developer
-                'expires_at': '2030-02-23',
-            },
-        }
-    }
-    john_user_model = user_model('john', 3588673)
-    harry_user_model = user_model('harry', 3588674)
-    sheila_user_model = user_model('sheila', 3588675)
+    def team_membership(request):
+        urlinfo = urlparse(request.url)
+        urlmatch = team_membership_regex.match(urlinfo.path)
+        org = urlmatch.group(1)
+        team = urlmatch.group(2)
+        username = urlmatch.group(3)
+        print(f"Request org = {org}, team = {team} username = {username}")
+        if org not in allowed_org_members:
+            print(f"Org not found: org = {org}")
+            return HTTPResponse(request, 404)
+        if team not in allowed_org_team_members[org]:
+            print(f"Team not found in org: team = {team}, org = {org}")
+            return HTTPResponse(request, 404)
+        if username not in allowed_org_team_members[org][team]:
+            print(
+                f"Member not found: org = {org}, team = {team}, username = {username}"
+            )
+            return HTTPResponse(request, 404)
+        return HTTPResponse(request, 204)
 
-    member_regex = re.compile(API_ENDPOINT + r'/projects/(.*)/members/all/(.*)')
+    ## Perform tests
 
-    def is_member(request):
-        urlinfo = urlparse(request.url)
-        project_id, uid = member_regex.match(urlinfo.path).group(1, 2)
+    client_hosts = github_client.hosts['api.github.com']
+    client_hosts.append((team_membership_regex, team_membership))
+    client_hosts.append((org_membership_regex, org_membership))
 
-        if user_projects.get(project_id) and user_projects.get(project_id).get(uid):
-            res = user_projects.get(project_id).get(uid)
-            return HTTPResponse(
-                request=request,
-                code=200,
-                buffer=BytesIO(json.dumps(res).encode('utf8')),
-                headers={'Content-Type': 'application/json'},
-            )
-        else:
-            return HTTPResponse(
-                request=request, code=404, buffer=BytesIO(''.encode('utf8'))
-            )
+    # Run tests twice, once with paginate and once without
+    for paginate in (False, True):
+        client_hosts.append((member_regex, functools.partial(org_members, paginate)))
 
-    client.hosts['gitlab.com'].append((member_regex, is_member))
+        # test org membership
+        authenticator.allowed_organizations = ["org1"]
 
-    authenticator.allowed_project_ids = [1231231]
+        handled_user_model = user_model("user1")
+        handler = github_client.handler_for_user(handled_user_model)
+        auth_model = await authenticator.get_authenticated_user(handler, None)
+        assert auth_model
+
+        handled_user_model = user_model("user-not-in-org")
+        handler = github_client.handler_for_user(handled_user_model)
+        auth_model = await authenticator.get_authenticated_user(handler, None)
+        assert auth_model is None
+
+        # test org team membership
+        authenticator.allowed_organizations = ["org1:team1"]
+
+        handled_user_model = user_model("user1")
+        handler = github_client.handler_for_user(handled_user_model)
+        auth_model = await authenticator.get_authenticated_user(handler, None)
+        assert auth_model
+
+        handled_user_model = user_model("user-not-in-org-team")
+        handler = github_client.handler_for_user(handled_user_model)
+        auth_model = await authenticator.get_authenticated_user(handler, None)
+        assert auth_model is None
+
+        client_hosts.pop()
+
+
+@mark.parametrize(
+    "test_variation_id,class_config,expect_config,expect_loglevel,expect_message",
+    [
+        (
+            "github_organization_whitelist",
+            {"github_organization_whitelist": {"dummy"}},
+            {"allowed_organizations": {"dummy"}},
+            logging.WARNING,
+            "GitHubOAuthenticator.github_organization_whitelist is deprecated in GitHubOAuthenticator 0.12.0, use GitHubOAuthenticator.allowed_organizations instead",
+        ),
+    ],
+)
+async def test_deprecated_config(
+    caplog,
+    test_variation_id,
+    class_config,
+    expect_config,
+    expect_loglevel,
+    expect_message,
+):
+    """
+    Tests that a warning is emitted when using a deprecated config and that
+    configuring the old config ends up configuring the new config.
+    """
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.GitHubOAuthenticator = Config(class_config)
+
+    test_logger = logging.getLogger('testlog')
+    if expect_loglevel == logging.ERROR:
+        with raises(ValueError, match=expect_message):
+            GitHubOAuthenticator(config=c, log=test_logger)
+    else:
+        authenticator = GitHubOAuthenticator(config=c, log=test_logger)
+        for key, value in expect_config.items():
+            assert getattr(authenticator, key) == value
 
-    # Forbidden since John has guest access
-    handler = client.handler_for_user(john_user_model)
-    user_info = await authenticator.authenticate(handler)
-    assert user_info is None
-
-    # Authenticated since Harry has developer access to the project
-    handler = client.handler_for_user(harry_user_model)
-    user_info = await authenticator.authenticate(handler)
-    name = user_info['name']
-    assert name == 'harry'
-
-    # Forbidden since Sheila doesn't have access to the project
-    handler = client.handler_for_user(sheila_user_model)
-    user_info = await authenticator.authenticate(handler)
-    assert user_info is None
-
-    authenticator.allowed_project_ids = [123123152543]
-
-    # Forbidden since the project does not exist.
-    handler = client.handler_for_user(harry_user_model)
-    user_info = await authenticator.authenticate(handler)
-    assert user_info is None
-
-    authenticator.allowed_project_ids = [123123152543, 1231231]
-
-    # Authenticated since Harry has developer access to one of the project in the list
-    handler = client.handler_for_user(harry_user_model)
-    user_info = await authenticator.authenticate(handler)
-    name = user_info['name']
-    assert name == 'harry'
-
-
-def test_deprecated_config(caplog):
-    cfg = Config()
-    cfg.GitLabOAuthenticator.gitlab_group_whitelist = {'red'}
-    cfg.GitLabOAuthenticator.whitelist = {"blue"}
-
-    log = logging.getLogger("testlog")
-    authenticator = GitLabOAuthenticator(config=cfg, log=log)
-    assert (
-        log.name,
-        logging.WARNING,
-        'GitLabOAuthenticator.gitlab_group_whitelist is deprecated in GitLabOAuthenticator 0.12.0, use '
-        'GitLabOAuthenticator.allowed_gitlab_groups instead',
-    ) in caplog.record_tuples
+    captured_log_tuples = caplog.record_tuples
+    print(captured_log_tuples)
 
-    assert authenticator.allowed_gitlab_groups == {'red'}
-    assert authenticator.allowed_users == {"blue"}
+    expected_log_tuple = (test_logger.name, expect_loglevel, expect_message)
+    assert expected_log_tuple in captured_log_tuples
```

### Comparing `oauthenticator-15.1.0/oauthenticator/tests/test_globus.py` & `oauthenticator-16.0.0/oauthenticator/tests/test_globus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import json
 from io import BytesIO
 from unittest.mock import Mock
 from urllib.parse import parse_qs
 
-from pytest import fixture, raises
+from pytest import fixture, mark, raises
 from tornado import web
 from tornado.httpclient import HTTPResponse
+from traitlets.config import Config
 
 from ..globus import GlobusLogoutHandler, GlobusOAuthenticator
 from ..oauth2 import STATE_COOKIE_NAME
 from .mocks import mock_handler, setup_oauth_mock
 
 
-def user_model(username, email=None):
+def user_model(username, **kwargs):
     """Return a user model"""
-    userinfo = {
-        'preferred_username': username,
+    return {
+        "preferred_username": username,
+        **kwargs,
     }
-    if email:
-        userinfo['email'] = email
-    return userinfo
 
 
 def revoke_token_request_handler(request):
     assert request.method == 'POST', request.method
     auth_header = request.headers.get('Authorization')
     if auth_header:
         resp = BytesIO(json.dumps({'active': False}).encode('utf8'))
@@ -68,29 +67,19 @@
         'scope': 'profile openid',
     }
 
 
 def get_groups_request_handler(request):
     mock_globus_groups_response = [
         {
-            'id': '21c6bc5d-fc12-4f60-b999-76766cd596c2',
-            'my_memberships': [{'role': 'manager'}],
-        },
-        {
-            'id': '915dcd61-c842-4ea4-97c6-57396b936016',
+            # group's IDs should really be UUIDs, but a simpler string is used
+            # for consistency between tests
+            'id': 'group1',
             'my_memberships': [{'role': 'member'}],
         },
-        {
-            'id': 'd11abe71-5132-4c04-a4ad-50926885dc8c',
-            'my_memberships': [
-                {
-                    'role': 'member',
-                }
-            ],
-        },
     ]
     assert request.method == 'GET', request.method
     resp = BytesIO(json.dumps(mock_globus_groups_response).encode('utf-8'))
     return HTTPResponse(
         request=request,
         code=200,
         headers={'Content-Type': 'application/json'},
@@ -126,14 +115,15 @@
     a bunch of other tokens, including an id_token. We want to make sure we
     capture the full Globus token response. This will attach the dict
     new_token_response to the built-in test response if it returns successfully"""
     # Find the existing endpoint, function pair in client.hosts
     url, func = next(
         filter(lambda host: host[0] == access_token_path, client.hosts[host])
     )
+
     # Wrap the built-in token response with our custom response, but only if
     # it returns successfully with an access token!
     def custom_token_response(request):
         response = func(request)
         if response.get('access_token'):
             # The original access_token is checked,
             new_token_response['access_token'] = response['access_token']
@@ -151,15 +141,14 @@
 def globus_client(client, mock_globus_token_response):
     setup_oauth_mock(
         client,
         host='auth.globus.org',
         access_token_path='/v2/oauth2/token',
         user_path='/v2/oauth2/userinfo',
         token_type='bearer',
-        token_request_style='post',
     )
     set_extended_token_response(
         client, 'auth.globus.org', '/v2/oauth2/token', mock_globus_token_response
     )
     client.add_host(
         'groups.api.globus.org',
         [
@@ -180,33 +169,169 @@
 
         async def save_auth_state(self, state):
             self.state = state
 
     return User()
 
 
-async def test_globus(globus_client):
-    authenticator = GlobusOAuthenticator()
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-    tokens = list(data['auth_state']['tokens'].keys())
-    assert tokens == ['transfer.api.globus.org']
+@mark.parametrize(
+    "test_variation_id,class_config,expect_allowed,expect_admin",
+    [
+        # no allow config tested
+        ("00", {}, False, None),
+        # allow config, individually tested
+        ("01", {"allow_all": True}, True, None),
+        ("02", {"allowed_users": {"user1"}}, True, None),
+        ("03", {"allowed_users": {"not-test-user"}}, False, None),
+        ("04", {"admin_users": {"user1"}}, True, True),
+        ("05", {"admin_users": {"not-test-user"}}, False, None),
+        ("06", {"allowed_globus_groups": {"group1"}}, True, None),
+        ("07", {"allowed_globus_groups": {"test-user-not-in-group"}}, False, None),
+        ("08", {"admin_globus_groups": {"group1"}}, True, True),
+        ("09", {"admin_globus_groups": {"test-user-not-in-group"}}, False, False),
+        # allow config, some combinations of two tested
+        (
+            "10",
+            {
+                "allow_all": False,
+                "allowed_users": {"not-test-user"},
+            },
+            False,
+            None,
+        ),
+        (
+            "11",
+            {
+                "allowed_users": {"not-test-user"},
+                "admin_users": {"user1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "12",
+            {
+                "allowed_globus_groups": {"group1"},
+                "admin_globus_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "13",
+            {
+                "allowed_globus_groups": {"group1"},
+                "admin_globus_groups": {"test-user-not-in-group"},
+            },
+            True,
+            False,
+        ),
+        (
+            "14",
+            {
+                "allowed_globus_groups": {"test-user-not-in-group"},
+                "admin_globus_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "15",
+            {
+                "allowed_globus_groups": {"test-user-not-in-group"},
+                "admin_globus_groups": {"test-user-not-in-group"},
+            },
+            False,
+            False,
+        ),
+        (
+            "16",
+            {
+                "admin_users": {"user1"},
+                "admin_globus_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "17",
+            {
+                "admin_users": {"user1"},
+                "admin_globus_groups": {"test-user-not-in-group"},
+            },
+            True,
+            True,
+        ),
+        (
+            "18",
+            {
+                "admin_users": {"not-test-user"},
+                "admin_globus_groups": {"group1"},
+            },
+            True,
+            True,
+        ),
+        (
+            "19",
+            {
+                "admin_users": {"not-test-user"},
+                "admin_globus_groups": {"test-user-not-in-group"},
+            },
+            False,
+            False,
+        ),
+    ],
+)
+async def test_globus(
+    globus_client,
+    test_variation_id,
+    class_config,
+    expect_allowed,
+    expect_admin,
+):
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.GlobusOAuthenticator = Config(class_config)
+    c.GlobusOAuthenticator.username_claim = "preferred_username"
+    authenticator = GlobusOAuthenticator(config=c)
+
+    handled_user_model = user_model("user1")
+    handler = globus_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+
+    if expect_allowed:
+        assert auth_model
+        assert set(auth_model) == {"name", "admin", "auth_state"}
+        assert auth_model["admin"] == expect_admin
+        auth_state = auth_model["auth_state"]
+        assert "tokens" in auth_state
+        assert "transfer.api.globus.org" in auth_state["tokens"]
+        user_info = auth_state[authenticator.user_auth_state_key]
+        assert auth_model["name"] == user_info[authenticator.username_claim]
+        if authenticator.allowed_globus_groups or authenticator.admin_globus_groups:
+            assert auth_state["globus_groups"] == {"group1"}
+    else:
+        assert auth_model == None
 
 
 async def test_globus_pre_spawn_start(mock_globus_user):
     authenticator = GlobusOAuthenticator()
     spawner = Mock()
     spawner.environment = {}
     await authenticator.pre_spawn_start(mock_globus_user, spawner)
     assert 'GLOBUS_DATA' in spawner.environment
 
 
-def test_globus_defaults():
+async def test_globus_defaults():
     authenticator = GlobusOAuthenticator()
+    print(f"userdata_url: {authenticator.userdata_url}")
+    print(f"authorize_url: {authenticator.authorize_url}")
+    print(f"revocation_url: {authenticator.revocation_url}")
+    print(f"token_url: {authenticator.token_url}")
+
     assert all(
         'https://auth.globus.org' in url
         for url in [
             authenticator.userdata_url,
             authenticator.authorize_url,
             authenticator.revocation_url,
             authenticator.token_url,
@@ -216,102 +341,100 @@
         'openid',
         'profile',
         'urn:globus:auth:scope:transfer.api.globus.org:all',
     ]
 
 
 async def test_restricted_domain(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.identity_provider = 'alliance.gov'
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
+    c = Config()
+    c.GlobusOAuthenticator.allow_all = True
+    c.GlobusOAuthenticator.identity_provider = "allowed.example.com"
+    authenticator = GlobusOAuthenticator(config=c)
+
+    handled_user_model = user_model("user1@example.com")
+    handler = globus_client.handler_for_user(handled_user_model)
     with raises(web.HTTPError) as exc:
-        await authenticator.authenticate(handler)
+        await authenticator.get_authenticated_user(handler, None)
     assert exc.value.status_code == 403
 
 
 async def test_namespaced_domain(globus_client):
-    authenticator = GlobusOAuthenticator()
-    # Allow any idp
-    authenticator.identity_provider = ''
-    um = user_model('wash@legitshipping.com@serenity.com')
-    handler = globus_client.handler_for_user(um)
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-
-
-async def test_username_from_email(globus_client):
-    authenticator = GlobusOAuthenticator()
-    # Allow any idp
-    authenticator.identity_provider = ''
-    authenticator.username_from_email = True
-    um = user_model('wash@legitshipping.com@serenity.com', 'alan@tudyk.org')
-    handler = globus_client.handler_for_user(um)
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'alan'
+    c = Config()
+    c.GlobusOAuthenticator.allow_all = True
+    authenticator = GlobusOAuthenticator(config=c)
+
+    handled_user_model = user_model('wash@legitshipping.com@serenity.com')
+    handler = globus_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+    assert auth_model['name'] == 'wash'
 
 
-async def test_username_not_from_email(globus_client):
-    authenticator = GlobusOAuthenticator()
-    # Allow any idp
-    authenticator.identity_provider = ''
-    um = user_model('wash@legitshipping.com@serenity.com', 'alan@tudyk.org')
-    handler = globus_client.handler_for_user(um)
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-
-
-async def test_email_scope_added(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.username_from_email = True
+async def test_username_from_email_scope_added(globus_client):
+    c = Config()
+    c.GlobusOAuthenticator.username_from_email = True
+    authenticator = GlobusOAuthenticator(config=c)
     assert authenticator.scope == [
         'openid',
         'profile',
         'urn:globus:auth:scope:transfer.api.globus.org:all',
         'email',
     ]
 
 
 async def test_username_from_email_restricted_pass(globus_client):
-    authenticator = GlobusOAuthenticator()
-    # Allow any idp
-    authenticator.identity_provider = 'serenity.com'
-    authenticator.username_from_email = True
-    um = user_model('wash@serenity.com', 'alan@serenity.com')
-    handler = globus_client.handler_for_user(um)
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'alan'
+    c = Config()
+    c.GlobusOAuthenticator.allow_all = True
+    c.GlobusOAuthenticator.username_from_email = True
+    c.GlobusOAuthenticator.identity_provider = "allowed.example.com"
+    authenticator = GlobusOAuthenticator(config=c)
+
+    handled_user_model = user_model(
+        'dummy@example.com', email='user1@allowed.example.com'
+    )
+    handler = globus_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+    assert auth_model
+    assert auth_model["name"] == "user1"
 
 
 async def test_username_from_email_restricted_fail(globus_client):
-    authenticator = GlobusOAuthenticator()
-    # Allow any idp
-    authenticator.identity_provider = 'serenity.com'
-    authenticator.username_from_email = True
-    um = user_model('wash@serenity.com', 'alan@tudyk.org')
-    handler = globus_client.handler_for_user(um)
+    c = Config()
+    c.GlobusOAuthenticator.allow_all = True
+    c.GlobusOAuthenticator.username_from_email = True
+    c.GlobusOAuthenticator.identity_provider = "allowed.example.com"
+    authenticator = GlobusOAuthenticator(config=c)
+
+    handled_user_model = user_model(
+        "user1@allowed.example.com", email="dummy@example.com"
+    )
+    handler = globus_client.handler_for_user(handled_user_model)
     with raises(web.HTTPError) as exc:
-        await authenticator.authenticate(handler)
+        await authenticator.get_authenticated_user(handler, None)
     assert exc.value.status_code == 403
 
 
 async def test_token_exclusion(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.exclude_tokens = [
-        'transfer.api.globus.org',
-        'auth.globus.org',
-        'groups.api.globus.org',
+    c = Config()
+    c.GlobusOAuthenticator.allow_all = True
+    c.GlobusOAuthenticator.exclude_tokens = [
+        "auth.globus.org",
+        "groups.api.globus.org",
+        "transfer.api.globus.org",
     ]
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-    assert list(data['auth_state']['tokens'].keys()) == []
+    authenticator = GlobusOAuthenticator(config=c)
 
+    handled_user_model = user_model("user1@example.com")
+    handler = globus_client.handler_for_user(handled_user_model)
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+    assert auth_model
+    assert auth_model['auth_state']
+    assert not auth_model['auth_state']['tokens']
 
-async def test_revoke_tokens(globus_client, mock_globus_user):
 
+async def test_revoke_tokens(globus_client, mock_globus_user):
     # Wrap the revocation host to 'revoke' tokens by setting them in user auth
     # state. This way, we can get feedback to tell if the token was actually
     # sent to our 'host'
     def tok_revoke(request):
         resp = revoke_token_request_handler(request)
         token = parse_qs(request.body.decode('utf8'))['token'][0]
         for token_dict in mock_globus_user.state['tokens'].values():
@@ -387,49 +510,14 @@
     await logout_handler.get()
     auth_state = await mock_globus_user.get_auth_state()
     assert auth_state == {'tokens': {}}
 
 
 async def test_group_scope_added(globus_client):
     authenticator = GlobusOAuthenticator()
-    authenticator.allowed_globus_groups = set({'21c6bc5d-fc12-4f60-b999-76766cd596c2'})
+    authenticator.allowed_globus_groups = {'group-manager'}
     assert authenticator.scope == [
         'openid',
         'profile',
         'urn:globus:auth:scope:transfer.api.globus.org:all',
         'urn:globus:auth:scope:groups.api.globus.org:view_my_groups_and_memberships',
     ]
-
-
-async def test_user_in_allowed_group(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.allowed_globus_groups = set({'21c6bc5d-fc12-4f60-b999-76766cd596c2'})
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-
-
-async def test_user_not_allowed(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.allowed_globus_groups = set({'3f1f85c4-f084-4173-9efb-7c7e0b44291a'})
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data == None
-
-
-async def test_user_is_admin(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.admin_globus_groups = set({'21c6bc5d-fc12-4f60-b999-76766cd596c2'})
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-    assert data['admin'] == True
-
-
-async def test_user_allowed_not_admin(globus_client):
-    authenticator = GlobusOAuthenticator()
-    authenticator.allowed_globus_groups = set({'21c6bc5d-fc12-4f60-b999-76766cd596c2'})
-    authenticator.admin_globus_groups = set({'3f1f85c4-f084-4173-9efb-7c7e0b44291a'})
-    handler = globus_client.handler_for_user(user_model('wash@uflightacademy.edu'))
-    data = await authenticator.authenticate(handler)
-    assert data['name'] == 'wash'
-    assert data['admin'] == False
```

### Comparing `oauthenticator-15.1.0/oauthenticator/tests/test_mediawiki.py` & `oauthenticator-16.0.0/oauthenticator/tests/test_mediawiki.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import json
 import re
 import time
 from unittest.mock import Mock
 
 import jwt
 import requests_mock
-from pytest import fixture
+from pytest import fixture, mark
 from tornado import web
+from traitlets.config import Config
 
 from ..mediawiki import AUTH_REQUEST_COOKIE_NAME, MWOAuthenticator
 from .mocks import mock_handler
 
-MW_URL = 'https://meta.wikimedia.org/w/index.php'
-
 
 @fixture
 def mediawiki():
     def post_token(request, context):
         authorization_header = request.headers['Authorization'].decode('utf8')
         request_nonce = re.search(r'oauth_nonce="(.*?)"', authorization_header).group(1)
         content = jwt.encode(
             {
-                'username': 'wash',
+                'username': 'user1',
                 'aud': 'client_id',
                 'iss': 'https://meta.wikimedia.org',
                 'iat': time.time(),
                 'nonce': request_nonce,
             },
             'client_secret',
         ).encode()
@@ -41,45 +40,93 @@
             '/w/index.php?title=Special%3AOAuth%2Ftoken',
             text='oauth_token=key&oauth_token_secret=secret',
         )
         mock.post('/w/index.php?title=Special%3AOAuth%2Fidentify', content=post_token)
         yield mock
 
 
-def new_authenticator():
-    return MWOAuthenticator(
-        client_id='client_id',
-        client_secret='client_secret',
-    )
-
+@mark.parametrize(
+    "test_variation_id,class_config,expect_allowed,expect_admin",
+    [
+        # no allow config tested
+        ("00", {}, False, None),
+        # allow config, individually tested
+        ("01", {"allow_all": True}, True, None),
+        ("02", {"allowed_users": {"user1"}}, True, None),
+        ("03", {"allowed_users": {"not-test-user"}}, False, None),
+        ("04", {"admin_users": {"user1"}}, True, True),
+        ("05", {"admin_users": {"not-test-user"}}, False, None),
+        # allow config, some combinations of two tested
+        (
+            "10",
+            {
+                "allow_all": False,
+                "allowed_users": {"not-test-user"},
+            },
+            False,
+            None,
+        ),
+        (
+            "11",
+            {
+                "admin_users": {"user1"},
+                "allowed_users": {"not-test-user"},
+            },
+            True,
+            True,
+        ),
+    ],
+)
+async def test_mediawiki(
+    mediawiki,
+    test_variation_id,
+    class_config,
+    expect_allowed,
+    expect_admin,
+):
+    print(f"Running test variation id {test_variation_id}")
+    c = Config()
+    c.MWOAuthenticator = Config(class_config)
+    c.MWOAuthenticator.client_id = "client_id"
+    c.MWOAuthenticator.client_secret = "client_secret"
+    c.MWOAuthenticator.username_claim = "username"
+    authenticator = MWOAuthenticator(config=c)
 
-async def test_mediawiki(mediawiki):
-    authenticator = new_authenticator()
     handler = Mock(
         spec=web.RequestHandler,
         get_secure_cookie=Mock(return_value=json.dumps(['key', 'secret'])),
         request=Mock(query='oauth_token=key&oauth_verifier=me'),
+        find_user=Mock(return_value=None),
     )
-    user = await authenticator.authenticate(handler, None)
-    assert user['name'] == 'wash'
-    auth_state = user['auth_state']
-    assert auth_state['ACCESS_TOKEN_KEY'] == 'key'
-    assert auth_state['ACCESS_TOKEN_SECRET'] == 'secret'
-    identity = auth_state['MEDIAWIKI_USER_IDENTITY']
-    assert identity['username'] == user['name']
+    auth_model = await authenticator.get_authenticated_user(handler, None)
+
+    if expect_allowed:
+        assert auth_model
+        assert set(auth_model) == {"name", "admin", "auth_state"}
+        assert auth_model["admin"] == expect_admin
+        auth_state = auth_model["auth_state"]
+        assert "ACCESS_TOKEN_KEY" in auth_state
+        assert "ACCESS_TOKEN_SECRET" in auth_state
+        user_info = auth_state[authenticator.user_auth_state_key]
+        assert auth_model["name"] == user_info[authenticator.username_claim]
+    else:
+        assert auth_model == None
 
 
 async def test_login_redirect(mediawiki):
-    authenticator = new_authenticator()
+    authenticator = MWOAuthenticator(
+        client_id='client_id',
+        client_secret='client_secret',
+    )
     record = []
     handler = mock_handler(
         authenticator.login_handler,
         'https://hub.example.com/hub/login',
         authenticator=authenticator,
     )
     handler.write = lambda buf: record.append(buf)
     await handler.get()
     assert handler.get_status() == 302
     assert 'Location' in handler._headers
-    assert handler._headers['Location'].startswith(MW_URL)
+    assert handler._headers['Location'].startswith(authenticator.mw_index_url)
     assert 'Set-Cookie' in handler._headers
     assert AUTH_REQUEST_COOKIE_NAME in handler._headers['Set-Cookie']
```

### Comparing `oauthenticator-15.1.0/oauthenticator.egg-info/PKG-INFO` & `oauthenticator-16.0.0/oauthenticator.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: oauthenticator
-Version: 15.1.0
+Version: 16.0.0
 Summary: OAuthenticator: Authenticate JupyterHub users with common OAuth providers
 Home-page: https://jupyter.org
 Author: Jupyter Development Team
 Author-email: jupyter@googlegroups.com
 License: BSD
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: Linux
 Platform: Mac OS X
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: azuread
 Provides-Extra: googlegroups
+Provides-Extra: mediawiki
+Provides-Extra: test
 License-File: LICENSE
 
 # OAuth + JupyterHub Authenticator = OAuthenticator :heart:
 
 [![Documentation build status](https://img.shields.io/readthedocs/oauthenticator?logo=read-the-docs)](https://oauthenticator.readthedocs.org/en/latest)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/jupyterhub/oauthenticator/Tests?logo=github)](https://github.com/jupyterhub/oauthenticator/actions)
+[![GitHub Workflow Status - Test](https://img.shields.io/github/actions/workflow/status/jupyterhub/oauthenticator/test.yml?logo=github&label=tests)](https://github.com/jupyterhub/oauthenticator/actions)
 [![Latest PyPI version](https://img.shields.io/pypi/v/oauthenticator?logo=pypi)](https://pypi.python.org/pypi/oauthenticator)
 [![Latest conda-forge version](https://img.shields.io/conda/vn/conda-forge/oauthenticator?logo=conda-forge)](https://anaconda.org/conda-forge/oauthenticator)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/jupyterhub/oauthenticator/issues)
 [![Discourse](https://img.shields.io/badge/help_forum-discourse-blue?logo=discourse)](https://discourse.jupyter.org/c/jupyterhub)
 [![Gitter](https://img.shields.io/badge/social_chat-gitter-blue?logo=gitter)](https://gitter.im/jupyterhub/jupyterhub)
 
 [OAuth](https://en.wikipedia.org/wiki/OAuth) is a token based login mechanism that doesn't rely on a username and password mapping.
@@ -43,40 +46,27 @@
 
 There is also a [GenericAuthenticator](oauthenticator/generic.py)
 that can be configured with any OAuth 2.0 identity provider or can be used
 to create a new authenticator class when additional customization is needed.
 
 ## Installation
 
-The installation guide can be found in the [docs](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#installation).
+The installation guide can be found in the [docs](https://oauthenticator.readthedocs.io/en/latest/tutorials/install.html).
 
-The docs also provide example setups for different OAuth2 identity providers:
-
-- [General Setup](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#general-setup)
-- [Azure AD](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#azure-ad-setup)
-- [FeiShu](https://github.com/tezignlab/jupyterhub_feishu_authenticator)
-- [GitHub](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#github-setup)
-- [GitLab](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#gitlab-setup)
-- [Google](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#google-setup)
-- [OpenShift](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#openshift-setup)
-- [Okpy](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#okpyauthenticator)
-- [Globus](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#globus-setup)
-- [Moodle](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#moodle-setup)
-- [Yandex](https://oauthenticator.readthedocs.io/en/latest/getting-started.html#yandex-setup)
+The [docs](https://oauthenticator.readthedocs.io/en/latest/tutorials/provider-specific-setup/index.html) also provide example setups for different OAuth2 identity providers.
 
 ## Running tests
 
-To run the tests locally:
+To run the tests locally, first setup a development environment as described in
+[CONTRIBUTING.md], and then do:
 
 ```
-$ pip install --upgrade --pre -r test-requirements.txt
-```
-
-```
-$ pytest -v ./oauthenticator/tests/
+pytest -v ./oauthenticator/tests/
 ```
 
 Or you run a specific test file with:
 
 ```
-$ pytest -v ./oauthenticator/tests/<test-file-name>
+pytest -v ./oauthenticator/tests/<test-file-name>
 ```
+
+[contributing.md]: https://github.com/jupyterhub/oauthenticator/blob/main/CONTRIBUTING.md
```

### Comparing `oauthenticator-15.1.0/oauthenticator.egg-info/SOURCES.txt` & `oauthenticator-16.0.0/oauthenticator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
-test-requirements.txt
 oauthenticator/__init__.py
 oauthenticator/_version.py
 oauthenticator/auth0.py
-oauthenticator/awscognito.py
 oauthenticator/azuread.py
-oauthenticator/azureadb2c.py
 oauthenticator/bitbucket.py
 oauthenticator/cilogon.py
-oauthenticator/common.py
 oauthenticator/generic.py
 oauthenticator/github.py
 oauthenticator/gitlab.py
 oauthenticator/globus.py
 oauthenticator/google.py
 oauthenticator/mediawiki.py
 oauthenticator/oauth2.py
 oauthenticator/okpy.py
 oauthenticator/openshift.py
-oauthenticator/traitlets.py
-oauthenticator/yandex.py
 oauthenticator.egg-info/PKG-INFO
 oauthenticator.egg-info/SOURCES.txt
 oauthenticator.egg-info/dependency_links.txt
 oauthenticator.egg-info/entry_points.txt
 oauthenticator.egg-info/requires.txt
 oauthenticator.egg-info/top_level.txt
 oauthenticator/schemas/cilogon-schema.yaml
```

### Comparing `oauthenticator-15.1.0/oauthenticator.egg-info/entry_points.txt` & `oauthenticator-16.0.0/oauthenticator.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oauthenticator-15.1.0/setup.py` & `oauthenticator-16.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 #!/usr/bin/env python
-# coding: utf-8
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 # -----------------------------------------------------------------------------
 # Minimal Python version sanity check (from IPython/Jupyterhub)
 # -----------------------------------------------------------------------------
-from __future__ import print_function
 
-import os
 import sys
 
 from setuptools import find_packages, setup
 from setuptools.command.bdist_egg import bdist_egg
 
 
 class bdist_egg_disabled(bdist_egg):
@@ -23,37 +20,28 @@
 
     def run(self):
         sys.exit(
             "Aborting implicit building of eggs. Use `pip install .` to install from source."
         )
 
 
-pjoin = os.path.join
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Get the current package version.
-version_ns = {}
-with open(pjoin(here, 'oauthenticator', '_version.py')) as f:
-    exec(f.read(), {}, version_ns)
-
-
 setup_args = dict(
     name='oauthenticator',
     packages=find_packages(),
-    version=version_ns['__version__'],
+    version="16.0.0",
     description="OAuthenticator: Authenticate JupyterHub users with common OAuth providers",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Jupyter Development Team",
     author_email="jupyter@googlegroups.com",
     url="https://jupyter.org",
     license="BSD",
     platforms="Linux, Mac OS X",
     keywords=['Interactive', 'Interpreter', 'Shell', 'Web'],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     include_package_data=True,
     entry_points={
         'jupyterhub.authenticators': [
             'auth0 = oauthenticator.auth0:Auth0OAuthenticator',
             'local-auth0 = oauthenticator.auth0:LocalAuth0OAuthenticator',
             'azuread = oauthenticator.azuread:AzureAdOAuthenticator',
             'local-azuread = oauthenticator.azuread:LocalAzureAdOAuthenticator',
@@ -98,15 +86,39 @@
         req = line.strip()
         if not req or req.startswith(('-e', '#')):
             continue
         install_requires.append(req)
 
 
 setup_args['extras_require'] = {
-    'googlegroups': ['google-api-python-client', 'google-auth-oauthlib'],
+    # azuread is required for use of AzureADOAuthenticator
+    'azuread': ['pyjwt>=2'],
+    # googlegroups is required for use of GoogleOAuthenticator configured with
+    # either admin_google_groups and/or allowed_google_groups.
+    'googlegroups': [
+        'google-api-python-client',
+        'google-auth-oauthlib',
+    ],
+    # mediawiki is required for use of MWOAuthenticator
+    'mediawiki': ['mwoauth>=0.3.8'],
+    # test is required to run tests, and includes all authenticator specific
+    # dependencies above.
+    'test': [
+        'pytest>=2.8',
+        'pytest-asyncio',
+        'pytest-cov',
+        'requests-mock',
+        # dependencies from azuread:
+        'pyjwt>=2',
+        # dependencies from googlegroups:
+        'google-api-python-client',
+        'google-auth-oauthlib',
+        # dependencies from mediawiki:
+        'mwoauth>=0.3.8',
+    ],
 }
 
 
 def main():
     setup(**setup_args)
```

