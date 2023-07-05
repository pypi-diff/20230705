# Comparing `tmp/zkg-2.8.0-py2.py3-none-any.whl.zip` & `tmp/zkg-2.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,15 @@
-Zip file size: 49732 bytes, number of entries: 11
--rw-r--r--  2.0 unx      587 b- defN 21-Mar-31 18:04 zeekpkg/__init__.py
--rw-r--r--  2.0 unx     6237 b- defN 21-Mar-09 20:46 zeekpkg/_util.py
--rw-r--r--  2.0 unx   113291 b- defN 21-Mar-31 17:52 zeekpkg/manager.py
--rw-r--r--  2.0 unx    15290 b- defN 21-Mar-09 20:46 zeekpkg/package.py
--rw-r--r--  2.0 unx     5039 b- defN 20-Dec-14 04:15 zeekpkg/source.py
--rwxr-xr-x  2.0 unx    91150 b- defN 21-Mar-31 18:05 zkg-2.8.0.data/scripts/zkg
--rw-r--r--  2.0 unx     1870 b- defN 21-Mar-31 18:05 zkg-2.8.0.dist-info/COPYING
--rw-r--r--  2.0 unx     1973 b- defN 21-Mar-31 18:05 zkg-2.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Mar-31 18:05 zkg-2.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 21-Mar-31 18:05 zkg-2.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 21-Mar-31 18:05 zkg-2.8.0.dist-info/RECORD
-11 files, 236380 bytes uncompressed, 48368 bytes compressed:  79.5%
+Zip file size: 61528 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      635 b- defN 21-May-18 22:07 zeekpkg/__init__.py
+-rw-r--r--  2.0 unx     8179 b- defN 21-May-18 18:47 zeekpkg/_util.py
+-rw-r--r--  2.0 unx   112541 b- defN 21-May-18 18:47 zeekpkg/manager.py
+-rw-r--r--  2.0 unx    14958 b- defN 21-May-18 18:47 zeekpkg/package.py
+-rw-r--r--  2.0 unx     5039 b- defN 21-May-18 18:47 zeekpkg/source.py
+-rw-r--r--  2.0 unx    26193 b- defN 21-May-18 21:56 zeekpkg/template.py
+-rw-r--r--  2.0 unx     5479 b- defN 21-May-18 20:32 zeekpkg/uservar.py
+-rwxr-xr-x  2.0 unx    99343 b- defN 21-May-18 22:10 zkg-2.9.0.data/scripts/zkg
+-rw-r--r--  2.0 unx     1870 b- defN 21-May-18 22:10 zkg-2.9.0.dist-info/COPYING
+-rw-r--r--  2.0 unx     1973 b- defN 21-May-18 22:10 zkg-2.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 21-May-18 22:10 zkg-2.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 21-May-18 22:10 zkg-2.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      977 b- defN 21-May-18 22:10 zkg-2.9.0.dist-info/RECORD
+13 files, 277305 bytes uncompressed, 59938 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -9,26 +9,32 @@
 
 Filename: zeekpkg/package.py
 Comment: 
 
 Filename: zeekpkg/source.py
 Comment: 
 
-Filename: zkg-2.8.0.data/scripts/zkg
+Filename: zeekpkg/template.py
 Comment: 
 
-Filename: zkg-2.8.0.dist-info/COPYING
+Filename: zeekpkg/uservar.py
 Comment: 
 
-Filename: zkg-2.8.0.dist-info/METADATA
+Filename: zkg-2.9.0.data/scripts/zkg
 Comment: 
 
-Filename: zkg-2.8.0.dist-info/WHEEL
+Filename: zkg-2.9.0.dist-info/COPYING
 Comment: 
 
-Filename: zkg-2.8.0.dist-info/top_level.txt
+Filename: zkg-2.9.0.dist-info/METADATA
 Comment: 
 
-Filename: zkg-2.8.0.dist-info/RECORD
+Filename: zkg-2.9.0.dist-info/WHEEL
+Comment: 
+
+Filename: zkg-2.9.0.dist-info/top_level.txt
+Comment: 
+
+Filename: zkg-2.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zeekpkg/__init__.py

```diff
@@ -1,20 +1,21 @@
 """
 This package defines a Python interface for installing, managing, querying,
 and performing other operations on Zeek Packages and Package Sources.
 The main entry point is the :class:`Manager <zeekpkg.manager.Manager>` class.
 
-This package provides a logger named `LOG` to which logging stream handlers may
-be added in order to help log/debug applications.
+This package provides a logger named ``LOG`` to which logging stream handlers
+may be added in order to help log/debug applications.
 """
 
 import logging
 
-__version__ = "2.8.0"
-__all__ = ['manager', 'package', 'source']
+__version__ = "2.9.0"
+__all__ = ['manager', 'package', 'source', 'template', 'uservar']
 
 LOG = logging.getLogger(__name__)
 LOG.addHandler(logging.NullHandler())
 
 from .manager import *
 from .package import *
 from .source import *
+from .uservar import *
```

## zeekpkg/_util.py

