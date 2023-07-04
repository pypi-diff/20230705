# Comparing `tmp/dagger_io-0.6.2.tar.gz` & `tmp/dagger_io-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.6.2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `dagger_io-0.6.2.tar` & `dagger_io-0.6.3.tar`

### file list

```diff
@@ -1,32 +1,38 @@
--rw-r--r--   0        0        0    10758 2023-06-15 23:19:36.174779 dagger_io-0.6.2/LICENSE
--rw-r--r--   0        0        0     4762 2023-06-15 23:19:36.174779 dagger_io-0.6.2/README.md
--rw-r--r--   0        0        0     6531 2023-06-15 23:20:36.607025 dagger_io-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/__init__.py
--rw-r--r--   0        0        0       71 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    11873 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/base.py
--rw-r--r--   0        0        0    91550 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/gen.py
--rw-r--r--   0        0        0    91142 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1683 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/cli.py
--rw-r--r--   0        0        0    20466 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/codegen.py
--rw-r--r--   0        0        0     1302 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/config.py
--rw-r--r--   0        0        0     1924 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4201 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2066 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8162 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/download.py
--rw-r--r--   0        0        0     4262 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/py.typed
--rw-r--r--   0        0        0     2319 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/__main__.py
--rw-r--r--   0        0        0      911 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3890 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5811 2023-06-15 23:19:36.178779 dagger_io-0.6.2/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 dagger_io-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/__main__.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/cli.py
+-rw-r--r--   0        0        0    27700 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/codegen.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/config.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/connection.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/context.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/exceptions.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/py.typed
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/session.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/api/__init__.py
+-rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/api/base.py
+-rw-r--r--   0        0        0    95496 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/api/gen.py
+-rw-r--r--   0        0        0    95046 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/engine/download.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/__main__.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_commands.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_context.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_converter.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_exceptions.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_server.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/_util.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/server/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 dagger_io-0.6.3/dagger/transport/httpx.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.6.3/.gitignore
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.6.3/LICENSE
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 dagger_io-0.6.3/README.md
+-rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 dagger_io-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 dagger_io-0.6.3/PKG-INFO
```

