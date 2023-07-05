# Comparing `tmp/prom-4.5.1.tar.gz` & `tmp/prom-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prom-4.5.1.tar", last modified: Fri Jun 30 00:00:29 2023, max compression
+gzip compressed data, was "prom-4.7.0.tar", last modified: Tue Jul  4 23:57:54 2023, max compression
```

## Comparing `prom-4.5.1.tar` & `prom-4.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.424041 prom-4.5.1/
--rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.5.1/LICENSE.txt
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-30 00:00:29.423909 prom-4.5.1/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.5.1/README.md
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.421858 prom-4.5.1/prom/
--rw-r--r--   0 jaymon     (501) staff       (20)     1456 2023-06-29 23:59:06.000000 prom-4.5.1/prom/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.5.1/prom/compat.py
--rw-r--r--   0 jaymon     (501) staff       (20)    50364 2023-06-29 23:48:39.000000 prom-4.5.1/prom/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.5.1/prom/exception.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.422798 prom-4.5.1/prom/extras/
--rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.5.1/prom/extras/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.5.1/prom/extras/config.py
--rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.5.1/prom/extras/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    25477 2023-06-29 22:42:57.000000 prom-4.5.1/prom/extras/testdata.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.423298 prom-4.5.1/prom/interface/
--rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.5.1/prom/interface/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)    27763 2023-03-27 23:38:55.000000 prom-4.5.1/prom/interface/base.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.423545 prom-4.5.1/prom/interface/postgres/
--rw-r--r--   0 jaymon     (501) staff       (20)    20308 2023-05-01 23:16:39.000000 prom-4.5.1/prom/interface/postgres/__init__.py
--rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.5.1/prom/interface/postgres/gevent.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35163 2023-06-29 22:42:57.000000 prom-4.5.1/prom/interface/sql.py
--rw-r--r--   0 jaymon     (501) staff       (20)    17737 2023-06-27 20:25:40.000000 prom-4.5.1/prom/interface/sqlite.py
--rw-r--r--   0 jaymon     (501) staff       (20)    24442 2023-06-29 23:58:07.000000 prom-4.5.1/prom/model.py
--rw-r--r--   0 jaymon     (501) staff       (20)    35676 2023-06-29 22:42:57.000000 prom-4.5.1/prom/query.py
--rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.5.1/prom/utils.py
-drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-06-30 00:00:29.422391 prom-4.5.1/prom.egg-info/
--rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/PKG-INFO
--rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/SOURCES.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/dependency_links.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/requires.txt
--rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-06-30 00:00:29.000000 prom-4.5.1/prom.egg-info/top_level.txt
--rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-06-30 00:00:29.424081 prom-4.5.1/setup.cfg
--rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.5.1/setup.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.058187 prom-4.7.0/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1080 2017-08-21 19:50:23.000000 prom-4.7.0/LICENSE.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-07-04 23:57:54.058033 prom-4.7.0/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)     5228 2021-05-05 22:06:50.000000 prom-4.7.0/README.md
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.055740 prom-4.7.0/prom/
+-rw-r--r--   0 jaymon     (501) staff       (20)     1684 2023-07-04 21:29:17.000000 prom-4.7.0/prom/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)      188 2021-05-05 21:14:27.000000 prom-4.7.0/prom/compat.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    50864 2023-07-04 22:43:46.000000 prom-4.7.0/prom/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2359 2023-03-27 21:02:23.000000 prom-4.7.0/prom/exception.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.056851 prom-4.7.0/prom/extras/
+-rw-r--r--   0 jaymon     (501) staff       (20)        0 2023-03-27 21:25:20.000000 prom-4.7.0/prom/extras/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     1262 2023-03-11 10:50:37.000000 prom-4.7.0/prom/extras/config.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     2447 2023-03-23 00:59:43.000000 prom-4.7.0/prom/extras/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    26283 2023-07-04 23:19:20.000000 prom-4.7.0/prom/extras/testdata.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.057350 prom-4.7.0/prom/interface/
+-rw-r--r--   0 jaymon     (501) staff       (20)     3032 2023-03-27 23:40:25.000000 prom-4.7.0/prom/interface/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    31357 2023-07-04 22:59:13.000000 prom-4.7.0/prom/interface/base.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.057605 prom-4.7.0/prom/interface/postgres/
+-rw-r--r--   0 jaymon     (501) staff       (20)    20910 2023-07-04 21:30:09.000000 prom-4.7.0/prom/interface/postgres/__init__.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     3109 2023-03-23 00:11:15.000000 prom-4.7.0/prom/interface/postgres/gevent.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35508 2023-07-04 21:38:33.000000 prom-4.7.0/prom/interface/sql.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    18180 2023-07-04 21:24:25.000000 prom-4.7.0/prom/interface/sqlite.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    25190 2023-07-02 21:40:15.000000 prom-4.7.0/prom/model.py
+-rw-r--r--   0 jaymon     (501) staff       (20)    35918 2023-07-04 21:37:54.000000 prom-4.7.0/prom/query.py
+-rw-r--r--   0 jaymon     (501) staff       (20)     4610 2020-12-07 23:23:45.000000 prom-4.7.0/prom/utils.py
+drwxr-xr-x   0 jaymon     (501) staff       (20)        0 2023-07-04 23:57:54.056396 prom-4.7.0/prom.egg-info/
+-rw-r--r--   0 jaymon     (501) staff       (20)     5916 2023-07-04 23:57:54.000000 prom-4.7.0/prom.egg-info/PKG-INFO
+-rw-r--r--   0 jaymon     (501) staff       (20)      534 2023-07-04 23:57:54.000000 prom-4.7.0/prom.egg-info/SOURCES.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        1 2023-07-04 23:57:54.000000 prom-4.7.0/prom.egg-info/dependency_links.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       57 2023-07-04 23:57:54.000000 prom-4.7.0/prom.egg-info/requires.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)        5 2023-07-04 23:57:54.000000 prom-4.7.0/prom.egg-info/top_level.txt
+-rw-r--r--   0 jaymon     (501) staff       (20)       38 2023-07-04 23:57:54.058230 prom-4.7.0/setup.cfg
+-rw-r--r--   0 jaymon     (501) staff       (20)     2201 2021-10-12 23:47:11.000000 prom-4.7.0/setup.py
```

### Comparing `prom-4.5.1/LICENSE.txt` & `prom-4.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/PKG-INFO` & `prom-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.5.1
+Version: 4.7.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.5.1/README.md` & `prom-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/__init__.py` & `prom-4.7.0/prom/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     UniqueError,
     CloseError,
 )
 
 from . import utils
 
 