```diff
@@ -1,16 +1,19 @@
 """
 These are meant to be private utility methods for internal use.
 """
 
-import os
 import errno
+import importlib.machinery
+import os
 import shutil
-import git
+import types
 
+import git
+import semantic_version as semver
 
 def make_dir(path):
     """Create a directory or do nothing if it already exists.
 
     Raises:
         OSError: if directory cannot be created
     """
@@ -19,14 +22,24 @@
     except OSError as exception:
         if exception.errno != errno.EEXIST:
             raise
         elif os.path.isfile(path):
             raise
 
 
+def normalize_version_tag(tag):
+    """Given version string "vX.Y.Z", returns "X.Y.Z".
+    Returns other input strings unchanged.
+    """
+    if len(tag) > 1 and tag[0] == 'v' and tag[1].isdigit():
+        return tag[1:]
+
+    return tag
+
+
 def delete_path(path):
     if os.path.islink(path):
         os.remove(path)
         return
 
     if not os.path.exists(path):
         return
@@ -170,14 +183,47 @@
         # See if there's a branch currently checked out
         return repo.head.ref.name
     except TypeError:
         # No branch checked out, return commit hash
         return repo.head.object.hexsha
 
 
+def git_version_tags(repo):
+    """Returns semver-sorted list of version tag strings in the given repo."""
+    tags = []
+
+    for tagref in repo.tags:
+        tag = str(tagref.name)
+        normal_tag = normalize_version_tag(tag)
+
+        try:
+            sv = semver.Version.coerce(normal_tag)
+        except ValueError:
+            # Skip tags that aren't compatible semantic versions.
+            continue
+        else:
+            tags.append((normal_tag, tag, sv))
+
+    return [t[1] for t in sorted(tags, key=lambda e: e[2])]
+
+
+def git_pull(repo):
+    """Does a git pull followed up a submodule update.
+
+    Args:
+        clone (git.Repo): the git clone on which to operate
+
+    Raises:
+        git.exc.GitCommandError: in case of git trouble
+    """
+    repo.git.pull()
+    repo.git.submodule('sync', '--recursive')
+    repo.git.submodule('update', '--recursive', '--init')
+
+
 def is_sha1(s):
     if not s:
         return False;
 
     if len(s) != 40:
         return False
 
@@ -233,7 +279,29 @@
 
     import subprocess
     cmd = subprocess.Popen([zeek_config, '--version'],
                            stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
                            bufsize=1, universal_newlines=True)
 
     return read_zeek_config_line(cmd.stdout)
+
+def load_source(filename):
+    """Loads given Python script from disk.
+
+    Args:
+        filename (str): name of a Python script file
+
+    Returns:
+        types.ModuleType: a module representing the loaded file
+    """
+    # https://stackoverflow.com/questions/67631/how-to-import-a-module-given-the-full-path
+    # We currrently require Python 3.5+, where the following looks sufficient:
+    absname = os.path.abspath(filename)
+    dirname = os.path.dirname(absname)
+
+    # Naming here is unimportant, since we access members of the new
+    # module via the returned instance.
+    loader = importlib.machinery.SourceFileLoader('template_' + dirname, absname)
+    mod = types.ModuleType(loader.name)
+    loader.exec_module(mod)
+
+    return mod
```

## zeekpkg/manager.py

