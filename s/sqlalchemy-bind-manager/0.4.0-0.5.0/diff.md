# Comparing `tmp/sqlalchemy_bind_manager-0.4.0.tar.gz` & `tmp/sqlalchemy_bind_manager-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_bind_manager-0.4.0.tar", max compression
+gzip compressed data, was "sqlalchemy_bind_manager-0.5.0.tar", max compression
```

## Comparing `sqlalchemy_bind_manager-0.4.0.tar` & `sqlalchemy_bind_manager-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-07-03 22:38:35.648099 sqlalchemy_bind_manager-0.4.0/LICENSE
--rw-r--r--   0        0        0     8733 2023-07-03 22:38:35.648099 sqlalchemy_bind_manager-0.4.0/README.md
--rw-r--r--   0        0        0     2375 2023-07-03 22:38:47.900125 sqlalchemy_bind_manager-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/__init__.py
--rw-r--r--   0        0        0     5241 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_bind_manager.py
--rw-r--r--   0        0        0      197 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/__init__.py
--rw-r--r--   0        0        0     6084 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/async_.py
--rw-r--r--   0        0        0    11340 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/base_repository.py
--rw-r--r--   0        0        0     1099 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/common.py
--rw-r--r--   0        0        0     7429 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/result_presenters.py
--rw-r--r--   0        0        0     5380 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/sync.py
--rw-r--r--   0        0        0     3229 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_transaction_handler.py
--rw-r--r--   0        0        0     1722 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
--rw-r--r--   0        0        0      310 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/exceptions.py
--rw-r--r--   0        0        0    11155 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/protocols.py
--rw-r--r--   0        0        0        0 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/py.typed
--rw-r--r--   0        0        0      242 2023-07-03 22:38:35.652099 sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/repository.py
--rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/LICENSE
+-rw-r--r--   0        0        0     8733 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/README.md
+-rw-r--r--   0        0        0     2375 2023-07-05 11:29:12.981766 sqlalchemy_bind_manager-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/__init__.py
+-rw-r--r--   0        0        0     5241 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_bind_manager.py
+-rw-r--r--   0        0        0      197 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/__init__.py
+-rw-r--r--   0        0        0     6080 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/async_.py
+-rw-r--r--   0        0        0    11340 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/base_repository.py
+-rw-r--r--   0        0        0     1099 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/common.py
+-rw-r--r--   0        0        0     7429 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/result_presenters.py
+-rw-r--r--   0        0        0     5376 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/sync.py
+-rw-r--r--   0        0        0     3118 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_session_handler.py
+-rw-r--r--   0        0        0     1704 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py
+-rw-r--r--   0        0        0      310 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/exceptions.py
+-rw-r--r--   0        0        0    11155 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/protocols.py
+-rw-r--r--   0        0        0        0 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/py.typed
+-rw-r--r--   0        0        0      242 2023-07-05 11:28:57.377510 sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/repository.py
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 sqlalchemy_bind_manager-0.5.0/PKG-INFO
```

### Comparing `sqlalchemy_bind_manager-0.4.0/LICENSE` & `sqlalchemy_bind_manager-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/README.md` & `sqlalchemy_bind_manager-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/pyproject.toml` & `sqlalchemy_bind_manager-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlalchemy-bind-manager"
-version = "0.4.0"
+version = "0.5.0"
 description = "A manager to easily handle multiple SQLAlchemy configurations"
 license = "MIT"
 authors = ["Federico Busetti <729029+febus982@users.noreply.github.com>"]
 repository = "https://github.com/febus982/sqlalchemy-bind-manager"
 homepage = "https://febus982.github.io/sqlalchemy-bind-manager"
 readme = "README.md"
 packages = [{include = "sqlalchemy_bind_manager"}]
