# Comparing `tmp/mkdocs-git-snippet-0.1.1.tar.gz` & `tmp/mkdocs-git-snippet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-snippet-0.1.1.tar", last modified: Tue Jan 19 09:47:53 2021, max compression
+gzip compressed data, was "mkdocs-git-snippet-0.1.2.tar", last modified: Wed Jul  5 01:14:14 2023, max compression
```

## Comparing `mkdocs-git-snippet-0.1.1.tar` & `mkdocs-git-snippet-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:47:53.819302 mkdocs-git-snippet-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)       43 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4160 2021-01-19 09:47:53.819302 mkdocs-git-snippet-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2865 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:47:53.815302 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1494 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/plugin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1832 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 09:47:53.815302 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4160 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      429 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       22 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       19 2021-01-19 09:47:53.000000 mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-01-19 09:47:53.819302 mkdocs-git-snippet-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1175 2021-01-19 09:47:41.000000 mkdocs-git-snippet-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:14:14.755391 mkdocs-git-snippet-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-05 01:14:14.751391 mkdocs-git-snippet-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:14:14.751391 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:14:14.751391 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 01:14:14.000000 mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:14:14.755391 mkdocs-git-snippet-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-05 01:14:03.000000 mkdocs-git-snippet-0.1.2/setup.py
```

### Comparing `mkdocs-git-snippet-0.1.1/PKG-INFO` & `mkdocs-git-snippet-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,140 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-snippet
-Version: 0.1.1
+Version: 0.1.2
 Summary: An MkDocs plugin that reads snippets from Github Repositories.
 Home-page: https://github.com/mercari/mkdocs-git-snippet
 Author: Mercari
 License: UNKNOWN