```diff
@@ -1,21 +1,21 @@
 """
 A module defining the main Zeek Package Manager interface which supplies
 methods to interact with and operate on Zeek packages.
 """
 
-import os
-import sys
+import configparser
 import copy
+import filecmp
 import json
+import os
 import shutil
-import filecmp
-import tarfile
 import subprocess
-import configparser
+import sys
+import tarfile
 
 try:
     from urllib.parse import urlparse
 except ImportError:
     from urlparse import urlparse
 
 import git
@@ -27,19 +27,22 @@
     make_dir,
     delete_path,
     make_symlink,
     copy_over_path,
     git_default_branch,
     git_checkout,
     git_clone,
+    git_pull,
+    git_version_tags,
     is_sha1,
     get_zeek_version,
     std_encoding,
     find_program,
     read_zeek_config_line,
+    normalize_version_tag,
 )
 from .source import (
     AGGREGATE_DATA_FILE,
     Source
 )
 from .package import (
     METADATA_FILENAME,
@@ -47,22 +50,24 @@
     TRACKING_METHOD_VERSION,
     TRACKING_METHOD_BRANCH,
     TRACKING_METHOD_COMMIT,
     PLUGIN_MAGIC_FILE,
     PLUGIN_MAGIC_FILE_DISABLED,
     name_from_path,
     aliases,
-    user_vars,
     canonical_url,
     is_valid_name as is_valid_package_name,
     Package,
     PackageInfo,
     PackageStatus,
     InstalledPackage
 )
+from .uservar import (
+    UserVar,
+)
 from . import (
     __version__,
     LOG,
 )
 
 
 class Manager(object):
@@ -815,17 +820,15 @@
         source.clone.git.clean('-f', '-x', '-d')
 
         if os.path.isfile(aggregate_file):
             shutil.copy2(aggregate_file, agg_file_their_orig)
 
         try:
             source.clone.git.fetch('--recurse-submodules=yes')
-            source.clone.git.pull()
-            source.clone.git.submodule('sync', '--recursive')
-            source.clone.git.submodule('update', '--recursive', '--init')
+            git_pull(source.clone)
         except git.exc.GitCommandError as error:
             LOG.error('failed to pull source %s: %s', name, error)
             return self.SourceAggregationResults(
                     'failed to pull from remote source: {}'.format(error))
 
         if os.path.isfile(agg_file_ours):
             if os.path.isfile(aggregate_file):
@@ -871,15 +874,15 @@
                         clone = git_clone(url, clonepath, shallow=True)
                     except git.exc.GitCommandError as error:
                         LOG.warn('failed to clone %s, skipping aggregation: %s',
                                  url, error)
                         aggregation_issues.append((url, repr(error)))
                         continue
 
-                    version_tags = _get_version_tags(clone)
+                    version_tags = git_version_tags(clone)
 
                     if len(version_tags):
                         version = version_tags[-1]
                     else:
                         version = git_default_branch(clone)
 
                     try:
@@ -991,20 +994,18 @@
             LOG.info('upgrading "%s": package not outdated', pkg_path)
             return "package is not outdated"
 
         clonepath = os.path.join(self.package_clonedir, ipkg.package.name)
         clone = git.Repo(clonepath)
 
         if ipkg.status.tracking_method == TRACKING_METHOD_VERSION:
-            version_tags = _get_version_tags(clone)
+            version_tags = git_version_tags(clone)
             return self._install(ipkg.package, version_tags[-1])
         elif ipkg.status.tracking_method == TRACKING_METHOD_BRANCH:
-            clone.git.pull()
-            clone.git.submodule('sync', '--recursive')
-            clone.git.submodule('update', '--recursive', '--init')
+            git_pull(clone)
             return self._install(ipkg.package, ipkg.status.current_version)
         elif ipkg.status.tracking_method == TRACKING_METHOD_COMMIT:
             # The above check for whether the installed package is outdated
             # also should have already caught this situation.
             return "package is not outdated"
         else:
             raise NotImplementedError
@@ -1557,15 +1558,15 @@
             A :class:`.package.PackageInfo` object.
 
         Raises:
             git.exc.GitCommandError: when failing to clone the package repo
         """
         clonepath = os.path.join(self.scratch_dir, package.name)
         clone = _clone_package(package, clonepath, version)
-        versions = _get_version_tags(clone)
+        versions = git_version_tags(clone)
 
         if not version:
 
             if len(versions):
                 version = versions[-1]
             else:
                 version = git_default_branch(clone)
@@ -1590,15 +1591,15 @@
 
         Returns:
             list of str: the version number tags.
         """
         name = installed_package.package.name
         clonepath = os.path.join(self.package_clonedir, name)
         clone = git.Repo(clonepath)
-        return _get_version_tags(clone)
+        return git_version_tags(clone)
 
     def validate_dependencies(self, requested_packages,
                               ignore_installed_packages=False,
                               ignore_suggestions=False):
         """Validates package dependencies.
 
         Args:
@@ -1843,15 +1844,15 @@
 
                         return (str.format(
                             'unsatisfiable dependency: requested "{}" ({}),'
                             ' but "{}" requires {}', node.name,
                             required_version, depender_name, version_spec),
                             new_pkgs)
                 else:
-                    normal_version = _normalize_version_tag(required_version)
+                    normal_version = normalize_version_tag(required_version)
                     req_semver = semver.Version.coerce(normal_version)
 
                     for depender_name, version_spec in node.dependers.items():
                         if version_spec.startswith('branch='):
                             version_spec = version_spec[len('branch='):]
                             return (str.format(
                                 'unsatisfiable dependency: requested "{}" ({}),'
@@ -1902,15 +1903,15 @@
 
                         return (str.format(
                             'unsatisfiable dependency: "{}" ({}) is installed,'
                             ' but "{}" requires {}', node.name,
                             required_version, depender_name, version_spec),
                             new_pkgs)
                     else:
-                        normal_version = _normalize_version_tag(required_version)
+                        normal_version = normalize_version_tag(required_version)
                         req_semver = semver.Version.coerce(normal_version)
 
                         if version_spec.startswith('branch='):
                             version_spec = version_spec[len('branch='):]
                             return (str.format(
                                 'unsatisfiable dependency: "{}" ({}) is installed,'
                                 ' but "{}" requires {}', node.name,
@@ -1972,15 +1973,15 @@
 
                     if branch_name:
                         best_version = branch_name
                     else:
                         best_version = node.info.default_branch
                 elif need_version:
                     for version in node.info.versions[::-1]:
-                        normal_version = _normalize_version_tag(version)
+                        normal_version = normalize_version_tag(version)
                         req_semver = semver.Version.coerce(normal_version)
 
                         satisfied = True
 
                         for depender_name, version_spec in node.dependers.items():
                             try:
                                 semver_spec = semver.Spec(version_spec)
@@ -2285,34 +2286,36 @@
         invalid_reason = _parse_package_metadata(
             raw_metadata_parser, metadata_file)
 
         if invalid_reason:
             return invalid_reason
 
         raw_metadata = _get_package_metadata(raw_metadata_parser)
-        requested_user_vars = user_vars(raw_metadata)
+
+
+        requested_user_vars = UserVar.parse_dict(raw_metadata)
 
         if requested_user_vars is None:
             return "package has malformed 'user_vars' metadata field"
 
         substitutions = {
             'bro_dist': self.zeek_dist,
             'zeek_dist': self.zeek_dist,
             'package_base': self.package_clonedir,
         }
         substitutions.update(self.user_vars)
 
-        for k, v, _ in requested_user_vars:
-            val_from_env = os.environ.get(k)
+        for uvar in requested_user_vars:
+            val_from_env = os.environ.get(uvar.name())
 
             if val_from_env:
-                substitutions[k] = val_from_env
+                substitutions[uvar.name()] = val_from_env
 
-            if k not in substitutions:
-                substitutions[k] = v
+            if uvar.name() not in substitutions:
+                substitutions[uvar.name()] = uvar.val()
 
         metadata_parser = configparser.ConfigParser(defaults=substitutions)
         invalid_reason = _parse_package_metadata(
             metadata_parser, metadata_file)
 
         if invalid_reason:
             return invalid_reason
@@ -2533,15 +2536,15 @@
         else:
             clone = _clone_package(package, clonepath, version)
 
         status = PackageStatus()
         status.is_loaded = ipkg.status.is_loaded if ipkg else False
         status.is_pinned = ipkg.status.is_pinned if ipkg else False
 
-        version_tags = _get_version_tags(clone)
+        version_tags = git_version_tags(clone)
 
         if version:
             if _is_commit_hash(clone, version):
                 status.tracking_method = TRACKING_METHOD_COMMIT
             elif version in version_tags:
                 status.tracking_method = TRACKING_METHOD_VERSION
             else:
@@ -2627,38 +2630,14 @@
                 if os.path.islink(old):
                     try:
                         os.unlink(old)
                         LOG.debug('removed link %s', old)
                     except:
                         LOG.warn('failed to remove link %s', old)
 
-def _normalize_version_tag(tag):
-    # Change vX.Y.Z into X.Y.Z
-    if len(tag) > 1 and tag[0] == 'v' and tag[1].isdigit():
-        return tag[1:]
-
-    return tag
-
-def _get_version_tags(clone):
-    tags = []
-
-    for tagref in clone.tags:
-        tag = str(tagref.name)
-        normal_tag = _normalize_version_tag(tag)
-
-        try:
-            sv = semver.Version.coerce(normal_tag)
-        except ValueError:
-            # Skip tags that aren't compatible semantic versions.
-            continue
-        else:
-            tags.append((normal_tag, tag, sv))
-
-    return [t[1] for t in sorted(tags, key=lambda e: e[2])]
-
 
 def _get_branch_names(clone):
     rval = []
 
     for ref in clone.references:
         branch_name = str(ref.name)
 
@@ -2667,17 +2646,17 @@
 
         rval.append(branch_name.split('origin/')[1])
 
     return rval
 
 
 def _is_version_outdated(clone, version):
-    version_tags = _get_version_tags(clone)
-    latest = _normalize_version_tag(version_tags[-1])
-    return _normalize_version_tag(version) != latest
+    version_tags = git_version_tags(clone)
+    latest = normalize_version_tag(version_tags[-1])
+    return normalize_version_tag(version) != latest
 
 
 def _is_branch_outdated(clone, branch):
     it = clone.iter_commits('{0}..origin/{0}'.format(branch))
     num_commits_behind = sum(1 for c in it)
     return num_commits_behind > 0
 
@@ -2813,15 +2792,15 @@
 
 def _info_from_clone(clone, package, status, version):
     """Retrieves information about a package.
 
     Returns:
         A :class:`.package.PackageInfo` object.
     """
-    versions = _get_version_tags(clone)
+    versions = git_version_tags(clone)
     default_branch = git_default_branch(clone)
 
     if _is_commit_hash(clone, version):
         version_type = TRACKING_METHOD_COMMIT
     elif version in versions:
         version_type = TRACKING_METHOD_VERSION
     else:
```

