# Comparing `tmp/z3c.sqlalchemy-2.0.tar.gz` & `tmp/z3c.sqlalchemy-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.sqlalchemy-2.0.tar", last modified: Wed Mar  1 06:28:11 2023, max compression
+gzip compressed data, was "z3c.sqlalchemy-2.1.tar", last modified: Wed Jul  5 06:17:07 2023, max compression
```

## Comparing `z3c.sqlalchemy-2.0.tar` & `z3c.sqlalchemy-2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.328993 z3c.sqlalchemy-2.0/
--rw-r--r--   0 mac        (513) staff       (20)    10444 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      196 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)    18681 2023-03-01 06:28:11.329152 z3c.sqlalchemy-2.0/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     6953 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/README.rst
--rw-r--r--   0 mac        (513) staff       (20)      103 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/buildout.cfg
--rw-r--r--   0 mac        (513) staff       (20)      423 2023-03-01 06:28:11.329957 z3c.sqlalchemy-2.0/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     2581 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.319532 z3c.sqlalchemy-2.0/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.323413 z3c.sqlalchemy-2.0/src/z3c/
--rw-r--r--   0 mac        (513) staff       (20)       76 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.328068 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/
--rw-r--r--   0 mac        (513) staff       (20)      600 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     5175 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/base.py
--rw-r--r--   0 mac        (513) staff       (20)     3534 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/interfaces.py
--rw-r--r--   0 mac        (513) staff       (20)     8220 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/mapper.py
--rw-r--r--   0 mac        (513) staff       (20)     4146 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/model.py
--rw-r--r--   0 mac        (513) staff       (20)     2347 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/postgres.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.328718 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/tests/
--rw-r--r--   0 mac        (513) staff       (20)      361 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/tests/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     7856 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py
--rw-r--r--   0 mac        (513) staff       (20)     4834 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/util.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-03-01 06:28:11.325805 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)    18681 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      724 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)      128 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        4 2023-03-01 06:28:11.000000 z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1423 2023-03-01 06:28:10.000000 z3c.sqlalchemy-2.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.064067 z3c.sqlalchemy-2.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    10550 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      196 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18542 2023-07-05 06:17:07.064281 z3c.sqlalchemy-2.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6708 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      103 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/buildout.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)      423 2023-07-05 06:17:07.065108 z3c.sqlalchemy-2.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2579 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.046912 z3c.sqlalchemy-2.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.049586 z3c.sqlalchemy-2.1/src/z3c/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.061664 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      600 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5201 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/base.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3534 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/interfaces.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8322 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/mapper.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4146 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/model.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2347 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/postgres.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.063370 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      361 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     7908 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4834 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/util.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-05 06:17:07.055662 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    18542 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      724 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      126 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        4 2023-07-05 06:17:07.000000 z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1423 2023-07-05 06:17:06.000000 z3c.sqlalchemy-2.1/tox.ini
```

### Comparing `z3c.sqlalchemy-2.0/CHANGES.rst` & `z3c.sqlalchemy-2.1/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,57 @@
 Change log
 ==========
 
+2.1 (2023-07-05)
+----------------
+
+- Support ``SQLAlchemy >= 2.0``.
+  (`#15 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/15>`_)
+
+
 2.0 (2023-03-01)
 ----------------
 
-  - Add support for Python 3.10, 3.11.
+- Add support for Python 3.10, 3.11.
 
-  - Drop support for Python 2.7, 3.5, 3.6.
+- Drop support for Python 2.7, 3.5, 3.6.
 
 
 1.5.2 (2020-11-13)
 ------------------
 
-- fix ``MANIFEST`` to include the change log
+- Fix ``MANIFEST`` to include the change log.
 
 
 1.5.1 (2020-11-13)
 ------------------
 
-- add linting to ``tox`` configuration and apply linting fixes
+- Add linting to ``tox`` configuration and apply linting fixes.
 
-- fixed installation error in setup.py (release 1.5.0 is broken)
+- Fix installation error in setup.py (release 1.5.0 is broken).
 
 
 1.5.0 (2020-11-13)
 ------------------
 
-- add support for Python 3.5-3.9
+- Add support for Python 3.5-3.9.
+
+- Standardize namespace __init__.
 
-- Standardize namespace __init__
+- Fix to work with zope.sqlalchemy 1.2.
 
-- Fix to work with zope.sqlalchemy 1.2
 
 1.4.0 (2009-12-02)
 ------------------
 
-- removed compatibility code with older Zope versions
+- Remove compatibility code with older Zope versions.
 
-- fixed import issue with modern zope.component versions
+- Fix import issue with modern zope.component versions.
 
-- fixed registering of custom mappers
+- Fix registering of custom mappers.
 
 1.3.11 (26.10.2009)
 -------------------
 
 - Don't create a new MetaData in LazyMapperCollection,
   but use the one created in the wrapper.
   In some cases, you could have some tables in the metadata created in the wrapper,
@@ -148,56 +156,56 @@
 -------------------
 
   - the SessionDataManager now supports ZODB savepoints
 
 1.1.0 (17.01.2008)
 -------------------
 
-  - WARNING: this version requires SA 0.4.X and higher 
+  - WARNING: this version requires SA 0.4.X and higher
 
   - fixed import issues with the upcoming SA 0.4.X series
 
   - create_session() calls (for SA 0.4.X)
 
   - the unittests support an optional $TEST_DSN environment in order
     to run the test against an existing database (other than SQLite)
-               
+
   - major overhoul of the Zope transaction integration: now using
-    one DataManager for the session object and the connection. The 
+    one DataManager for the session object and the connection. The
     connection as returned through the 'connection' property is also
     used for creating a new 'session'. Older z3c.sqlalchemy version
     used separate connections. This allows applications to use both
     a session and a connection within the same Zope request/thread
     without running into transaction problems. SQL actions and
     session related modifications should happen within the same
     transaction.
 
