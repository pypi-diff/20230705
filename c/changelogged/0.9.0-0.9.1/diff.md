# Comparing `tmp/changelogged-0.9.0.tar.gz` & `tmp/changelogged-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelogged-0.9.0.tar", max compression
+gzip compressed data, was "changelogged-0.9.1.tar", max compression
```

## Comparing `changelogged-0.9.0.tar` & `changelogged-0.9.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/__init__.py
--rw-r--r--   0        0        0       64 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/__main__.py
--rw-r--r--   0        0        0     1797 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/__init__.py
--rw-r--r--   0        0        0     2255 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/add.py
--rw-r--r--   0        0        0     2834 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/check.py
--rw-r--r--   0        0        0     7591 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/init.py
--rw-r--r--   0        0        0     2015 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/notes.py
--rw-r--r--   0        0        0     1665 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/upgrade.py
--rw-r--r--   0        0        0      957 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/commands/versions.py
--rw-r--r--   0        0        0     1127 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/app/prompts.py
--rw-r--r--   0        0        0      207 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/assets/.cl.links.jinja2
--rw-r--r--   0        0        0      274 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/assets/.cl.overview.jinja2
--rw-r--r--   0        0        0      865 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/assets/changelog.jinja2
--rw-r--r--   0        0        0     4944 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/changelog.py
--rw-r--r--   0        0        0        0 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/conf/__init__.py
--rw-r--r--   0        0        0      510 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/conf/defaults.py
--rw-r--r--   0        0        0      994 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/conf/git.py
--rw-r--r--   0        0        0     2859 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/conf/models.py
--rw-r--r--   0        0        0      963 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/conf/settings.py
--rw-r--r--   0        0        0      196 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/models/__init__.py
--rw-r--r--   0        0        0     1731 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/models/domain_models.py
--rw-r--r--   0        0        0     1524 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/templating.py
--rw-r--r--   0        0        0      178 2023-03-04 22:05:31.000597 changelogged-0.9.0/changelogger/utils.py
--rw-r--r--   0        0        0    10388 2023-03-04 22:05:31.004597 changelogged-0.9.0/docs/README.md
--rw-r--r--   0        0        0     1292 2023-03-04 22:05:31.004597 changelogged-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11503 1970-01-01 00:00:00.000000 changelogged-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/__init__.py
+-rw-r--r--   0        0        0       64 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/__main__.py
+-rw-r--r--   0        0        0     1797 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/__init__.py
+-rw-r--r--   0        0        0     2255 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/add.py
+-rw-r--r--   0        0        0     4367 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/check.py
+-rw-r--r--   0        0        0     7591 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/init.py
+-rw-r--r--   0        0        0     2015 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/notes.py
+-rw-r--r--   0        0        0     1665 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/upgrade.py
+-rw-r--r--   0        0        0      957 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/commands/versions.py
+-rw-r--r--   0        0        0     1127 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/app/prompts.py
+-rw-r--r--   0        0        0      207 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/assets/.cl.links.jinja2
+-rw-r--r--   0        0        0      274 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/assets/.cl.overview.jinja2
+-rw-r--r--   0        0        0      865 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/assets/changelog.jinja2
+-rw-r--r--   0        0        0     4892 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/changelog.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/conf/__init__.py
+-rw-r--r--   0        0        0      510 2023-03-05 05:55:11.805114 changelogged-0.9.1/changelogger/conf/defaults.py
+-rw-r--r--   0        0        0      994 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/conf/git.py
+-rw-r--r--   0        0        0     2859 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/conf/models.py
+-rw-r--r--   0        0        0      963 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/conf/settings.py
+-rw-r--r--   0        0        0      196 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/models/__init__.py
+-rw-r--r--   0        0        0     1731 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/models/domain_models.py
+-rw-r--r--   0        0        0     1592 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/templating.py
+-rw-r--r--   0        0        0      178 2023-03-05 05:55:11.809114 changelogged-0.9.1/changelogger/utils.py
+-rw-r--r--   0        0        0    10735 2023-03-05 05:55:11.809114 changelogged-0.9.1/docs/README.md
+-rw-r--r--   0        0        0     1292 2023-03-05 05:55:11.809114 changelogged-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11850 1970-01-01 00:00:00.000000 changelogged-0.9.1/PKG-INFO
```

### Comparing `changelogged-0.9.0/changelogger/app/__init__.py` & `changelogged-0.9.1/changelogger/app/__init__.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/commands/add.py` & `changelogged-0.9.1/changelogger/app/commands/add.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/commands/init.py` & `changelogged-0.9.1/changelogger/app/commands/init.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/commands/notes.py` & `changelogged-0.9.1/changelogger/app/commands/notes.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/commands/upgrade.py` & `changelogged-0.9.1/changelogger/app/commands/upgrade.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/commands/versions.py` & `changelogged-0.9.1/changelogger/app/commands/versions.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/app/prompts.py` & `changelogged-0.9.1/changelogger/app/prompts.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/assets/changelog.jinja2` & `changelogged-0.9.1/changelogger/assets/changelog.jinja2`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/changelog.py` & `changelogged-0.9.1/changelogger/changelog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from pathlib import Path
 from typing import Literal
 
+from changelogger import templating
 from changelogger.conf import settings
 from changelogger.conf.models import VersionedFile
 from changelogger.exceptions import (
     CommandException,
     RollbackException,
     UpgradeException,
 )
 from changelogger.models.domain_models import (
     ChangelogUpdate,
     ReleaseNotes,
     VersionInfo,
 )
-from changelogger.templating import update_with_jinja
 from changelogger.utils import cached_compile
 
 CHANGELOG_PARTITION_RELEASE_NOTES = "RELEASE NOTES"
 CHANGELOG_PARTITION_LINKS = "LINKS"
 
 
 def _get_changelog_parition(partition: str) -> str:
@@ -162,18 +162,17 @@
 def update_versioned_files(
     update: ChangelogUpdate,
     versioned_files: list[VersionedFile],
 ) -> None:
     rollback: list[tuple[Path, str]] = []
     try:
         for file in versioned_files:
-            update_fn = update_with_jinja(file)
             content = file.rel_path.read_text()
             rollback.append((file.rel_path, content))
-            new_content = update_fn(content, update)
+            new_content = templating.update(file, update, content)
             file.rel_path.write_text(new_content)
     except Exception as upgrade_exc:
         try:
             # Need to reverse rollback list for proper rollback
             _rollback(rollback[::-1])
         except Exception as rollback_exc:
             raise RollbackException(
```

