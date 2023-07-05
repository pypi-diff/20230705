# Comparing `tmp/idf_build_apps-1.0.1.tar.gz` & `tmp/idf_build_apps-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.1.tar` & `idf_build_apps-1.0.2.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0      351 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.editorconfig
--rw-r--r--   0        0        0      123 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.gitattributes
--rw-r--r--   0        0        0      253 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3767 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.gitignore
--rw-r--r--   0        0        0     1077 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/.readthedocs.yml
--rw-r--r--   0        0        0     5204 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1882 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/LICENSE
--rw-r--r--   0        0        0     3843 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/README.md
--rw-r--r--   0        0        0       33 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/config_file.md
--rw-r--r--   0        0        0    10473 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/index.rst
--rw-r--r--   0        0        0     5717 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    26619 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/config.py
--rw-r--r--   0        0        0     2187 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6328 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/log.py
--rw-r--r--   0        0        0    30607 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6321 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     6748 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/license_header.txt
--rw-r--r--   0        0        0     1911 2023-06-12 08:52:33.078932 idf_build_apps-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_build.py
--rw-r--r--   0        0        0    16908 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_finder.py
--rw-r--r--   0        0        0      995 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_manifest.py
--rw-r--r--   0        0        0     3710 2023-06-12 08:52:33.082932 idf_build_apps-1.0.1/tests/test_utils.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.1/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.editorconfig
+-rw-r--r--   0        0        0      123 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-07-05 01:10:03.945090 idf_build_apps-1.0.2/.gitattributes
+-rw-r--r--   0        0        0      513 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      253 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3870 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1077 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/.readthedocs.yml
+-rw-r--r--   0        0        0     5408 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3843 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/README.md
+-rw-r--r--   0        0        0       33 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0     5894 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    27051 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2182 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30607 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6368 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     5956 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7081 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-07-05 01:10:03.949090 idf_build_apps-1.0.2/license_header.txt
+-rw-r--r--   0        0        0     2060 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_build.py
+-rw-r--r--   0        0        0    16908 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_finder.py
+-rw-r--r--   0        0        0     1568 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-07-05 01:10:03.953090 idf_build_apps-1.0.2/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.2/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.2/PKG-INFO
```

### Comparing `idf_build_apps-1.0.1/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.2/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.2/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.2/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.2/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.2/.github/workflows/test-build-idf-apps.yml`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
           name: wheel
       - name: Build the Apps
         run: |
           export PYENV_ROOT="$HOME/.pyenv" && export PATH="$PYENV_ROOT/bin:$PATH" && eval "$(pyenv init --path)"
           pyenv global ${{ matrix.python-version }}
           rm $(which python3)
           echo "urllib3<1.25,>=1.21.1" >> $IDF_PATH/requirements.txt
+          sed -i 's/idf-component-manager~=1.0/idf-component-manager<1.3/g' $IDF_PATH/requirements.txt
           bash $IDF_PATH/install.sh
           . $IDF_PATH/export.sh
           pip install idf_build_apps-*-py2.py3-none-any.whl
           python -m idf_build_apps build -vv -t esp32 \
             -p $IDF_PATH/examples/get-started/hello_world \
             --size-file size_info.json \
             --ignore-warning-str \
```

### Comparing `idf_build_apps-1.0.1/.gitignore` & `idf_build_apps-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/.pre-commit-config.yaml` & `idf_build_apps-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/CHANGELOG.md` & `idf_build_apps-1.0.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-## [1.0.1] (2023-06-12)
+## v1.0.2 (2023-07-05)
 
-## Fixed
+### Feat
+
+- support placeholder "@v"
+- Support keyword `IDF_VERSION` in the if statement
+
+### Fix
+
+- non-ascii character
+- build failed with warnings even without passing `--check-warnings`
+
+## v1.0.1 (2023-06-12)
+
+### Fixed
 
 - glob patterns are matched recursively
 
-## [1.0.0] (2023-05-25)
+## v1.0.0 (2023-05-25)
 
-## Added
+### Added
 
 - Support keyword `depends_filepatterns` in the manifest file
 - Support expanding environment variables in the manifest files
 
