# Comparing `tmp/appcensus_dynamic_repos-0.6.0.76.tar.gz` & `tmp/appcensus_dynamic_repos-0.6.1.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appcensus_dynamic_repos-0.6.0.76.tar", max compression
+gzip compressed data, was "appcensus_dynamic_repos-0.6.1.91.tar", max compression
```

## Comparing `appcensus_dynamic_repos-0.6.0.76.tar` & `appcensus_dynamic_repos-0.6.1.91.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/README-public.md
--rw-r--r--   0        0        0     5006 2022-12-22 18:47:32.095497 appcensus_dynamic_repos-0.6.0.76/pyproject.toml
--rw-r--r--   0        0        0       68 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/__init__.py
--rw-r--r--   0        0        0     6491 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/auth.py
--rw-r--r--   0        0        0     9595 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/commands.py
--rw-r--r--   0        0        0     4822 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/models.py
--rw-r--r--   0        0        0     4382 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/plugin.py
--rw-r--r--   0        0        0     3306 2022-12-22 18:47:16.027369 appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/repo_collector.py
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-0.6.0.76/setup.py
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-0.6.0.76/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-05 15:33:34.313230 appcensus_dynamic_repos-0.6.1.91/README-public.md
+-rwxr-xr-x   0        0        0     5004 2023-07-05 15:33:47.685480 appcensus_dynamic_repos-0.6.1.91/pyproject.toml
+-rw-r--r--   0        0        0      606 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/__init__.py
+-rw-r--r--   0        0        0     6491 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/auth.py
+-rw-r--r--   0        0        0     9816 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/commands.py
+-rw-r--r--   0        0        0     4893 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/models.py
+-rw-r--r--   0        0        0     4414 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/plugin.py
+-rw-r--r--   0        0        0     3426 2023-07-05 15:33:34.317230 appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/repo_collector.py
+-rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-0.6.1.91/setup.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 appcensus_dynamic_repos-0.6.1.91/PKG-INFO
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/pyproject.toml` & `appcensus_dynamic_repos-0.6.1.91/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "appcensus.dynamic_repos"
-version = "0.6.0.76"
+version = "0.6.1.91"
 description = "Dynamic Poetry Repositories for AppCensus"
 authors = ["AppCensus <engineering@appcensus.io>"]
 license = "(c) 2022 App Census - All Rights Reserved"
 readme = "README-public.md"
 packages = [{include = "appcensus", from = 'src'}]
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
-poetry = "^1.3.0"
+poetry = "=1.3.2"
 poetry-core = "^1.3.0"
 tomlkit = "^0.11.0"
-pydantic = "^1.10.0"
-cryptography = "^38.0.0"
+pydantic = "^2.0.1"
+cryptography = ">=38.0.0"
 pytz = "^2022.5"
 boto3 = "^1.26.0"
 botocore = "^1.29.0"
+tomli = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
-pydantic = "^1.10"
 flake8 = "^5.0"
 pytest-cov = "^4.0"
 shellcheck-py = "^0.8"
 safety = "^2.3"
 pyupgrade = "^3.1"
 isort = "^5.10"
 black = "^22.10"
-mypy = "^0.981"
+mypy = "^1.4.1"
 commitizen = "^2.35"
 types-pytz = "^2022.5"
 pre-commit = "^2.20"
 poethepoet = "^0.16.5"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/auth.py` & `appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/auth.py`

 * *Files identical despite different names*

### Comparing `appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/commands.py` & `appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
-from typing import Optional, cast
+from typing import List, Optional, Union, cast
 
 import tomlkit
 from cleo.helpers import argument
+from cleo.ui.table_cell import TableCell
+from cleo.ui.table_separator import TableSeparator
 from poetry.config.source import Source
 from poetry.console.commands.command import Command
 from poetry.utils.password_manager import PasswordManager
 from tomlkit.items import Table
 from tomlkit.toml_document import TOMLDocument
 
 from appcensus.dynamic_repos import REPO_FILE_PATH
@@ -32,15 +34,15 @@
                 creds = CredentialCache.get(repo.name)
                 table = self.table(style="compact")
                 active_state = f" : <c1>{'yes' if creds and creds.valid() else 'no'}</>"
                 if creds:
                     active_state += (
                         f" expires <c1>{creds.expires.isoformat() if creds.expires else 'never'}</>"
                     )