### Comparing `changelogged-0.9.0/changelogger/conf/git.py` & `changelogged-0.9.1/changelogger/conf/git.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/conf/models.py` & `changelogged-0.9.1/changelogger/conf/models.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/conf/settings.py` & `changelogged-0.9.1/changelogger/conf/settings.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/models/domain_models.py` & `changelogged-0.9.1/changelogger/models/domain_models.py`

 * *Files identical despite different names*

### Comparing `changelogged-0.9.0/changelogger/templating.py` & `changelogged-0.9.1/changelogger/templating.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,57 @@
-from collections.abc import Callable
 from datetime import date
 from typing import Any
 
 from jinja2 import BaseLoader, Environment, Template
 
 from changelogger.conf.models import VersionedFile
 from changelogger.models.domain_models import ChangelogUpdate
 from changelogger.utils import cached_compile
 
 
+def update(
+    file: VersionedFile,
+    update: ChangelogUpdate,
+    content: str,
+) -> str:
+    """Replaces the versioned files rendered pattern in the supplied content."""
+
+    replacement_str = file.jinja
+    if not replacement_str:
+        assert file.jinja_rel_path, "No valid jinja template found."
+        replacement_str = file.jinja_rel_path.read_text()
+
+    variables = _get_variables(file, update)
+    pattern = render_jinja(file.pattern, variables)
+    replacement = render_jinja(replacement_str, variables)
+
+    return cached_compile(pattern).sub(replacement, content)
+
+
+def render_pattern(
+    file: VersionedFile,
+    update: ChangelogUpdate,
+) -> str:
+    variables = _get_variables(file, update)
+    return render_jinja(file.pattern, variables)
+
+
+def render_jinja(tmpl: str, variables: dict[str, Any]) -> str:
+    return _tmpl(tmpl).render(**variables)
+
+
 def _tmpl(jinja: str) -> Template:
     template_env = Environment(loader=BaseLoader())
     return template_env.from_string(jinja)
 
 