-## BREAKING CHANGES
+### BREAKING CHANGES
 
 - Attributes Renamed
   - `App.requires_components` renamed to `App.depends_components`
   - `FolderRule.requires_components` renamed to `FolderRule.depends_components`
 - Functions Renamed
   - `Manifest.requires_components()` renamed to `Manifest.depends_components()`
 - Signatures Changed
@@ -34,21 +46,21 @@
 - Removed the deprecated CLI call methods, now these options only support space-separated list
   - `--exclude`
   - `--config`
   - `--manifest-file`
   - `--ignore-warning-str`
   - `--default-build-targets`
 
-## [0.6.1] (2023-05-10)
+## v0.6.1 (2023-05-10)
 
 ### Fixed
 
 - Add missing dependency `pyyaml`. It's wrongly removed in 0.6.0.
 
-## [0.6.0] (2023-05-08) (yanked)
+## v0.6.0 (2023-05-08) (yanked)
 
 ### Added
 
 - Support configuration file with
   - `tool.idf-build-apps` section under `pyproject.toml` file
   - `.idf_build_apps.toml` file
 - Improve help message, include default value, config name, and config type
@@ -67,51 +79,51 @@
 - Remove unused dependency `pyyaml`
 
 ### Refactored
 
 - Move `utils.setup_logging()` to `log.setup_logging()`
 - Make CLI option `--default-build-targets` from comma-separated list to space-separated list (comma-separated list support will be removed in 1.0.0)
 
-## [0.5.2] (2023-04-07)
+## v0.5.2 (2023-04-07)
 
 ### Fixed
 
 - Remove empty expanded sdkconfig files folder after build
 - Split up expanded sdkconfig files folder for different build
 
-## [0.5.1] (2023-04-06)
+## v0.5.1 (2023-04-06)
 
 ### Fixed
 
 - Build with expanded sdkconfig file would respect the target-specific one under the original path
 
-## [0.5.0] (2023-03-29)
+## v0.5.0 (2023-03-29)
 
 ### Added
 
 - Add an executable script `idf-build-apps`. Now this tool could be run via `idf-build-apps build ...` instead of `python -m idf_build_apps build ...`
 - Support specify `-DSDKCONFIG_DEFAULTS` for `idf.py build`
   - via CLI option `--sdkconfig-defaults`
   - via environment variable `SDKCONFIG_DEFAULTS`
 
 ### Fixed
 
 - CLI option `-t`, `--target` is required, improve the error message
 
-## [0.4.1] (2023-03-15)
+## v0.4.1 (2023-03-15)
 
 ### Fixed
 
 - Stop writing `app_info` and `size_info` if the build got skipped
 - `IDF_VERSION_MAJOR`, `IDF_VERSION_MINOR`, `IDF_VERSION_PATCH` now are integers
 - Skip exclude files while removing build directory if files not exist
 - Use log level `INFO` for ignored warnings
 - Can't use `and` in if clauses
 
-## [0.4.0] (2023-03-09)
+## v0.4.0 (2023-03-09)
 
 This is the last version to support ESP-IDF v4.1 since it's EOL on Feb. 24th, 2023.
 
 ### Added
 
 - Support new keywords `IDF_VERSION_MAJOR`, `IDF_VERSION_MINOR`, `IDF_VERSION_PATCH` in the manifest file
 - Support colored output by default in UNIX-like systems
@@ -120,48 +132,48 @@
   - Add `--ignore-component-dependencies-file-patterns` CLI option
   - Add `--depends-on-files` CLI option
 
 ### Fixed
 
 - Improve the readability of the generated logs
 
-## [0.3.2] (2023-03-08)
+## v0.3.2 (2023-03-08)
 
 ### Fixed
 
 - `idf.py reconfigure` without setting `IDF_TARGET`
 - wrong log level on "Loading manifest file: ...". Set from `INFO` to `DEBUG`
 - wrong log level on "Building app \[ID\]: ...". Set from `DEBUG` to `INFO`
 
-## [0.3.1] (2023-02-20)
+## v0.3.1 (2023-02-20)
 
 ### Fixed
 
 - Relative path defined in the manifest files depend on the current work path
 
   Added `manifest_rootpath` argument in `find_apps()`. Will use this value instead as the root folder for calculating absolute path
 