```

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_bind_manager.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_bind_manager.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/async_.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/async_.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Union,
 )
 
 from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 
 from .._bind_manager import SQLAlchemyAsyncBind
-from .._transaction_handler import AsyncSessionHandler
+from .._session_handler import AsyncSessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
 )
 from .common import (
     MODEL,
     PRIMARY_KEY,
```

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/base_repository.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/base_repository.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/common.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/common.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/result_presenters.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/result_presenters.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_repository/sync.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_repository/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Union,
 )
 
 from sqlalchemy import select
 from sqlalchemy.orm import Session
 
 from .._bind_manager import SQLAlchemyBind
-from .._transaction_handler import SessionHandler
+from .._session_handler import SessionHandler
 from ..exceptions import InvalidConfig, ModelNotFound
 from .base_repository import (
     BaseRepository,
 )
 from .common import (
     MODEL,
     PRIMARY_KEY,
```

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_transaction_handler.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_session_handler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import asyncio
 from contextlib import asynccontextmanager, contextmanager
 from typing import AsyncIterator, Iterator
-from uuid import uuid4
 
 from sqlalchemy.ext.asyncio import (
     AsyncSession,
     async_scoped_session,
 )
 from sqlalchemy.orm import Session, scoped_session
 
@@ -13,95 +12,91 @@
     SQLAlchemyAsyncBind,
     SQLAlchemyBind,
 )
 from sqlalchemy_bind_manager.exceptions import UnsupportedBind
 
 
 class SessionHandler:
-    _session_class: scoped_session
-    session: Session
+    scoped_session: scoped_session
 
     def __init__(self, bind: SQLAlchemyBind):
         if not isinstance(bind, SQLAlchemyBind):
             raise UnsupportedBind("Bind is not an instance of SQLAlchemyBind")
         else:
-            u = uuid4()
-            self._session_class = scoped_session(
-                bind.session_class, scopefunc=lambda: str(u)
-            )
-            self.session = self._session_class()
+            self.scoped_session = scoped_session(bind.session_class)
 
     def __del__(self):
-        if getattr(self, "_session_class", None):
-            self._session_class.remove()
+        if getattr(self, "scoped_session", None):
+            self.scoped_session.remove()
 
     @contextmanager
     def get_session(self, read_only: bool = False) -> Iterator[Session]:
+        session = self.scoped_session()
         try:
-            self.session.begin()
-            yield self.session
+            session.begin()
+            yield session
             if not read_only:
-                self.commit()
+                self.commit(session)
         finally:
-            self.session.close()
+            session.close()
 
-    def commit(self) -> None:
+    def commit(self, session: Session) -> None:
         """Commits the session and handles rollback on errors.
 
+        :param session: The session object.
+        :type session: Session
         :raises Exception: Any error is re-raised after the rollback.
         """
         try:
-            self.session.commit()
+            session.commit()
         except:
-            self.session.rollback()
+            session.rollback()
             raise
 
 
 class AsyncSessionHandler:
-    _session_class: async_scoped_session
-    session: AsyncSession
+    scoped_session: async_scoped_session
 
     def __init__(self, bind: SQLAlchemyAsyncBind):
         if not isinstance(bind, SQLAlchemyAsyncBind):
             raise UnsupportedBind("Bind is not an instance of SQLAlchemyAsyncBind")
         else:
-            u = uuid4()
-            self._session_class = async_scoped_session(
-                bind.session_class, scopefunc=lambda: str(u)
+            self.scoped_session = async_scoped_session(
+                bind.session_class, asyncio.current_task
             )
-            self.session = self._session_class()
 
     def __del__(self):
-        if not getattr(self, "_session_class", None):
+        if not getattr(self, "scoped_session", None):
             return
 
         try:
             loop = asyncio.get_event_loop()
             if loop.is_running():
-                loop.create_task(self._session_class.remove())
+                loop.create_task(self.scoped_session.remove())
             else:
-                loop.run_until_complete(self._session_class.remove())
+                loop.run_until_complete(self.scoped_session.remove())
         except RuntimeError:
-            asyncio.run(self._session_class.remove())
+            asyncio.run(self.scoped_session.remove())
 
     @asynccontextmanager
     async def get_session(self, read_only: bool = False) -> AsyncIterator[AsyncSession]:
+        session = self.scoped_session()
         try:
-            await self.session.begin()
-            yield self.session
+            await session.begin()
+            yield session
             if not read_only:
-                await self.commit()
+                await self.commit(session)
         finally:
-            await self.session.close()
+            await session.close()
 
-    async def commit(self) -> None:
+    async def commit(self, session: AsyncSession) -> None:
         """Commits the session and handles rollback on errors.
 
         :param session: The session object.
-        :type session: Session
+        :type session: AsyncSession
         :raises Exception: Any error is re-raised after the rollback.
         """
         try:
-            await self.session.commit()
+            await session.commit()
         except:
-            await self.session.rollback()
+            await session.rollback()
             raise
```

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/_unit_of_work/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from contextlib import asynccontextmanager, contextmanager
 from typing import AsyncIterator, Iterable, Iterator, Type
 
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.orm import Session
 
 from sqlalchemy_bind_manager._bind_manager import SQLAlchemyAsyncBind, SQLAlchemyBind
-from sqlalchemy_bind_manager._transaction_handler import (
+from sqlalchemy_bind_manager._session_handler import (
     AsyncSessionHandler,
     SessionHandler,
 )
 from sqlalchemy_bind_manager.repository import (
     SQLAlchemyAsyncRepository,
     SQLAlchemyRepository,
 )
 
 
 class UnitOfWork:
-    _transaction_handler: SessionHandler
+    _session_handler: SessionHandler
 
     def __init__(
         self, bind: SQLAlchemyBind, repositories: Iterable[Type[SQLAlchemyRepository]]
     ) -> None:
         super().__init__()
-        self._transaction_handler = SessionHandler(bind)
+        self._session_handler = SessionHandler(bind)
         for r in repositories:
-            setattr(self, r.__name__, r(session=self._transaction_handler.session))
+            setattr(self, r.__name__, r(session=self._session_handler.scoped_session()))
 
     @contextmanager
     def transaction(self, read_only: bool = False) -> Iterator[Session]:
-        with self._transaction_handler.get_session(read_only=read_only) as _s:
+        with self._session_handler.get_session(read_only=read_only) as _s:
             yield _s
 
 
 class AsyncUnitOfWork:
-    _transaction_handler: AsyncSessionHandler
+    _session_handler: AsyncSessionHandler
 
     def __init__(
         self,
         bind: SQLAlchemyAsyncBind,
         repositories: Iterable[Type[SQLAlchemyAsyncRepository]],
     ) -> None:
         super().__init__()
-        self._transaction_handler = AsyncSessionHandler(bind)
+        self._session_handler = AsyncSessionHandler(bind)
         for r in repositories:
-            setattr(self, r.__name__, r(session=self._transaction_handler.session))
+            setattr(self, r.__name__, r(session=self._session_handler.scoped_session()))
 
     @asynccontextmanager
     async def transaction(self, read_only: bool = False) -> AsyncIterator[AsyncSession]:
-        async with self._transaction_handler.get_session(read_only=read_only) as _s:
+        async with self._session_handler.get_session(read_only=read_only) as _s:
             yield _s
```

### Comparing `sqlalchemy_bind_manager-0.4.0/sqlalchemy_bind_manager/protocols.py` & `sqlalchemy_bind_manager-0.5.0/sqlalchemy_bind_manager/protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_bind_manager-0.4.0/PKG-INFO` & `sqlalchemy_bind_manager-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-bind-manager
-Version: 0.4.0
+Version: 0.5.0
 Summary: A manager to easily handle multiple SQLAlchemy configurations
 Home-page: https://febus982.github.io/sqlalchemy-bind-manager
 License: MIT
 Keywords: sqlalchemy,config,manager
 Author: Federico Busetti
 Author-email: 729029+febus982@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
```