## zeekpkg/package.py

```diff
@@ -2,14 +2,15 @@
 A module with various data structures used for interacting with and querying
 the properties and status of Zeek packages.
 """
 
 import os
 import re
 
+from .uservar import UserVar
 from ._util import find_sentence_end
 
 #: The name of files used by packages to store their metadata.
 METADATA_FILENAME = 'zkg.meta'
 LEGACY_METADATA_FILENAME = 'bro-pkg.meta'
 
 TRACKING_METHOD_VERSION = 'version'
@@ -84,45 +85,26 @@
 
     return rval.lstrip()
 
 
 def user_vars(metadata_dict):
     """Returns a list of (str, str, str) from metadata's 'user_vars' field.
 
-    Each entry in the returned list is a the name of a variable, it's value,
+    Each entry in the returned list is a the name of a variable, its value,
     and its description.
 
     If the 'user_vars' field is not present, an empty list is returned.  If it
     is malformed, then None is returned.
     """
-    text = metadata_dict.get('user_vars')
+    uvars = UserVar.parse_dict(metadata_dict)
 
-    if not text:
-        return []
-
-    rval = []
-
-    text = text.strip()
-    entries = re.split('(\w+\s+\\[.*\\]\s+".*")\s+', text)
-    entries = list(filter(None, entries))
-
-    for entry in entries:
-        m = re.match('(\w+)\s+\\[(.*)\\]\s+"(.*)"', entry)
-
-        if not m:
-            return None
-
-        groups = m.groups()
-
-        if len(groups) != 3:
-            return None
-
-        rval.append((groups[0], groups[1], groups[2]))
+    if uvars is None:
+        return None
 
-    return rval
+    return [(uvar.name(), uvar.val(), uvar.desc()) for uvar in uvars]
 
 
 def dependencies(metadata_dict, field='depends'):
     """Returns a dictionary of (str, str) based on metadata's dependency field.
 
     The keys indicate the name of a package (shorthand name or full git URL).
     The names 'zeek' or 'zkg' may also be keys that indicate a dependency on a
@@ -279,23 +261,23 @@
 
         If the dependency field is malformed (e.g. number of keys not equal to
         number of values), then None is returned.
         """
         return dependencies(self.metadata, field)
 
     def user_vars(self):
-        """Returns a list of (str, str, str) from metadata's 'user_vars' field.
-
-        Each entry in the returned list is a the name of a variable, it's value,
-        and its description.
+        """Returns a list of user variables parsed from metadata's 'user_vars' field.
 
         If the 'user_vars' field is not present, an empty list is returned.  If
         it is malformed, then None is returned.
+
+        Returns:
+            list of zeekpkg.uservar.UserVar, or None on error
         """
-        return user_vars(self.metadata)
+        return UserVar.parse_dict(self.metadata)
 
     def best_version(self):
         """Returns the best/latest version of the package that is available.
 
         If the package has any git release tags, this returns the highest one,
         else it returns the default branch like 'main' or 'master'.
         """
```

## zeekpkg/source.py

 * *Ordering differences only*

```diff
@@ -2,18 +2,18 @@
 A module containing the definition of a "package source": a git repository
 containing a collection of :file:`zkg.index` (or legacy :file:`bro-pkg.index`)
 files.  These are simple INI files that can describe many Zeek packages.  Each
 section of the file names a Zeek package along with the git URL where it is
 located and metadata tags that help classify/describe it.
 """
 
+import configparser
+import git
 import os
 import shutil
-import git
-import configparser
 
 from . import LOG
 from .package import (
     name_from_path,
     Package
 )
 from ._util import (
```