-  - Wrapper constructor now accepts two new optional dicts 
-    'engine_options' and 'session_options' that will be passed down 
-    to the engine and the sessionmaker.  Patch provided by 
+  - Wrapper constructor now accepts two new optional dicts
+    'engine_options' and 'session_options' that will be passed down
+    to the engine and the sessionmaker.  Patch provided by
     Klaus Barthelmann.
 
-  - mapped objects now provide a method asDict() to return the values 
+  - mapped objects now provide a method asDict() to return the values
     of an objects as dict.
 
- 
+
 1.0.11 (30.07.2007)
 -------------------
 
   - replaced BoundMetaData() with MetaData() (requires SA 0.3.9+)
 
   - removed zope.* dependencies in order to avoid zope.* version
     mismatches for now
 
 
 1.0.10 (16.07.2007)
 -------------------
 
-  - using Zope 3.3.X as a fixed depenceny 
- 
+  - using Zope 3.3.X as a fixed depenceny
+
 
 1.0.9 (08.07.2007)
 ------------------
 
   - added namespace declarations
 
   - reST-ified documentation
@@ -261,15 +269,15 @@
    - more checks in Model.add()
 
 
 1.0.0 (05.05.2007)
 ------------------
 
    - source code polishing
-   
+
    - documentation update
 
 
 0.1.13 (05.05.2007)
 -------------------
 
    - sessions were returned from the wrong cache
@@ -289,15 +297,15 @@
 0.1.11 (02.05.2007)
 -------------------
 
    - added check for the 'mapper_class' attribute (classes from now
      on must be a subclass of MapperClassBase)
 
    - a Zope-aware SAWrapper now has a 'connection' property that can
-     be used to execute SQL statements directly. 'connection' is an 
+     be used to execute SQL statements directly. 'connection' is an
      instance of sqlalchemy.Connection and directly tied to the current
      Zope transaction.
 
    - changed the caching of the connection and session object for Zope wrapper
      since the id of a transaction is not reliable (different transaction
      object can re-use the same memory address leading to cache errors)
 
@@ -320,27 +328,27 @@
 0.1.9 (26.04.2007)
 ------------------
 
    - base.py: the 'model' parameter can now also be a callable
      returning an instance of model.Model
 
    - base.py: calling a model provider or a method providing a
-     model with a BoundMetaData instance in order to allow 
+     model with a BoundMetaData instance in order to allow
      table auto-loading
 
    - Model.add() got a new parameter 'primary_key' in order to specify a
      primary_key hint. This is useful when you are trying to auto-load a view
      as Table() having no primary key information. The 'primary_key' parameter is
      either None or a sequence of column names.
 
 
 0.1.8 (23.04.2007)
 ------------------
 
-   - added shorter method names as aliases 
+   - added shorter method names as aliases
 
    - don't generate a new mapper class if a custom mapper
      class is defined within the model
 
 
 0.1.7 (21.04.2007)
 ------------------
@@ -351,38 +359,38 @@
      passed directly to create_engine()
 
    - fixed the documentation a bit
 
    - added registerMapper() to BaseWrapper class
 
    - registerSQLAlchemyWrapper() now defers the registration until
-     the Wrapper is used first when calling getSQLAlchemyWrapper() 
+     the Wrapper is used first when calling getSQLAlchemyWrapper()
 
    - the 'name' parameter of Model.add() now supports schemas (if
      available). E.g. when using Postgres you can reference as
      table within a different schema through '<schema>.<tablename>'.
 
    - Model.add() accepts a new optional parameter 'table_name' that
      can be used to specify the name of a table (including schema
      information) when you want to use the 'name' parameter as
      an alias for the related table/mapper.
 
- 
+
 0.1.6 (28.03.2007)
 ------------------
 
    - fixed a bug in registerSQLAlchemyWrapper
 
 0.1.5 (28.03.2007)
 ------------------
-  
+
    - registerSQLAlchemyWrapper() should now work with Zope 2.8-2.10
 
    - abort() was defined twice inside the DataManager class
- 
+
 0.1.4 (21.03.2007)
 ------------------
 
    - the Model class now behave (where needed) as a sorted
      dictionary. Its items() method must returned all items
      in insertion order.
```

### Comparing `z3c.sqlalchemy-2.0/CONTRIBUTING.md` & `z3c.sqlalchemy-2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/LICENSE.txt` & `z3c.sqlalchemy-2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/PKG-INFO` & `z3c.sqlalchemy-2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.sqlalchemy
-Version: 2.0
+Version: 2.1
 Summary: A SQLAlchemy wrapper for Zope
 Home-page: https://github.com/zopefoundation/z3c.sqlalchemy
 Author: Andreas Jung
 Author-email: info@zopyx.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zope-dev@zope.dev
 License: ZPL 2.1
@@ -41,61 +41,58 @@
 z3c.sqlalchemy is yet another wrapper around SQLAlchemy. The functionality of
 the wrapper is basically focused on easy integration with Zope.
 The wrapper cares about connection handling, optional transaction integration
 with Zope and wrapper management (caching, introspection). z3c.sqlalchemy
 gives you flexible control over the mapper creation. Mapper classes can be
 
 - auto-generated (with or without autodetection of table relationships)
-- configured by the developer 
+- configured by the developer
 
 
 What z3c.sqlalchemy does not do and won't do:
 =============================================
 
-- no support for Zope 3 schemas 
+- no support for Zope 3 schemas
 - no support for Archetypes schemas
 
 z3c.sqlachemy just tries to provide you with the basic functionalities you need
 to write SQLAlchemy-based applications with Zope. Higher-level
 functionalities like integration with Archetypes/Zope 3 schemas are subject to
 higher-level frameworks.  z3c.sqlalchemy does not address these frameworks.
 
 
 Requirements:
 =============
 
-- Zope 4+
-- SQLAlchemy 0.5.5 or higher
+- Zope 5 or higher
+- SQLAlchemy 1.4 or higher
 - zope.sqlalchemy 1.2.0 or higher
-- Python 2.7 or 3.5-3.9
+- Python 3.7 or higher
 
 
 Installation:
 =============
 
