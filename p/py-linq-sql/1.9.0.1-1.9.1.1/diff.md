# Comparing `tmp/py_linq_sql-1.9.0.1.tar.gz` & `tmp/py_linq_sql-1.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_linq_sql-1.9.0.1.tar", max compression
+gzip compressed data, was "py_linq_sql-1.9.1.1.tar", max compression
```

## Comparing `py_linq_sql-1.9.0.1.tar` & `py_linq_sql-1.9.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    13863 2023-02-09 11:20:10.641920 py_linq_sql-1.9.0.1/LICENSE.md
--rw-r--r--   0        0        0    13621 2023-03-30 09:53:07.893915 py_linq_sql-1.9.0.1/README.md
--rw-r--r--   0        0        0     2180 2023-05-04 08:57:57.458763 py_linq_sql-1.9.0.1/py_linq_sql/__init__.py
--rw-r--r--   0        0        0       58 2023-02-09 11:20:10.661920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/__init__.py
--rw-r--r--   0        0        0     8599 2023-02-09 11:20:10.661920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/alter.py
--rw-r--r--   0        0        0     7090 2023-02-09 11:20:10.661920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/build.py
--rw-r--r--   0        0        0    18390 2023-03-28 19:41:49.934189 py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult.py
--rw-r--r--   0        0        0     3042 2023-02-09 11:20:10.661920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_aggregate.py
--rw-r--r--   0        0        0     6607 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_context.py
--rw-r--r--   0        0        0     4581 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_terminal.py
--rw-r--r--   0        0        0     3399 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/build_request/one.py
--rw-r--r--   0        0        0       60 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/config/__init__.py
--rw-r--r--   0        0        0     5292 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/config/config.py
--rw-r--r--   0        0        0       50 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/exception/__init__.py
--rw-r--r--   0        0        0    12084 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/exception/exception.py
--rw-r--r--   0        0        0        0 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/py.typed
--rw-r--r--   0        0        0       88 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/sql_enumerable/__init__.py
--rw-r--r--   0        0        0    55958 2023-07-05 09:41:22.206109 py_linq_sql-1.9.0.1/py_linq_sql/sql_enumerable/sql_enumerable.py
--rw-r--r--   0        0        0       56 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/__init__.py
--rw-r--r--   0        0        0       31 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/__init__.py
--rw-r--r--   0        0        0     2497 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/enum.py
--rw-r--r--   0        0        0    33426 2023-07-05 09:41:22.206109 py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/magicdotpath.py
--rw-r--r--   0        0        0    13358 2023-02-15 10:32:33.463229 py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py
--rw-r--r--   0        0        0     4293 2023-02-09 14:30:57.412659 py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/other_classes.py
--rw-r--r--   0        0        0     1560 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/db.py
--rw-r--r--   0        0        0    11053 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/execute.py
--rw-r--r--   0        0        0       33 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/__init__.py
--rw-r--r--   0        0        0     3699 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/aggregate_functions.py
--rw-r--r--   0        0        0     3286 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/join_functions.py
--rw-r--r--   0        0        0     3147 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py
--rw-r--r--   0        0        0    11744 2023-02-15 10:32:33.463229 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py
--rw-r--r--   0        0        0      843 2023-03-30 09:52:31.421599 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_other_functions.py
--rw-r--r--   0        0        0     1810 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_str_functions.py
--rw-r--r--   0        0        0     8601 2023-02-15 10:32:33.467229 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py
--rw-r--r--   0        0        0     7818 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/other_functions.py
--rw-r--r--   0        0        0     6205 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/path_functions.py
--rw-r--r--   0        0        0     2388 2023-02-09 11:20:10.665920 py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/predicate_functions.py
--rw-r--r--   0        0        0     5415 2023-07-05 09:41:22.206109 py_linq_sql-1.9.0.1/pyproject.toml
--rw-r--r--   0        0        0    15101 1970-01-01 00:00:00.000000 py_linq_sql-1.9.0.1/setup.py
--rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 py_linq_sql-1.9.0.1/PKG-INFO
+-rw-r--r--   0        0        0    13863 2023-02-09 11:20:10.641920 py_linq_sql-1.9.1.1/LICENSE.md
+-rw-r--r--   0        0        0    13621 2023-03-30 09:53:07.893915 py_linq_sql-1.9.1.1/README.md
+-rw-r--r--   0        0        0     2180 2023-05-04 08:57:57.458763 py_linq_sql-1.9.1.1/py_linq_sql/__init__.py
+-rw-r--r--   0        0        0       58 2023-02-09 11:20:10.661920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/__init__.py
+-rw-r--r--   0        0        0     8599 2023-02-09 11:20:10.661920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/alter.py
+-rw-r--r--   0        0        0     7090 2023-02-09 11:20:10.661920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/build.py
+-rw-r--r--   0        0        0    18390 2023-03-28 19:41:49.934189 py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult.py
+-rw-r--r--   0        0        0     3042 2023-02-09 11:20:10.661920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_aggregate.py
+-rw-r--r--   0        0        0     6607 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_context.py
+-rw-r--r--   0        0        0     4581 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_terminal.py
+-rw-r--r--   0        0        0     3399 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/build_request/one.py
+-rw-r--r--   0        0        0       60 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/config/__init__.py
+-rw-r--r--   0        0        0     5292 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/config/config.py
+-rw-r--r--   0        0        0       50 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/exception/__init__.py
+-rw-r--r--   0        0        0    12084 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/exception/exception.py
+-rw-r--r--   0        0        0        0 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/py.typed
+-rw-r--r--   0        0        0       88 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/sql_enumerable/__init__.py
+-rw-r--r--   0        0        0    56268 2023-07-05 13:34:57.621310 py_linq_sql-1.9.1.1/py_linq_sql/sql_enumerable/sql_enumerable.py
+-rw-r--r--   0        0        0       56 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/__init__.py
+-rw-r--r--   0        0        0       31 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/__init__.py
+-rw-r--r--   0        0        0     2497 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/enum.py
+-rw-r--r--   0        0        0    34105 2023-07-05 13:34:57.621310 py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/magicdotpath.py
+-rw-r--r--   0        0        0    13358 2023-02-15 10:32:33.463229 py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py
+-rw-r--r--   0        0        0     4293 2023-02-09 14:30:57.412659 py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/other_classes.py
+-rw-r--r--   0        0        0     1560 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/db.py
+-rw-r--r--   0        0        0    11053 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/execute.py
+-rw-r--r--   0        0        0       33 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/__init__.py
+-rw-r--r--   0        0        0     3699 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/aggregate_functions.py
+-rw-r--r--   0        0        0     3286 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/join_functions.py
+-rw-r--r--   0        0        0     3147 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py
+-rw-r--r--   0        0        0    11744 2023-02-15 10:32:33.463229 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py
+-rw-r--r--   0        0        0      843 2023-03-30 09:52:31.421599 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_other_functions.py
+-rw-r--r--   0        0        0     1810 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_str_functions.py
+-rw-r--r--   0        0        0     8601 2023-02-15 10:32:33.467229 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py
+-rw-r--r--   0        0        0     7818 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/other_functions.py
+-rw-r--r--   0        0        0     6205 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/path_functions.py
+-rw-r--r--   0        0        0     2388 2023-02-09 11:20:10.665920 py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/predicate_functions.py
+-rw-r--r--   0        0        0     5458 2023-07-05 13:34:57.621310 py_linq_sql-1.9.1.1/pyproject.toml
+-rw-r--r--   0        0        0    15101 1970-01-01 00:00:00.000000 py_linq_sql-1.9.1.1/setup.py
+-rw-r--r--   0        0        0    14819 1970-01-01 00:00:00.000000 py_linq_sql-1.9.1.1/PKG-INFO
```

### Comparing `py_linq_sql-1.9.0.1/LICENSE.md` & `py_linq_sql-1.9.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/README.md` & `py_linq_sql-1.9.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/__init__.py` & `py_linq_sql-1.9.1.1/py_linq_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/alter.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/alter.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/build.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/build.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_aggregate.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_aggregate.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_context.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_context.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/consult_terminal.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/consult_terminal.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/build_request/one.py` & `py_linq_sql-1.9.1.1/py_linq_sql/build_request/one.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/config/config.py` & `py_linq_sql-1.9.1.1/py_linq_sql/config/config.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/exception/exception.py` & `py_linq_sql-1.9.1.1/py_linq_sql/exception/exception.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/sql_enumerable/sql_enumerable.py` & `py_linq_sql-1.9.1.1/py_linq_sql/sql_enumerable/sql_enumerable.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,17 +90,23 @@
 
         Raises:
             psycopg.Error: Indirect raise by `safe`.
             TablePermissionDeniedError: Indirect raise by
                 `is_valid_table_name_with_white_and_black_list`.
         """
         if isinstance(self.table, str):
-            if not is_valid_table_name_with_white_and_black_list(self.table):
-                raise TablePermissionDeniedError(self.table)
-            self.table = safe(self.connection, self.table)
+            tables = self.table.split(".") if "." in self.table else [f'"{self.table}"']
+            safed_tables = []
+            for table in tables:
+                without_quotes = table[1:-1]
+                if not is_valid_table_name_with_white_and_black_list(without_quotes):
+                    raise TablePermissionDeniedError(without_quotes)
+                safed_tables.append(safe(self.connection, without_quotes))
+            self.table = ".".join([f'"{stab[1:-1]}"' for stab in safed_tables])
+
         self.cmd = []
 
     def __eq__(self, other: Any) -> bool:
         """
         Try equality between two SQL_Enumerable.
 
         SQL_Enumerable_1 == SQL_Enumerable_2.