-__version__ = '4.5.1'
+__version__ = '4.7.0'
 
 
 def transaction(connection_name="", **kwargs):
     """Create a transaction 
 
     Sometimes you just need to batch a whole bunch of operation across a whole bunch
     of different models, this allows you to create a transaction outside of any
@@ -46,12 +46,16 @@
         with prom.transaction(prefix="batch") as conn:
             o = FooOrm(foo=1)
             o.save(connection=conn)
 
     :param connection_name: str, the connection name corresponding to the anchor
         of the DSN, defaults to the default "" connection
     :param **kwargs: passed through to the Interface.transaction context manager
-        prefix: the name of the transaction you want to use
+        * prefix: str, the name of the transaction you want to use
+        * nest: bool, True if you want nested transactions to be created, False
+            to ignore nested transactions
     :returns: Connection instance
     """
+    kwargs.setdefault("nest", False)
+    kwargs.setdefault("prefix", f"prom_{connection_name}_tx")
     return get_interface(connection_name).transaction(**kwargs)
```

### Comparing `prom-4.5.1/prom/config.py` & `prom-4.7.0/prom/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,31 @@
 
     @property
     def pk_names(self):
         """Returns all the field names comprising the primary key as a list"""
         pk_name = self.pk_name
         return [pk_name] if pk_name else []
 
+    @property
+    def schemas(self):
+        """Find and return all the schemas that are needed for this schema to 
+        install successfully
+
+        Another way to put this is all the schemas this Schema touches
+
+        :returns: list, a list of Schema instances, self will be at the end
+        """
+        schemas = []
+        for f in self.fields.values():
+            if s := f.schema:
+                schemas.extend(s.schemas)
+        schemas.append(self)
+
+        return schemas
+
     @classmethod
     def get_instance(cls, orm_class, **kwargs):
         """return a Schema singleton instance for the given orm_class
 
         if there isn't already an instance in cache then a new instance will be
         created. If a Schema instance is already in cache then it will be returned
 
@@ -646,15 +663,15 @@
     """True if this field is indexed"""
 
     orm_class = None
     """Holds the model class this field is defined on"""
 
     @cachedproperty(cached="_schema")
     def schema(self):
-        """return the schema instance if this is reference to another table
+        """return the schema instance if this field is a reference to another table
 
         see .set_type() for an explanation on why we defer figuring this out until now
         """
         field_type = self.original_type
         module, klass = utils.get_objects(field_type)
         schema = klass.schema
         if not schema:
```

### Comparing `prom-4.5.1/prom/exception.py` & `prom-4.7.0/prom/exception.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/extras/config.py` & `prom-4.7.0/prom/extras/config.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/extras/model.py` & `prom-4.7.0/prom/extras/model.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/extras/testdata.py` & `prom-4.7.0/prom/extras/testdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,33 @@
 
         It relies on a method .ensure_safe_env being defined in the project code
         """
         if self.ensure_safe_env(): # this method needs to be defined in project code
             for inter in get_interfaces().values():
                 inter.unsafe_delete_tables()
 
+    def unsafe_install_orms(self, modulepaths):
+        """Go through and install all the Orm subclasses found in the passed in
+        module paths
+
+        :param modulepaths: Sequence[str], a list of modpaths (eg ["foo.bar", "che"])
+        """
+        # import the module paths to load the Orms into memory
+        for modulepath in modulepaths:
+            rm = ReflectModule(modulepath)
+            m = rm.module() 
+
+        # now go through all the orm classes that have been loaded and install them
+        seen_table_names = set()
+        for orm_class in self._orm_classes():
+            for s in orm_class.schema.schemas:
+                if s.table_name not in seen_table_names:
+                    s.orm_class.install()
+                    seen_table_names.add(s.table_name)
+
     def assure_orm_field_names(self, orm_class, **kwargs):
         """Field instances can have aliases, in order to allow you to pass in aliases,
         this will go through kwargs and normalize the field names
 
         :Example:
             class Foobar(Orm):
                 che = Field(str, aliases=["baz"]
@@ -434,15 +453,15 @@
         :param orm_class: Orm
         :param **kwargs:
         :returns: Orm, the orm saved into the db
         """
         kwargs.setdefault("ignore_refs", False)
         instance = self._get(orm_class, **kwargs)
         try:
-            instance.save()
+            instance.save(nest=True)
 
         except UniqueError as e:
             logger.warning(" ".join([
                 f"Creating {orm_class.__name__} failed because it exists.",
                 "Fetching the existing instance without updating it",
             ]))
             instance = instance.requery()
@@ -472,15 +491,15 @@
             count: int, how many instances you want
             <MODEL_NAME>_count: int, alias for count
         :returns: list, a list of Orm instances that have all been saved into the db
         """
         kwargs.setdefault("ignore_refs", False)
         instances = self._gets(orm_class, **kwargs)
         for instance in instances:
-            instance.save()
+            instance.save(nest=True)
         return instances
 
     def get_orm_class(self, model_name, **kwargs):
         """get the orm class found at model_name
 
         :param model_name: str, the name of the orm class
         :returns: Orm, the orm_class.model_name that matches model_name
```

### Comparing `prom-4.5.1/prom/interface/__init__.py` & `prom-4.7.0/prom/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/interface/base.py` & `prom-4.7.0/prom/interface/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,130 +31,196 @@
 
 logger = logging.getLogger(__name__)
 
 
 class ConnectionABC(LogMixin):
     """Subclasses should extend Connection and implement the methods in this class"""
     def _transaction_start(self):
+        """Called when the first transaction is started"""
         pass
 
-    def _transaction_started(self, name):
+    def _transaction_starting(self, tx):
+        """Called when a nested transaction is started"""
+        pass
+
+    def _transaction_ignoring(self, tx):
+        """Called when nested transaction is ignored instead of started"""
         pass
 
     def _transaction_stop(self):
+        """Called when the last transaction is stopped"""
         pass
 
-    def _transaction_stopping(self):
+    def _transaction_stopping(self, tx):
+        """Called when a nested transaction is stopped"""
         pass
 
     def _transaction_fail(self):
+        """Called when the last transaction is failed"""
         pass
 
-    def _transaction_failing(self, name):
+    def _transaction_failing(self, tx):
+        """Called when a nested transaction is failed"""
         pass
 
 
 class Connection(ConnectionABC):
     """holds common methods that all raw connections should have"""
-
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # counting semaphore, greater than 0 if in a transaction, 0 if no current transaction.
+        # counting semaphore, greater than 0 if in a transaction, 0 if no current
+        # transaction.
         #
-        # This will be incremented everytime transaction_start() is called, and decremented
-        # everytime transaction_stop() is called.
+        # This will be incremented everytime transaction_start() is called, and
+        # decremented everytime transaction_stop() is called.
         #
         # transaction_fail will set this back to 0 and rollback the transaction
         #
-        # Holds the active transaction names
+        # Holds the active transactions
         self.transactions = Stack()
 
-    @property
     def transaction_count(self):
         """How many active transactions there currently are"""
         return len(self.transactions)
 
     def transaction_names(self):
-        return " > ".join(reversed(self.transactions))
+        return " > ".join((r["name"] for r in reversed(self.transactions)))
 
-    def transaction_name(self, prefix=""):
+    def transaction_name(self, **kwargs):
         """generate a random transaction name for use in start_transaction() and
         fail_transaction()
 
         :param prefix: str, to better track transactions in logs you can give a
             prefix name that will be prepended to the auto-generated name
         """
-        name = str(uuid.uuid4())[-5:]
-        #tcount = self.transaction_count + 1
-        prefix = prefix or "p"
-        return f"{prefix}_{name}"
+        if not (name := kwargs.get("name", "")):
+            suffix = str(uuid.uuid4())[-5:]
+            prefix = kwargs.get("prefix", "") or "p"
+            name = f"{prefix}_{suffix}"
+        return name
+
+    def transaction_create(self, **kwargs):
+        """Create a new transaction dict that will be placed on the .transactions
+        stack
+
+        :param **kwargs:
+            - nest: bool, True if this (and children unless passed in) will run
+                nested transactions. If this is False then subsequent calls to
+                .transaction_start will be ignored unless nest=True is passed in
+                again
+            - name: str, the transaction name
+            - prefix: str, used to create a transaction name (see
+              .transaction_name)
+        :returns: dict[str], the created transaction with keys:
+            - nest: bool, the value of kwargs["nest"] or of
+              .transaction_current()["nest"]
+            - name: str, the tx name
+            - ignored: bool, True if this tx is going to be ignored
+            - index: int, the depth of the transaction
+        """
+        name = self.transaction_name(**kwargs)
+        current_tx = self.transaction_current()
+        nest = kwargs.get("nest", current_tx.get("nest", True))
+
+        ignored = False
+        if current_tx:
+            ignored = not nest
+
+        else:
+            ignored = False
+
+        index = self.transaction_count() + 1
+
+        return {
+            "nest": nest,
+            "name": name,
+            "ignored": ignored,
+            "index": index
+        }
+
+    def transaction_current(self):
+        """Returns the current transaction dict, or empty dict if no tx"""
+        return self.transactions[-1] if self.transactions else {}
 
     def transaction_exists(self):
         """return true if currently in a transaction
 
         this was previously named .in_transaction but it turns out SQLite has a
         property with that name
         """
-        return self.transaction_count > 0
+        return self.transaction_count() > 0
 
     def transaction_start(self, **kwargs):
         """start a transaction
 
         this will increment transaction semaphore and pass it to _transaction_start()
         """
-        if not (name := kwargs.get("name", "")):
-            name = self.transaction_name(prefix=kwargs.get("prefix", ""))
+        tx = self.transaction_create(**kwargs)
+        self.transactions.push(tx)
+
+        transaction_count = tx["index"]
+        if tx["ignored"]:
+            self.log_debug([
+                f"{transaction_count}.",
+                f"Ignoring {self} transaction {self.transaction_names()}",
+            ])
+            self._transaction_ignoring(tx)
 
-        self.transactions.push(name)
-        transaction_count = self.transaction_count
-        self.log_debug([
-            f"{transaction_count}.", 
-            f"Start 0x{id(self):02x} transaction {self.transaction_names()}",
-        ])
-        if transaction_count == 1:
-            self._transaction_start()
         else:
-            self._transaction_started(name)
+            self.log_debug([
+                f"{transaction_count}.", 
+                f"Start {self} transaction {self.transaction_names()}",
+            ])
+            if transaction_count == 1:
+                self._transaction_start()
+
+            else:
+                self._transaction_starting(tx)
 
         return transaction_count
 
     def transaction_stop(self):
         """stop/commit a transaction if ready"""
-        transaction_count = self.transaction_count
+        transaction_count = self.transaction_count()
         if transaction_count > 0:
+            tx = self.transactions.pop()
+            if not tx["ignored"]:
+                self.log_debug([
+                    f"{transaction_count}.", 
+                    f"Stopping {self} transaction {self.transaction_names()}",
+                ])
 
-            self.log_debug([
-                f"{transaction_count}.", 
-                f"Stopping 0x{id(self):02x} transaction {self.transaction_names()}",
-            ])
+                if transaction_count == 1:
+                    self._transaction_stop()
 
-            name = self.transactions.pop()
-            if transaction_count == 1:
-                self._transaction_stop()
-            else:
-                self._transaction_stopping(name)
+                else:
+                    self._transaction_stopping(tx)
 
         return self.transaction_count
 
     def transaction_fail(self):
         """rollback a transaction if currently in one"""
-        transaction_count = self.transaction_count
+        transaction_count = self.transaction_count()
         if transaction_count > 0:
+            tx = self.transactions.pop()
+            if not tx["ignored"]:
+                self.log_debug([
+                    f"{transaction_count}.",
+                    f"Failing {self} transaction {self.transaction_names()}",
+                ])
 
-            self.log_debug([
-                f"{transaction_count}.", 
-                f"Failing 0x{id(self):02x} transaction {self.transaction_names()}",
-            ])
+                if transaction_count == 1:
+                    self._transaction_fail()
 
-            name = self.transactions.pop()
-            if transaction_count == 1:
-                self._transaction_fail()
-            else:
-                self._transaction_failing(name)
+                else:
+                    self._transaction_failing(tx)
+
+    def __str__(self):
+        return f"0x{id(self):02x}"
 
 
 class InterfaceABC(LogMixin):
     """This is just a convenience abstract base class so child interfaces can easily
     see what methods they need to implement. They should extend Interface and then
     implement the methods in this class"""
     def _connect(self, config):
@@ -196,14 +262,17 @@
 
     def _set_index(self, schema, name, field_names, **kwargs):
         raise NotImplementedError()
 
     def _insert(self, schema, fields, **kwargs):
         raise NotImplementedError()
 
+    def _inserts(self, schema, field_names, field_values, **kwargs):
+        raise NotImplementedError()
+
     def _update(self, schema, fields, query, **kwargs):
         raise NotImplementedError()
 
     def _upsert(self, schema, insert_fields, update_fields, conflict_field_names, **kwargs):
         raise NotImplementedError()
 
     def _delete(self, schema, query, **kwargs):
@@ -330,22 +399,26 @@
         if connection.closed:
             # we've gotten into a bad state so let's try reconnecting
             self.reconnect()
             connection = self._get_connection()
 
         connection.interface = self
 
-        self.log_debug(f"Getting {self.config.interface_name} connection 0x{id(connection):02x}")
+        self.log_debug(
+            f"Getting {self.config.interface_name} connection {connection}"
+        )
         return connection
 
     def free_connection(self, connection):
         """When .connection is done with a connection it calls this method"""
         #connection.interface = None
         if self.is_connected():
-            self.log_debug(f"Freeing {self.config.interface_name} connection 0x{id(connection):02x}")
+            self.log_debug(
+                f"Freeing {self.config.interface_name} connection {connection}"
+            )
             self._free_connection(connection)
 
     def is_connected(self):
         return self.connected
 
     def close(self):
         """close an open connection"""
@@ -387,22 +460,26 @@
             with self.connection(**kwargs) as connection:
                 # do something with connection
         """
         free_connection = False
         try:
             if connection:
                 if connection.closed:
-                    self.log_warning("Passed in connection is closed and must be refreshed")
+                    self.log_warning(
+                        "Passed in connection is closed and must be refreshed"
+                    )
                     if connection.transaction_exists():
-                        self.log_error("Closed connection had open transactions!")
+                        self.log_warning("Closed connection had open transactions!")
 
                     connection = None
 
                 else:
-                    self.log_debug(f"Connection call using existing connection 0x{id(connection):02x}")
+                    self.log_debug(
+                        f"Connection call using existing connection {connection}"
+                    )
                     yield connection
 
             if connection is None:
                 free_connection = True
                 connection = self.get_connection()
                 yield connection
 
@@ -410,66 +487,61 @@
             self.raise_error(e)
 
         finally:
             if free_connection and connection:
                 self.free_connection(connection)
 
             else:
-                self.log_debug(f"Connection call NOT freeing existing connection 0x{id(connection):02x}")
+                self.log_debug(
+                    f"Connection call NOT freeing existing connection {connection}"
+                )
 
     @contextmanager
     def transaction(self, connection=None, **kwargs):
         """A simple context manager useful for when you want to wrap a bunch of
         db calls in a transaction, this is used internally for any write statements
 
         :Example:
             with self.transaction() as connection
                 # do a bunch of calls
             # those db calls will be committed by this line
         """
         with self.connection(connection) as connection:
-            if not kwargs.get("nest", True) and connection.transaction_exists():
-                # internal write transactions don't nest
-                self.log_debug("Transaction call IS NOT creating a new transaction")
+            connection.transaction_start(**kwargs)
+            try:
                 yield connection
 
-            else:
-                self.log_debug("Transaction call IS creating a new transaction")
-                connection.transaction_start(**kwargs)
-                try:
-                    yield connection
-
-                except Exception:
-                    connection.transaction_fail()
-                    raise
+            except Exception:
+                connection.transaction_fail()
+                raise
 
-                else:
-                    connection.transaction_stop()
+            else:
+                connection.transaction_stop()
 
     def execute_write(self, callback, *args, **kwargs):
         """Any write statements will use this method
 
         CREATE, DELETE, DROP, INSERT, or UPDATE (collectively "write statements")
         """
-        kwargs.setdefault("nest", True)
         kwargs.setdefault("execute_in_transaction", True)
 
         return self.execute(callback, *args, **kwargs)
 
     def execute_read(self, callback, *args, **kwargs):
         """Any write statements will use this method
 
         SELECT (collectively "read statements")
         """
         with self.connection(**kwargs) as connection:
             kwargs["connection"] = connection
 
-            in_transaction = connection.transaction_exists()
-            kwargs.setdefault("nest", in_transaction)
-            kwargs.setdefault("execute_in_transaction", in_transaction)
+            kwargs.setdefault(
+                "execute_in_transaction",
+                connection.transaction_exists()
+            )
 
             return self.execute(callback, *args, **kwargs)
 
     def execute(self, callback, *args, **kwargs):
         """Internal method. Execute the callback with args and kwargs, retrying
         the query if an error is raised that it thinks it successfully handled
 
@@ -636,14 +708,49 @@
         return self.execute_write(
             self._insert,
             schema=schema,
             fields=fields,
             **kwargs
         )
 
+    def inserts(self, schema, field_names, field_rows, **kwargs):
+        """Persist the field names found in all the field rows
+
+        :param schema: Schema
+        :param field_names: list, the field names that will be checked for each
+            row in field_rows and used to turn each dict in field_rows to a tuple
+        :param field_rows: Sequence, if an iterator of dict instances with keys found
+            in field_names, if a key is missing it will have None set as the value,
+            if it's an iterator of values then the tuple value ordering should match
+            with field_names
+        :param **kwargs: passed through
+        :returns: bool, True if the query executed successfully
+        """
+        kwargs.setdefault("prefix", "inserts")
+
+        def field_values(field_names, field_rows):
+            for fields in field_rows:
+                if isinstance(fields, Mapping):
+                    row = []
+                    for field_name in field_names:
+                        row.append(fields.get(field_name, None))
+                    yield row
+
+                else:
+                    yield fields
+
+        self.execute_write(
+            self._inserts,
+            schema=schema,
+            field_names=field_names,
+            field_values=field_values(field_names, field_rows),
+            **kwargs,
+        )
+        return True
+
     def update(self, schema, fields, query, **kwargs):
         """Persist the query.fields into the db that match query.fields_where
 
         :param schema: Schema instance, the table the query will run against
         :param fields: dict, the fields {field_name: field_value} to persist
         :param query: Query instance, will be used to create the where clause
         :param **kwargs: passed through
```

### Comparing `prom-4.5.1/prom/interface/postgres/__init__.py` & `prom-4.7.0/prom/interface/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,29 @@
             query_str += ' AND schemaname = %s'
             query_args.append(schema_name)
 
         ret = self._raw(query_str, *query_args, **kwargs)
         # http://www.postgresql.org/message-id/CA+mi_8Y6UXtAmYKKBZAHBoY7F6giuT5WfE0wi3hR44XXYDsXzg@mail.gmail.com
         return [r['tablename'] for r in ret]
 
+    def _inserts(self, schema, field_names, field_values, **kwargs):
+        """
+        https://www.psycopg.org/docs/cursor.html#cursor.executemany
+        https://www.psycopg.org/docs/extras.html#fast-exec
+        https://www.psycopg.org/docs/extras.html#psycopg2.extras.execute_batch
+        """
+        query_str = self.render_inserts_sql(schema, field_names, **kwargs)
+        with self.connection(**kwargs) as connection:
+            cur = connection.cursor()
+            psycopg2.extras.execute_batch(
+                cur,
+                query_str,
+                field_values,
+            )
+
     def _delete_table(self, schema, **kwargs):
         """
         https://www.postgresql.org/docs/current/sql-droptable.html
         """
         query_str = 'DROP TABLE IF EXISTS {} CASCADE'.format(self.render_table_name_sql(schema))
         self._raw(query_str, ignore_result=True, **kwargs)
```

### Comparing `prom-4.5.1/prom/interface/postgres/gevent.py` & `prom-4.7.0/prom/interface/postgres/gevent.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom/interface/sql.py` & `prom-4.7.0/prom/interface/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,37 +28,43 @@
     https://docs.python.org/3.9/library/sqlite3.html#sqlite3-controlling-transactions
     https://www.sqlite.org/lockingv3.html
     https://www.sqlite.org/lang_transaction.html
     """
     def _transaction_start(self):
         self._execute("BEGIN")
 
-    def _transaction_started(self, name):
+    def _transaction_starting(self, tx):
         # http://www.postgresql.org/docs/9.2/static/sql-savepoint.html
-        self._execute("SAVEPOINT {}".format(self.interface.render_field_name_sql(name)))
+        self._execute("SAVEPOINT {}".format(
+            self.interface.render_field_name_sql(tx["name"])
+        ))
 
     def _transaction_stop(self):
         """
         http://initd.org/psycopg/docs/usage.html#transactions-control
         https://news.ycombinator.com/item?id=4269241
         """
         self._execute("COMMIT")
 
-    def _transaction_stopping(self, name):
-        self._execute("RELEASE {}".format(self.interface.render_field_name_sql(name)))
+    def _transaction_stopping(self, tx):
+        self._execute("RELEASE {}".format(
+            self.interface.render_field_name_sql(tx["name"])
+        ))
 
     def _transaction_fail(self):
         self._execute("ROLLBACK")
 
-    def _transaction_failing(self, name):
+    def _transaction_failing(self, tx):
         # http://www.postgresql.org/docs/9.2/static/sql-rollback-to.html
-        self._execute("ROLLBACK TO SAVEPOINT {}".format(self.interface.render_field_name_sql(name)))
+        self._execute("ROLLBACK TO SAVEPOINT {}".format(
+            self.interface.render_field_name_sql(tx["name"])
+        ))
 
     def _execute(self, query_str):
-        self.log_info(f"0x{id(self):02x} - {query_str}")
+        self.log_info(f"{self} - {query_str}")
         cur = self.cursor()
         cur.execute(query_str)
         cur.close()
 
 
 class SQLInterfaceABC(Interface):
     """SQL database interfaces should extend SQLInterface and implement all these
@@ -304,16 +310,16 @@
 
             if cursor_result:
                 # https://stackoverflow.com/a/125140
                 cur.arraysize = kwargs.get("arraysize", 500)
 
             if query_args:
                 self.log_for(
-                    debug=(["0x{:02x} - {}\n{}", id(connection), query_str, query_args],),
-                    info=([f"0x{id(connection):02x} - {query_str}"],)
+                    debug=(["0x{} - {}\n{}", connection, query_str, query_args],),
+                    info=([f"{connection} - {query_str}"],)
                 )
 
                 try:
                     cur.execute(query_str, query_args)
 
                 except Exception as e:
                     self.raise_error(
@@ -322,15 +328,15 @@
                             query_str,
                             query_args,
                             self.PLACEHOLDER,
                         ]
                     )
 
             else:
-                self.log_info(f"0x{id(connection):02x} - {query_str}")
+                self.log_info(f"{connection} - {query_str}")
                 cur.execute(query_str)
 
             if cursor_result:
                 ret = cur
 
             elif ignore_result:
                 cur.close()
@@ -801,36 +807,46 @@
         query_str = "\n".join(query_str)
         return query_str, query_args
 
     def render_insert_sql(self, schema, fields, **kwargs):
         """
         https://www.sqlite.org/lang_insert.html
         """
-        field_formats = []
         field_names = []
         query_vals = []
         for field_name, field_val in fields.items():
-            field_names.append(self.render_field_name_sql(field_name))
-            field_formats.append(self.PLACEHOLDER)
+            field_names.append(field_name)
             query_vals.append(field_val)
 
-        query_str = 'INSERT INTO {} ({}) VALUES ({})'.format(
-            self.render_table_name_sql(schema),
-            ', '.join(field_names),
-            ', '.join(field_formats),
-        )
+        query_str = self.render_inserts_sql(schema, field_names, **kwargs)
 
         if not kwargs.get("ignore_return_clause", False):
             # https://www.sqlite.org/lang_returning.html
             pk_name = schema.pk_name
             if pk_name:
                 query_str += ' RETURNING {}'.format(self.render_field_name_sql(pk_name))
 
         return query_str, query_vals
 