## Comparing `zkg-2.8.0.data/scripts/zkg` & `zkg-2.9.0.data/scripts/zkg`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!python
 
-import os
-import io
-import errno
 import argparse
-import logging
-import threading
+import configparser
+import errno
 import filecmp
+import io
+import json
+import logging
+import os
 import shutil
 import subprocess
-import json
-import configparser
 import sys
+import threading
 
 from collections import OrderedDict
 
 try:
     import git
     import semantic_version as semver # lgtm[py/unused-import]
 except ImportError as error:
@@ -64,24 +64,35 @@
 ZEEK_ZKG_STATE_DIR = os.getenv('ZEEK_ZKG_STATE_DIR') or '@ZEEK_ZKG_STATE_DIR@'
 if not os.path.isdir(ZEEK_ZKG_STATE_DIR):
     ZEEK_ZKG_STATE_DIR = None
 
 # The default package source we fall back to as needed
 ZKG_DEFAULT_SOURCE = 'https://github.com/zeek/packages'
 
+# The default package template
+ZKG_DEFAULT_TEMPLATE = 'https://github.com/zeek/package-template'
+
 from zeekpkg._util import (
+    delete_path,
     make_dir,
     make_symlink,
     find_program,
     read_zeek_config_line,
     std_encoding,
 )
 from zeekpkg.package import (
     TRACKING_METHOD_VERSION,
 )
+from zeekpkg.template import (
+    LoadError,
+    Template,
+)
+from zeekpkg.uservar import (
+    UserVar,
+)
 
 import zeekpkg
 
 
 def confirmation_prompt(prompt, default_to_yes=True):
     yes = {'y', 'ye', 'yes'}
 
@@ -102,64 +113,34 @@
     if choice in yes:
         return True
 
     print('Abort.')
     return False
 
 
-def prompt_for_user_vars(manager, config, configfile, force, pkg_infos):
+def prompt_for_user_vars(manager, config, configfile, args, pkg_infos):
     answers = {}
 
     for info in pkg_infos:
         name = info.package.qualified_name()
         requested_user_vars = info.user_vars()
 
         if requested_user_vars is None:
             print_error(str.format('error: malformed user_vars in "{}"', name))
             sys.exit(1)
 
-        if not requested_user_vars:
-            continue
-
-        for key, value, desc in requested_user_vars:
-            from_env = False
-            default_value = os.environ.get(key)
-
-            if default_value:
-                from_env = True
-            else:
-                if config.has_section('user_vars'):
-                    v = config.get('user_vars', key, fallback=None)
-
-                    if v:
-                        default_value = v
-                    else:
-                        default_value = value
-                else:
-                    default_value = value
-
-            if force:
-                answers[key] = default_value
-            else:
-                if from_env:
-                    print(str.format(
-                        '{} will use value of {} ({}) from environment: {}',
-                        name, key, desc, default_value))
-                    answers[key] = default_value
-                else:
-                    prompt = '{} asks for {} ({}) ? [{}] '.format(
-                        name, key, desc, default_value)
-                    response = input(prompt)
-
-                    if response:
-                        answers[key] = response
-                    else:
-                        answers[key] = default_value
+        for uvar in requested_user_vars:
+            try:
+                answers[uvar.name()] = uvar.resolve(name, config, args.user_var, args.force)
+            except ValueError:
+                print_error(str.format('error: could not determine value of user variable "{}",'
+                                       ' provide via environment or --user-var', uvar.name()))
+                sys.exit(1)
 
-    if not force and answers:
+    if not args.force and answers:
         for key, value in answers.items():
             if not config.has_section('user_vars'):
                 config.add_section('user_vars')
 
             config.set('user_vars', key, value)
 
         if configfile:
@@ -249,19 +230,27 @@
 
     if not config.has_section('sources'):
         config.add_section('sources')
 
     if not config.has_section('paths'):
         config.add_section('paths')
 
+    if not config.has_section('templates'):
+        config.add_section('templates')
+
     if not configfile:
         default = os.getenv('ZKG_DEFAULT_SOURCE', ZKG_DEFAULT_SOURCE)
         if default:
             config.set('sources', 'zeek', default)
 
+    if not configfile or not config.has_option('templates', 'default'):
+        default = os.getenv('ZKG_DEFAULT_TEMPLATE', ZKG_DEFAULT_TEMPLATE)
+        if default:
+            config.set('templates', 'default', default)
+
     def config_option_set(config, section, option):
         return config.has_option(section, option) and config.get(section,
                                                                  option)
 
     def get_option(config, section, option, default):
         if config_option_set(config, section, option):
             return config.get(section, option)
@@ -295,14 +284,15 @@
     def expand_config_values(config, section):
         for key, value in config.items(section):
             value = os.path.expandvars(os.path.expanduser(value))
             config.set(section, key, value)
 
     expand_config_values(config, 'sources')
     expand_config_values(config, 'paths')
+    expand_config_values(config, 'templates')
 
     for key, value in config.items('paths'):
         if value and not os.path.isabs(value):
             print_error(str.format('error: invalid config file value for key'
                                    ' "{}" in section [paths]: "{}" is not'
                                    ' an absolute path', key, value))
             sys.exit(1)
@@ -604,15 +594,15 @@
             print(extdep_listing)
 
         if not confirmation_prompt('Proceed?'):
             return
 
     package_infos += new_pkgs
 
-    prompt_for_user_vars(manager, config, configfile, args.force,
+    prompt_for_user_vars(manager, config, configfile, args,
                          [info for info, _, _ in package_infos])
 
     if not args.skiptests:
         for info, version, _ in package_infos:
             name = info.package.qualified_name()
 
             if 'test_command' not in info.metadata:
@@ -928,15 +918,15 @@
                   '(Ensure their installation on all relevant systems before'
                   ' proceeding):')
             print(extdep_listing)
 
         if not confirmation_prompt('Proceed?'):
             return
 