```

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/enum.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/enum.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/magicdotpath.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/magicdotpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -863,14 +863,28 @@
             Name but verified by psycopg.sql.Identifier.
 
         Raises:
             psycopg.Error: Indirect raise by `sql.Identifier` or `as_string`.
         """
         return sql.Identifier(name).as_string(self.connection)
 
+    def format_table_with_dot(self) -> str:
+        """
+        Get the table with dot in good format.
+
+        Returns:
+            The table in the good psql format.
+        """
+        return ".".join(
+            [
+                f'"{tab}"'
+                for tab in self.with_table.split(".")  # type: ignore[union-attr]
+            ]
+        )
+
     def jsonb_path(self, as_str: bool) -> str:
         """
         Get the corresponding jsonb path from a MagicDotPath.
 
         Args:
             as_str: Boolean to force the request with json in str.
 
@@ -881,38 +895,48 @@
             psycopg.Error: Indirect raise by `safe`.
         """
         self.column = self.safe(self.attributes[0][1:-1])
 
         res = ""
 
         if self.with_table:
-            res += f"{self.with_table}."
+            table = (
+                self.format_table_with_dot()
+                if "." in self.with_table
+                else f"{self.with_table}."
+            )
+            res = f"{res}{table}"
 
         if len(self.attributes) == 1:
-            res += self.column
+            res = f"{res}{self.column}"
         else:
             if as_str:
                 path_item = self.attributes[1:-1].copy()
                 path_item.insert(0, self.column)
-                res += f'{"->".join(path_item)}->>{self.attributes[-1]}'
+                res = f'{res}{"->".join(path_item)}->>{self.attributes[-1]}'
             else:
-                res += f'{self.column}->{"->".join(self.attributes[1:])}'
+                res = f'{res}{self.column}->{"->".join(self.attributes[1:])}'
         return res
 
     def col_name(self) -> str:
         """
         Get the corresponding column name form a MagicDotPath.
 
         Returns:
             A column name with the correct format.
         """
         result = []
 
         if self.with_table:
-            result.append(self.with_table[1:-1])
+            table = (
+                self.format_table_with_dot()
+                if "." in self.with_table
+                else self.with_table
+            )
+            result.append(table[1:-1])
 
         for att in self.attributes:
             result.append(att[1:-1])
 
         return "_".join(result)
```

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/op_and_func_of_mdp.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/classes/other_classes.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/classes/other_classes.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/db.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/db.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/execute.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/execute.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/aggregate_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/aggregate_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/join_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/join_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_hyperb_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_maths_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_other_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_other_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_str_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_str_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/magic_dp_trigo_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/other_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/other_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/path_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/path_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/py_linq_sql/utils/functions/predicate_functions.py` & `py_linq_sql-1.9.1.1/py_linq_sql/utils/functions/predicate_functions.py`

 * *Files identical despite different names*

### Comparing `py_linq_sql-1.9.0.1/pyproject.toml` & `py_linq_sql-1.9.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-linq-sql"
-version = "1.9.0.1"
+version = "1.9.1.1"
 description = "A Python module used for interacting with sql database using LINQ syntax."
 license = "EUPL v1.2"
 authors = ["CHOSSON Ulysse <ulysse.chosson@obspm.fr>"]
 maintainers = ["CHOSSON Ulysse <ulysse.chosson@obspm.fr>", "MARTIN Pierre-Yves <pierre-yves.martin@obspm.fr>"]
 readme = "README.md"
 repository = "https://gitlab.obspm.fr/exoplanet/py-linq-sql"
 documentation = "https://py-linq-sql.readthedocs.io/en/latest/"