+    def render_inserts_sql(self, schema, field_names, **kwargs):
+        """
+        https://www.sqlite.org/lang_insert.html
+        """
+        sql_names = []
+        sql_formats = []
+        for field_name in field_names:
+            sql_names.append(self.render_field_name_sql(field_name))
+            sql_formats.append(self.PLACEHOLDER)
+
+        return "INSERT INTO {} ({}) VALUES ({})".format(
+            self.render_table_name_sql(schema),
+            ", ".join(sql_names),
+            ", ".join(sql_formats),
+        )
+
     def render_update_sql(self, schema, fields, query, **kwargs):
         query_str = ''
         query_args = []
 
         if not kwargs.get("only_set_clause", False):
             query_str = 'UPDATE {} '.format(self.render_table_name_sql(schema))
```

### Comparing `prom-4.5.1/prom/interface/sqlite.py` & `prom-4.7.0/prom/interface/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,14 +335,26 @@
         """
         https://www.sqlite.org/lang_droptable.html
         """
         #query_str = 'DROP TABLE IF EXISTS {}'.format(str(schema))
         query_str = "DROP TABLE IF EXISTS {}".format(self.render_table_name_sql(schema))
         self._raw(query_str, ignore_result=True, **kwargs)
 
+    def _inserts(self, schema, field_names, field_values, **kwargs):
+        """
+        https://docs.python.org/3/library/sqlite3.html#sqlite3.Cursor.executemany
+        """
+        query_str = self.render_inserts_sql(schema, field_names, **kwargs)
+        with self.connection(**kwargs) as connection:
+            cur = connection.cursor()
+            cur.executemany(
+                query_str,
+                field_values,
+            )
+
     def create_error(self, e, **kwargs):
         kwargs.setdefault("error_module", sqlite3)
         if isinstance(e, sqlite3.OperationalError):
             e_msg = str(e)
             if "no such column" in e_msg or "has no column" in e_msg:
                 #INSERT: "table yscrmiklbgdtx has no column named che"
                 #SELECT: "no such column: che"