-Either using easy_install::
+Using pip::
 
-  easy_install z3c.sqlalchemy
+  pip install z3c.sqlalchemy
 
-or using Python directly::
-
-  python2.7 setup.py install
 
 Note:
 -----
 z3c.sqlalchemy depends on the modules **zope.component**, **zope.schema**
 and **zope.interface**. If you are using z3c.sqlalchemy in a Python-only
 environment, ensure the these components have to be installed either
 as eggs or by setting the PYTHONPATH to a corresponding Zope installation.
 
 
 Usage
 =====
 
-Basic usage:: 
+Basic usage::
 
    from z3c.sqlalchemy import createSAWrapper
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB')
    session = wrapper.session
    FormatMapper = wrapper.getMapper('format') # auto-generated mapper for table 'format'
    for row in session.query(FormatMapper).select(...): print row
    session.flush() # if necessary
@@ -106,15 +103,15 @@
 same transaction and same thread.
 
 For a real-world application you don't want to create a new wrapper for every
 new request.  Instead you want to register a wrapper instance as named utility
 (ISQLAlchemyWrapper) and lookup up the wrapper (the utility!) by name from
 within your application. This approach is very similiar to looking up an
 databases adapter or a ZSQL method through acquisition.
-   
+
 By default "wrapper.getMapper(name)" will always auto-generate a new mapper
 class by using SQLAlchemy auto-load feature. The drawback of this approach is
 that the mapper class does not know about relationships to other tables. Assume
 we have a one-to-many relationship between table A and B and you want
 z3c.sqlalchemy to generate a mapper that is aware of this relationship. For
 this purpose you can create a wrapper with a "model" as optional parameter. A
 model is basically a configuration or a series of hints in order to tell
@@ -122,15 +119,15 @@
 
 Example::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', relations=('B',))
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 This will generate a mapper AMapper where all instances of AMapper have a
 property 'B' that relates to all corresponding rows in B (see the SQLAlchemy
 documentation on mappers, properties and relation()). In this example you
 define the relationship between A and B explictly through the 'relations'
 parameter (as a sequence of related table names).
 
@@ -139,15 +136,15 @@
 way. Therefore this feature of z3c.sqlalchemy is highly experimental and currently
 only available for Postgres (tested with Postgres 8.X).::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', autodetect_relations=True)
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 In this case z3c.sqlalchemy will scan all tables in order to detect
 relationships automatically and build the mapper class and its properties
 according to the found relationships. Warning: this feature is experimental and
 it might take some time to scan all tables before the first request. Currently
 only Postgres tables in the 'public' schema are supported).
 
@@ -198,81 +195,78 @@
 z3c.sqlalchemy was written by Andreas Jung for Haufe Mediengruppe, Freiburg, Germany
 and ZOPYX Ltd. & Co. KG, Tuebingen, Germany.
 
 
 License
 =======
 
-z3c.sqlalchemy is licensed under the Zope Public License 2.1. 
+z3c.sqlalchemy is licensed under the Zope Public License 2.1.
 
 See LICENSE.txt.
 
 
-Contact
-=======
-
-| ZOPYX Ltd. & Co. KG
-| Andreas Jung
-| Charlottenstr. 37/1
-| D-72070 Tuebingen, Germany 
-| E-mail: info at zopyx dot com
-| Web: http://www.zopyx.com
-
-
 Credits
 =======
 
 Parts of the code are influenced by z3c.zalchemy (Juergen Kartnaller, Michael
 Bernstein & others) and Alchemist/ore.alchemist (Kapil Thangavelu). Thanks to
 Martin Aspeli for giving valuable feedback.
 
 
 
 Change log
 ==========
 
+2.1 (2023-07-05)
+----------------
+
+- Support ``SQLAlchemy >= 2.0``.
+  (`#15 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/15>`_)
+
+
 2.0 (2023-03-01)
 ----------------
 
-  - Add support for Python 3.10, 3.11.
+- Add support for Python 3.10, 3.11.
 
-  - Drop support for Python 2.7, 3.5, 3.6.
+- Drop support for Python 2.7, 3.5, 3.6.
 
 
 1.5.2 (2020-11-13)
 ------------------
 
-- fix ``MANIFEST`` to include the change log
+- Fix ``MANIFEST`` to include the change log.
 
 
 1.5.1 (2020-11-13)
 ------------------
 
-- add linting to ``tox`` configuration and apply linting fixes
+- Add linting to ``tox`` configuration and apply linting fixes.
 
-- fixed installation error in setup.py (release 1.5.0 is broken)
+- Fix installation error in setup.py (release 1.5.0 is broken).
 
 
 1.5.0 (2020-11-13)
 ------------------
 
-- add support for Python 3.5-3.9
+- Add support for Python 3.5-3.9.
+
+- Standardize namespace __init__.
 
-- Standardize namespace __init__
+- Fix to work with zope.sqlalchemy 1.2.
 
-- Fix to work with zope.sqlalchemy 1.2
 
 1.4.0 (2009-12-02)
 ------------------
 
-- removed compatibility code with older Zope versions
+- Remove compatibility code with older Zope versions.
 
-- fixed import issue with modern zope.component versions
+- Fix import issue with modern zope.component versions.
 
-- fixed registering of custom mappers
+- Fix registering of custom mappers.
 
 1.3.11 (26.10.2009)
 -------------------
 
 - Don't create a new MetaData in LazyMapperCollection,
   but use the one created in the wrapper.
   In some cases, you could have some tables in the metadata created in the wrapper,
@@ -377,56 +371,56 @@
 -------------------
 
   - the SessionDataManager now supports ZODB savepoints
 
 1.1.0 (17.01.2008)
 -------------------
 
-  - WARNING: this version requires SA 0.4.X and higher 
+  - WARNING: this version requires SA 0.4.X and higher
 
   - fixed import issues with the upcoming SA 0.4.X series
 
   - create_session() calls (for SA 0.4.X)
 
   - the unittests support an optional $TEST_DSN environment in order
     to run the test against an existing database (other than SQLite)