-    prompt_for_user_vars(manager, config, configfile, args.force,
+    prompt_for_user_vars(manager, config, configfile, args,
                          [info for _, _, info in bundle_info])
 
     error = manager.unbundle(args.bundle_filename)
 
     if error:
         print_error('error: failed to unbundle {}: {}'.format(
             args.bundle_filename, error))
@@ -1302,15 +1292,15 @@
                   '(Ensure their installation on all relevant systems before'
                   ' proceeding):')
             print(extdep_listing)
 
         if not confirmation_prompt('Proceed?'):
             return
 
-    prompt_for_user_vars(manager, config, configfile, args.force,
+    prompt_for_user_vars(manager, config, configfile, args,
                          [info for info, _, _ in allpkgs])
 
     if not args.skiptests:
         to_test = [(info, next_version)
                    for info, next_version, _ in outdated_packages]
 
         for info, version, _ in new_pkgs:
@@ -2023,14 +2013,136 @@
         print(u'export BROPATH={}'.format(':'.join(zeekpaths)))
         print(u'export BRO_PLUGIN_PATH={}'.format(':'.join(pluginpaths)))
         print(u'export ZEEKPATH={}'.format(':'.join(zeekpaths)))
         print(u'export ZEEK_PLUGIN_PATH={}'.format(':'.join(pluginpaths)))
         print(u'export PATH={}:$PATH'.format(manager.bin_dir))
 
 
+def cmd_create(manager, args, config, configfile):
+
+    tmplname = (args.template
+                or config.get('templates', 'default', fallback=None)
+                or ZKG_DEFAULT_TEMPLATE)
+    try:
+        tmpl = Template.load(config, tmplname, args.version)
+    except LoadError as error:
+        msg = 'problem while loading template {}: {}'.format(tmplname, error)
+        zeekpkg.LOG.exception(msg)
+        print_error('error: ' + msg)
+        sys.exit(1)
+
+    try:
+        package = tmpl.package()
+        uvars = tmpl.define_user_vars()
+        uvar_names = set(package.needed_user_vars())
+
+        # Overlay any requested features onto the package.
+        if args.features:
+            # If the user provided comma-separated values, split the
+            # strings. (Argparse expects space separation.) Also
+            # filter any duplicates.
+            fnames = set()
+            for feat in args.features:
+                fnames |= set([f.strip() for f in feat.split(',') if f])
+            features = tmpl.features()
+            for feature in features:
+                if feature.name() in fnames:
+                    package.add_feature(feature)
+                    uvar_names |= set(feature.needed_user_vars())
+                    fnames.remove(feature.name())
+            if len(fnames) > 0:
+                # Alert if the user requested an unknown feature.
+                knowns = ', '.join([f'"{f.name()}"' for f in features])
+                unknowns = ', '.join([f'"{name}"' for name in fnames])
+                print_error('error: the following features are unknown: {}.'
+                            ' Template "{}" offers {}.'.format(
+                                unknowns, tmpl.name(), knowns or 'no features'))
+                sys.exit(1)
+
+        # Remove user vars we don't actually require from consideration
+        uvars = [uvar for uvar in uvars if uvar.name() in uvar_names]
+
+        # Resolve the variables via user input, args, etc
+        for uvar in uvars:
+            try:
+                uvar.resolve(tmpl.name(), config, args.user_var, args.force)
+            except ValueError:
+                print_error(str.format('error: could not determine value of user variable "{}",'
+                                       ' provide via environment or --user-var', uvar.name()))
+                sys.exit(1)
+
+        # Apply them to the template. After this, any parameter can be
+        # retrieved from the template via tmpl.lookup_param().
+        tmpl._set_user_vars(uvars)
+
+        # Verify that resulting template parameters are formatted correctly
+        try:
+            package.do_validate(tmpl)
+        except zeekpkg.template.InputError as error:
+            print_error('error: template input invalid, ' + str(error))
+            sys.exit(1)
+
+        # And finally, instantiate the package.
+        try:
+            if os.path.isdir(args.packagedir):
+                if not args.force:
+                    print('Package directory {} already exists.'
+                          .format(args.packagedir))
+                    if not confirmation_prompt('Delete?'):
+                        sys.exit(1)
+                try:
+                    delete_path(args.packagedir)
+                    zeekpkg.LOG.info('Removed existing package directory %s', args.packagedir)
+                except OSError as err:
+                    print_error('error: could not remove package directory {}: {}'
+                                .format(args.packagedir, err))
+                    sys.exit(1)
+
+            package.do_instantiate(tmpl, args.packagedir, args.force)
+        except zeekpkg.template.OutputError as error:
+            print_error('error: template instantiation failed, ' + str(error))
+            sys.exit(1)
+    except Exception as error:
+        msg = 'problem during template instantiation: {}'.format(error)
+        zeekpkg.LOG.exception(msg)
+        print_error('error: ' + msg)
+        sys.exit(1)
+
+
+def cmd_template_info(manager, args, config, configfile):
+    tmplname = (args.template
+                or config.get('templates', 'default', fallback=None)
+                or ZKG_DEFAULT_TEMPLATE)
+
+    try:
+        tmpl = Template.load(config, tmplname, args.version)
+    except LoadError as error:
+        msg = 'problem while loading template {}: {}'.format(tmplname, error)
+        zeekpkg.LOG.exception(msg)
+        print_error('error: ' + msg)
+        sys.exit(1)
+
+    tmplinfo = tmpl.info()
+
+    if args.json:
+        print(json.dumps(tmplinfo, indent=args.jsonpretty, sort_keys=True))
+    else:
+        print('API version: ' + tmplinfo['api_version'])
+        print('features: ' + ', '.join(tmplinfo['features']))
+        print('origin: ' + tmplinfo['origin'])
+        print('provides package: ' + str(tmplinfo['provides_package']).lower())
+        print('user vars:')
+        for uvar_name, uvar_info in tmplinfo['user_vars'].items():
+            print('\t{}: {}, {}, used by {}'.format(
+                uvar_name, uvar_info['description'],
+                uvar_info['default'] or 'no default',
+                ', '.join(uvar_info['used_by']) or 'not used'))
+        print('versions: ' + ', '.join(tmplinfo['versions']))
+
+
 class BundleHelpFormatter(argparse.ArgumentDefaultsHelpFormatter):
     # Workaround for underlying argparse bug: https://bugs.python.org/issue9338
     def _format_args(self, action, default_metavar):
         rval = super(BundleHelpFormatter, self)._format_args(
                 action, default_metavar)
 
         if action.nargs == argparse.ZERO_OR_MORE:
@@ -2045,16 +2157,18 @@
     top_parser = argparse.ArgumentParser(
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description='A command-line package manager for Zeek.',
         epilog='Environment Variables:\n\n'
         '    ``ZKG_CONFIG_FILE``:\t'
         'Same as ``--configfile`` option, but has less precedence.\n'
         '    ``ZKG_DEFAULT_SOURCE``:\t'
-        'The default package source to use (normally {}).'
-        .format(ZKG_DEFAULT_SOURCE)
+        'The default package source to use (normally {}).\n'
+        '    ``ZKG_DEFAULT_TEMPLATE``:\t'
+        'The default package template to use (normally {}).\n'
+        .format(ZKG_DEFAULT_SOURCE, ZKG_DEFAULT_TEMPLATE)
     )
     top_parser.add_argument('--version', action='version',
                             version='%(prog)s ' + zeekpkg.__version__)
 
     group = top_parser.add_mutually_exclusive_group()
     group.add_argument('--configfile', metavar='FILE',
                        help='Path to Zeek Package Manager config file. Precludes --user.')
@@ -2081,14 +2195,31 @@
                     ' the ambiguity. A full git URL may also be used to refer' \
                     ' to a package that does not belong to a source. E.g. for' \
                     ' a package source called "zeek" that has a package named' \
                     ' "foo" located in either "alice/zkg.index" or' \
                     ' "alice/bro-pkg.index", the following' \
                     ' names work: "foo", "alice/foo", "zeek/alice/foo".'
 
+    def add_uservar_args(parser, force_help=None):
+        parser.add_argument(
+            '--force', action='store_true',
+            help=force_help or "Don't prompt for confirmation or user variables.")
+        parser.add_argument(
+            '--user-var', action='append', metavar='NAME=VAL', type=UserVar.parse_arg,
+            help='A user variable assignment. This avoids prompting'
+            ' for input and lets you provide a value when using --force.'
+            ' Use repeatedly as needed for multiple values.')
+
+    def add_json_args(parser, help_text):
+        parser.add_argument('--json', action='store_true', help=help_text)
+        parser.add_argument(
+            '--jsonpretty', type=int, default=None, metavar='SPACES',
+            help='Optional number of spaces to indent for pretty-printed'
+            ' JSON output.')
+
     top_parser = top_level_parser()
     command_parser = top_parser.add_subparsers(
         title='commands', dest='command',
         help='See `%(prog)s <command> -h` for per-command usage info.')
     command_parser.required = True
 
     # test
@@ -2121,17 +2252,14 @@
                     ' directly from a git URL.  After installing, the package'
                     ' is marked as being "loaded" (see the ``load`` command).',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     sub_parser.set_defaults(run_cmd=cmd_install)
     sub_parser.add_argument(
         'package', nargs='+', help=pkg_name_help)
     sub_parser.add_argument(
-        '--force', action='store_true',
-        help='Skip the confirmation prompt.')
-    sub_parser.add_argument(
         '--skiptests', action='store_true',
         help='Skip running unit tests for packages before installation.')
     sub_parser.add_argument(
         '--nodeps', action='store_true',
         help='Skip all dependency resolution/checks.  Note that using this'
         ' option risks putting your installed package collection into a'
         ' broken or unusable state.')
@@ -2144,14 +2272,15 @@
         ' specified at a time when using this flag.  A version tag, branch'
         ' name, or commit hash may be specified here.'
         ' If the package name refers to a local git repo with a working tree,'
         ' then its currently active branch is used.'
         ' The default for other cases is to use'
         ' the latest version tag, or if a package has none,'
         ' the default branch, like "main" or "master".')