```

### Comparing `prom-4.5.1/prom/model.py` & `prom-4.7.0/prom/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,33 @@
         return a new OrmPool instance
 
         return -- OrmPool -- the orm pool instance will be tied to this Orm
         """
         return OrmPool(orm_class=cls, maxsize=maxsize)
 
     @classmethod
+    def transaction(cls, **kwargs):
+        """Create a transaction for this Orm
+
+        :Example:
+            with FooOrm.transaction() as conn:
+                o = FooOrm(foo=1)
+                o.save(connection=conn)
+
+        :param **kwargs: passed through to the Interface.transaction context manager
+            * prefix: str, the name of the transaction you want to use
+            * nest: bool, True if you want nested transactions to be created, False
+                to ignore nested transactions
+        :returns: Connection instance
+        """
+        kwargs.setdefault("nest", False)
+        kwargs.setdefault("prefix", f"{cls.__name__}_{cls.connection_name}_tx")
+        return cls.interface.transaction(**kwargs)
+
+    @classmethod
     def create(cls, *args, **kwargs):
         """
         create an instance of cls with the passed in fields and set it into the db
 
         this method takes *args, **kwargs because a child class can override .__init__
         and it's nice to not have to modify this method also
```

### Comparing `prom-4.5.1/prom/query.py` & `prom-4.7.0/prom/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     def __getitem__(self, i):
         it = self.copy()
         q = it.query
 
         b = q.bounds
         limit = b.limit if b.has_limit() else self.count()