-               
+
   - major overhoul of the Zope transaction integration: now using
-    one DataManager for the session object and the connection. The 
+    one DataManager for the session object and the connection. The
     connection as returned through the 'connection' property is also
     used for creating a new 'session'. Older z3c.sqlalchemy version
     used separate connections. This allows applications to use both
     a session and a connection within the same Zope request/thread
     without running into transaction problems. SQL actions and
     session related modifications should happen within the same
     transaction.
 
-  - Wrapper constructor now accepts two new optional dicts 
-    'engine_options' and 'session_options' that will be passed down 
-    to the engine and the sessionmaker.  Patch provided by 
+  - Wrapper constructor now accepts two new optional dicts
+    'engine_options' and 'session_options' that will be passed down
+    to the engine and the sessionmaker.  Patch provided by
     Klaus Barthelmann.
 
-  - mapped objects now provide a method asDict() to return the values 
+  - mapped objects now provide a method asDict() to return the values
     of an objects as dict.
 
- 
+
 1.0.11 (30.07.2007)
 -------------------
 
   - replaced BoundMetaData() with MetaData() (requires SA 0.3.9+)
 
   - removed zope.* dependencies in order to avoid zope.* version
     mismatches for now
 
 
 1.0.10 (16.07.2007)
 -------------------
 
-  - using Zope 3.3.X as a fixed depenceny 
- 
+  - using Zope 3.3.X as a fixed depenceny
+
 
 1.0.9 (08.07.2007)
 ------------------
 
   - added namespace declarations
 
   - reST-ified documentation
@@ -490,15 +484,15 @@
    - more checks in Model.add()
 
 
 1.0.0 (05.05.2007)
 ------------------
 
    - source code polishing
-   
+
    - documentation update
 
 
 0.1.13 (05.05.2007)
 -------------------
 
    - sessions were returned from the wrong cache
@@ -518,15 +512,15 @@
 0.1.11 (02.05.2007)
 -------------------
 
    - added check for the 'mapper_class' attribute (classes from now
      on must be a subclass of MapperClassBase)
 
    - a Zope-aware SAWrapper now has a 'connection' property that can
-     be used to execute SQL statements directly. 'connection' is an 
+     be used to execute SQL statements directly. 'connection' is an
      instance of sqlalchemy.Connection and directly tied to the current
      Zope transaction.
 
    - changed the caching of the connection and session object for Zope wrapper
      since the id of a transaction is not reliable (different transaction
      object can re-use the same memory address leading to cache errors)
 
@@ -549,27 +543,27 @@
 0.1.9 (26.04.2007)
 ------------------
 
    - base.py: the 'model' parameter can now also be a callable
      returning an instance of model.Model
 
    - base.py: calling a model provider or a method providing a
-     model with a BoundMetaData instance in order to allow 
+     model with a BoundMetaData instance in order to allow
      table auto-loading
 
    - Model.add() got a new parameter 'primary_key' in order to specify a
      primary_key hint. This is useful when you are trying to auto-load a view
      as Table() having no primary key information. The 'primary_key' parameter is
      either None or a sequence of column names.
 
 
 0.1.8 (23.04.2007)
 ------------------
 
-   - added shorter method names as aliases 
+   - added shorter method names as aliases
 
    - don't generate a new mapper class if a custom mapper
      class is defined within the model
 
 
 0.1.7 (21.04.2007)
 ------------------
@@ -580,38 +574,38 @@
      passed directly to create_engine()
 
    - fixed the documentation a bit
 
    - added registerMapper() to BaseWrapper class
 
    - registerSQLAlchemyWrapper() now defers the registration until
-     the Wrapper is used first when calling getSQLAlchemyWrapper() 
+     the Wrapper is used first when calling getSQLAlchemyWrapper()
 
    - the 'name' parameter of Model.add() now supports schemas (if
      available). E.g. when using Postgres you can reference as
      table within a different schema through '<schema>.<tablename>'.
 
    - Model.add() accepts a new optional parameter 'table_name' that
      can be used to specify the name of a table (including schema
      information) when you want to use the 'name' parameter as
      an alias for the related table/mapper.
 
- 
+
 0.1.6 (28.03.2007)
 ------------------
 
    - fixed a bug in registerSQLAlchemyWrapper
 
 0.1.5 (28.03.2007)
 ------------------
-  
+
    - registerSQLAlchemyWrapper() should now work with Zope 2.8-2.10
 
    - abort() was defined twice inside the DataManager class
- 
+
 0.1.4 (21.03.2007)
 ------------------
 
    - the Model class now behave (where needed) as a sorted
      dictionary. Its items() method must returned all items
      in insertion order.
```

### Comparing `z3c.sqlalchemy-2.0/README.rst` & `z3c.sqlalchemy-2.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,61 +9,58 @@
 z3c.sqlalchemy is yet another wrapper around SQLAlchemy. The functionality of
 the wrapper is basically focused on easy integration with Zope.
 The wrapper cares about connection handling, optional transaction integration
 with Zope and wrapper management (caching, introspection). z3c.sqlalchemy
 gives you flexible control over the mapper creation. Mapper classes can be
 
 - auto-generated (with or without autodetection of table relationships)
-- configured by the developer 
+- configured by the developer
 
 
 What z3c.sqlalchemy does not do and won't do:
 =============================================
 
-- no support for Zope 3 schemas 
+- no support for Zope 3 schemas
 - no support for Archetypes schemas
 
 z3c.sqlachemy just tries to provide you with the basic functionalities you need
 to write SQLAlchemy-based applications with Zope. Higher-level
 functionalities like integration with Archetypes/Zope 3 schemas are subject to
 higher-level frameworks.  z3c.sqlalchemy does not address these frameworks.
 
 
 Requirements:
 =============
 
-- Zope 4+
-- SQLAlchemy 0.5.5 or higher
+- Zope 5 or higher
+- SQLAlchemy 1.4 or higher
 - zope.sqlalchemy 1.2.0 or higher