-Description: # mkdocs-git-snippet [![Test][test-badge]][test] [![Code style: black][black-badge]][black]
-        
-        <!-- badge links -->
-        [test-badge]: https://github.com/mercari/mkdocs-git-snippet/workflows/Test/badge.svg
-        [test]: https://github.com/mercari/mkdocs-git-snippet/actions?query=workflow%3ATest
-        [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-        [black]: https://github.com/psf/black
-        
-        Mkdocs Plugin for snippet from git repository.
-        
-        ## Installation
-        
-        ```shell
-        pip install mkdocs-git-snippet
-        ```
-        
-        ## Configuration
-        
-        Enable the plugin in your mkdocs.yml.
-        
-        ```markdown
-        plugins:
-          - git-snippet
-        ```
-        
-        If the folder name that contain your documentation source files is not default `docs`, you need specify it with `base_path` option.
-        
-        ```markdown
-        plugins:
-          - git-snippet:
-                base_path: docs
-        ```
-        
-        By default, this plugin works for all pages. You can enable only for the specific page by setting `all_pages` option to false.
-        
-        ```markdown
-        plugins:
-          - git-snippet:
-              all_pages: false
-        ```
-        
-        When `all_pages` is false, this plugin only works for the page that added `git-snippet: enable`.
-        
-        ```markdown
-        <!-- git-snippet: enable -->
-        
-        # Your document
-        ....
-        ```
-        
-        ## Usage
-        
-        ### All files from default branch
-        
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') }}
-        ```
-        
-        It works for non markdown file too. The snippet format is raw text.
-        Please format it if needed.
-        
-        ````
-        ```python
-        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py') }}
-        ```
-        ````
-        
-        ### All files from specific branch/tag/commit
-        
-        ````
-        ```python
-        { gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '1.1')
-        ```
-        ````
-        
-        ````
-        ```python
-        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '520314fed933aed8de62b08dd7fc6e25c0ff482b') }}
-        ```
-        ````
-        
-        ### Snippet a section
-        
-        For markdown file, it is possible to specify a section.
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', section='## Using Plugins') }}
-        ```
-        or
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', 'master', '## Using Plugins') }}
-        ```
-        
-        ### Insert indent
-        
-        You can insert indent to snippet using `indent`.
-        `indent` has an argument `width`, which means the number of space to indent by. The default is 4.
-        See more details of `indent` [here](https://jinja.palletsprojects.com/en/master/templates/#indent).
-        
-        ````
-        ??? example "Plugin.md"
-        
-            {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') | indent }}
-        
-            !!! note
-        
-                ```python
-                {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py) | indent(width=8) }}
-                ```
-        ````
-        
-        ## Contribution
-        
-        Please read the CLA carefully before submitting your contribution to Mercari.
-        Under any circumstances, by submitting your contribution, you are deemed to accept and agree to be bound by the terms and conditions of the CLA.
-        
-        https://www.mercari.com/cla/
-        
-        ## License
-        
-        Copyright 2021 Mercari, Inc.
-        
-        Licensed under the MIT License.
-        
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mkdocs-git-snippet [![Test][test-badge]][test] [![Code style: black][black-badge]][black]
+
+<!-- badge links -->
+[test-badge]: https://github.com/mercari/mkdocs-git-snippet/workflows/Test/badge.svg
+[test]: https://github.com/mercari/mkdocs-git-snippet/actions?query=workflow%3ATest
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black]: https://github.com/psf/black
+
+Mkdocs Plugin for snippet from git repository.
+
+## Installation
+
+```shell
+pip install mkdocs-git-snippet
+```
+
+## Configuration
+
+Enable the plugin in your mkdocs.yml.
+
+```markdown
+plugins:
+  - git-snippet
+```
+
+If the folder name that contain your documentation source files is not default `docs`, you need specify it with `base_path` option.
+
+```markdown
+plugins:
+  - git-snippet:
+        base_path: docs
+```
+
+By default, this plugin works for all pages. You can enable only for the specific page by setting `all_pages` option to false.
+
+```markdown
+plugins:
+  - git-snippet:
+      all_pages: false
+```
+
+When `all_pages` is false, this plugin only works for the page that added `git-snippet: enable`.
+
+```markdown
+<!-- git-snippet: enable -->
+
+# Your document
+....
+```
+
+### Acessing Private Repositories
+
+To add a snippet from a private repository set the `GITHUB_TOKEN` environment variable while building mkdocs documentation.
+
+## Usage
+
+### All files from default branch
+
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') }}
+```
+
+It works for non markdown file too. The snippet format is raw text.
+Please format it if needed.
+
+````
+```python
+{{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py') }}
+```
+````
+
+### All files from specific branch/tag/commit
+
+````
+```python
+{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '1.1')
+```
+````
+
+````
+```python
+{{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '520314fed933aed8de62b08dd7fc6e25c0ff482b') }}
+```
+````
+
+### Snippet a section
+
+For markdown file, it is possible to specify a section.
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', section='## Using Plugins') }}
+```
+or
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', 'master', '## Using Plugins') }}
+```
+
+### Insert indent
+
+You can insert indent to snippet using `indent`.
+`indent` has an argument `width`, which means the number of space to indent by. The default is 4.
+See more details of `indent` [here](https://jinja.palletsprojects.com/en/master/templates/#indent).
+
+````
+??? example "Plugin.md"
+
+    {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') | indent }}
+
+    !!! note
+
+        ```python
+        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py) | indent(width=8) }}
+        ```
+````
+
+## Contribution
+
+Please read the CLA carefully before submitting your contribution to Mercari.
+Under any circumstances, by submitting your contribution, you are deemed to accept and agree to be bound by the terms and conditions of the CLA.
+
+https://www.mercari.com/cla/
+
+## License
+
+Copyright 2021 Mercari, Inc.
+
+Licensed under the MIT License.
+
+
```

### Comparing `mkdocs-git-snippet-0.1.1/README.md` & `mkdocs-git-snippet-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 ```markdown
 <!-- git-snippet: enable -->
 
 # Your document
 ....
 ```
 
+### Acessing Private Repositories
+
+To add a snippet from a private repository set the `GITHUB_TOKEN` environment variable while building mkdocs documentation.
+
 ## Usage
 
 ### All files from default branch
 
 ```
 {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') }}
 ```
```

### Comparing `mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/plugin.py` & `mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import mkdocs
 from mkdocs.plugins import BasePlugin
 from jinja2 import Template
-from github import Github, GithubObject
+from github import Auth, Github, GithubObject
 
 from mkdocs_git_snippet.util import (
     skip_page,
     copy_markdown_images,
     get_markdown_section,
 )
 
@@ -16,15 +16,15 @@
     config_scheme = (
         ("base_path", mkdocs.config.config_options.Type(str, default="docs")),
         ("all_pages", mkdocs.config.config_options.Type(bool, default=True)),
     )
     page = None
 
     def _git_snippet(self, repository: str, file: str, ref: str, section: str) -> str:
-        g = Github(os.getenv("GITHUB_TOKEN"))
+        g = Github(auth=Auth.Token(os.getenv("GITHUB_TOKEN")))
         repo = g.get_repo(repository)
         f = repo.get_contents(file, ref=ref)
         content = f.decoded_content.decode("utf-8")
         if section:
             content = get_markdown_section(content, section)
 
         root = f"{self.config['base_path']}/{self.page.url}"
```

### Comparing `mkdocs-git-snippet-0.1.1/mkdocs_git_snippet/util.py` & `mkdocs-git-snippet-0.1.2/mkdocs_git_snippet/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-snippet-0.1.1/mkdocs_git_snippet.egg-info/PKG-INFO` & `mkdocs-git-snippet-0.1.2/mkdocs_git_snippet.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,140 @@
 Metadata-Version: 2.1
 Name: mkdocs-git-snippet
-Version: 0.1.1
+Version: 0.1.2
 Summary: An MkDocs plugin that reads snippets from Github Repositories.
 Home-page: https://github.com/mercari/mkdocs-git-snippet
 Author: Mercari
 License: UNKNOWN
-Description: # mkdocs-git-snippet [![Test][test-badge]][test] [![Code style: black][black-badge]][black]
-        
-        <!-- badge links -->
-        [test-badge]: https://github.com/mercari/mkdocs-git-snippet/workflows/Test/badge.svg
-        [test]: https://github.com/mercari/mkdocs-git-snippet/actions?query=workflow%3ATest
-        [black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
-        [black]: https://github.com/psf/black
-        
-        Mkdocs Plugin for snippet from git repository.
-        
-        ## Installation
-        
-        ```shell
-        pip install mkdocs-git-snippet
-        ```
-        
-        ## Configuration
-        
-        Enable the plugin in your mkdocs.yml.
-        
-        ```markdown
-        plugins:
-          - git-snippet
-        ```
-        
-        If the folder name that contain your documentation source files is not default `docs`, you need specify it with `base_path` option.
-        
-        ```markdown
-        plugins:
-          - git-snippet:
-                base_path: docs
-        ```
-        
-        By default, this plugin works for all pages. You can enable only for the specific page by setting `all_pages` option to false.
-        
-        ```markdown
-        plugins:
-          - git-snippet:
-              all_pages: false
-        ```
-        
-        When `all_pages` is false, this plugin only works for the page that added `git-snippet: enable`.
-        
-        ```markdown
-        <!-- git-snippet: enable -->
-        
-        # Your document
-        ....
-        ```
-        
-        ## Usage
-        
-        ### All files from default branch
-        
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') }}
-        ```
-        
-        It works for non markdown file too. The snippet format is raw text.
-        Please format it if needed.
-        
-        ````
-        ```python
-        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py') }}
-        ```
-        ````
-        
-        ### All files from specific branch/tag/commit
-        
-        ````
-        ```python
-        { gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '1.1')
-        ```
-        ````
-        
-        ````
-        ```python
-        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '520314fed933aed8de62b08dd7fc6e25c0ff482b') }}
-        ```
-        ````
-        
-        ### Snippet a section
-        
-        For markdown file, it is possible to specify a section.
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', section='## Using Plugins') }}
-        ```
-        or
-        ```
-        {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', 'master', '## Using Plugins') }}
-        ```
-        
-        ### Insert indent
-        
-        You can insert indent to snippet using `indent`.
-        `indent` has an argument `width`, which means the number of space to indent by. The default is 4.
-        See more details of `indent` [here](https://jinja.palletsprojects.com/en/master/templates/#indent).
-        
-        ````
-        ??? example "Plugin.md"
-        
-            {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') | indent }}
-        
-            !!! note
-        
-                ```python
-                {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py) | indent(width=8) }}
-                ```
-        ````
-        
-        ## Contribution
-        
-        Please read the CLA carefully before submitting your contribution to Mercari.
-        Under any circumstances, by submitting your contribution, you are deemed to accept and agree to be bound by the terms and conditions of the CLA.
-        
-        https://www.mercari.com/cla/
-        
-        ## License
-        
-        Copyright 2021 Mercari, Inc.
-        
-        Licensed under the MIT License.
-        
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# mkdocs-git-snippet [![Test][test-badge]][test] [![Code style: black][black-badge]][black]
+
+<!-- badge links -->
+[test-badge]: https://github.com/mercari/mkdocs-git-snippet/workflows/Test/badge.svg
+[test]: https://github.com/mercari/mkdocs-git-snippet/actions?query=workflow%3ATest
+[black-badge]: https://img.shields.io/badge/code%20style-black-000000.svg
+[black]: https://github.com/psf/black
+
+Mkdocs Plugin for snippet from git repository.
+
+## Installation
+
+```shell
+pip install mkdocs-git-snippet
+```
+
+## Configuration
+
+Enable the plugin in your mkdocs.yml.
+
+```markdown
+plugins:
+  - git-snippet
+```
+
+If the folder name that contain your documentation source files is not default `docs`, you need specify it with `base_path` option.
+
+```markdown
+plugins:
+  - git-snippet:
+        base_path: docs
+```
+
+By default, this plugin works for all pages. You can enable only for the specific page by setting `all_pages` option to false.
+
+```markdown
+plugins:
+  - git-snippet:
+      all_pages: false
+```
+
+When `all_pages` is false, this plugin only works for the page that added `git-snippet: enable`.
+
+```markdown
+<!-- git-snippet: enable -->
+
+# Your document
+....
+```
+
+### Acessing Private Repositories
+
+To add a snippet from a private repository set the `GITHUB_TOKEN` environment variable while building mkdocs documentation.
+
+## Usage
+
+### All files from default branch
+
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') }}
+```
+
+It works for non markdown file too. The snippet format is raw text.
+Please format it if needed.
+
+````
+```python
+{{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py') }}
+```
+````
+
+### All files from specific branch/tag/commit
+
+````
+```python
+{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '1.1')
+```
+````
+
+````
+```python
+{{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py', '520314fed933aed8de62b08dd7fc6e25c0ff482b') }}
+```
+````
+
+### Snippet a section
+
+For markdown file, it is possible to specify a section.
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', section='## Using Plugins') }}
+```
+or
+```
+{{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md', 'master', '## Using Plugins') }}
+```
+
+### Insert indent
+
+You can insert indent to snippet using `indent`.
+`indent` has an argument `width`, which means the number of space to indent by. The default is 4.
+See more details of `indent` [here](https://jinja.palletsprojects.com/en/master/templates/#indent).
+
+````
+??? example "Plugin.md"
+
+    {{ gitsnippet('mkdocs/mkdocs', 'docs/user-guide/plugins.md') | indent }}
+
+    !!! note
+
+        ```python
+        {{ gitsnippet('mkdocs/mkdocs', 'mkdocs/config/base.py) | indent(width=8) }}
+        ```
+````
+
+## Contribution
+
+Please read the CLA carefully before submitting your contribution to Mercari.
+Under any circumstances, by submitting your contribution, you are deemed to accept and agree to be bound by the terms and conditions of the CLA.
+
+https://www.mercari.com/cla/
+
+## License
+
+Copyright 2021 Mercari, Inc.
+
+Licensed under the MIT License.
+
+
```

### Comparing `mkdocs-git-snippet-0.1.1/setup.py` & `mkdocs-git-snippet-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 import os
 from distutils.command.upload import upload as upload_orig
 from setuptools import find_packages, setup
 from typing import List
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 
 
 def generate_install_requires() -> List[str]:
     # Path agnostic way to open requirements
     abspath = os.path.abspath(__file__)
     project_root = os.path.dirname(abspath)
     req_path = os.path.join(project_root, "requirements.txt")
```