-## [0.3.0] (2023-01-10)
+## v0.3.0 (2023-01-10)
 
 ### Added
 
 - `find_apps`, `build_apps` support `--depends-on-components`, will only find or build apps that require specified components
 - manifest file support `requires_components`
 
 ### Fixed
 
 -  Wrong `App.verified_targets` when `CONFIG_IDF_TARGET` set in app's `sdkconfig.defaults` file
 
-## [0.2.1] (2022-09-02)
+## v0.2.1 (2022-09-02)
 
 ### Fixed
 
 - Fix `--format json` incompatible issue for IDF branches earlier than 5.0
 - Fix type annotations incompatible issue for python versions earlier than 3.7
 - Fix f-string incompatible issue for python versions earlier than 3.7
 - Fix unpack dictionary ending comma syntax error for python 3.4
 
-## [0.2.0] (2022-08-31)
+## v0.2.0 (2022-08-31)
 
 ### Added
 
 - Use `--format json` instead of `--json` with `idf_size.py`
```

### Comparing `idf_build_apps-1.0.1/CONTRIBUTING.md` & `idf_build_apps-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/LICENSE` & `idf_build_apps-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/README.md` & `idf_build_apps-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/Makefile` & `idf_build_apps-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.2/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.2/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/conf.py` & `idf_build_apps-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/config_file.md` & `idf_build_apps-1.0.2/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/find_build.md` & `idf_build_apps-1.0.2/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/docs/manifest.md` & `idf_build_apps-1.0.2/docs/manifest.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ## `if` Clauses
 
 ### Operands
 
 - Capitalized Words
   - Variables start with `SOC_`. The value would be parsed from `IDF_PATH/components/soc/[TARGET]/include/soc/*_caps.h`
   - `IDF_TARGET`