-- Python 2.7 or 3.5-3.9
+- Python 3.7 or higher
 
 
 Installation:
 =============
 
-Either using easy_install::
+Using pip::
 
-  easy_install z3c.sqlalchemy
+  pip install z3c.sqlalchemy
 
-or using Python directly::
-
-  python2.7 setup.py install
 
 Note:
 -----
 z3c.sqlalchemy depends on the modules **zope.component**, **zope.schema**
 and **zope.interface**. If you are using z3c.sqlalchemy in a Python-only
 environment, ensure the these components have to be installed either
 as eggs or by setting the PYTHONPATH to a corresponding Zope installation.
 
 
 Usage
 =====
 
-Basic usage:: 
+Basic usage::
 
    from z3c.sqlalchemy import createSAWrapper
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB')
    session = wrapper.session
    FormatMapper = wrapper.getMapper('format') # auto-generated mapper for table 'format'
    for row in session.query(FormatMapper).select(...): print row
    session.flush() # if necessary
@@ -74,15 +71,15 @@
 same transaction and same thread.
 
 For a real-world application you don't want to create a new wrapper for every
 new request.  Instead you want to register a wrapper instance as named utility
 (ISQLAlchemyWrapper) and lookup up the wrapper (the utility!) by name from
 within your application. This approach is very similiar to looking up an
 databases adapter or a ZSQL method through acquisition.
-   
+
 By default "wrapper.getMapper(name)" will always auto-generate a new mapper
 class by using SQLAlchemy auto-load feature. The drawback of this approach is
 that the mapper class does not know about relationships to other tables. Assume
 we have a one-to-many relationship between table A and B and you want
 z3c.sqlalchemy to generate a mapper that is aware of this relationship. For
 this purpose you can create a wrapper with a "model" as optional parameter. A
 model is basically a configuration or a series of hints in order to tell
@@ -90,15 +87,15 @@
 
 Example::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', relations=('B',))
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 This will generate a mapper AMapper where all instances of AMapper have a
 property 'B' that relates to all corresponding rows in B (see the SQLAlchemy
 documentation on mappers, properties and relation()). In this example you
 define the relationship between A and B explictly through the 'relations'
 parameter (as a sequence of related table names).
 
@@ -107,15 +104,15 @@
 way. Therefore this feature of z3c.sqlalchemy is highly experimental and currently
 only available for Postgres (tested with Postgres 8.X).::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', autodetect_relations=True)
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 In this case z3c.sqlalchemy will scan all tables in order to detect
 relationships automatically and build the mapper class and its properties
 according to the found relationships. Warning: this feature is experimental and
 it might take some time to scan all tables before the first request. Currently
 only Postgres tables in the 'public' schema are supported).
 
@@ -166,30 +163,19 @@
 z3c.sqlalchemy was written by Andreas Jung for Haufe Mediengruppe, Freiburg, Germany
 and ZOPYX Ltd. & Co. KG, Tuebingen, Germany.
 
 
 License
 =======
 
-z3c.sqlalchemy is licensed under the Zope Public License 2.1. 
+z3c.sqlalchemy is licensed under the Zope Public License 2.1.
 
 See LICENSE.txt.
 
 
-Contact
-=======
-
-| ZOPYX Ltd. & Co. KG
-| Andreas Jung
-| Charlottenstr. 37/1
-| D-72070 Tuebingen, Germany 
-| E-mail: info at zopyx dot com
-| Web: http://www.zopyx.com
-
-
 Credits
 =======
 
 Parts of the code are influenced by z3c.zalchemy (Juergen Kartnaller, Michael
 Bernstein & others) and Alchemist/ore.alchemist (Kapil Thangavelu). Thanks to
 Martin Aspeli for giving valuable feedback.
```

### Comparing `z3c.sqlalchemy-2.0/setup.py` & `z3c.sqlalchemy-2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def _read_file(filename):
     with open(os.path.join(HERE, filename)) as f:
         return f.read()
 
 
 README = _read_file('README.rst')
 CHANGES = _read_file('CHANGES.rst')