-        b = Bounds(limit=limit, offset=q.bounds.offset)
+        b = q.bounds_class(limit=limit, offset=q.bounds.offset)
 
         if isinstance(i, slice):
             if i.step:
                 raise ValueError("slice stepping is not supported")
 
             if i.start:
                 start = b.find_offset(i.start)
@@ -245,15 +245,15 @@
                 r = orm_class.hydrate(d)
             else:
                 r = d
 
         return r
 
 
-class Bounds(object):
+class QueryBounds(object):
     @property
     def limit(self):
         l = self._limit
         #l = self.limit_paginate if self.paginate else self._limit
         return l if l else 0
 
     @limit.setter
@@ -388,15 +388,15 @@
         return offset
 
     def find_more_index(self):
         #return self.offset + self.limit_paginate
         return self.offset + self.limit
 
 
-class Field(object):
+class QueryField(object):
     @property
     def schema(self):
         return self.query.schema if self.query else None
 
     def __init__(self, query, field_name, field_val=None, **kwargs):
         self.query = query
         self.operator = kwargs.pop("operator", None)
@@ -458,15 +458,15 @@
 
             except AttributeError:
                 field_name = schema.field_model_name(field_name)
 
         return field_name, function_name
 
 
-class Fields(list):
+class QueryFields(list):
     @property
     def fields(self):
         """Returns a dict of field_name: field_value"""
         ret = {}
         for f in self:
             ret[f.name] = f.value
         return ret