@@ -199,8 +199,11 @@
     "objects",
     "satellite",
     "relational_objects",
     "relational_satellite",
     "relational_one_column_objects",
     "relational_array_column_objects",
     "mixed_objects",
-    "rel_objects"]
+    "rel_objects",
+    "test_sc",
+    "test",
+    "test_rel"]
```

### Comparing `py_linq_sql-1.9.0.1/setup.py` & `py_linq_sql-1.9.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'strenum>=0.4.8,<0.5.0',
  'toml>=0.10.2,<0.11.0',
  'types-pyyaml>=6.0.12.1,<7.0.0.0',
  'types-toml>=0.10.8,<0.11.0']
 
 setup_kwargs = {
     'name': 'py-linq-sql',
-    'version': '1.9.0.1',
+    'version': '1.9.1.1',
     'description': 'A Python module used for interacting with sql database using LINQ syntax.',
     'long_description': '<!-- markdownlint-disable-file MD024 MD041 -->\n\n![maintenance](https://img.shields.io/maintenance/yes/2023)\n![open issue](https://img.shields.io/gitlab/issues/open-raw/exoplanet/py-linq-sql?gitlab_url=https%3A%2F%2Fgitlab.obspm.fr)\n\n[![pipeline status](https://gitlab.obspm.fr/exoplanet/py-linq-sql/badges/main/pipeline.svg)](https://gitlab.obspm.fr/exoplanet/py-linq-sql/-/commits/main)\n[![coverage report](https://gitlab.obspm.fr/exoplanet/py-linq-sql/badges/main/coverage.svg)](https://gitlab.obspm.fr/exoplanet/py-linq-sql/-/commits/main)\n\n![Banner](https://py-linq-sql.readthedocs.io/en/latest/banner.png)\n\n# Py-Linq-SQL\n\nA Python module used for interacting with sql database using [LINQ](https://docs.microsoft.com/fr-fr/dotnet/api/system.linq.enumerable?view=net-6.0)\nsyntax. The project is under [EUPL License v1.2](LICENSE.md).\n\nPy-linq-sql allows you to go from (SQLAlchemy using direct text query):\n\n```python\nconn.execute(\n  text(\n    """SELECT "data"->\'obj\'->\'name\' as name """\n    """FROM "objects" """\n    """WHERE "data"->\'obj\'->>\'name\' == "earth" """\n    """AND CAST("data"->\'obj\'->\'mass\' > 0.5 AS Decimal) """\n    """LIMIT 1 OFFSET 2"""\n  )\n)\n```\n\nto the safer and easier to read:\n\n```python\nsqle = (\n  SQLEnumerable(conn, "objects")  # objects is the name of the table\n  .select(lambda x: {"name": x.data.obj.name})  # data is a JSONB column\n  .where(lambda x: x.data.obj.mass > 0.5)  # data is a JSONB column\n  .skip(2)\n  .take(1)  # this is the last part of the query, till there nothing is executed\n  .execute()  # now we ask for the whole query to be executed on the DB server\n)\n```\n\nPro :\n\n- all the query expression are expressed in pure python expression\n- easy support of JSON database using a simple object notation\n- very difficult to have an SQL injection (only the names of the tables are strings)\n- standardized syntax/API of LINQ (used in java, C# and many .net languages)\n- very fast: even very long and complex queries are executed in one single query on the\n  server\n- no need to define a class for every table in the DB as you would do in an ORM here you\n  write query assuming the tables, columns and fields exist, if not then you get a clear\n  error about it\n- results are pylinq Enumerable that are themselves queryable in same way but locally\n- all kinds of join (inner, outer and full, with or without intersections) are easy to\n  use and combine with any kind of query\n\nCons :\n\n- currently only support PostgresQL\n\nAny feedback is welcome see [Contributing](CONTRIBUTING.md).\n\n## Contacts\n\n- Author: Ulysse CHOSSON (LESIA)\n- Maintainer: Ulysse CHOSSON (LESIA)\n- Email: <ulysse.chosson@obspm.fr>\n- Contributors:\n  - Pierre-Yves MARTIN (LESIA)\n\n## Table of Content\n\n- [Py-Linq-SQL](#py-linq-sql)\n  - [Contacts](#contacts)\n  - [Table of Content](#table-of-content)\n  - [Install](#install)\n  - [Implemented functions](#implemented-functions)\n    - [LINQ functions](#linq-functions)\n    - [Custom functions](#custom-functions)\n  - [Not implemented functions](#not-implemented-functions)\n    - [LINQ functions](#linq-functions-1)\n    - [Py-Linq functions](#py-linq-functions)\n  - [Contributing and info for developers](#contributing-and-info-for-developers)\n  - [Full documentation](#full-documentation)\n\n## Install\n\nFor all specific commands to this project, we use [just](https://github.com/casey/just).\n**You need to install it.**\n\nAfter you can install the dependencies:\n\n```bash\n$ just install\npwd\n/home/uchosson/Documents/py-linq-sql\npoetry install --no-dev --remove-untracked\nInstalling dependencies from lock file\nWarning: The lock file is not up to date with the latest changes in pyproject.toml.\nYou may be getting outdated dependencies. Run update to update them.\n\nNo dependencies to install or update\n\nInstalling the current project: py-linq-sql (0.109.0)\n```\n\nAnd if you need to develop the project, install development dependencies:\n\n```bash\n$ just install-all\npwd\n/home/uchosson/Documents/py-linq-sql\npoetry install --remove-untracked\nInstalling dependencies from lock file\nWarning: The lock file is not up to date with the latest changes in pyproject.toml.\nYou may be getting outdated dependencies. Run update to update them.\n\nNo dependencies to install or update\n\nInstalling the current project: py-linq-sql (0.109.0)\nnpm install\n\nup to date, audited 8 packages in 793ms\n\n1 package is looking for funding\n  run `npm fund` for details\n\nfound 0 vulnerabilities\nsudo npm install markdownlint-cli2 --global\n\nchanged 36 packages, and audited 37 packages in 2s\n\n8 packages are looking for funding\n  run `npm fund` for details\n\nfound 0 vulnerabilities\n```\n\nand the pre-commit dependencies:\n\n```bash\n$ just preinstall\npwd\n/home/uchosson/Documents/py-linq-sql\npre-commit clean\nCleaned /home/uchosson/.cache/pre-commit.\npre-commit autoupdate\nUpdating https://github.com/pre-commit/pre-commit-hooks ...\n[INFO] Initializing environment for https://github.com/pre-commit/pre-commit-hooks.\nalready up to date.\nUpdating https://github.com/pre-commit/pre-commit-hooks ... already up to date.\nUpdating https://github.com/pycqa/isort ...\n[INFO] Initializing environment for https://github.com/pycqa/isort.\nalready up to date.\nUpdating https://github.com/ambv/black ...\n[INFO] Initializing environment for https://github.com/ambv/black.\nalready up to date.\nUpdating https://github.com/codespell-project/codespell ...\n[INFO] Initializing environment for https://github.com/codespell-project/codespell.\nalready up to date.\nUpdating https://github.com/sqlfluff/sqlfluff ...\n[INFO] Initializing environment for https://github.com/sqlfluff/sqlfluff.\nupdating 1.1.0 -> 1.2.1.\nUpdating https://github.com/pycqa/flake8 ...\n[INFO] Initializing environment for https://github.com/pycqa/flake8.\nalready up to date.\nUpdating https://github.com/DavidAnson/markdownlint-cli2 ...\n[INFO] Initializing environment for https://github.com/DavidAnson/markdownlint-cli2.\nalready up to date.\npre-commit install --hook-type pre-merge-commit\npre-commit installed at .git/hooks/pre-merge-commit\npre-commit install --hook-type pre-push\npre-commit installed at .git/hooks/pre-push\npre-commit install --hook-type post-rewrite\npre-commit installed at .git/hooks/post-rewrite\npre-commit install-hooks\n[INFO] Installing environment for https://github.com/pre-commit/pre-commit-hooks.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/pycqa/isort.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/ambv/black.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/codespell-project/codespell.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/sqlfluff/sqlfluff.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/pycqa/flake8.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\n[INFO] Installing environment for https://github.com/DavidAnson/markdownlint-cli2.\n[INFO] Once installed this environment will be reused.\n[INFO] This may take a few minutes...\npre-commit install\npre-commit installed at .git/hooks/pre-commit\n```\n\n## Implemented functions\n\n### LINQ functions\n\n[LINQ documentation](https://docs.microsoft.com/fr-fr/dotnet/api/system.linq.enumerable?view=net-6.0)\n\nAll function make before an `.execute()` are executed by the database server.\n\nMDPA = MagicDotPathAggregate\n<!-- markdownlint-disable MD013 -->\n|Method Name           |Description                                                          |Output        |\n|:---------------------|:--------------------------------------------------------------------|:-------------|\n|all                   |Return True if all elements match the predicate.                     |SQLEnumerable |\n|any                   |Return True if any elements match the predicate.                     |SQLEnumerable |\n|avg                   |Aggregation function to get the average of the predicate.            |MDPA          |\n|contains              |Return True if at least one element match the predicate.             |SQLEnumerable |\n|concat                |Aggregation function to concat a predicate.                          |MDPA          |\n|count                 |Return the number of line in a table.                                |SQLEnumerable |\n|count                 |Aggregation function to count a predicate.                           |MDPA          |\n|distinct              |Return all elements that are not duplicate.                          |SQLEnumerable |\n|element_at            |Return the element at the specific index.                            |SQLEnumerable |\n|element_at_or_default |Return the element at the specific index or None if index > len.     |SQLEnumerable |\n|except                |Returns all elements except elements from another SQLEnumerable.     |SQLEnumerable |\n|first                 |Return the first element match the predicate.                        |SQLEnumerable |\n|first_or_default      |Return the first element match the predicate or None if none match.  |SQLEnumerable |\n|group_by              |Return the selection group by a predicate.                           |SQLEnumerable |\n|group_join            |Return the join between 2 selections group by a predicate.           |SQLEnumerable |\n|intersect             |Return the intersection between 2 selections.                        |SQLEnumerable |\n|join                  |Return the join between 2 selections.                                |SQLEnumerable |\n|last                  |Return the last element match the predicate.                         |SQLEnumerable |\n|last_or_default       |Return the last element match the predicate or None if none match.   |SQLEnumerable |\n|max                   |Return the max element.                                              |SQLEnumerable |\n|max                   |Aggregate function to get the max of predicate.                      |MDPA          |\n|min                   |Return the min element.                                              |SQLEnumerable |\n|min                   |Aggregate function to get the min of predicate.                      |MDPA          |\n|order_by              |Return the selection order by key(s).                                |SQLEnumerable |\n|order_by_descending   |Return the selection order by descending by key(s).                  |SQLEnumerable |\n|select                |Return a selection of elements.                                      |SQLEnumerable |\n|single                |Return the only element match the predicate.                         |SQLEnumerable |\n|single_or_default     |Return the only element match the predicate or None if many matches. |SQLEnumerable |\n|skip                  |Return the selection minus _X_ first elements.                       |SQLEnumerable |\n|skip_last             |Return the selection minus _X_ last elements.                        |SQLEnumerable |\n|sum                   |Aggregation function to get the sum of a predicate.                  |MDPA          |\n|take                  |Return _X_ first element of the selection.                           |SQLEnumerable |\n|take_last             |Return _X_ last element of the selection.                            |SQLEnumerable |\n|union                 |Return the union between 2 selections.                               |SQLEnumerable |\n|where                 |Return the selection with all elements match the predicate.          |SQLEnumerable |\n<!-- markdownlint-enable MD013 -->\n\nFor more information see the [detailed documentation](https://py-linq-sql.readthedocs.io/en/latest/api/sqle/sqlenumerable/).\n\n### Custom functions\n\n|Method Name |Description                              |Output                         |\n|:-----------|:----------------------------------------|:------------------------------|\n|delete      |Delete data in a SQL table.              |SQLEnumerable                  |\n|execute     |Execute a request from an SQLEnumerable. |Enumerable | int | bool | dict |\n|insert      |Insert data in a SQL table.              |SQLEnumerable                  |\n|update      |Update data in a table.                  |SQLEnumerable                  |\n\n## Not implemented functions\n\n### LINQ functions\n\n|Method Name      |Description     |\n|:----------------|:---------------|\n|append           |Not implemented |\n|default_if_empty |Not implemented |\n|empty            |Not implemented |\n|prepend          |Not implemented |\n|range            |Not implemented |\n|repeat           |Not implemented |\n|reverse          |Not implemented |\n|select_many      |Not implemented |\n|skip_while       |Not implemented |\n|take_while       |Not implemented |\n|to_dictionary    |Not implemented |\n|to_list          |Not implemented |\n|zip              |Not implemented |\n\n### Py-Linq functions\n\n|Method Name|Description     |\n|:----------|:---------------|\n|add        |Not implemented |\n|median     |Not implemented |\n\n[Py-Linq link](https://viralogic.github.io/py-enumerable)\n\n## Contributing and info for developers\n\n- [Changelog](CHANGELOG.md)\n- [Contributing](CONTRIBUTING.md)\n- [Our git workflow](https://py-linq-sql.readthedocs.io/en/latest/workflow/)\n\n## Full documentation\n\n- [Py-LINQ-SQL Documentation](https://py-linq-sql.readthedocs.io/en/latest/)\n',
     'author': 'CHOSSON Ulysse',
     'author_email': 'ulysse.chosson@obspm.fr',
     'maintainer': 'CHOSSON Ulysse',
     'maintainer_email': 'ulysse.chosson@obspm.fr',
     'url': 'https://gitlab.obspm.fr/exoplanet/py-linq-sql',
```

### Comparing `py_linq_sql-1.9.0.1/PKG-INFO` & `py_linq_sql-1.9.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-linq-sql
-Version: 1.9.0.1
+Version: 1.9.1.1
 Summary: A Python module used for interacting with sql database using LINQ syntax.
 Home-page: https://gitlab.obspm.fr/exoplanet/py-linq-sql
 License: EUPL v1.2
 Keywords: linq,py-linq,sql,database,requests
 Author: CHOSSON Ulysse
 Author-email: ulysse.chosson@obspm.fr
 Maintainer: CHOSSON Ulysse
```