### Comparing `dagger_io-0.6.2/LICENSE` & `dagger_io-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/README.md` & `dagger_io-0.6.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -95,46 +95,42 @@
 
 - [Documentation](https://docs.dagger.io/sdk/python)
 - [API Reference](https://dagger-io.readthedocs.org)
 - [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)
 
 ## Development
 
-This library is maintained with [Poetry](https://python-poetry.org/docs/).
-
-If you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:
-
-```shell
-poetry install
-```
+This library is maintained with [Hatch](https://hatch.pypa.io/).
 
 The following commands are available:
-- `poe test`: Run tests.
-- `poe fmt`: Re-format code following common styling conventions.
-- `poe lint`: Check for linting violations.
-- `poe generate`: Regenerate API client after changes to the codegen.
-- `poe docs`: Build reference docs locally (needs `poetry install --with docs`).
+- `hatch run test`: Run tests.
+- `hatch run fmt`: Re-format code following common styling conventions.
+- `hatch run lint`: Check for linting violations.
+- `hatch run generate`: Regenerate API client after changes to the codegen.
+- `hatch run typing:check`: Run the type checker.
+- `hatch run docs:build`: Build reference docs locally (check with `(cd docs/_build && python -m http.server)`).
 
 ### Engine changes
 
 Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
 
 The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
 
 ```shell
-../../hack/make sdk:python:test
 ../../hack/make sdk:python:generate
+../../hack/make sdk:python:lint
+../../hack/make sdk:python:test
 ```
 
 You can also build the CLI and use it directly within the Python SDK:
 
 ```shell
-../../hack/dev poe test
+../../hack/dev hatch test
 ```
 
 Or build it separately and tell the SDK to use it directly (or any other CLI binary):
 
 ```shell
 ../../hack/make
-_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test
+_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger hatch test
 ```
```

### Comparing `dagger_io-0.6.2/pyproject.toml` & `dagger_io-0.6.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,154 +1,121 @@
 [build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+requires = ["hatchling", "hatch-vcs"]
+build-backend = "hatchling.build"
 
-[tool.poetry]
+[project]
 name = "dagger-io"
-version = "0.6.2"
+dynamic = ["version"]
 description = "A client package for running Dagger pipelines in Python."
-license = "Apache-2.0"
-authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
-homepage = "https://dagger.io"
-documentation = "https://docs.dagger.io/sdk/python"
-repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
+license = "Apache-2.0"
+authors = [
+    {name = "Dagger", email = "hello@dagger.io"},
+]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Framework :: AnyIO",
     "Framework :: Pytest",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
-    # TODO: just waiting on windows tests for this
-    # "Operating System :: OS Independent",
+    "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
-packages = [
-    { include = "dagger", from = "src" },
-]
-
-[tool.poetry.urls]
+requires-python = ">=3.10"
+dependencies = [
+    "anyio>=3.6.2",
+    "cattrs>=22.2.0",
+    "graphql-core>=3.2.3",
+    # TODO: replace next two lines with the following when gql version 3.5.0 is released
+    # "gql[httpx]>=3.5.0",
+    "gql>=3.4.0",
+    "httpx>=0.23.1",
+    "beartype>=0.11.0",
+    "platformdirs>=2.6.2",
+    "typing_extensions>=4.4.0",
+]
+
+[project.optional-dependencies]
+cli = [
+    "typer[all]>=0.6.1",
+]
+server = [
+    "typer[all]>=0.6.1",
+    "strawberry-graphql>=0.187.0",
+]
+
+[project.urls]
+"Homepage" = "https://dagger.io"
+"Documentation" = "https://docs.dagger.io/sdk/python"
+"Repository" = "https://github.com/dagger/dagger/tree/main/sdk/python"
 "Tracker" = "https://github.com/dagger/dagger/issues"
 "Release Notes" = "https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0"
 "Community" = "https://discord.gg/ufnyBtc8uY"
 "Twitter" = "https://twitter.com/dagger_io"
 
-[tool.poetry.dependencies]
-python = "^3.10"
-anyio = ">=3.6.2"
-attrs = ">=22.1.0"
-cattrs = ">=22.2.0"
-graphql-core = ">=3.2.3"
-# TODO: replace next two lines with the following when gql version 3.5.0 is released
-# gql = {version = ">=3.5.0", extras = ["httpx"]}
-gql = ">=3.4.0"
-httpx = ">=0.23.1"
-beartype = ">=0.11.0"
-platformdirs = ">=2.6.2"
-typing_extensions = ">=4.4.0"
-rich = ">=12.6.0"
-typer = {version = ">=0.6.1", extras = ["all"]}
-strawberry-graphql = {version = ">=0.133.5", optional = true}
-
-[tool.poetry.extras]
-server = ["strawberry-graphql"]
-
-[tool.poetry.group.test.dependencies]
-pytest = ">=7.2.0"
-pytest-mock = ">=3.10.0"
-pytest-subprocess = ">=1.4.2"
-pytest-lazy-fixture = "^0.6.3"
-pytest-httpx = ">=0.21.3"
-
-[tool.poetry.group.lint.dependencies]
-black = ">=22.3.0"
-mypy = ">=0.942"
-ruff = ">=0.0.218"
-
-[tool.poetry.group.dev.dependencies]
-poethepoet = ">=0.16.4"
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-sphinx = ">=5.3.0"
-sphinx-rtd-theme = "^1.1.1"
-
-[tool.poe.env]
-GEN_PATH = "./src/dagger/api"
-
-[tool.poe.env.DOCS_SNIPPETS]
-default = "../../docs/current"
-
-[tool.poe.tasks]
-test = "pytest"
-unittest = "pytest -m 'not slow'"
-typing = "mypy src/dagger tests"
-
-[tool.poe.tasks.docs]
-cmd = "sphinx-build -v . _build"
-cwd = "docs"
-
-[tool.poe.tasks.lint]
-sequence = [
-    "ruff check ${target}",
-    "black --preview --check ${target}",
-]
-default_item_type = "cmd"
-
-[[tool.poe.tasks.lint.args]]
-name = "target"
-positional = true
-multiple = true
-default = "."
-
-[tool.poe.tasks.lint-docs]
-ref = "lint ${DOCS_SNIPPETS}"
-
-[tool.poe.tasks.lint-all]
-sequence = [
-    "lint",
-    "lint-docs",
-]
-
-[tool.poe.tasks.fmt]
-sequence = [
-    "ruff --fix-only -e ${target}",
-    "black --preview ${target}",
-]
-default_item_type = "cmd"
-
-[[tool.poe.tasks.fmt.args]]
-name = "target"
-positional = true
-multiple = true
-default = "."
-
-[tool.poe.tasks.fmt-docs]
-ref = "fmt ${DOCS_SNIPPETS}"
-
-[tool.poe.tasks.fmt-all]
-sequence = [
-    "fmt",
-    "fmt-docs",
-]
-
-[tool.poe.tasks.generate]
-sequence = [
-    "python -m dagger generate --output ${GEN_PATH}/gen.py",
-    "python -m dagger generate --output ${GEN_PATH}/gen_sync.py --sync",
-    "black --preview ${GEN_PATH}/gen*.py",
+[tool.hatch.version]
+source = "vcs"
+fallback-version = "0.0.0"
+
+[tool.hatch.build]
+packages = ["src/dagger"]
+
+[tool.hatch.envs.default]
+features = ["cli", "server"]
+dependencies = [
+    "black>=22.3.0",
+    "ruff>=0.0.218",
+    "pytest>=7.2.0",
+    "pytest-mock>=3.10.0",
+    "pytest-subprocess>=1.4.2",
+    "pytest-lazy-fixture>=0.6.3",
+    "pytest-httpx>=0.21.3",
+]
+
+[tool.hatch.envs.default.scripts]
+generate = [
+    "python -m dagger generate --output src/dagger/api/gen.py",
+    "python -m dagger generate --output src/dagger/api/gen_sync.py --sync",
+    "black --preview src/dagger/api/gen*.py",
+]
+fmt = [
+    "ruff --fix-only -e {args:. ../../docs/current}",
+    "black --preview {args:. ../../docs/current}",
+]
+lint = [
+    "ruff check {args:. ../../docs/current}",
+    "black --preview --check {args:. ../../docs/current}",
+]
+test = "pytest -W default"
+testunit = "pytest -m 'not slow'"
+
+# Lock dependencies for CI, otherwise we could get failing checks on
+# unrelated PRs but not needed locally because it can help catch issues
+# early from dependency updates.
+lock = "hatch dep show requirements --all | pip-compile --annotate --resolver=backtracking -U -o requirements.txt -"
+
+[tool.hatch.envs.default.env-vars]
+CUSTOM_COMPILE_COMMAND = "hatch run lock"
+
+[tool.hatch.envs.typing]
+extra-dependencies = ["mypy>=0.942"]
+scripts = {check = "mypy {args:src/dagger tests}"}
+
+[tool.hatch.envs.docs]
+template = "docs"
+dependencies = [
+    "sphinx>=5.3.0",
+    "sphinx-rtd-theme~=1.1.1",
 ]
-default_item_type = "cmd"
+scripts = {build = "sphinx-build -v docs docs/_build"}
 
 [tool.pytest.ini_options]
 testpaths = ["tests/"]
 addopts = [
     "--import-mode=importlib",
 ]
 markers = [
@@ -173,14 +140,15 @@
 
 [tool.black]
 include = '\.pyi?$'
 target-version = ["py310", "py311"]
 
 [tool.ruff]
 src = ["src", "tests"]
+exclude = ["experimental/*/pyproject.toml"]
 target-version = "py310"
 select = ["ALL"]
 ignore = [
     # Type inferrance is ok in a lot of places.
     "ANN",
     # This rule doesn't know to ignore a subclass override
     # so we get false positives for unused arguments.
@@ -230,14 +198,16 @@
     # Note: We could detect built-in shadowing like the reserved
     # keywords but these built-ins aren't being used in the generated
     # code so no need to bother.
     "A",
     "D",
     # Too hard to properly wrap long lines in codegen.
     "E501",
+    # Allow access to private members as it's controlled by our own library.
+    "SLF001",
     # Too many arguments to function call.
     "PLR0913",
     # `Optional` is preferred over `| None` because of how
     # beartype handles forward references.
     "UP007",
 ]
 # Ignore built-in shadowing in test mocks.
```

### Comparing `dagger_io-0.6.2/src/dagger/api/base.py` & `dagger_io-0.6.3/dagger/api/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 import contextlib
 import enum
 import functools
 import logging
 import typing
 from collections import deque
 from collections.abc import Callable, Sequence
-from typing import Annotated, Any, ParamSpec, TypeGuard, TypeVar, overload
+from dataclasses import MISSING, asdict, dataclass, field, is_dataclass, replace
+from typing import (
+    Annotated,
+    Any,
+    ParamSpec,
+    TypeGuard,
+    TypeVar,
+    get_type_hints,
+    overload,
+)
 
 import anyio
-import attrs
 import cattrs
 import graphql
 import httpx
 from beartype import beartype
 from beartype.door import TypeHint
 from beartype.roar import BeartypeCallHintViolation
-from beartype.vale import Is, IsInstance
+from beartype.vale import Is, IsInstance, IsSubclass
 from cattrs.preconf.json import make_converter
 from gql.client import AsyncClientSession, SyncClientSession
 from gql.dsl import DSLField, DSLQuery, DSLSchema, DSLSelectable, DSLType, dsl_gql
 from gql.transport.exceptions import (
     TransportClosed,
     TransportProtocolError,
     TransportQueryError,
@@ -36,61 +44,103 @@
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
-@attrs.define
+@dataclass(slots=True)
 class Field:
     type_name: str
     name: str
     args: dict[str, Any]
+    children: dict[str, "Field"] = field(default_factory=dict)
 
     def to_dsl(self, schema: DSLSchema) -> DSLField:
         type_: DSLType = getattr(schema, self.type_name)
-        field: DSLField = getattr(type_, self.name)(**self.args)
-        return field
+        field_ = getattr(type_, self.name)(**self.args)
+        if self.children:
+            field_ = field_.select(
+                **{name: child.to_dsl(schema) for name, child in self.children.items()}
+            )
+        return field_
 
+    def add_child(self, child: "Field") -> "Field":
+        return replace(self, children={child.name: child})
 
-@attrs.define
+
+@dataclass(slots=True)
 class Context:
     session: AsyncClientSession | SyncClientSession
     schema: DSLSchema
-    selections: deque[Field] = attrs.field(factory=deque)
-    converter: cattrs.Converter = attrs.field(
-        factory=functools.partial(make_converter, detailed_validation=False)
-    )
+    selections: deque[Field] = field(default_factory=deque)
+    converter: cattrs.Converter = field(init=False)
+
+    def __post_init__(self):
+        conv = make_converter(detailed_validation=False)
+
+        # For types that were returned from a list we need to set
+        # their private attributes with a custom structuring function.
+
+        def _needs_hook(cls: type) -> bool:
+            return issubclass(cls, Type) and hasattr(cls, "__slots__")
+
+        def _struct(d: dict[str, Any], cls: type) -> Any:
+            obj = cls(self)
+            hints = get_type_hints(cls)
+            for slot in getattr(cls, "__slots__", ()):
+                t = hints.get(slot)
+                if t and slot in d:
+                    setattr(obj, slot, conv.structure(d[slot], t))
+            return obj
+
+        conv.register_structure_hook_func(
+            _needs_hook,
+            _struct,
+        )
+
+        self.converter = conv
 
     def select(
-        self,
-        type_name: str,
-        field_name: str,
-        args: dict[str, Any],
+        self, type_name: str, field_name: str, args: dict[str, Any]
     ) -> "Context":
-        field = Field(type_name, field_name, args)
-
+        field_ = Field(type_name, field_name, args)
         selections = self.selections.copy()
-        selections.append(field)
+        selections.append(field_)
+        return replace(self, selections=selections)
 
-        return attrs.evolve(self, selections=selections)
+    def select_multiple(self, type_name: str, **fields: str) -> "Context":
+        selections = self.selections.copy()
+        parent = selections.pop()
+        # When selecting multiple fields, set them as children of the last
+        # selection to make `build` logic simpler.
+        field_ = replace(
+            parent,
+            # Using kwargs for alias names. This way the returned result
+            # is already formatted with the python name we expect.
+            children={k: Field(type_name, v, {}) for k, v in fields.items()},
+        )
+        selections.append(field_)
+        return replace(self, selections=selections)
 
     def build(self) -> DSLSelectable:
         if not self.selections:
             msg = "No field has been selected"
             raise InvalidQueryError(msg)
 
-        selections = self.selections.copy()
-        selectable = selections.pop().to_dsl(self.schema)
+        def _collapse(child: Field, field_: Field):
+            return field_.add_child(child)
 
-        while selections:
-            parent = selections.pop().to_dsl(self.schema)
-            selectable = parent.select(selectable)
+        # This transforms the selection set into a single root Field, where
+        # the `children` attribute is set to the next selection in the set,
+        # and so on...
+        root = functools.reduce(_collapse, reversed(self.selections))
 
-        return selectable
+        # `to_dsl` will cascade to all children, until the end.
+        return root.to_dsl(self.schema)
 
     def query(self) -> graphql.DocumentNode:
         return dsl_gql(DSLQuery(self.build()))
 
     @overload
     async def execute(self, return_type: None = None) -> None:
         ...
@@ -119,14 +169,38 @@
         assert isinstance(self.session, SyncClientSession)
         self.resolve_ids_sync()
         query = self.query()
         with self._handle_execute(query):
             result = self.session.execute(query)
         return self.get_value(result, return_type) if return_type else None
 
+    @overload
+    def get_value(self, value: None, return_type: Any) -> None:
+        ...
+
+    @overload
+    def get_value(self, value: dict[str, Any], return_type: type[T]) -> T:
+        ...
+
+    def get_value(self, value: dict[str, Any] | None, return_type: type[T]) -> T | None:
+        type_hint = TypeHint(return_type)
+
+        for f in self.selections:
+            if not isinstance(value, dict):
+                break
+            value = value[f.name]
+
+        if value is None and not type_hint.is_bearable(value):
+            msg = (
+                "Required field got a null response. Check if parent fields are valid."
+            )
+            raise InvalidQueryError(msg)
+
+        return self.converter.structure(value, return_type)
+
     async def resolve_ids(self) -> None:
         """Replace Type object instances with their ID implicitly."""
 
         # mutating to avoid re-fetching on forked pipeline
         async def _resolve_id(pos: int, k: str, v: IDType):
             sel = self.selections[pos]
             sel.args[k] = await v.id()
@@ -192,89 +266,84 @@
             raise TransportError(msg) from e
 
         except TransportQueryError as e:
             if error := QueryError.from_transport(e, query):
                 raise error from e
             raise
 
-    def get_value(self, value: dict[str, Any] | None, return_type: type[T]) -> T:
-        if value is not None:
-            value = self.structure_response(value, return_type)
-        if value is None and not TypeHint(return_type).is_bearable(None):
-            msg = (
-                "Required field got a null response. Check if parent fields are valid."
-            )
-            raise InvalidQueryError(msg)
-        return value
-
-    def structure_response(self, response: dict[str, Any], return_type: type[T]) -> T:
-        for f in self.selections:
-            response = response[f.name]
-            if response is None:
-                return None
-        return self.converter.structure(response, return_type)
-
 
 class Arg(typing.NamedTuple):
     name: str  # GraphQL name
     value: Any
-    default: Any = attrs.NOTHING
+    default: Any = MISSING
 
 
 class Scalar(str):
     """Custom scalar."""
 
+    __slots__ = ()
+
 
 class Enum(str, enum.Enum):
     """Custom enumeration."""
 
+    __slots__ = ()
+
     def __str__(self) -> str:
         return str(self.value)
 
 
 class Object:
     """Base for object types."""
 
-    @property
-    def graphql_name(self) -> str:
-        return self.__class__.__name__
+    @classmethod
+    def _graphql_name(cls) -> str:
+        return cls.__name__
 
 
 class Input(Object):
     """Input object type."""
 
 
-InputType = Annotated[Input, Is[lambda o: attrs.has(o)]]
+InputType = Annotated[Input, Is[lambda o: is_dataclass(o)]]
 InputTypeSeq = Annotated[Sequence[InputType], ~IsInstance[str]]
 
 InputHint = TypeHint(InputType)
 InputSeqHint = TypeHint(InputTypeSeq)
 
 
 def as_input_arg(val):
     if InputHint.is_bearable(val):
-        return attrs.asdict(val)
+        return asdict(val)
     if InputSeqHint.is_bearable(val):
-        return [attrs.asdict(v) for v in val]
+        return [asdict(v) for v in val]
     return val
 
 
-@attrs.define
 class Type(Object):
     """Object type."""
 
-    _ctx: Context
+    __slots__ = ("_ctx",)
+
+    def __init__(self, ctx: Context) -> None:
+        self._ctx = ctx
 
-    def _select(self, field_name: str, args: typing.Sequence[Arg]) -> Context:
+    def _select(self, field_name: str, args: typing.Sequence[Arg]):
         _args = {
             arg.name: as_input_arg(arg.value)
             for arg in args
             if arg.value is not arg.default
         }
-        return self._ctx.select(self.graphql_name, field_name, _args)
+        return self._ctx.select(self._graphql_name(), field_name, _args)
+
+    def _root_select(self, field_name: str, args: typing.Sequence[Arg]):
+        return Root._from_context(self._ctx)._select(field_name, args)  # noqa: SLF001
+
+    def _select_multiple(self, **kwargs):
+        return self._ctx.select_multiple(self._graphql_name(), **kwargs)
 
     def with_(self, cb: Callable[[Self], Self]) -> Self:
         """
         Use a callable to add to the current object.
 
         This allows reusing funcionality (e.g., adding mounts)
         without breaking the pipeline chain.
@@ -295,29 +364,68 @@
         ...     .with_exec(["printenv", "FOO"])
         ...     .stdout()
         ... )
         """
         return cb(self)
 
 
+@typing.runtime_checkable
+class FromIDType(typing.Protocol):
+    @classmethod
+    def _id_type(cls) -> Scalar:
+        ...
+
+    @classmethod
+    def _from_id_query_field(cls) -> str:
+        ...
+
+
+IDTypeSubclass = Annotated[FromIDType, IsSubclass[Type, FromIDType]]
+IDTypeSubclassHint = TypeHint(IDTypeSubclass)
+
+
+def is_id_type_subclass(v: type) -> TypeGuard[type[IDTypeSubclass]]:
+    return IDTypeSubclassHint.is_bearable(v)
+
+
+_Type = TypeVar("_Type", bound=Type)
+
+
 class Root(Type):
     """Top level query object type (a.k.a. Query)."""
 
     @classmethod
+    def _graphql_name(cls) -> str:
+        return "Query"
+
+    @classmethod
     def from_session(cls, session: AsyncClientSession):
         assert (
             session.client.schema is not None
         ), "GraphQL session has not been initialized"
         ds = DSLSchema(session.client.schema)
         ctx = Context(session, ds)
         return cls(ctx)
 
-    @property
-    def graphql_name(self) -> str:
-        return "Query"
+    @classmethod
+    def _from_context(cls, ctx: Context):
+        return cls(replace(ctx, selections=deque()))
+
+    def _get_object_instance(self, id_: str | Scalar, cls: type[_Type]) -> _Type:
+        if not is_id_type_subclass(cls):
+            msg = f"Unsupported type '{cls.__name__}'"
+            raise TypeError(msg)
+
+        if type(id_) is not cls._id_type() and not isinstance(id_, str):
+            msg = f"Expected id type '{cls._id_type()}', got '{type(id_)}'"
+            raise TypeError(msg)
+
+        assert issubclass(cls, Type)
+        ctx = self._select(cls._from_id_query_field(), [Arg("id", id_)])
+        return cls(ctx)
 
 
 @typing.runtime_checkable
 class HasID(typing.Protocol):
     async def id(self) -> Scalar:  # noqa: A003
         ...
```

### Comparing `dagger_io-0.6.2/src/dagger/api/gen.py` & `dagger_io-0.6.3/dagger/api/gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Code generated by dagger. DO NOT EDIT.
 
 import warnings
 from collections.abc import Sequence
+from dataclasses import dataclass
 from typing import Optional
 
-import attrs
-
 from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
 
 
 class CacheID(Scalar):
     """A global cache volume identifier."""
 
 
@@ -81,26 +80,26 @@
     TCP = "TCP"
     """TCP (Transmission Control Protocol)"""
 
     UDP = "UDP"
     """UDP (User Datagram Protocol)"""
 
 
-@attrs.define
+@dataclass(slots=True)
 class BuildArg(Input):
     """Key value object that represents a build argument."""
 
     name: str
     """The build argument name."""
 
     value: str
     """The build argument value."""
 
 
-@attrs.define
+@dataclass(slots=True)
 class PipelineLabel(Input):
     """Key value object that represents a Pipeline label."""
 
     name: str
     """Label name."""
 
     value: str
@@ -128,14 +127,18 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(CacheID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return CacheID
+
 
 class Container(Type):
     """An OCI-compatible container, also known as a docker container."""
 
     @typecheck
     def build(
         self,
@@ -304,19 +307,23 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
-    def env_variables(self) -> "EnvVariable":
+    async def env_variables(self) -> list["EnvVariable"]:
         """Retrieves the list of environment variables passed to commands."""
         _args: list[Arg] = []
         _ctx = self._select("envVariables", _args)
-        return EnvVariable(_ctx)
+        _ctx = EnvVariable(_ctx)._select_multiple(
+            _name="name",
+            _value="value",
+        )
+        return await _ctx.execute(list[EnvVariable])
 
     @typecheck
     def exec(
         self,
         args: Optional[Sequence[str]] = None,
         stdin: Optional[str] = None,
         redirect_stdout: Optional[str] = None,
@@ -439,26 +446,31 @@
             Arg("platformVariants", platform_variants, None),
             Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("export", _args)
         return await _ctx.execute(bool)
 
     @typecheck
-    def exposed_ports(self) -> "Port":
+    async def exposed_ports(self) -> list["Port"]:
         """Retrieves the list of exposed ports.
 
         This includes ports already exposed by the image, even if not
         explicitly added with dagger.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
         """
         _args: list[Arg] = []
         _ctx = self._select("exposedPorts", _args)
-        return Port(_ctx)
+        _ctx = Port(_ctx)._select_multiple(
+            _description="description",
+            _port="port",
+            _protocol="protocol",
+        )
+        return await _ctx.execute(list[Port])
 
     @typecheck
     def file(self, path: str) -> "File":
         """Retrieves a file at the given path.
 
         Mounts are included.
 
@@ -553,14 +565,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ContainerID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ContainerID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "container"
+
     @typecheck
     async def image_ref(self) -> Optional[str]:
         """The unique image reference which can only be retrieved immediately
         after the 'Container.From' call.
 
         Returns
         -------
@@ -630,19 +650,23 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("label", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
-    def labels(self) -> "Label":
+    async def labels(self) -> list["Label"]:
         """Retrieves the list of labels passed to container."""
         _args: list[Arg] = []
         _ctx = self._select("labels", _args)
-        return Label(_ctx)
+        _ctx = Label(_ctx)._select_multiple(
+            _name="name",
+            _value="value",
+        )
+        return await _ctx.execute(list[Label])
 
     @typecheck
     async def mounts(self) -> list[str]:
         """Retrieves the list of paths where a directory is mounted.
 
         Returns
         -------
@@ -832,16 +856,17 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
-        await _ctx.execute()
-        return self
+        _id = await _ctx.execute(ContainerID)
+        _ctx = self._root_select("container", [Arg("id", _id)])
+        return Container(_ctx)
 
     def __await__(self):
         return self.sync().__await__()
 
     @typecheck
     async def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
@@ -1746,14 +1771,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(DirectoryID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return DirectoryID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "directory"
+
     @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Directory":
@@ -1935,14 +1968,22 @@
         return Directory(_ctx)
 
 
 class EnvVariable(Type):
     """A simple key value object that represents an environment
     variable."""
 
+    __slots__ = (
+        "_name",
+        "_value",
+    )
+
+    _name: Optional[str]
+    _value: Optional[str]
+
     @typecheck
     async def name(self) -> str:
         """The environment variable name.
 
         Returns
         -------
         str
@@ -1953,14 +1994,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def value(self) -> str:
         """The environment variable value.
@@ -1975,14 +2018,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_value"):
+            return self._value
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
         return await _ctx.execute(str)
 
 
 class File(Type):
     """A file."""
@@ -2065,14 +2110,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FileID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return FileID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "file"
+
     @typecheck
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
@@ -2416,14 +2469,22 @@
         _ctx = self._select("value", _args)
         return await _ctx.execute(str)
 
 
 class Label(Type):
     """A simple key value object that represents a label."""
 
+    __slots__ = (
+        "_name",
+        "_value",
+    )
+
+    _name: Optional[str]
+    _value: Optional[str]
+
     @typecheck
     async def name(self) -> str:
         """The label name.
 
         Returns
         -------
         str
@@ -2434,14 +2495,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def value(self) -> str:
         """The label value.
@@ -2456,22 +2519,34 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_value"):
+            return self._value
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
         return await _ctx.execute(str)
 
 
 class Port(Type):
     """A port exposed by a container."""
 
+    __slots__ = (
+        "_description",
+        "_port",
+        "_protocol",
+    )
+
+    _description: Optional[str]
+    _port: Optional[int]
+    _protocol: Optional[NetworkProtocol]
+
     @typecheck
     async def description(self) -> Optional[str]:
         """The port description.
 
         Returns
         -------
         Optional[str]
@@ -2482,14 +2557,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
     async def port(self) -> int:
         """The port number.
@@ -2504,14 +2581,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_port"):
+            return self._port
         _args: list[Arg] = []
         _ctx = self._select("port", _args)
         return await _ctx.execute(int)
 
     @typecheck
     async def protocol(self) -> NetworkProtocol:
         """The transport layer network protocol.
@@ -2524,29 +2603,36 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_protocol"):
+            return self._protocol
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
         return await _ctx.execute(NetworkProtocol)
 
 
 class Project(Type):
     """A collection of Dagger resources that can be queried and
     invoked."""
 
     @typecheck
-    def commands(self) -> "ProjectCommand":
+    async def commands(self) -> list["ProjectCommand"]:
         """Commands provided by this project"""
         _args: list[Arg] = []
         _ctx = self._select("commands", _args)
-        return ProjectCommand(_ctx)
+        _ctx = ProjectCommand(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+            _result_type="resultType",
+        )
+        return await _ctx.execute(list[ProjectCommand])
 
     @typecheck
     async def id(self) -> ProjectID:
         """A unique identifier for this project.
 
         Note
         ----
@@ -2564,14 +2650,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ProjectID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ProjectID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "project"
+
     @typecheck
     def load(
         self,
         source: Directory,
         config_path: str,
     ) -> "Project":
         """Initialize this project from the given directory and config path"""
@@ -2604,14 +2698,24 @@
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
 
 class ProjectCommand(Type):
     """A command defined in a project that can be invoked from the CLI."""
 
+    __slots__ = (
+        "_description",
+        "_name",
+        "_result_type",
+    )
+
+    _description: Optional[str]
+    _name: Optional[str]
+    _result_type: Optional[str]
+
     @typecheck
     async def description(self) -> Optional[str]:
         """Documentation for what this command does.
 
         Returns
         -------
         Optional[str]
@@ -2622,24 +2726,30 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
-    def flags(self) -> "ProjectCommandFlag":
+    async def flags(self) -> list["ProjectCommandFlag"]:
         """Flags accepted by this command."""
         _args: list[Arg] = []
         _ctx = self._select("flags", _args)
-        return ProjectCommandFlag(_ctx)
+        _ctx = ProjectCommandFlag(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+        )
+        return await _ctx.execute(list[ProjectCommandFlag])
 
     @typecheck
     async def id(self) -> ProjectCommandID:
         """A unique identifier for this command.
 
         Note
         ----
@@ -2657,14 +2767,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ProjectCommandID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ProjectCommandID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "projectCommand"
+
     @typecheck
     async def name(self) -> str:
         """The name of the command.
 
         Returns
         -------
         str
@@ -2675,14 +2793,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def result_type(self) -> Optional[str]:
         """The name of the type returned by this command.
@@ -2697,29 +2817,44 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_result_type"):
+            return self._result_type
         _args: list[Arg] = []
         _ctx = self._select("resultType", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
-    def subcommands(self) -> "ProjectCommand":
+    async def subcommands(self) -> list["ProjectCommand"]:
         """Subcommands, if any, that this command provides."""
         _args: list[Arg] = []
         _ctx = self._select("subcommands", _args)
-        return ProjectCommand(_ctx)
+        _ctx = ProjectCommand(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+            _result_type="resultType",
+        )
+        return await _ctx.execute(list[ProjectCommand])
 
 
 class ProjectCommandFlag(Type):
     """A flag accepted by a project command."""
 
+    __slots__ = (
+        "_description",
+        "_name",
+    )
+
+    _description: Optional[str]
+    _name: Optional[str]
+
     @typecheck
     async def description(self) -> Optional[str]:
         """Documentation for what this flag sets.
 
         Returns
         -------
         Optional[str]
@@ -2730,14 +2865,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(Optional[str])
 
     @typecheck
     async def name(self) -> str:
         """The name of the flag.
@@ -2752,14 +2889,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
 
 class Client(Root):
     @typecheck
@@ -3006,14 +3145,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(SecretID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return SecretID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "secret"
+
     @typecheck
     async def plaintext(self) -> str:
         """The value of this secret.
 
         Returns
         -------
         str
@@ -3054,41 +3201,49 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(SocketID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return SocketID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "socket"
+
 
 __all__ = [
+    "BuildArg",
     "CacheID",
-    "ContainerID",
-    "DirectoryID",
-    "FileID",
-    "Platform",
-    "ProjectCommandID",
-    "ProjectID",
-    "SecretID",
-    "SocketID",
     "CacheSharingMode",
-    "ImageLayerCompression",
-    "NetworkProtocol",
-    "BuildArg",
-    "PipelineLabel",
     "CacheVolume",
+    "Client",
     "Container",
+    "ContainerID",
     "Directory",
+    "DirectoryID",
     "EnvVariable",
     "File",
+    "FileID",
     "GitRef",
     "GitRepository",
     "Host",
     "HostVariable",
+    "ImageLayerCompression",
     "Label",
+    "NetworkProtocol",
+    "PipelineLabel",
+    "Platform",
     "Port",
     "Project",
     "ProjectCommand",
     "ProjectCommandFlag",
-    "Client",
+    "ProjectCommandID",
+    "ProjectID",
     "Secret",
+    "SecretID",
     "Socket",
+    "SocketID",
 ]
```

### Comparing `dagger_io-0.6.2/src/dagger/api/gen_sync.py` & `dagger_io-0.6.3/dagger/api/gen_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Code generated by dagger. DO NOT EDIT.
 
 import warnings
 from collections.abc import Sequence
+from dataclasses import dataclass
 from typing import Optional
 
-import attrs
-
 from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
 
 
 class CacheID(Scalar):
     """A global cache volume identifier."""
 
 
@@ -81,26 +80,26 @@
     TCP = "TCP"
     """TCP (Transmission Control Protocol)"""
 
     UDP = "UDP"
     """UDP (User Datagram Protocol)"""
 
 
-@attrs.define
+@dataclass(slots=True)
 class BuildArg(Input):
     """Key value object that represents a build argument."""
 
     name: str
     """The build argument name."""
 
     value: str
     """The build argument value."""
 
 
-@attrs.define
+@dataclass(slots=True)
 class PipelineLabel(Input):
     """Key value object that represents a Pipeline label."""
 
     name: str
     """Label name."""
 
     value: str
@@ -128,14 +127,18 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(CacheID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return CacheID
+
 
 class Container(Type):
     """An OCI-compatible container, also known as a docker container."""
 
     @typecheck
     def build(
         self,
@@ -304,19 +307,23 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    def env_variables(self) -> "EnvVariable":
+    def env_variables(self) -> list["EnvVariable"]:
         """Retrieves the list of environment variables passed to commands."""
         _args: list[Arg] = []
         _ctx = self._select("envVariables", _args)
-        return EnvVariable(_ctx)
+        _ctx = EnvVariable(_ctx)._select_multiple(
+            _name="name",
+            _value="value",
+        )
+        return _ctx.execute_sync(list[EnvVariable])
 
     @typecheck
     def exec(
         self,
         args: Optional[Sequence[str]] = None,
         stdin: Optional[str] = None,
         redirect_stdout: Optional[str] = None,
@@ -439,26 +446,31 @@
             Arg("platformVariants", platform_variants, None),
             Arg("forcedCompression", forced_compression, None),
         ]
         _ctx = self._select("export", _args)
         return _ctx.execute_sync(bool)
 
     @typecheck
-    def exposed_ports(self) -> "Port":
+    def exposed_ports(self) -> list["Port"]:
         """Retrieves the list of exposed ports.
 
         This includes ports already exposed by the image, even if not
         explicitly added with dagger.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
         """
         _args: list[Arg] = []
         _ctx = self._select("exposedPorts", _args)
-        return Port(_ctx)
+        _ctx = Port(_ctx)._select_multiple(
+            _description="description",
+            _port="port",
+            _protocol="protocol",
+        )
+        return _ctx.execute_sync(list[Port])
 
     @typecheck
     def file(self, path: str) -> "File":
         """Retrieves a file at the given path.
 
         Mounts are included.
 
@@ -553,14 +565,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(ContainerID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ContainerID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "container"
+
     @typecheck
     def image_ref(self) -> Optional[str]:
         """The unique image reference which can only be retrieved immediately
         after the 'Container.From' call.
 
         Returns
         -------
@@ -630,19 +650,23 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("label", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    def labels(self) -> "Label":
+    def labels(self) -> list["Label"]:
         """Retrieves the list of labels passed to container."""
         _args: list[Arg] = []
         _ctx = self._select("labels", _args)
-        return Label(_ctx)
+        _ctx = Label(_ctx)._select_multiple(
+            _name="name",
+            _value="value",
+        )
+        return _ctx.execute_sync(list[Label])
 
     @typecheck
     def mounts(self) -> list[str]:
         """Retrieves the list of paths where a directory is mounted.
 
         Returns
         -------
@@ -832,16 +856,17 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sync", _args)
-        _ctx.execute_sync()
-        return self
+        _id = _ctx.execute_sync(ContainerID)
+        _ctx = self._root_select("container", [Arg("id", _id)])
+        return Container(_ctx)
 
     @typecheck
     def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
@@ -1743,14 +1768,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(DirectoryID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return DirectoryID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "directory"
+
     @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
     ) -> "Directory":
@@ -1932,14 +1965,22 @@
         return Directory(_ctx)
 
 
 class EnvVariable(Type):
     """A simple key value object that represents an environment
     variable."""
 
+    __slots__ = (
+        "_name",
+        "_value",
+    )
+
+    _name: Optional[str]
+    _value: Optional[str]
+
     @typecheck
     def name(self) -> str:
         """The environment variable name.
 
         Returns
         -------
         str
@@ -1950,14 +1991,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
     def value(self) -> str:
         """The environment variable value.
@@ -1972,14 +2015,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_value"):
+            return self._value
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
         return _ctx.execute_sync(str)
 
 
 class File(Type):
     """A file."""
@@ -2062,14 +2107,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(FileID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return FileID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "file"
+
     @typecheck
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
@@ -2413,14 +2466,22 @@
         _ctx = self._select("value", _args)
         return _ctx.execute_sync(str)
 
 
 class Label(Type):
     """A simple key value object that represents a label."""
 
+    __slots__ = (
+        "_name",
+        "_value",
+    )
+
+    _name: Optional[str]
+    _value: Optional[str]
+
     @typecheck
     def name(self) -> str:
         """The label name.
 
         Returns
         -------
         str
@@ -2431,14 +2492,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
     def value(self) -> str:
         """The label value.
@@ -2453,22 +2516,34 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_value"):
+            return self._value
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
         return _ctx.execute_sync(str)
 
 
 class Port(Type):
     """A port exposed by a container."""
 
+    __slots__ = (
+        "_description",
+        "_port",
+        "_protocol",
+    )
+
+    _description: Optional[str]
+    _port: Optional[int]
+    _protocol: Optional[NetworkProtocol]
+
     @typecheck
     def description(self) -> Optional[str]:
         """The port description.
 
         Returns
         -------
         Optional[str]
@@ -2479,14 +2554,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def port(self) -> int:
         """The port number.
@@ -2501,14 +2578,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_port"):
+            return self._port
         _args: list[Arg] = []
         _ctx = self._select("port", _args)
         return _ctx.execute_sync(int)
 
     @typecheck
     def protocol(self) -> NetworkProtocol:
         """The transport layer network protocol.
@@ -2521,29 +2600,36 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_protocol"):
+            return self._protocol
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
         return _ctx.execute_sync(NetworkProtocol)
 
 
 class Project(Type):
     """A collection of Dagger resources that can be queried and
     invoked."""
 
     @typecheck
-    def commands(self) -> "ProjectCommand":
+    def commands(self) -> list["ProjectCommand"]:
         """Commands provided by this project"""
         _args: list[Arg] = []
         _ctx = self._select("commands", _args)
-        return ProjectCommand(_ctx)
+        _ctx = ProjectCommand(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+            _result_type="resultType",
+        )
+        return _ctx.execute_sync(list[ProjectCommand])
 
     @typecheck
     def id(self) -> ProjectID:
         """A unique identifier for this project.
 
         Note
         ----
@@ -2561,14 +2647,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(ProjectID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ProjectID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "project"
+
     @typecheck
     def load(
         self,
         source: Directory,
         config_path: str,
     ) -> "Project":
         """Initialize this project from the given directory and config path"""
@@ -2601,14 +2695,24 @@
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
 
 class ProjectCommand(Type):
     """A command defined in a project that can be invoked from the CLI."""
 
+    __slots__ = (
+        "_description",
+        "_name",
+        "_result_type",
+    )
+
+    _description: Optional[str]
+    _name: Optional[str]
+    _result_type: Optional[str]
+
     @typecheck
     def description(self) -> Optional[str]:
         """Documentation for what this command does.
 
         Returns
         -------
         Optional[str]
@@ -2619,24 +2723,30 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    def flags(self) -> "ProjectCommandFlag":
+    def flags(self) -> list["ProjectCommandFlag"]:
         """Flags accepted by this command."""
         _args: list[Arg] = []
         _ctx = self._select("flags", _args)
-        return ProjectCommandFlag(_ctx)
+        _ctx = ProjectCommandFlag(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+        )
+        return _ctx.execute_sync(list[ProjectCommandFlag])
 
     @typecheck
     def id(self) -> ProjectCommandID:
         """A unique identifier for this command.
 
         Note
         ----
@@ -2654,14 +2764,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(ProjectCommandID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return ProjectCommandID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "projectCommand"
+
     @typecheck
     def name(self) -> str:
         """The name of the command.
 
         Returns
         -------
         str
@@ -2672,14 +2790,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
     def result_type(self) -> Optional[str]:
         """The name of the type returned by this command.
@@ -2694,29 +2814,44 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_result_type"):
+            return self._result_type
         _args: list[Arg] = []
         _ctx = self._select("resultType", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    def subcommands(self) -> "ProjectCommand":
+    def subcommands(self) -> list["ProjectCommand"]:
         """Subcommands, if any, that this command provides."""
         _args: list[Arg] = []
         _ctx = self._select("subcommands", _args)
-        return ProjectCommand(_ctx)
+        _ctx = ProjectCommand(_ctx)._select_multiple(
+            _description="description",
+            _name="name",
+            _result_type="resultType",
+        )
+        return _ctx.execute_sync(list[ProjectCommand])
 
 
 class ProjectCommandFlag(Type):
     """A flag accepted by a project command."""
 
+    __slots__ = (
+        "_description",
+        "_name",
+    )
+
+    _description: Optional[str]
+    _name: Optional[str]
+
     @typecheck
     def description(self) -> Optional[str]:
         """Documentation for what this flag sets.
 
         Returns
         -------
         Optional[str]
@@ -2727,14 +2862,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_description"):
+            return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def name(self) -> str:
         """The name of the flag.
@@ -2749,14 +2886,16 @@
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
+        if hasattr(self, "_name"):
+            return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
 
 class Client(Root):
     @typecheck
@@ -3003,14 +3142,22 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(SecretID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return SecretID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "secret"
+
     @typecheck
     def plaintext(self) -> str:
         """The value of this secret.
 
         Returns
         -------
         str
@@ -3051,41 +3198,49 @@
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return _ctx.execute_sync(SocketID)
 
+    @classmethod
+    def _id_type(cls) -> type[Scalar]:
+        return SocketID
+
+    @classmethod
+    def _from_id_query_field(cls):
+        return "socket"
+
 
 __all__ = [
+    "BuildArg",
     "CacheID",
-    "ContainerID",
-    "DirectoryID",
-    "FileID",
-    "Platform",
-    "ProjectCommandID",
-    "ProjectID",
-    "SecretID",
-    "SocketID",
     "CacheSharingMode",
-    "ImageLayerCompression",
-    "NetworkProtocol",
-    "BuildArg",
-    "PipelineLabel",
     "CacheVolume",
+    "Client",
     "Container",
+    "ContainerID",
     "Directory",
+    "DirectoryID",
     "EnvVariable",
     "File",
+    "FileID",
     "GitRef",
     "GitRepository",
     "Host",
     "HostVariable",
+    "ImageLayerCompression",
     "Label",
+    "NetworkProtocol",
+    "PipelineLabel",
+    "Platform",
     "Port",
     "Project",
     "ProjectCommand",
     "ProjectCommandFlag",
-    "Client",
+    "ProjectCommandID",
+    "ProjectID",
     "Secret",
+    "SecretID",
     "Socket",
+    "SocketID",
 ]
```

### Comparing `dagger_io-0.6.2/src/dagger/cli.py` & `dagger_io-0.6.3/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/src/dagger/codegen.py` & `dagger_io-0.6.3/dagger/codegen.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import enum
 import functools
+import itertools
 import logging
 import re
 import textwrap
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Iterator
+from dataclasses import InitVar, dataclass, field
 from datetime import date, datetime, time
 from decimal import Decimal
 from functools import partial
 from itertools import chain, groupby
 from keyword import iskeyword
-from operator import attrgetter
+from operator import attrgetter, itemgetter
 from typing import (
-    Any,
     ClassVar,
     Generic,
     ParamSpec,
     Protocol,
     TypeAlias,
     TypeGuard,
     TypeVar,
     cast,
 )
 
-import attrs
 from graphql import (
     GraphQLArgument,
     GraphQLEnumType,
     GraphQLField,
     GraphQLFieldMap,
     GraphQLInputField,
     GraphQLInputFieldMap,
@@ -40,18 +40,22 @@
     GraphQLObjectType,
     GraphQLOutputType,
     GraphQLScalarType,
     GraphQLSchema,
     GraphQLType,
     GraphQLWrappingType,
     Undefined,
+    assert_leaf_type,
+    assert_object_type,
     get_named_type,
     is_leaf_type,
+    is_required_argument,
 )
 from graphql.pyutils import camel_to_snake
+from graphql.type.schema import TypeMap
 
 ACRONYM_RE = re.compile(r"([A-Z\d]+)(?=[A-Z\d]|$)")
 """Pattern for grouping initialisms."""
 
 DEPRECATION_RE = re.compile(r"`([a-zA-Z\d_]+)`")
 """Pattern for extracting replaced references in deprecations."""
 
@@ -60,17 +64,36 @@
 indent = partial(textwrap.indent, prefix=" " * 4)
 wrap = textwrap.wrap
 wrap_indent = partial(wrap, initial_indent=" " * 4, subsequent_indent=" " * 4)
 
 
 T_ParamSpec = ParamSpec("T_ParamSpec")
 
+# These alias types are used to make the code more self-documenting.
 IDName: TypeAlias = str
 TypeName: TypeAlias = str
+FieldName: TypeAlias = str
+PythonName: TypeAlias = str
+OutputTypeFormat: TypeAlias = str
+
 IDMap: TypeAlias = dict[IDName, TypeName]
+IDQueryMap: TypeAlias = dict[IDName, FieldName]
+
+SimpleFieldMap: TypeAlias = dict[FieldName, "SimpleField"]
+SimpleObjectsMap: TypeAlias = dict[TypeName, SimpleFieldMap]
+
+
+def joiner(func: Callable[T_ParamSpec, Iterator[str]]) -> Callable[T_ParamSpec, str]:
+    """Join elements with a new line from an iterator."""
+
+    @functools.wraps(func)
+    def wrapper(*args: T_ParamSpec.args, **kwargs: T_ParamSpec.kwargs) -> str:
+        return "\n".join(func(*args, **kwargs))
+
+    return wrapper
 
 
 class Scalars(enum.Enum):
     ID = str
     Int = int
     String = str  # noqa: PIE796
     Float = float
@@ -84,137 +107,292 @@
     def from_type(cls, t: GraphQLScalarType) -> str:
         try:
             return cls[t.name].value.__name__
         except KeyError:
             return t.name
 
 
-def joiner(func: Callable[T_ParamSpec, Iterator[str]]) -> Callable[T_ParamSpec, str]:
-    """Join elements with a new line from an iterator."""
-
-    @functools.wraps(func)
-    def wrapper(*args: T_ParamSpec.args, **kwargs: T_ParamSpec.kwargs) -> str:
-        return "\n".join(func(*args, **kwargs))
-
-    return wrapper
-
-
-@attrs.define
+@dataclass
 class Context:
     """Shared state during execution."""
 
-    sync: bool = False
+    sync: bool
     """Sync or async client."""
 
-    id_map: IDMap = attrs.Factory(dict)
+    id_map: IDMap
     """Map to convert ids (custom scalars) to corresponding types."""
 
-    remaining: set[str] = attrs.Factory(set)
+    id_query_map: IDQueryMap
+    """Map to convert types to ids."""
+
+    simple_objects_map: SimpleObjectsMap
+    """Map of simple leaf fields for types that are returned in lists."""
+
+    defined: set[str] = field(default_factory=set)
+    """Types that have already been defined."""
+
+    remaining: set[str] = field(default_factory=set)
     """Remaining type names that haven't been defined yet."""
 
+    def process_type(self, name: str):
+        # This is only needed to keep track of remaining types because
+        # of forward references.
+        self.remaining.remove(name)
+        self.defined.add(name)
+
+
+_H = TypeVar("_H", bound=GraphQLNamedType)
+"""Handler generic type"""
+
+
+Predicate: TypeAlias = Callable[..., bool]
+
+
+@dataclass
+class Handler(ABC, Generic[_H]):
+    ctx: Context
+    """Generation execution context."""
+
+    predicate: ClassVar[Predicate] = staticmethod(lambda _: False)
+    """Does this handler render the given type?"""
+
+    def supertype_name(self, _: _H) -> str:
+        return self.__class__.__name__
+
+    def type_name(self, t: _H) -> str:
+        return t.name
+
+    @joiner
+    def render(self, t: _H) -> Iterator[str]:
+        yield ""
+        yield self.render_head(t)
+        yield indent(self.render_body(t))
+        yield ""
+
+    def render_head(self, t: _H) -> str:
+        return f"class {self.type_name(t)}({self.supertype_name(t)}):"
+
+    @joiner
+    def render_body(self, t: _H) -> Iterator[str]:
+        if t.description:
+            yield from wrap(doc(t.description))
+
 
-# TODO: break into class
 @joiner
-def generate(  # noqa: C901
+def generate(
     schema: GraphQLSchema,
     sync: bool = False,  # noqa: FBT001, FBT002
 ) -> Iterator[str]:
     """Code generation main function."""
     yield textwrap.dedent(
         """\
         # Code generated by dagger. DO NOT EDIT.
 
         import warnings
         from collections.abc import Sequence
+        from dataclasses import dataclass
         from typing import Optional
 
-        import attrs
-
         from dagger.api.base import Arg, Enum, Input, Root, Scalar, Type, typecheck
         """,
     )
 
+    # Pre-create handy maps to make handler code simpler.
+    id_map = create_id_map(schema.type_map)
+    id_query_map = create_id_query_map(id_map, schema.type_map)
+    simple_objects_map = create_simple_objects_map(schema.type_map)
+
     # shared state between all handler instances
-    ctx = Context(sync)
+    ctx = Context(
+        sync=sync,
+        id_map=id_map,
+        id_query_map=id_query_map,
+        simple_objects_map=simple_objects_map,
+    )
 
     handlers: tuple[Handler, ...] = (
         Scalar(ctx),
         Enum(ctx),
         Input(ctx),
         Object(ctx),
     )
 
-    # collect object types for all id return types
-    # used to replace custom scalars by objects in inputs
-    for name, t in schema.type_map.items():
-        if is_wrapping_type(t):
-            t = t.of_type  # noqa: PLW2901
-        if not is_object_type(t):
-            continue
-        fields: dict[str, GraphQLField] = t.fields
-        for field_name, f in fields.items():
-            if field_name != "id":
-                continue
-            field_type = f.type
-            if is_wrapping_type(field_type):
-                field_type = field_type.of_type
-            ctx.id_map[field_type.name] = name
-
-    def sort_key(t: GraphQLNamedType) -> tuple[int, str]:
-        for i, handler in enumerate(handlers):
-            if handler.predicate(t):
-                return i, t.name
-        return -1, t.name
-
-    def group_key(t: GraphQLNamedType) -> Handler | None:
-        for handler in handlers:
-            if handler.predicate(t):
-                return handler
-        return None
-
-    def type_name(t: GraphQLNamedType) -> str:
-        if t.name.startswith("_") or (
-            is_scalar_type(t) and not is_custom_scalar_type(t)
-        ):
-            return ""
-        return t.name.replace("Query", "Client")
+    # Split into two iterators to update ctx.remaining.
+    types_n, types_g = itertools.tee(get_grouped_types(handlers, schema.type_map))
 
-    all_types = sorted(schema.type_map.values(), key=sort_key)
-    remaining = {type_name(t) for t in all_types}
-    ctx.remaining = {n for n in remaining if n}
-
-    defined = []
-    for handler, types in groupby(all_types, group_key):
-        for t in types:
-            name = type_name(t)
-            if not handler or not name:
-                ctx.remaining.discard(name)
-                continue
-            yield handler.render(t)
-            defined.append(name)
-            ctx.remaining.discard(name)
+    # Track types that haven't been defined yet, to format as a forward reference.
+    ctx.remaining.update(name for _, name, _ in types_n)
+
+    for handler, type_name, named_type in types_g:
+        yield handler.render(named_type)
+        ctx.process_type(type_name)
 
     yield ""
     yield "__all__ = ["
-    yield from (indent(f'"{name}",') for name in defined)
+    yield from (indent(f"{quote(name)},") for name in sorted(ctx.defined))
     yield "]"
 
 
+def create_id_map(type_map: TypeMap) -> IDMap:
+    """Create a map of id type names to object type names.
+
+    Used to replace custom scalars by objects in inputs.
+    """
+
+    def _iter():
+        for type_name, t in type_map.items():
+            if not is_object_type(t):
+                continue
+            fields: dict[str, GraphQLField] = t.fields
+            for field_name, f in fields.items():
+                if field_name == "id":
+                    field_type = get_named_type(f.type)
+                    yield field_type.name, type_name
+
+    return dict(_iter())
+
+
+def create_id_query_map(id_map: IDMap, type_map: TypeMap) -> IDQueryMap:
+    """Create a map of id type names to Query field names.
+
+    Collects fields under Query that receive an id argument and return
+    an object type that also has an id field that returns the same
+    id type as the Query field argument.
+
+    Example:
+      `Query.directory(id: DirectoryID): Directory` matches
+      `Directory.id(): DirectoryID`
+
+    Used to create a classmethod that returns a Directory instance
+    from a DirectoryID by telling us which field to query for.
+    """
+    root_type = cast(GraphQLObjectType, type_map["Query"])
+    root_fields: dict[str, GraphQLField] = root_type.fields
+
+    def _iter():
+        for field_name, f in root_fields.items():
+            field_type = get_named_type(f.type)
+            id_arg = f.args.get("id")
+            # Ignore fields that have required arguments other than id.
+            if not id_arg or any(
+                is_required_argument(arg)
+                for arg_name, arg in f.args.items()
+                if arg_name != "id"
+            ):
+                continue
+            id_type = get_named_type(id_arg.type)
+            if id_map.get(id_type.name) == field_type.name:
+                yield id_type.name, field_name
+
+    return dict(_iter())
+
+
+@dataclass(slots=True)
+class SimpleField:
+    name: InitVar[str]
+    graphql_type: InitVar[GraphQLLeafType]
+    python_name: str = field(init=False)
+    graphql_name: str = field(init=False)
+    type_format: str = field(init=False)
+
+    def __post_init__(self, name: str, graphql_field: GraphQLLeafType):
+        graphql_field = assert_leaf_type(graphql_field)
+        self.graphql_name = name
+        # Create a private version of the field to avoid name clashes.
+        self.python_name = f"_{format_name(name)}"
+        self.type_format = format_output_type(graphql_field)
+
+    def as_kwarg(self) -> str:
+        return f"{self}={quote(self.graphql_name)}"
+
+    def as_attr(self) -> str:
+        return f"{self}: {self.type_format}"
+
+    def __str__(self) -> str:
+        return self.python_name
+
+
+def create_simple_objects_map(type_map: TypeMap) -> SimpleObjectsMap:
+    """Create a map of object type names that are returned in lists.
+
+    The values are maps of python attribute names to the simple leaf
+    GraphQL fields that they represent.
+
+    This is used to populate object types with pre-selected fields
+    when they are returned in lists because our simple chainable API
+    makes it hard to query a field that comes from a list (i.e., which
+    index in the list to get the result from?).
+    """
+
+    def _leaf_fields(named_type: GraphQLNamedType):
+        # Assertion for type checker. Already guaranteed by get_lists_of_object_types
+        object_type = assert_object_type(named_type)
+        for f_name, f in object_type.fields.items():
+            field_name = str(f_name)
+            # This strips all wrapping (e.g., List, NonNull) from the type.
+            named_field_type = get_named_type(f.type)
+            # Ignore id fields which have special meaning.
+            if field_name != "id" and is_leaf_type(named_field_type):
+                yield field_name, SimpleField(field_name, named_field_type)
+
+    return {
+        named_type.name: dict(_leaf_fields(type_map[named_type.name]))
+        for named_type in set(get_lists_of_object_types(type_map))
+    }
+
+
+def get_lists_of_object_types(type_map: TypeMap):
+    """Get object types that are returned in lists."""
+    for t in type_map.values():
+        if t.name.startswith("_") or not is_object_type(t):
+            continue
+        for f in t.fields.values():
+            if is_list_of_objects_type(f.type):
+                yield get_named_type(f.type)
+
+
+def get_grouped_types(handlers: tuple[Handler, ...], type_map: TypeMap):
+    """Group types by handler and sorted by their name."""
+
+    def _filtered():
+        for n, t in type_map.items():
+            if n.startswith("_") or is_builtin_scalar_type(t):
+                continue
+            for i, handler in enumerate(handlers):
+                if handler.predicate(t):
+                    yield i, n
+
+    for _, items in groupby(sorted(_filtered()), itemgetter(0)):
+        for index, name in items:
+            named_type = type_map[name]
+            handler = handlers[index]
+            formatted_name = handler.type_name(named_type)
+            yield handler, formatted_name, named_type
+
+
 # TODO: these typeguards should be contributed upstream
 #        https://github.com/graphql-python/graphql-core/issues/183
 
 
 def is_required_type(t: GraphQLType) -> TypeGuard[GraphQLNonNull]:
     return isinstance(t, GraphQLNonNull)
 
 
 def is_list_type(t: GraphQLType) -> TypeGuard[GraphQLList]:
+    if is_required_type(t):
+        t = t.of_type
     return isinstance(t, GraphQLList)
 
 
+def is_list_of_objects_type(
+    t: GraphQLType,
+) -> TypeGuard[GraphQLList[GraphQLObjectType]]:
+    return is_list_type(t) and is_object_type(get_named_type(t))
+
+
 def is_wrapping_type(t: GraphQLType) -> TypeGuard[GraphQLWrappingType]:
     return isinstance(t, GraphQLWrappingType)
 
 
 def is_scalar_type(t: GraphQLType) -> TypeGuard[GraphQLScalarType]:
     return isinstance(t, GraphQLScalarType)
 
@@ -227,24 +405,29 @@
     return isinstance(t, GraphQLObjectType)
 
 
 def is_output_leaf_type(t: GraphQLOutputType) -> TypeGuard[GraphQLLeafType]:
     return is_leaf_type(get_named_type(t))
 
 
-def is_custom_scalar_type(t: GraphQLNamedType) -> TypeGuard[GraphQLScalarType]:
+def is_custom_scalar_type(t: GraphQLType) -> TypeGuard[GraphQLScalarType]:
     t = get_named_type(t)
     return is_scalar_type(t) and t.name not in Scalars.__members__
 
 
+def is_builtin_scalar_type(t: GraphQLNamedType) -> TypeGuard[GraphQLScalarType]:
+    return is_scalar_type(t) and not is_custom_scalar_type(t)
+
+
 def is_enum_type(t: GraphQLNamedType) -> TypeGuard[GraphQLEnumType]:
     return isinstance(t, GraphQLEnumType)
 
 
 def format_name(s: str) -> str:
+    """Format a GraphQL field or argument name into Python."""
     # rewrite acronyms, initialisms and abbreviations
     s = ACRONYM_RE.sub(lambda m: m.group(0).title(), s)
     s = camel_to_snake(s)
     if iskeyword(s):
         s += "_"
     return s
 
@@ -259,32 +442,24 @@
 
     if is_list_type(t):
         return fmt % f"list[{format_input_type(t.of_type, id_map)}]"
 
     if is_custom_scalar_type(t) and t.name in id_map:
         return fmt % id_map[t.name]
 
-    return fmt % (Scalars.from_type(t) if is_scalar_type(t) else t.name)
+    return fmt % (Scalars.from_type(t) if is_scalar_type(t) else get_named_type(t).name)
 
 
 def format_output_type(t: GraphQLOutputType) -> str:
     """May be used as the output type of an object field."""
-    # only wrap optional and list when ready
-    if is_output_leaf_type(t):
-        return format_input_type(t, {})
-
-    # when building the query return shouldn't be None
-    # even if optional to not break the chain while
-    # we're only building the query
-    # TODO: detect this when returning the scalar
-    #        since it affects the result
-    if is_wrapping_type(t):
-        return format_output_type(t.of_type)
-
-    return Scalars.from_type(t) if is_scalar_type(t) else t.name
+    # When returning objects we're in query building mode, so don't return
+    # None even if the field's return is optional.
+    if not is_output_leaf_type(t) and not is_required_type(t):
+        t = GraphQLNonNull(t)
+    return format_input_type(t, {})
 
 
 def output_type_description(t: GraphQLOutputType) -> str:
     if is_wrapping_type(t):
         return output_type_description(t.of_type)
     if isinstance(t, GraphQLNamedType) and t.description:
         return t.description
@@ -294,14 +469,19 @@
 def doc(s: str) -> str:
     """Wrap string in docstring quotes."""
     if "\n" in s:
         s = f"{s}\n"
     return f'"""{s}"""'
 
 
+def quote(s: str) -> str:
+    """Wrap string in quotes."""
+    return f'"{s}"'
+
+
 class _InputField:
     """Input object field or object field argument."""
 
     def __init__(
         self,
         ctx: Context,
         name: str,
@@ -363,15 +543,15 @@
         yield f"{self.name}:"
         if self.description:
             for line in self.description.split("\n"):
                 yield from wrap_indent(line)
 
     def as_arg(self) -> str:
         """As a Arg object for the query builder."""
-        params = [f'"{self.graphql_name}"', self.name]
+        params = [quote(self.graphql_name), self.name]
         if self.has_default:
             # repr uses single quotes for strings, contrary to black
             params.append(repr(self.default_value).replace("'", '"'))
         return f"Arg({', '.join(params)}),"
 
 
 class _ObjectField:
@@ -392,39 +572,53 @@
         self.named_type = get_named_type(field.type)
         self.args = sorted(
             (_InputField(ctx, *args, parent=self) for args in field.args.items()),
             key=attrgetter("has_default"),
         )
         self.description = field.description
 
-        self.is_leaf = is_output_leaf_type(field.type)
         self.is_custom_scalar = is_custom_scalar_type(field.type)
+        self.is_leaf = is_output_leaf_type(field.type)
+        self.is_exec = self.is_leaf
         self.type = format_output_type(field.type).replace("Query", "Client")
-        self.convert_id = False
+        self.parent_name = get_named_type(parent).name
+
+        # If this field returns a list of objects, get the type's fields
+        # for pre-selection.
+        self.sub_select_slots = ()
+        if is_list_of_objects_type(field.type):
+            self.is_exec = True
+            self.sub_select_slots = tuple(
+                ctx.simple_objects_map.get(self.named_type.name, {}).values()
+            )
+
+        # Slot fields are fields that can be prefilled from the result of a list.
+        self.slot_field = self.ctx.simple_objects_map.get(self.parent_name, {}).get(
+            name
+        )
 
-        # TODO: We don't have a simple way to convert any ID to its
-        # corresponding object (in codegen) so for now just return the
-        # current instance. Currently, `sync` is the only field where
-        # the error is what we care about but more could be added later.
+        # Currently, `sync` is the only field where the error is all we
+        # care about but more could be added later.
         # To avoid wasting a result, we return the ID which is a leaf value
         # and triggers execution, but then convert to object in the SDK to
-        # allow continued chaining. For this, we're assuming the returned
-        # ID represents the exact same object but if that changes, we'll
-        # need to adjust.
+        # allow continued chaining.
+        self.convert_id = False
         if (
             name != "id"
             and self.is_leaf
             and self.is_custom_scalar
             and self.named_type.name in ctx.id_map
         ):
             converted = ctx.id_map[self.named_type.name]
-            if get_named_type(parent).name == converted:
+            if self.parent_name == converted:
                 self.type = converted
                 self.convert_id = True
 
+        self.id_query_field = self.ctx.id_query_map.get(self.named_type.name)
+
     @joiner
     def __str__(self) -> Iterator[str]:
         yield from (
             "",
             "@typecheck",
             self.func_signature(),
             indent(self.func_body()),
@@ -435,21 +629,38 @@
         if not self.ctx.sync and self.is_leaf and self.name == "sync":
             yield from (
                 "",
                 "def __await__(self):",
                 indent("return self.sync().__await__()"),
             )
 
+        if self.name == "id":
+            yield from (
+                "",
+                "@classmethod",
+                "def _id_type(cls) -> type[Scalar]:",
+                indent(f"return {self.type}"),
+            )
+            if self.id_query_field:
+                yield from (
+                    "",
+                    "@classmethod",
+                    "def _from_id_query_field(cls):",
+                    indent(f'return "{self.id_query_field}"'),
+                )
+
     def func_signature(self) -> str:
         params = ", ".join(chain(("self",), (a.as_param() for a in self.args)))
         # arbitrary heuristic to force trailing comma in long signatures
         if len(params) > 40:  # noqa: PLR2004
             params = f"{params},"
-        prefix = "" if self.ctx.sync or not self.is_leaf else "async "
-        sig = f"{prefix}def {self.name}({params}) -> {self.type}:"
+        sig = f"def {self.name}({params}) -> {self.type}:"
+        if self.is_exec and not self.ctx.sync:
+            sig = f"async {sig}"
+        # Add quotes around types that haven't been defined yet (forward references).
         if self.ctx.remaining:
             sig = re.sub(rf"\b({'|'.join(self.ctx.remaining)})\b", r'"\1"', sig)
         return sig
 
     @joiner
     def func_body(self) -> Iterator[str]:
         if docstring := self.func_doc():
@@ -463,29 +674,42 @@
                 warnings.warn(
                     "{msg}",
                     DeprecationWarning,
                     stacklevel=4,
                 )\
                 """)
 
+        if self.slot_field:
+            yield f'if hasattr(self, "{self.slot_field.python_name}"):'
+            yield indent(f"return self.{self.slot_field.python_name}")
+
         if not self.args:
             yield "_args: list[Arg] = []"
         else:
             yield "_args = ["
             yield from (indent(arg.as_arg()) for arg in self.args)
             yield "]"
 
         yield f'_ctx = self._select("{self.graphql_name}", _args)'
 
-        if self.is_leaf:
+        if self.is_exec:
             exec_ = "_ctx.execute_sync" if self.ctx.sync else "await _ctx.execute"
             if self.convert_id:
-                yield f"{exec_}()"
-                yield "return self"
+                if _field := self.id_query_field:
+                    yield f"_id = {exec_}({self.named_type.name})"
+                    yield f'_ctx = self._root_select("{_field}", [Arg("id", _id)])'
+                    yield f"return {self.type}(_ctx)"
+                else:
+                    yield f"{exec_}()"
+                    yield "return self"
             else:
+                if slots := self.sub_select_slots:
+                    target = self.named_type.name
+                    kwargs = ", ".join(s.as_kwarg() for s in slots)
+                    yield f"_ctx = {target}(_ctx)._select_multiple({kwargs},)"
                 yield f"return {exec_}({self.type})"
         else:
             yield f"return {self.type}(_ctx)"
 
     def func_doc(self) -> str:
         def _out():
             if self.description:
@@ -551,65 +775,26 @@
         return (
             DEPRECATION_RE.sub(_format_name, reason)
             if (reason := self.graphql.deprecation_reason)
             else ""
         )
 
 
-_H = TypeVar("_H", bound=GraphQLNamedType)
-"""Handler generic type"""
-
-
-class Predicate(Protocol):
-    def __call__(self, _: Any) -> bool:
-        ...
-
-
-@attrs.define
-class Handler(ABC, Generic[_H]):
-    ctx: Context
-    """Generation execution context."""
-
-    predicate: ClassVar[Predicate] = staticmethod(lambda _: False)
-    """Does this handler render the given type?"""
-
-    @joiner
-    def render(self, t: _H) -> Iterator[str]:
-        yield ""
-        yield self.render_head(t)
-        yield indent(self.render_body(t))
-        yield ""
-
-    def render_head(self, t: _H) -> str:
-        return f"class {t.name}(Type):"
-
-    @joiner
-    def render_body(self, t: _H) -> Iterator[str]:
-        if t.description:
-            yield from wrap(doc(t.description))
-
-
-@attrs.define
+@dataclass
 class Scalar(Handler[GraphQLScalarType]):
     predicate: ClassVar[Predicate] = staticmethod(is_custom_scalar_type)
 
-    def render_head(self, t: GraphQLScalarType) -> str:
-        return super().render_head(t).replace("Type", "Scalar")
-
     def render_body(self, t: GraphQLScalarType) -> str:
         return super().render_body(t) or "..."
 
 
-@attrs.define
+@dataclass
 class Enum(Handler[GraphQLEnumType]):
     predicate: ClassVar[Predicate] = staticmethod(is_enum_type)
 
-    def render_head(self, t: GraphQLEnumType) -> str:
-        return super().render_head(t).replace("Type", "Enum")
-
     @joiner
     def render_body(self, t: GraphQLEnumType) -> Iterator[str]:
         if body := super().render_body(t):
             yield body
 
         for name, value in sorted(t.values.items()):
             yield ""
@@ -641,39 +826,49 @@
     def fields(self, t: _O) -> Iterator[_F]:
         ...
 
     @joiner
     def render_body(self, t: _O) -> Iterator[str]:
         if body := super().render_body(t):
             yield body
+
+        if slots := self.ctx.simple_objects_map.get(t.name):
+            yield ""
+            yield f"__slots__ = ({', '.join(quote(str(s)) for s in slots.values())},)"
+            yield ""
+            yield from (s.as_attr() for s in slots.values())
+
         yield from (
             str(field)
-            # sorting by graphql name rather than pytnon name for
-            # consistency with other SDKs
+            # Sorting by graphql name rather than python name for
+            # consistency with other SDKs.
             for field in sorted(self.fields(t), key=attrgetter("graphql_name"))
         )
 
 
 class Input(ObjectHandler[GraphQLInputObjectType]):
     predicate: ClassVar[Predicate] = staticmethod(is_input_object_type)
 
     def render_head(self, t: GraphQLInputObjectType) -> str:
-        return f"@attrs.define\nclass {t.name}(Input):"
+        return f"@dataclass(slots=True)\n{super().render_head(t)}"
 
     def fields(self, t: GraphQLInputObjectType) -> Iterator[_InputField]:
         return (
             _InputField(self.ctx, *args)
             for args in cast(GraphQLInputFieldMap, t.fields).items()
         )
 
 
 class Object(ObjectHandler[GraphQLObjectType]):
     predicate: ClassVar[Predicate] = staticmethod(is_object_type)
 
-    def render_head(self, t: GraphQLObjectType) -> str:
-        return super().render_head(t).replace("Query(Type)", "Client(Root)")
+    def supertype_name(self, t: GraphQLObjectType) -> str:
+        return "Root" if t.name == "Query" else "Type"
+
+    def type_name(self, t: GraphQLObjectType) -> str:
+        return super().type_name(t).replace("Query", "Client")
 
     def fields(self, t: GraphQLObjectType) -> Iterator[_ObjectField]:
         return (
             _ObjectField(self.ctx, *args, t)
             for args in cast(GraphQLFieldMap, t.fields).items()
         )
```

### Comparing `dagger_io-0.6.2/src/dagger/connection.py` & `dagger_io-0.6.3/dagger/connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/src/dagger/engine/cli.py` & `dagger_io-0.6.3/dagger/engine/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,14 @@
+import json
 import logging
 import subprocess
 import time
 from importlib import metadata
-from json.decoder import JSONDecodeError
 from pathlib import Path
 
-import cattrs
-from cattrs.preconf.json import JsonConverter
-
 import dagger
 from dagger.config import ConnectParams
 from dagger.context import SyncResourceManager
 from dagger.exceptions import SessionError
 
 logger = logging.getLogger(__name__)
 
@@ -29,15 +26,14 @@
 class CLISession(SyncResourceManager):
     """Start an engine session with a provided CLI path."""
 
     def __init__(self, cfg: dagger.Config, path: str) -> None:
         super().__init__()
         self.cfg = cfg
         self.path = path
-        self.converter = JsonConverter()
         # no constructor param intentional
         self.is_async = True
 
     def __enter__(self) -> ConnectParams:
         with self.get_sync_stack() as stack:
             try:
                 proc = self._start()
@@ -90,14 +86,15 @@
                 return proc
 
         msg = "CLI busy"
         raise SessionError(msg)
 
     def _get_conn(self, proc: subprocess.Popen) -> ConnectParams:
         # TODO: implement engine session timeout (self.cfg.engine_timeout?)
+        assert proc.stdout
         conn = proc.stdout.readline()
 
         # Check if subprocess exited with an error
         if ret := proc.poll():
             out = conn + proc.stdout.read()
             err = proc.stderr.read() if proc.stderr and proc.stderr.readable() else None
 
@@ -113,11 +110,11 @@
             raise SessionError(msg)
 
         if not conn:
             msg = "No connection params"
             raise SessionError(msg)
 
         try:
-            return self.converter.loads(conn, ConnectParams)
-        except (JSONDecodeError, cattrs.BaseValidationError) as e:
+            return ConnectParams(**json.loads(conn))
+        except (ValueError, TypeError) as e:
             msg = f"Invalid connection params: {conn}"
             raise SessionError(msg) from e
```

### Comparing `dagger_io-0.6.2/src/dagger/engine/conn.py` & `dagger_io-0.6.3/dagger/engine/conn.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,22 @@
     def from_env(self) -> ConnectParams | None:
         if not (port := os.environ.get("DAGGER_SESSION_PORT")):
             return None
         if not (token := os.environ.get("DAGGER_SESSION_TOKEN")):
             msg = "DAGGER_SESSION_TOKEN must be set when using DAGGER_SESSION_PORT"
             raise ProvisionError(msg)
         try:
-            return ConnectParams(port, token)
+            return ConnectParams(port=int(port), session_token=token)
         except ValueError as e:
             # only port is validated
             msg = f"Invalid DAGGER_SESSION_PORT: {port}"
             raise ProvisionError(msg) from e
 
     def from_cli(self) -> ConnectParams:
-        cli_bin = os.environ.get("_EXPERIMENTAL_DAGGER_CLI_BIN")
-        if not cli_bin:
-            cli_bin = Downloader().get()
+        cli_bin = os.environ.get("_EXPERIMENTAL_DAGGER_CLI_BIN") or Downloader().get()
         cli_session = CLISession(self.cfg, cli_bin)
         cli_session.is_async = self.is_async
         with self.get_sync_stack() as stack:
             return stack.enter_context(cli_session)
 
     def start(self) -> ConnectParams:
         return self.from_env() or self.from_cli()
```

### Comparing `dagger_io-0.6.2/src/dagger/engine/download.py` & `dagger_io-0.6.3/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/src/dagger/exceptions.py` & `dagger_io-0.6.3/dagger/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from dataclasses import dataclass, field
 from typing import Any
 
-import attrs
 import cattrs
 import graphql
 from gql.transport.exceptions import TransportQueryError
 
 
 class DaggerError(Exception):
     """Base exception for all Dagger exceptions."""
@@ -50,30 +50,30 @@
     """Timeout while executing a query."""
 
 
 class InvalidQueryError(ClientError):
     """Misuse of the query builder."""
 
 
-@attrs.define
+@dataclass
 class QueryErrorLocation:
     """Error location returned by the API."""
 
     line: int
     column: int
 
 
-@attrs.define
+@dataclass
 class QueryErrorValue:
     """Error value returned by the API."""
 
     message: str
     locations: list[QueryErrorLocation]
     path: list[str]
-    extensions: dict[str, Any] = attrs.Factory(dict)
+    extensions: dict[str, Any] = field(default_factory=dict)
 
     def __str__(self) -> str:
         return self.message
 
 
 class QueryError(ClientError):
     """The server returned an error for a specific query."""
```

### Comparing `dagger_io-0.6.2/src/dagger/session.py` & `dagger_io-0.6.3/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/src/dagger/transport/httpx.py` & `dagger_io-0.6.3/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.2/PKG-INFO` & `dagger_io-0.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.6.2
+Version: 0.6.3
 Summary: A client package for running Dagger pipelines in Python.
-Home-page: https://dagger.io
-License: Apache-2.0
-Author: Dagger
-Author-email: hello@dagger.io
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://dagger.io
+Project-URL: Documentation, https://docs.dagger.io/sdk/python
+Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
+Project-URL: Tracker, https://github.com/dagger/dagger/issues
+Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
+Project-URL: Community, https://discord.gg/ufnyBtc8uY
+Project-URL: Twitter, https://twitter.com/dagger_io
+Author-email: Dagger <hello@dagger.io>
+License-Expression: Apache-2.0
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AnyIO
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
+Requires-Python: >=3.10
+Requires-Dist: anyio>=3.6.2
+Requires-Dist: beartype>=0.11.0
+Requires-Dist: cattrs>=22.2.0
+Requires-Dist: gql>=3.4.0
+Requires-Dist: graphql-core>=3.2.3
+Requires-Dist: httpx>=0.23.1
+Requires-Dist: platformdirs>=2.6.2
+Requires-Dist: typing-extensions>=4.4.0
+Provides-Extra: cli
+Requires-Dist: typer[all]>=0.6.1; extra == 'cli'
 Provides-Extra: server
-Requires-Dist: anyio (>=3.6.2)
-Requires-Dist: attrs (>=22.1.0)
-Requires-Dist: beartype (>=0.11.0)
-Requires-Dist: cattrs (>=22.2.0)
-Requires-Dist: gql (>=3.4.0)
-Requires-Dist: graphql-core (>=3.2.3)
-Requires-Dist: httpx (>=0.23.1)
-Requires-Dist: platformdirs (>=2.6.2)
-Requires-Dist: rich (>=12.6.0)
-Requires-Dist: strawberry-graphql (>=0.133.5) ; extra == "server"
-Requires-Dist: typer[all] (>=0.6.1)
-Requires-Dist: typing_extensions (>=4.4.0)
-Project-URL: Community, https://discord.gg/ufnyBtc8uY
-Project-URL: Documentation, https://docs.dagger.io/sdk/python
-Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
-Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
-Project-URL: Tracker, https://github.com/dagger/dagger/issues
-Project-URL: Twitter, https://twitter.com/dagger_io
+Requires-Dist: strawberry-graphql>=0.187.0; extra == 'server'
+Requires-Dist: typer[all]>=0.6.1; extra == 'server'
 Description-Content-Type: text/markdown
 
 # Dagger Python SDK
 
 [![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)
@@ -136,47 +137,42 @@
 
 - [Documentation](https://docs.dagger.io/sdk/python)
 - [API Reference](https://dagger-io.readthedocs.org)
 - [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)
 
 ## Development
 
-This library is maintained with [Poetry](https://python-poetry.org/docs/).
-
-If you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:
-
-```shell
-poetry install
-```
+This library is maintained with [Hatch](https://hatch.pypa.io/).
 
 The following commands are available:
-- `poe test`: Run tests.
-- `poe fmt`: Re-format code following common styling conventions.
-- `poe lint`: Check for linting violations.
-- `poe generate`: Regenerate API client after changes to the codegen.
-- `poe docs`: Build reference docs locally (needs `poetry install --with docs`).
+- `hatch run test`: Run tests.
+- `hatch run fmt`: Re-format code following common styling conventions.
+- `hatch run lint`: Check for linting violations.
+- `hatch run generate`: Regenerate API client after changes to the codegen.
+- `hatch run typing:check`: Run the type checker.
+- `hatch run docs:build`: Build reference docs locally (check with `(cd docs/_build && python -m http.server)`).
 
 ### Engine changes
 
 Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
 
 The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
 
 ```shell
-../../hack/make sdk:python:test
 ../../hack/make sdk:python:generate
+../../hack/make sdk:python:lint
+../../hack/make sdk:python:test
 ```
 
 You can also build the CLI and use it directly within the Python SDK:
 
 ```shell
-../../hack/dev poe test
+../../hack/dev hatch test
 ```
 
 Or build it separately and tell the SDK to use it directly (or any other CLI binary):
 
 ```shell
 ../../hack/make
-_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test
+_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger hatch test
 ```
 
-
```