@@ -482,45 +482,51 @@
             if f.name not in seen:
                 ret.append(f.name)
                 seen.add(f.name)
         return ret
 
     def append(self, field):
         index = len(self)
-        super(Fields, self).append(field)
+        super().append(field)
         self.field_names[field.name].append(index)
 
     def __contains__(self, field_name):
         return field_name in self.field_names
 
     def __setitem__(self, *args, **kwargs):
         raise NotImplementedError()
     __delitem__ = __setitem__
 
     def clear(self):
         self.field_names = defaultdict(list)
         self.options = {}
-        self[:]
+        super().clear()
 
 
 class Query(object):
-    """
-    Handle standard query creation and allow interface querying
+    """Handle standard query creation and allow interface querying
 
     :example:
         q = Query(orm_class)
         q.eq_foo(1).desc_bar().limit(10).page(2).get()
-        # SELECT * FROM <orm_class.table_name> WHERE foo = 1 ORDER BY bar DESC LIMIT 10 OFFSET 20
+        # SELECT
+        #   *
+        # FROM
+        #   <orm_class.table_name>
+        # WHERE
+        #   foo = 1
+        # ORDER BY bar DESC
+        # LIMIT 10 OFFSET 20
     """
-    field_class = Field
-    fields_set_class = Fields
-    fields_select_class = Fields
-    fields_where_class = Fields
-    fields_sort_class = Fields
-    bounds_class = Bounds
+    field_class = QueryField
+    fields_set_class = QueryFields
+    fields_select_class = QueryFields
+    fields_where_class = QueryFields
+    fields_sort_class = QueryFields
+    bounds_class = QueryBounds
     iterator_class = Iterator
 
     @property
     def interface(self):
         return self.orm_class.interface if self.orm_class else None
 
     @property
@@ -584,15 +590,14 @@
     def __init__(self, orm_class=None, **kwargs):
         # needed to use the db querying methods like get(), if you just want to build
         # a query then you don't need to bother passing this in
         self.orm_class = orm_class
         self.reset()
 
     def reset(self):
-        #self.interface = None
         self._ifilter = None
         self.fields_set = self.fields_set_class()
         self.fields_select = self.fields_select_class()
         self.fields_where = self.fields_where_class()
         self.fields_sort = self.fields_sort_class()
         self.bounds = self.bounds_class()
         self.compounds = []
@@ -615,14 +620,17 @@
         if isinstance(orm_classpath, basestring):
             orm_module, orm_class = get_objects(orm_classpath)
         else:
             orm_class = orm_classpath
 
         return orm_class.query
 
+    def ref_class(self, orm_classpath):
+        return self.ref(orm_classpath)
+
     def __iter__(self):
         return self.get()
 
     def find_methods(self, method_name):
         """Given a method name like <OPERATOR>_<FIELD_NAME> or <FIELD_NAME>_<OPERATOR>,
         split those into <OPERATOR> and <FIELD_NAME> if there is an existing
         <OPERATOR>_field method that exists
@@ -696,15 +704,19 @@
         return callback
 
     def create_field(self, field_name, field_val=None, **kwargs):
         f = self.field_class(self, field_name, field_val, **kwargs)
         return f
 
     def create_iterator(self, query):
-        return self.orm_class.iterator_class(query) if self.orm_class else self.iterator_class(query)
+        if self.orm_class:
+            iterator = self.orm_class.iterator_class(query)
+        else:
+            iterator = self.iterator_class(query)
+        return iterator
 
     def append_compound(self, operator, queries, **kwargs):
         """Internal method used by .intersect(), .union(), and .difference()"""
         for i, query in enumerate(queries):
             if self.fields_select:
                 if not query.fields_select:
                     if self.schema == query.schema:
```

### Comparing `prom-4.5.1/prom/utils.py` & `prom-4.7.0/prom/utils.py`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/prom.egg-info/PKG-INFO` & `prom-4.7.0/prom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prom
-Version: 4.5.1
+Version: 4.7.0
 Summary: A sensible orm for PostgreSQL or SQLite
 Home-page: http://github.com/jaymon/prom
 Author: Jay Marcyes
 Author-email: jay@marcyes.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `prom-4.5.1/prom.egg-info/SOURCES.txt` & `prom-4.7.0/prom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prom-4.5.1/setup.py` & `prom-4.7.0/setup.py`

 * *Files identical despite different names*