-def _render_variables(
+def _get_variables(
     versioned_file: VersionedFile,
     update: ChangelogUpdate,
 ) -> dict[str, Any]:
     return dict(
         new_version=update.new_version,
         old_version=update.old_version,
         today=date.today(),
         sections=update.release_notes.dict(),
         context=versioned_file.context,
     )
-
-
-def render_jinja(tmpl: str, variables: dict[str, Any]) -> str:
-    return _tmpl(tmpl).render(**variables)
-
-
-def update_with_jinja(
-    file: VersionedFile,
-) -> Callable:
-    assert file.jinja or file.jinja_rel_path, "No valid jinja template found."
-
-    replacement_str = file.jinja
-    if not replacement_str and file.jinja_rel_path:
-        replacement_str = file.jinja_rel_path.read_text()
-
-    def update_fn(content: str, update: ChangelogUpdate) -> str:
-        assert replacement_str
-        render_kwargs = _render_variables(file, update)
-
-        pattern = render_jinja(file.pattern, render_kwargs)
-        replacement = render_jinja(replacement_str, render_kwargs)
-
-        return cached_compile(pattern).sub(replacement, content)
-
-    return update_fn
```

### Comparing `changelogged-0.9.0/docs/README.md` & `changelogged-0.9.1/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Changelogger
 
 [![Continuous Deployment](https://github.com/award28/changelogger/actions/workflows/continuous_deployment.yml/badge.svg)](https://github.com/award28/changelogger/actions/workflows/continuous_deployment.yml)
+[![Continuous Integration](https://github.com/award28/changelogger/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/award28/changelogger/actions/workflows/continuous_integration.yml)
 [![codecov](https://codecov.io/gh/award28/changelogger/branch/main/graph/badge.svg?token=M0I9MA4ZNW)](https://codecov.io/gh/award28/changelogger)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
 
 Automated management of your CHANGELOG.md and other versioned files, following
 the principles of [Keep a Changelog](https://keepachangelog.com) and
 [Semantic Versioning](https://semver.org).
 
 
 This project uses [Jinja](https://jinja.palletsprojects.com/) for simple yet
```

### Comparing `changelogged-0.9.0/pyproject.toml` & `changelogged-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changelogged"
-version = "0.9.0"
+version = "0.9.1"
 description = "Automated management of your changelog and other versioned files, following the principles of Keep a Changelog and Semantic Versioning."
 license = "MIT"
 authors = ["award28 <austin.ward@klaviyo.com>"]
 maintainers = ["award28 <austin.ward@klaviyo.com>"]
 readme = "docs/README.md"
 repository = "https://github.com/award28/changelogger"
 packages = [
```

### Comparing `changelogged-0.9.0/PKG-INFO` & `changelogged-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: changelogged
-Version: 0.9.0
+Version: 0.9.1
 Summary: Automated management of your changelog and other versioned files, following the principles of Keep a Changelog and Semantic Versioning.
 Home-page: https://github.com/award28/changelogger
 License: MIT
 Keywords: changelog,version,semver,changelogger,changelogged
 Author: award28
 Author-email: austin.ward@klaviyo.com
 Maintainer: award28
@@ -26,15 +26,18 @@
 Requires-Dist: typer (==0.7.0)
 Project-URL: Repository, https://github.com/award28/changelogger
 Description-Content-Type: text/markdown
 
 # Changelogger
 
 [![Continuous Deployment](https://github.com/award28/changelogger/actions/workflows/continuous_deployment.yml/badge.svg)](https://github.com/award28/changelogger/actions/workflows/continuous_deployment.yml)
+[![Continuous Integration](https://github.com/award28/changelogger/actions/workflows/continuous_integration.yml/badge.svg)](https://github.com/award28/changelogger/actions/workflows/continuous_integration.yml)
 [![codecov](https://codecov.io/gh/award28/changelogger/branch/main/graph/badge.svg?token=M0I9MA4ZNW)](https://codecov.io/gh/award28/changelogger)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
 
 Automated management of your CHANGELOG.md and other versioned files, following
 the principles of [Keep a Changelog](https://keepachangelog.com) and
 [Semantic Versioning](https://semver.org).
 
 
 This project uses [Jinja](https://jinja.palletsprojects.com/) for simple yet
```