-                rows = [
+                rows: List[Union[List[Union[str, TableCell]], TableSeparator]] = [
                     [
                         "<info>name</>",
                         f" : <c1>{repo.name}</>",
                     ],
                     ["<info>priority</>", f" : {self._flags2prio(repo)}"],
                     ["<info>url</>", f" : {repo.url}"],
                     ["<info>active auth</info>", active_state]
@@ -197,15 +199,15 @@
             if specific_repo:
                 cache_entries = filter(lambda n: n == specific_repo, cache_entries)
             self.line(f"Found <c1>{len(cache_entries)}</> entries")
             pm = PasswordManager(self.poetry.config)
             for name in cache_entries:
                 cache_entry = CredentialCache.get(name)
                 table = self.table(style="compact")
-                rows = [
+                rows: List[Union[List[Union[str, TableCell]], TableSeparator]] = [
                     [
                         "<info>name</>",
                         f" : <c1>{name}</>",
                     ],
                     ["<info>fingerprint</>", f" : {cache_entry.fingerprint}"],
                     [
                         "<info>expires</>",
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/models.py` & `appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from abc import abstractmethod
 from datetime import datetime, timedelta
 from functools import cached_property
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 
+import tomli
 import tomlkit
 from cryptography.hazmat.primitives.hashes import SHA256, Hash
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from pytz import UTC
 from tomlkit.items import KeyType, SingleKey, Table
 
 from appcensus.dynamic_repos import REPO_FILE_PATH
 
 
 class Auth(BaseModel):
     authtype: str
     cache: bool = False
-    timeout: Optional[int]
+    timeout: Optional[int] = None
 
     def to_table(self) -> Table:
         table = tomlkit.table(is_super_table=True)
         table.add("authtype", self.authtype)
         table.add("cache", self.cache)
         if self.timeout:
             table.add("timeout", self.timeout)
         return table
 
 
 class BasicAuth(Auth):
-    authtype: str = "basic"
+    authtype: Literal["basic"] = "basic"
     cache: bool = True
 
 
 class CodeArtifactAuth(Auth):
-    authtype: str = "codeartifact"
+    authtype: Literal["codeartifact"] = "codeartifact"
     domain: str
     owner: str
-    region: Optional[str]
-    profile: Optional[str]
+    region: Optional[str] = None
+    profile: Optional[str] = None
 
     def to_table(self) -> Table:
         table = super().to_table()
         table.add("domain", self.domain)
         table.add("owner", self.owner)
         if self.region:
             table.add("region", self.region)
@@ -49,15 +50,15 @@
             table.add("profile", self.profile)
         return table
 
 
 class RepoCredentials(BaseModel):
     class Config:
         arbitrary_types_allowed = True
-        keep_untouched = (cached_property,)
+        ignored_types = (cached_property,)
 
     authtype: str
 
     @cached_property
     @abstractmethod
     def fingerprint(self) -> str:
         raise NotImplementedError()
@@ -79,38 +80,38 @@
         return digest.finalize().hex()
 
 
 class CachedCredentialSet(BaseModel):
     VALID_WINDOW: int = 30
 
     authtype: str
-    expires: Optional[datetime]
+    expires: Optional[datetime] = None
     fingerprint: str
 
     def valid(self) -> bool:
         """Ensures that a set of credentials is valid for at least VALID_WINDOW seconds"""
         if not self.expires:
             return True
         return (datetime.now() + timedelta(seconds=self.VALID_WINDOW)).astimezone(
             UTC
         ) < self.expires.astimezone(UTC)
 
-    def to_table(self) -> tomlkit.item:
+    def to_table(self) -> tomlkit.items.Item:
         table = tomlkit.table(is_super_table=True)
         table.append("authtype", self.authtype)
         table.append("fingerprint", self.fingerprint)
         if self.expires:
             table.append("expires", self.expires)
         return table
 
 
 class Repo(BaseModel):
     name: str
     url: str
-    auth: Union[None, CodeArtifactAuth, BasicAuth]
+    auth: Union[None, CodeArtifactAuth, BasicAuth] = Field(None, discriminator="authtype")
     enabled: bool
     default: bool
     secondary: bool
 
     def to_table(self) -> Table:
         table = tomlkit.table(is_super_table=True)
         table.append("enabled", self.enabled)
@@ -139,21 +140,20 @@
         return None
 
     @classmethod
     def load(self, file_path: Path = REPO_FILE_PATH) -> None:
         self._repos = {}
         if file_path.exists():
             with file_path.open("r") as fh:
-                doc = tomlkit.parse(fh.read())
+                doc = tomli.loads(fh.read())
                 if "repo" not in doc.keys():
                     raise ValueError(f"No repos declared in {file_path}")
-                repo_attrs = doc["repo"].unwrap()
-                for repo_id in repo_attrs.keys():
-                    repo_attrs[repo_id]["name"] = repo_id
-                    repo = Repo.parse_obj(repo_attrs[repo_id])
+                for repo_id, repo_attrs in doc["repo"].items():
+                    repo_attrs["name"] = repo_id
+                    repo = Repo(**repo_attrs)
                     self._repos[repo.name] = repo
 
     @classmethod
     def save(cls, file_path: Path = REPO_FILE_PATH) -> None:
         doc = tomlkit.document()
 
         repos = tomlkit.table(is_super_table=True)
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/plugin.py` & `appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,8 +110,9 @@
             RepoShowCredentials,
             RepoClearCredentials,
             RepoUseCommand,
         ]
 
     def activate(self, application: Application) -> None:
         for command in self.commands:
+            assert command.name
             application.command_loader.register_factory(command.name, command)
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/src/appcensus/dynamic_repos/repo_collector.py` & `appcensus_dynamic_repos-0.6.1.91/src/appcensus/dynamic_repos/repo_collector.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 # In 1.2, the pool keeps an index marker for the beginning of the secondaries in a list of repos.
 class IndexedRepoStrategy(RepoStrategy):
     def __init__(self, pool: RepositoryPool):
         super().__init__(pool)
 
     def repositories(self) -> List[Source]:
         repos = []
-        secondary_start = self._pool._secondary_start_idx
+        secondary_start = self._pool._secondary_start_idx  # type: ignore[attr-defined]
         for rx, repo in enumerate(self._pool.repositories):
             repos.append(
                 Source(
                     name=repo.name,
-                    url=repo.url,
+                    url=repo.url,  # type: ignore[attr-defined]
                     default=True if rx == 0 else False,
                     secondary=True if secondary_start and rx >= secondary_start else False,
                 )
             )
         return repos
 
 
@@ -46,26 +46,26 @@
 # However, the priority is discarded and a priority-ordered list is returned for .repositories.
 # We mine internals for the attached priority, and set the flags appropriately.
 class PrioritizedRepoStrategy(RepoStrategy):
     def __init__(self, pool: RepositoryPool):
         super().__init__(pool)
 
     def _get_repo_priority(self, repo: Repository) -> Priority:
-        return self._pool._repositories[repo.name]
+        return self._pool._repositories[repo.name]  # type: ignore[return-value]
 
     def repositories(self) -> List[Source]:
         repos = []
         for repo in self._pool.repositories:
             if type(repo) is PyPiRepository:
                 continue
             prio = self._get_repo_priority(repo)
             repos.append(
                 Source(
                     name=repo.name,
-                    url=repo.url,
+                    url=repo.url,  # type: ignore[attr-defined]
                     default=(prio == Priority.DEFAULT),
                     secondary=(prio == Priority.SECONDARY),
                 )
             )
         return repos
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/setup.py` & `appcensus_dynamic_repos-0.6.1.91/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['boto3>=1.26.0,<2.0.0',
  'botocore>=1.29.0,<2.0.0',
- 'cryptography>=38.0.0,<39.0.0',
+ 'cryptography>=38.0.0',
  'poetry-core>=1.3.0,<2.0.0',
- 'poetry>=1.3.0,<2.0.0',
- 'pydantic>=1.10.0,<2.0.0',
+ 'poetry==1.3.2',
+ 'pydantic>=2.0.1,<3.0.0',
  'pytz>=2022.5,<2023.0',
+ 'tomli>=2.0.1,<3.0.0',
  'tomlkit>=0.11.0,<0.12.0']
 
 entry_points = \
 {'poetry.application.plugin': ['foo-command = '
                                'appcensus.dynamic_repos.plugin:DynamicReposApplication'],
  'poetry.plugin': ['dynamic_repos = '
                    'appcensus.dynamic_repos.plugin:DynamicRepos']}
 
 setup_kwargs = {
     'name': 'appcensus-dynamic-repos',
-    'version': '0.6.0.76',
+    'version': '0.6.1.91',
     'description': 'Dynamic Poetry Repositories for AppCensus',
     'long_description': '',
     'author': 'AppCensus',
     'author_email': 'engineering@appcensus.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `appcensus_dynamic_repos-0.6.0.76/PKG-INFO` & `appcensus_dynamic_repos-0.6.1.91/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: appcensus-dynamic-repos
-Version: 0.6.0.76
+Version: 0.6.1.91
 Summary: Dynamic Poetry Repositories for AppCensus
 License: (c) 2022 App Census - All Rights Reserved
 Author: AppCensus
 Author-email: engineering@appcensus.io
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.0,<2.0.0)
 Requires-Dist: botocore (>=1.29.0,<2.0.0)
-Requires-Dist: cryptography (>=38.0.0,<39.0.0)
-Requires-Dist: poetry (>=1.3.0,<2.0.0)
+Requires-Dist: cryptography (>=38.0.0)
+Requires-Dist: poetry (==1.3.2)
 Requires-Dist: poetry-core (>=1.3.0,<2.0.0)
-Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0.1,<3.0.0)
 Requires-Dist: pytz (>=2022.5,<2023.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomlkit (>=0.11.0,<0.12.0)
 Description-Content-Type: text/markdown
```