+    add_uservar_args(sub_parser)
 
     # bundle
     sub_parser = command_parser.add_parser(
         'bundle',
         help='Creates a bundle file containing a collection of Zeek packages.',
         description='This command creates a bundle file containing a collection'
                     ' of Zeek packages.  If ``--manifest`` is used, the user'
@@ -2207,20 +2336,18 @@
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     sub_parser.set_defaults(run_cmd=cmd_unbundle)
     sub_parser.add_argument(
         'bundle_filename',
         metavar='filename.bundle',
         help='The path of the bundle file to install.')
     sub_parser.add_argument(
-        '--force', action='store_true',
-        help='Skip the confirmation prompt.')
-    sub_parser.add_argument(
         '--replace', action='store_true',
         help='Using this flag first removes all installed packages before then'
         ' installing the packages from the bundle.')
+    add_uservar_args(sub_parser)
 
     # remove
     sub_parser = command_parser.add_parser(
         'remove',
         help='Uninstall a package.',
         description='Unloads (see the ``unload`` command) and uninstalls a'
         ' previously installed package.',
@@ -2287,27 +2414,25 @@
         ' package is updated to the latest commit on that branch, else the'
         ' package is updated to the highest available git version tag.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     sub_parser.set_defaults(run_cmd=cmd_upgrade)
     sub_parser.add_argument(
         'package', nargs='*', default=[], help=pkg_name_help)
     sub_parser.add_argument(
-        '--force', action='store_true',
-        help='Skip the confirmation prompt.')
-    sub_parser.add_argument(
         '--skiptests', action='store_true',
         help='Skip running unit tests for packages before installation.')
     sub_parser.add_argument(
         '--nodeps', action='store_true',
         help='Skip all dependency resolution/checks.  Note that using this'
         ' option risks putting your installed package collection into a'
         ' broken or unusable state.')
     sub_parser.add_argument(
         '--nosuggestions', action='store_true',
         help='Skip automatically installing suggested packages.')
+    add_uservar_args(sub_parser)
 
     # load
     sub_parser = command_parser.add_parser(
         'load',
         help='Register packages to be be auto-loaded by Zeek.',
         description='The Zeek Package Manager keeps track of all packages that'
         ' are marked as "loaded" and maintains a single Zeek script that, when'
@@ -2420,21 +2545,15 @@
         ' the metadata will be pulled from the installed version.  If not'
         ' installed, the latest version tag is used, or if a package has no'
         ' version tags, the default branch, like "main" or "master", is used.')
     sub_parser.add_argument(
         '--nolocal', action='store_true',
         help='Do not read information from locally installed packages.'
         ' Instead read info from remote GitHub.')
-    sub_parser.add_argument(
-        '--json', action='store_true',
-        help='Output package information as JSON.')
-    sub_parser.add_argument(
-        '--jsonpretty', type=int, default=None, metavar='SPACES',
-        help='Optional number of spaces to indent for pretty-printed'
-        ' JSON output.')
+    add_json_args(sub_parser, 'Output package information as JSON.')
     sub_parser.add_argument(
         '--allvers', action='store_true',
         help='When outputting package information as JSON, show metadata for'
         ' all versions. This option can be slow since remote repositories'
         ' may be cloned multiple times. Also, installed packages will show'
         ' metadata only for the installed version unless the --nolocal '
         ' option is given.')
@@ -2486,14 +2605,72 @@
         ' script (installed by zeek) in ``PATH``, or have the ``ZEEKPATH`` and'
         ' ``ZEEK_PLUGIN_PATH`` (or ``BROPATH`` and ``BRO_PLUGIN_PATH``)'
         ' environment variables already set so this command'
         ' can append package-specific paths to them.',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     sub_parser.set_defaults(run_cmd=cmd_env)
 
+    # create
+    sub_parser = command_parser.add_parser(
+        'create', help='Create a new Zeek package.',
+        description='This command creates a new Zeek package in the directory'
+        ' provided via --packagedir. If this directory exists, zkg will not'
+        ' modify it unless you provide --force.',
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    sub_parser.add_argument(
+        '--packagedir', metavar='DIR', required=True,
+        help='Output directory into which to produce the new package. Required.')
+    sub_parser.add_argument(
+        '--version',
+        help='The template version to use.  A version tag, branch name, or'
+        ' commit hash may be specified here.  If --template refers to a local'
+        ' git repo with a working tree, then zkg uses it as-is and the version'
+        ' is ignored.  The default for other cases is to use the latest'
+        ' version tag, or if a template has none, the default branch, like'
+        ' "main" or "master".')
+    sub_parser.add_argument(
+        '--features', nargs='+', metavar='FEATURE',
+        help='Additional features to include in your package. Use the ``template'
+        ' info`` command for information about available features.')
+    sub_parser.add_argument(
+        '--template', metavar='URL',
+        help='By default, zkg uses its own package template. This makes it'
+        ' select an alternative.')
+    sub_parser.set_defaults(run_cmd=cmd_create)
+    add_uservar_args(sub_parser)
+
+    # Template management commands
+
+    sub_parser = command_parser.add_parser(
+        'template', help='Manage package templates.')
+
+    template_command_parser = sub_parser.add_subparsers(
+        title='template commands',
+        help='See `%(prog)s template <command> -h for per-command usage info.')
+
+    # template info
+
+    sub_parser = template_command_parser.add_parser(
+        'info', help='Shows information about a package template.',
+        description='This command shows versions and supported features for'
+        ' a given package.')
+    add_json_args(sub_parser, 'Output template information as JSON.')
+    sub_parser.add_argument(
+        '--version',
+        help='The template version to report on.  A version tag, branch name,'
+        ' or commit hash may be specified here.  If the selected template'
+        ' refers to a local git repo, the version is ignored.  The default'
+        ' for other cases is to use the latest version tag, or if a template'
+        ' has none, the default branch, like "main" or "master".')
+    sub_parser.add_argument(
+        'template', metavar='URL', nargs='?',
+        help='URL of a package template repository, or local path to one.'
+        ' When not provided, the configured default template is used.')
+    sub_parser.set_defaults(run_cmd=cmd_template_info)
+
     return top_parser
 
 
 def main():
     args = argparser().parse_args()
 
     if args.verbose > 0:
```

## Comparing `zkg-2.8.0.dist-info/COPYING` & `zkg-2.9.0.dist-info/COPYING`

 * *Files identical despite different names*

## Comparing `zkg-2.8.0.dist-info/METADATA` & `zkg-2.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkg
-Version: 2.8.0
+Version: 2.9.0
 Summary: The Zeek Package Manager
 Home-page: https://github.com/zeek/package-manager
 Maintainer: The Zeek Project
 Maintainer-email: info@zeek.org
 License: University of Illinois/NCSA Open Source License
 Keywords: zeek zeekctl zeekcontrol package manager scripts plugins security
 Platform: UNKNOWN
```