-version = '2.0'
+version = '2.1'
 
 
 setup(name='z3c.sqlalchemy',
       version=version,
       url='https://github.com/zopefoundation/z3c.sqlalchemy',
       project_urls={
           'Issue Tracker': ('https://github.com/zopefoundation/'
@@ -62,15 +62,15 @@
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       namespace_packages=['z3c'],
       python_requires='>=3.7',
       install_requires=[
           'setuptools',
-          'SQLAlchemy>=0.5.5',
+          'SQLAlchemy>=1.4',
           'zope.sqlalchemy>=1.2.0',
           'zope.component',
           'zope.interface',
           'zope.testing',
           'zope.schema',
       ],
       extras_require=dict(test=['zope.testing']))
```

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/__init__.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/base.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,21 +92,21 @@
         # mappers must be initialized at last since we need to acces
         # the 'model' from within the constructor of LazyMapperCollection
         self._mappers = LazyMapperCollection(self)
 
     @property
     def metadata(self):
         if not hasattr(self, '_v_metadata'):
-            self._v_metadata = MetaData(self._engine)
+            self._v_metadata = MetaData()
         return self._v_metadata
 
     @property
     def session(self):
         """ Return thread-local session """
-        return self._sessionmaker()
+        return self._session
 
     @property
     def connection(self):
         """ Return underlying connection """
         session = self.session
         # Return the ConnectionFairy
         return session.connection().connection
@@ -136,7 +136,8 @@
         self._engine = create_engine(self.dsn, **self.engine_options)
         self._sessionmaker = scoped_session(sessionmaker(bind=self._engine,
                                             autocommit=not self.transactional,
                                             twophase=self.twophase,
                                             autoflush=True,
                                             **self.session_options))
         register(self._sessionmaker)
+        self._session = self._sessionmaker()
```

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/interfaces.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/mapper.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 """
 
 import threading
 
 from sqlalchemy import Table
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy.orm import class_mapper
-from sqlalchemy.orm import mapper
-from sqlalchemy.orm import relation
+from sqlalchemy.orm import registry
+from sqlalchemy.orm import relationship
 
 
 marker = object
 
 
 class Proxy(dict):
     """ Dict-Proxy for mapped objects providing
@@ -108,16 +108,15 @@
         """
 
         if cls is None:
             newCls = type('_mapped_%s' % str(table.name),
                           (MappedClassBase,), {})
         else:
             newCls = cls
-
-        mapper(newCls, table, properties=properties)
+        registry().map_imperatively(newCls, table, properties=properties)
         return newCls
 
 
 class LazyMapperCollection(dict):
     """ Implements a cache for table mappers """
 
     def __init__(self, wrapper):
@@ -159,15 +158,15 @@
                     schema, tablename = table_name.split('.')
                 else:
                     tablename, schema = table_name, None
 
                 table = Table(tablename,
                               self._metadata,
                               schema=schema,
-                              autoload=True)
+                              autoload_with=self._engine)
 
             # check if the model contains an optional mapper class
             mapper_class = None
             if name in self._model:
                 mapper_class = self._model[name].get('mapper_class')
 
             # use auto-introspected table dependencies for creating
@@ -205,16 +204,19 @@
             # find all dependent tables (referencing the current table)
             for table_refname in dependent_table_names:
                 # create or get a mapper for the referencing table
                 table_ref_mapper = self.getMapper(table_refname)
 
                 # add the mapper as relation to the properties dict
                 properties[table_refname] = (
-                    relation(table_ref_mapper,
-                             cascade=self._model.get(name, {}).get('cascade')))
+                    relationship(
+                        table_ref_mapper,
+                        cascade=self._model.get(name, {}).get('cascade'),
+                    )
+                )
 
             # create a mapper and cache it
             if mapper_class and 'c' in mapper_class.__dict__:
                 mapper = mapper_class
             else:
                 mapper = self._mapper_factory(table,
                                               properties=properties,
```

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/model.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/model.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/postgres.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/postgres.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/tests/test_SQLAlchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import sqlalchemy.orm
 from sqlalchemy import Column
 from sqlalchemy import Integer
 from sqlalchemy import MetaData
 from sqlalchemy import String
 from sqlalchemy import Table
 from sqlalchemy import exc
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 from zope.interface.verify import verifyClass
 
 from z3c.sqlalchemy import Model
 from z3c.sqlalchemy import createSAWrapper
 from z3c.sqlalchemy import getSAWrapper
 from z3c.sqlalchemy import registerSAWrapper
 from z3c.sqlalchemy.interfaces import IModel
@@ -42,26 +42,26 @@
 
         self.dsn = os.environ.get('TEST_DSN')
         self.tempfile = None
         if not self.dsn:
             self.tempfile = tempfile.mktemp()
             self.dsn = 'sqlite:///%s' % self.tempfile
         self.db = wrapper = createSAWrapper(self.dsn)
-        metadata = MetaData(bind=wrapper.engine)
+        metadata = MetaData()
 
         Table('users', metadata,
               Column('id', Integer, primary_key=True),
               Column('firstname', String(255)),
               Column('lastname', String(255)))
 
         Table('skills', metadata,
               Column('user_id', Integer, primary_key=True),
               Column('name', String(255)))
 
-        metadata.create_all()
+        metadata.create_all(bind=wrapper.engine)
 
     def tearDown(self):
         if self.tempfile:
             os.remove(self.tempfile)
         else:
             metadata = MetaData(bind=self.db.engine)
             metadata.drop_all()
@@ -110,15 +110,16 @@
         mytable = Table(
             'mytable', self.db.metadata,
             Column('id', Integer, primary_key=True),
         )
 
         class MyClass:
             pass
-        mapper = sqlalchemy.orm.mapper(MyClass, mytable)
+        registry = sqlalchemy.orm.registry()
+        mapper = registry.map_imperatively(MyClass, mytable)
         self.db.registerMapper(mapper, 'mymapper')
 
 #    def testCustomMapperClassWithWrongType(self):
 #
 #        class myUser(object):
 #            pass
 #
@@ -230,15 +231,15 @@
             class Foo(Base):
                 __tablename__ = 'foo'
 
                 id = Column('id', Integer, primary_key=True)
                 name = Column('name', String(50))
 
             model.add('foo', mapper_class=Foo)
-            Base.metadata.create_all()
+            Base.metadata.create_all(self.db._engine)
             return model
 
         db = createSAWrapper(self.dsn, model=getModel)
         session = db.session
         Foo = db.getMapper('foo')
 
         session.add(Foo(id=1, name='Andreas Jung'))
```

### Comparing `z3c.sqlalchemy-2.0/src/z3c/sqlalchemy/util.py` & `z3c.sqlalchemy-2.1/src/z3c/sqlalchemy/util.py`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/PKG-INFO` & `z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.sqlalchemy
-Version: 2.0
+Version: 2.1
 Summary: A SQLAlchemy wrapper for Zope
 Home-page: https://github.com/zopefoundation/z3c.sqlalchemy
 Author: Andreas Jung
 Author-email: info@zopyx.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zope-dev@zope.dev
 License: ZPL 2.1
@@ -41,61 +41,58 @@
 z3c.sqlalchemy is yet another wrapper around SQLAlchemy. The functionality of
 the wrapper is basically focused on easy integration with Zope.
 The wrapper cares about connection handling, optional transaction integration
 with Zope and wrapper management (caching, introspection). z3c.sqlalchemy
 gives you flexible control over the mapper creation. Mapper classes can be
 
 - auto-generated (with or without autodetection of table relationships)
-- configured by the developer 
+- configured by the developer
 
 
 What z3c.sqlalchemy does not do and won't do:
 =============================================
 
-- no support for Zope 3 schemas 
+- no support for Zope 3 schemas
 - no support for Archetypes schemas
 
 z3c.sqlachemy just tries to provide you with the basic functionalities you need
 to write SQLAlchemy-based applications with Zope. Higher-level
 functionalities like integration with Archetypes/Zope 3 schemas are subject to
 higher-level frameworks.  z3c.sqlalchemy does not address these frameworks.
 
 
 Requirements:
 =============
 
-- Zope 4+
-- SQLAlchemy 0.5.5 or higher
+- Zope 5 or higher
+- SQLAlchemy 1.4 or higher
 - zope.sqlalchemy 1.2.0 or higher
-- Python 2.7 or 3.5-3.9
+- Python 3.7 or higher
 
 
 Installation:
 =============
 
-Either using easy_install::
+Using pip::
 
-  easy_install z3c.sqlalchemy
+  pip install z3c.sqlalchemy
 
-or using Python directly::
-
-  python2.7 setup.py install
 
 Note:
 -----
 z3c.sqlalchemy depends on the modules **zope.component**, **zope.schema**
 and **zope.interface**. If you are using z3c.sqlalchemy in a Python-only
 environment, ensure the these components have to be installed either
 as eggs or by setting the PYTHONPATH to a corresponding Zope installation.
 
 
 Usage
 =====
 
-Basic usage:: 
+Basic usage::
 
    from z3c.sqlalchemy import createSAWrapper
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB')
    session = wrapper.session
    FormatMapper = wrapper.getMapper('format') # auto-generated mapper for table 'format'
    for row in session.query(FormatMapper).select(...): print row
    session.flush() # if necessary
@@ -106,15 +103,15 @@
 same transaction and same thread.
 
 For a real-world application you don't want to create a new wrapper for every
 new request.  Instead you want to register a wrapper instance as named utility
 (ISQLAlchemyWrapper) and lookup up the wrapper (the utility!) by name from
 within your application. This approach is very similiar to looking up an
 databases adapter or a ZSQL method through acquisition.
-   
+
 By default "wrapper.getMapper(name)" will always auto-generate a new mapper
 class by using SQLAlchemy auto-load feature. The drawback of this approach is
 that the mapper class does not know about relationships to other tables. Assume
 we have a one-to-many relationship between table A and B and you want
 z3c.sqlalchemy to generate a mapper that is aware of this relationship. For
 this purpose you can create a wrapper with a "model" as optional parameter. A
 model is basically a configuration or a series of hints in order to tell
@@ -122,15 +119,15 @@
 
 Example::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', relations=('B',))
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 This will generate a mapper AMapper where all instances of AMapper have a
 property 'B' that relates to all corresponding rows in B (see the SQLAlchemy
 documentation on mappers, properties and relation()). In this example you
 define the relationship between A and B explictly through the 'relations'
 parameter (as a sequence of related table names).
 
@@ -139,15 +136,15 @@
 way. Therefore this feature of z3c.sqlalchemy is highly experimental and currently
 only available for Postgres (tested with Postgres 8.X).::
 
    from z3c.sqlalchemy import createSAWrapper, Model
    model = Model()
    model.add(name='A', autodetect_relations=True)
    wrapper = createSAWrapper('postgres://postgres:postgres@host/someDB', model=model)
-   AMapper= wrapper.getMapper('A') 
+   AMapper= wrapper.getMapper('A')
 
 In this case z3c.sqlalchemy will scan all tables in order to detect
 relationships automatically and build the mapper class and its properties
 according to the found relationships. Warning: this feature is experimental and
 it might take some time to scan all tables before the first request. Currently
 only Postgres tables in the 'public' schema are supported).
 
@@ -198,81 +195,78 @@
 z3c.sqlalchemy was written by Andreas Jung for Haufe Mediengruppe, Freiburg, Germany
 and ZOPYX Ltd. & Co. KG, Tuebingen, Germany.
 
 
 License
 =======
 
-z3c.sqlalchemy is licensed under the Zope Public License 2.1. 
+z3c.sqlalchemy is licensed under the Zope Public License 2.1.
 
 See LICENSE.txt.
 
 
-Contact
-=======
-
-| ZOPYX Ltd. & Co. KG
-| Andreas Jung
-| Charlottenstr. 37/1
-| D-72070 Tuebingen, Germany 
-| E-mail: info at zopyx dot com
-| Web: http://www.zopyx.com
-
-
 Credits
 =======
 
 Parts of the code are influenced by z3c.zalchemy (Juergen Kartnaller, Michael
 Bernstein & others) and Alchemist/ore.alchemist (Kapil Thangavelu). Thanks to
 Martin Aspeli for giving valuable feedback.
 
 
 
 Change log
 ==========
 
+2.1 (2023-07-05)
+----------------
+
+- Support ``SQLAlchemy >= 2.0``.
+  (`#15 <https://github.com/zopefoundation/z3c.sqlalchemy/issues/15>`_)
+
+
 2.0 (2023-03-01)
 ----------------
 
-  - Add support for Python 3.10, 3.11.
+- Add support for Python 3.10, 3.11.
 
-  - Drop support for Python 2.7, 3.5, 3.6.
+- Drop support for Python 2.7, 3.5, 3.6.
 
 
 1.5.2 (2020-11-13)
 ------------------
 
-- fix ``MANIFEST`` to include the change log
+- Fix ``MANIFEST`` to include the change log.
 
 
 1.5.1 (2020-11-13)
 ------------------
 
-- add linting to ``tox`` configuration and apply linting fixes
+- Add linting to ``tox`` configuration and apply linting fixes.
 
-- fixed installation error in setup.py (release 1.5.0 is broken)
+- Fix installation error in setup.py (release 1.5.0 is broken).
 
 
 1.5.0 (2020-11-13)
 ------------------
 
-- add support for Python 3.5-3.9
+- Add support for Python 3.5-3.9.
+
+- Standardize namespace __init__.
 
-- Standardize namespace __init__
+- Fix to work with zope.sqlalchemy 1.2.
 
-- Fix to work with zope.sqlalchemy 1.2
 
 1.4.0 (2009-12-02)
 ------------------
 
-- removed compatibility code with older Zope versions
+- Remove compatibility code with older Zope versions.
 
-- fixed import issue with modern zope.component versions
+- Fix import issue with modern zope.component versions.
 
-- fixed registering of custom mappers
+- Fix registering of custom mappers.
 
 1.3.11 (26.10.2009)
 -------------------
 
 - Don't create a new MetaData in LazyMapperCollection,
   but use the one created in the wrapper.
   In some cases, you could have some tables in the metadata created in the wrapper,
@@ -377,56 +371,56 @@
 -------------------
 
   - the SessionDataManager now supports ZODB savepoints
 
 1.1.0 (17.01.2008)
 -------------------
 
-  - WARNING: this version requires SA 0.4.X and higher 
+  - WARNING: this version requires SA 0.4.X and higher
 
   - fixed import issues with the upcoming SA 0.4.X series
 
   - create_session() calls (for SA 0.4.X)
 
   - the unittests support an optional $TEST_DSN environment in order
     to run the test against an existing database (other than SQLite)
-               
+
   - major overhoul of the Zope transaction integration: now using
-    one DataManager for the session object and the connection. The 
+    one DataManager for the session object and the connection. The
     connection as returned through the 'connection' property is also
     used for creating a new 'session'. Older z3c.sqlalchemy version
     used separate connections. This allows applications to use both
     a session and a connection within the same Zope request/thread
     without running into transaction problems. SQL actions and
     session related modifications should happen within the same
     transaction.
 
-  - Wrapper constructor now accepts two new optional dicts 
-    'engine_options' and 'session_options' that will be passed down 
-    to the engine and the sessionmaker.  Patch provided by 
+  - Wrapper constructor now accepts two new optional dicts
+    'engine_options' and 'session_options' that will be passed down
+    to the engine and the sessionmaker.  Patch provided by
     Klaus Barthelmann.
 
-  - mapped objects now provide a method asDict() to return the values 
+  - mapped objects now provide a method asDict() to return the values
     of an objects as dict.
 
- 
+
 1.0.11 (30.07.2007)
 -------------------
 
   - replaced BoundMetaData() with MetaData() (requires SA 0.3.9+)
 
   - removed zope.* dependencies in order to avoid zope.* version
     mismatches for now
 
 
 1.0.10 (16.07.2007)
 -------------------
 
-  - using Zope 3.3.X as a fixed depenceny 
- 
+  - using Zope 3.3.X as a fixed depenceny
+
 
 1.0.9 (08.07.2007)
 ------------------
 
   - added namespace declarations
 
   - reST-ified documentation
@@ -490,15 +484,15 @@
    - more checks in Model.add()
 
 
 1.0.0 (05.05.2007)
 ------------------
 
    - source code polishing
-   
+
    - documentation update
 
 
 0.1.13 (05.05.2007)
 -------------------
 
    - sessions were returned from the wrong cache
@@ -518,15 +512,15 @@
 0.1.11 (02.05.2007)
 -------------------
 
    - added check for the 'mapper_class' attribute (classes from now
      on must be a subclass of MapperClassBase)
 
    - a Zope-aware SAWrapper now has a 'connection' property that can
-     be used to execute SQL statements directly. 'connection' is an 
+     be used to execute SQL statements directly. 'connection' is an
      instance of sqlalchemy.Connection and directly tied to the current
      Zope transaction.
 
    - changed the caching of the connection and session object for Zope wrapper
      since the id of a transaction is not reliable (different transaction
      object can re-use the same memory address leading to cache errors)
 
@@ -549,27 +543,27 @@
 0.1.9 (26.04.2007)
 ------------------
 
    - base.py: the 'model' parameter can now also be a callable
      returning an instance of model.Model
 
    - base.py: calling a model provider or a method providing a
-     model with a BoundMetaData instance in order to allow 
+     model with a BoundMetaData instance in order to allow
      table auto-loading
 
    - Model.add() got a new parameter 'primary_key' in order to specify a
      primary_key hint. This is useful when you are trying to auto-load a view
      as Table() having no primary key information. The 'primary_key' parameter is
      either None or a sequence of column names.
 
 
 0.1.8 (23.04.2007)
 ------------------
 
-   - added shorter method names as aliases 
+   - added shorter method names as aliases
 
    - don't generate a new mapper class if a custom mapper
      class is defined within the model
 
 
 0.1.7 (21.04.2007)
 ------------------
@@ -580,38 +574,38 @@
      passed directly to create_engine()
 
    - fixed the documentation a bit
 
    - added registerMapper() to BaseWrapper class
 
    - registerSQLAlchemyWrapper() now defers the registration until
-     the Wrapper is used first when calling getSQLAlchemyWrapper() 
+     the Wrapper is used first when calling getSQLAlchemyWrapper()
 
    - the 'name' parameter of Model.add() now supports schemas (if
      available). E.g. when using Postgres you can reference as
      table within a different schema through '<schema>.<tablename>'.
 
    - Model.add() accepts a new optional parameter 'table_name' that
      can be used to specify the name of a table (including schema
      information) when you want to use the 'name' parameter as
      an alias for the related table/mapper.
 
- 
+
 0.1.6 (28.03.2007)
 ------------------
 
    - fixed a bug in registerSQLAlchemyWrapper
 
 0.1.5 (28.03.2007)
 ------------------
-  
+
    - registerSQLAlchemyWrapper() should now work with Zope 2.8-2.10
 
    - abort() was defined twice inside the DataManager class
- 
+
 0.1.4 (21.03.2007)
 ------------------
 
    - the Model class now behave (where needed) as a sorted
      dictionary. Its items() method must returned all items
      in insertion order.
```

### Comparing `z3c.sqlalchemy-2.0/src/z3c.sqlalchemy.egg-info/SOURCES.txt` & `z3c.sqlalchemy-2.1/src/z3c.sqlalchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.sqlalchemy-2.0/tox.ini` & `z3c.sqlalchemy-2.1/tox.ini`

 * *Files identical despite different names*