+  - `IDF_VERSION` (IDF_VERSION_MAJOR.IDF_VERSION_MINOR.IDF_VERSION_PATCH. e.g., 5.2.0. Will convert to Version object to do a version comparison instead of a string comparison)
   - `IDF_VERSION_MAJOR`
   - `IDF_VERSION_MINOR`
   - `IDF_VERSION_PATCH`
   - `INCLUDE_DEFAULT` (The default value of officially supported targets is 1, otherwise is 0)
   - `CONFIG_NAME` (config name defined in [](project:#config-rules))
   - environment variables, default to `0` if not set
 - String, must be double-quoted. e.g., `"esp32"`, `"12345"`
```

### Comparing `idf_build_apps-1.0.1/idf_build_apps/app.py` & `idf_build_apps-1.0.2/idf_build_apps/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     LOGGER,
 )
 from .constants import (
     DEFAULT_SDKCONFIG,
     IDF_PY,
     IDF_SIZE_PY,
     IDF_VERSION,
+    IDF_VERSION_MAJOR,
+    IDF_VERSION_MINOR,
+    IDF_VERSION_PATCH,
     PROJECT_DESCRIPTION_JSON,
 )
 from .manifest.manifest import (
     FolderRule,
     Manifest,
 )
 from .utils import (
@@ -60,14 +63,15 @@
 class App(object):
     TARGET_PLACEHOLDER = '@t'  # replace it with self.target
     WILDCARD_PLACEHOLDER = '@w'  # replace it with the wildcard, usually the sdkconfig
     NAME_PLACEHOLDER = '@n'  # replace it with self.name
     FULL_NAME_PLACEHOLDER = '@f'  # replace it with escaped self.app_dir
     INDEX_PLACEHOLDER = '@i'  # replace it with the build index
     PARALLEL_INDEX_PLACEHOLDER = '@p'  # replace it with the parallel index
+    IDF_VERSION_PLACEHOLDER = '@v'  # replace it with the IDF version
 
     BUILD_SYSTEM = 'unknown'
 
     SDKCONFIG_LINE_REGEX = re.compile(r"^([^=]+)=\"?([^\"\n]*)\"?\n*$")
 
     # could be assigned later, used for filtering out apps by supported_targets
     MANIFEST = None  # type: Manifest | None
@@ -204,14 +208,17 @@
         """
         if not path:
             return path
 
         if self.index is not None:
             path = path.replace(self.INDEX_PLACEHOLDER, str(self.index))
         path = path.replace(self.PARALLEL_INDEX_PLACEHOLDER, str(self.parallel_index))
+        path = path.replace(
+            self.IDF_VERSION_PLACEHOLDER, '{}_{}_{}'.format(IDF_VERSION_MAJOR, IDF_VERSION_MINOR, IDF_VERSION_PATCH)
+        )
         path = path.replace(self.TARGET_PLACEHOLDER, self.target)
         path = path.replace(self.NAME_PLACEHOLDER, self.name)
         if self.FULL_NAME_PLACEHOLDER in path:  # to avoid recursion to the call to app_dir in the next line:
             path = path.replace(self.FULL_NAME_PLACEHOLDER, self.app_dir.replace(os.path.sep, '_'))
         wildcard_pos = path.find(self.WILDCARD_PLACEHOLDER)
         if wildcard_pos != -1:
             if self.config_name:
@@ -728,18 +735,22 @@
                 self.build_path,
                 exclude_file_patterns=exclude_list,
             )
 
         if returncode != 0:
             raise BuildError('Build failed with exit code {}'.format(returncode))
 
-        if has_unignored_warning:
+        if self.check_warnings and has_unignored_warning:
             raise BuildError('Build succeeded with warnings')
 
-        LOGGER.info('=> Build succeeded')
+        if has_unignored_warning:
+            LOGGER.info('=> Build succeeded with warnings')
+        else:
+            LOGGER.info('=> Build succeeded')
+
         return True
 
     @classmethod
     def is_app(cls, path):  # type: (str) -> bool
         cmakelists_path = os.path.join(path, 'CMakeLists.txt')
         if not os.path.exists(cmakelists_path):
             return False
```

### Comparing `idf_build_apps-1.0.1/idf_build_apps/config.py` & `idf_build_apps-1.0.2/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/constants.py` & `idf_build_apps-1.0.2/idf_build_apps/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import re
 import sys
 import tempfile
 from pathlib import (
     Path,
 )
 
-from packaging.version import (
-    Version,
+from .utils import (
+    to_version,
 )
 
 _BUILDING_DOCS = bool(os.getenv('BUILDING_DOCS'))
 if _BUILDING_DOCS:
     print('Building Docs... Faking lots of constant values')
 
 
@@ -65,8 +65,8 @@
 
 
 if _BUILDING_DOCS:
     IDF_VERSION_MAJOR, IDF_VERSION_MINOR, IDF_VERSION_PATCH = 1, 0, 0
 else:
     IDF_VERSION_MAJOR, IDF_VERSION_MINOR, IDF_VERSION_PATCH = _idf_version_from_cmake()
 
-IDF_VERSION = Version('{}.{}.{}'.format(IDF_VERSION_MAJOR, IDF_VERSION_MINOR, IDF_VERSION_PATCH))
+IDF_VERSION = to_version('{}.{}.{}'.format(IDF_VERSION_MAJOR, IDF_VERSION_MINOR, IDF_VERSION_PATCH))
```

### Comparing `idf_build_apps-1.0.1/idf_build_apps/finder.py` & `idf_build_apps-1.0.2/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/log.py` & `idf_build_apps-1.0.2/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/main.py` & `idf_build_apps-1.0.2/idf_build_apps/main.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.2/idf_build_apps/manifest/if_parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 from ast import (
     literal_eval,
 )
 
+from packaging.version import (
+    Version,
+)
 from pyparsing import (
     Keyword,
     Literal,
     QuotedString,
     Suppress,
     Word,
     alphas,
@@ -17,18 +20,23 @@
     hexnums,
     infixNotation,
     nums,
     opAssoc,
 )
 
 from ..constants import (
+    IDF_VERSION,
     IDF_VERSION_MAJOR,
     IDF_VERSION_MINOR,
     IDF_VERSION_PATCH,
 )
+from ..utils import (
+    InvalidInput,
+    to_version,
+)
 from .soc_header import (
     SOC_HEADERS,
 )
 
 
 class Stmt:
     """
@@ -68,14 +76,17 @@
 
         if self.attr == 'IDF_TARGET':
             return target
 
         if self.attr == 'INCLUDE_DEFAULT':
             return 1 if target in FolderRule.DEFAULT_BUILD_TARGETS else 0
 
+        if self.attr == 'IDF_VERSION':
+            return IDF_VERSION
+
         if self.attr == 'IDF_VERSION_MAJOR':
             return IDF_VERSION_MAJOR
 
         if self.attr == 'IDF_VERSION_MINOR':
             return IDF_VERSION_MINOR
 
         if self.attr == 'IDF_VERSION_PATCH':
@@ -115,45 +126,50 @@
         self.expr = t
 
     def get_value(self, target, config_name):  # type: (str, str) -> any
         return [item.get_value(target, config_name) for item in self.expr]
 
 
 class BoolStmt(Stmt):
+    _OP_DICT = {
+        '==': lambda x, y: x == y,
+        '!=': lambda x, y: x != y,
+        '>': lambda x, y: x > y,
+        '>=': lambda x, y: x >= y,
+        '<': lambda x, y: x < y,
+        '<=': lambda x, y: x <= y,
+        'not in': lambda x, y: x not in y,
+        'in': lambda x, y: x in y,
+    }
+
     def __init__(self, t):
         self.left = t[0]  # type: Stmt
         self.comparison = t[1]  # type: str
         self.right = t[2]  # type: Stmt
 
     def get_value(self, target, config_name):  # type: (str, str) -> any
-        if self.comparison == '==':
-            return self.left.get_value(target, config_name) == self.right.get_value(target, config_name)
-
-        if self.comparison == '!=':
-            return self.left.get_value(target, config_name) != self.right.get_value(target, config_name)
-
-        if self.comparison == '>':
-            return self.left.get_value(target, config_name) > self.right.get_value(target, config_name)
-
-        if self.comparison == '>=':
-            return self.left.get_value(target, config_name) >= self.right.get_value(target, config_name)
-
-        if self.comparison == '<':
-            return self.left.get_value(target, config_name) < self.right.get_value(target, config_name)
-
-        if self.comparison == '<=':
-            return self.left.get_value(target, config_name) <= self.right.get_value(target, config_name)
+        _l = self.left.get_value(target, config_name)
+        _r = self.right.get_value(target, config_name)
 
-        if self.comparison == 'not in':
-            return self.left.get_value(target, config_name) not in self.right.get_value(target, config_name)
+        if self.comparison not in ['in', 'not in']:
+            # will use version comparison if any of the operands is a Version
+            if any(isinstance(x, Version) for x in [_l, _r]):
+                _l = to_version(_l)
+                _r = to_version(_r)
+        else:
+            # use str for "in" and "not in" operator
+            if isinstance(_l, Version):
+                _l = str(_l)
+            if isinstance(_r, Version):
+                _r = str(_r)
 
-        if self.comparison == 'in':
-            return self.left.get_value(target, config_name) in self.right.get_value(target, config_name)
+        if self.comparison in self._OP_DICT:
+            return self._OP_DICT[self.comparison](_l, _r)
 
-        raise ValueError('Unsupported comparison operator: "{}"'.format(self.comparison))
+        raise InvalidInput('Unsupported comparison operator: "{}"'.format(self.comparison))
 
 
 class BoolExpr(Stmt):
     pass
 
 
 class BoolAnd(BoolExpr):
```

### Comparing `idf_build_apps-1.0.1/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.2/idf_build_apps/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.2/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/idf_build_apps/utils.py` & `idf_build_apps-1.0.2/idf_build_apps/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from copy import (
     deepcopy,
 )
 from pathlib import (
     Path,
 )
 
+from packaging.version import (
+    Version,
+)
+
 from . import (
     LOGGER,
 )
 
 try:
     import typing as t
 except ImportError:
@@ -31,15 +35,15 @@
 
 class ConfigRule:
     def __init__(self, file_name, config_name):  # type: (str, str) -> None
         """
         ConfigRule represents the sdkconfig file and the config name.
 
         For example:
-            - filename='', config_name='default' — represents the default app configuration, and gives it a name
+            - filename='', config_name='default' - represents the default app configuration, and gives it a name
                 'default'
             - filename='sdkconfig.*', config_name=None - represents the set of configurations, names match the wildcard
                 value
 
         :param file_name: name of the sdkconfig file fragment, optionally with a single wildcard ('*' character).
             can also be empty to indicate that the default configuration of the app should be used
         :param config_name: name of the corresponding build configuration, or None if the value of wildcard is to be
@@ -99,14 +103,18 @@
 
 
 class InvalidCommand(SystemExit):
     def __init__(self, msg):
         super(InvalidCommand, self).__init__('Invalid Command: ' + msg.strip())
 
 
+class InvalidInput(SystemExit):
+    """Invalid input from user"""
+
+
 def rmdir(path, exclude_file_patterns=None):
     if not exclude_file_patterns:
         shutil.rmtree(path, ignore_errors=True)
         return
 
     for root, dirs, files in os.walk(path, topdown=False):
         for f in files:
@@ -210,14 +218,24 @@
     sp = Path(os.path.expanduser(s))
     if sp.is_absolute():
         return sp.resolve()
     else:
         return (rp / sp).resolve()
 
 
+def to_version(s):  # type: (any) -> Version
+    if isinstance(s, Version):
+        return s
+
+    try:
+        return Version(str(s))
+    except ValueError:
+        raise InvalidInput('Invalid version: {}'.format(s))
+
+
 def files_matches_patterns(
     files,  # type: list[str] | str
     patterns,  # type: list[str] | str
     rootpath=None,  # type: str
 ):  # type: (...) -> bool
     # can't match an absolute pattern with a relative path
     # change all to absolute paths
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `idf_build_apps-1.0.1/pyproject.toml` & `idf_build_apps-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,22 @@
 repository = "https://github.com/espressif/idf-build-apps"
 documentation = "https://docs.espressif.com/projects/idf-build-apps"
 changelog = "https://github.com/espressif/idf-build-apps/blob/master/CHANGELOG.md"
 
 [project.scripts]
 idf-build-apps = "idf_build_apps:main.main"
 
+[tool.commitizen]
+name = "cz_conventional_commits"
+version = "1.0.2"
+tag_format = "v$version"
+version_files = [
+    "idf_build_apps/__init__.py",
+]
+
 [tool.pytest.ini_options]
 addopts = "-s --log-cli-level DEBUG"
 testpaths = [
     "tests",
 ]
 
 [tool.isort]
```

### Comparing `idf_build_apps-1.0.1/tests/conftest.py` & `idf_build_apps-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/tests/test_build.py` & `idf_build_apps-1.0.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/tests/test_finder.py` & `idf_build_apps-1.0.2/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/tests/test_manifest.py` & `idf_build_apps-1.0.2/tests/test_manifest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # SPDX-FileCopyrightText: 2022-2023 Espressif Systems (Shanghai) CO LTD
 # SPDX-License-Identifier: Apache-2.0
 
 import os
 
+from packaging.version import (
+    Version,
+)
+
+import idf_build_apps.constants
+from idf_build_apps.manifest.if_parser import (
+    BOOL_STMT,
+)
 from idf_build_apps.manifest.manifest import (
     Manifest,
 )
 
 
 def test_manifest(tmpdir):
     yaml_file = tmpdir / 'test.yml'
@@ -30,7 +38,17 @@
     Manifest.ROOTPATH = tmpdir
     manifest = Manifest.from_file(yaml_file)
 
     assert manifest.enable_build_targets('test1') == ['esp32', 'esp32c3', 'esp32s2']
     assert manifest.enable_test_targets('test1') == ['esp32', 'esp32s2']
     assert manifest.enable_build_targets('test2') == ['linux']
     assert manifest.enable_test_targets('test2') == ['linux']
+
+
+class TestIfParser:
+    def test_idf_version(self, monkeypatch):
+        monkeypatch.setattr(idf_build_apps.manifest.if_parser, 'IDF_VERSION', Version('5.9.0'))
+        statement = 'IDF_VERSION > "5.10.0"'
+        assert BOOL_STMT.parseString(statement)[0].get_value('esp32', 'foo') is False
+
+        statement = 'IDF_VERSION in  ["5.9.0"]'
+        assert BOOL_STMT.parseString(statement)[0].get_value('esp32', 'foo') is True
```

### Comparing `idf_build_apps-1.0.1/tests/test_utils.py` & `idf_build_apps-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.1/setup.py` & `idf_build_apps-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.1',
+      version='1.0.2',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.1/PKG-INFO` & `idf_build_apps-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.1
+Version: 1.0.2
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

