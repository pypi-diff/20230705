# Comparing `tmp/ocdskingfishercolab-0.3.8.tar.gz` & `tmp/ocdskingfishercolab-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocdskingfishercolab-0.3.8.tar", last modified: Wed Apr 27 14:35:31 2022, max compression
+gzip compressed data, was "ocdskingfishercolab-0.3.9.tar", last modified: Thu Jun 30 18:11:06 2022, max compression
```

## Comparing `ocdskingfishercolab-0.3.8.tar` & `ocdskingfishercolab-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/ocdskingfishercolab/
--rw-r--r--   0 runner    (1001) docker     (121)    19812 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-04-27 14:35:30.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-04-27 14:35:31.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 14:35:30.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-04-27 14:35:30.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-04-27 14:35:31.000000 ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 14:35:31.108187 ocdskingfishercolab-0.3.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)     4608 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/tests/fixtures/flattened.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/tests/fixtures/release_package.json
--rw-r--r--   0 runner    (1001) docker     (121)    10797 2022-04-27 14:35:22.000000 ocdskingfishercolab-0.3.8/tests/test_module.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:06.706023 ocdskingfishercolab-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-06-30 18:11:06.702023 ocdskingfishercolab-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:06.702023 ocdskingfishercolab-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     7900 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2715 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:06.702023 ocdskingfishercolab-0.3.9/ocdskingfishercolab/
+-rw-r--r--   0 runner    (1001) docker     (121)    20817 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:06.702023 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-06-30 18:11:06.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-06-30 18:11:06.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-30 18:11:06.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-06-30 18:11:06.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-30 18:11:06.000000 ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-30 18:11:06.706023 ocdskingfishercolab-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:06.702023 ocdskingfishercolab-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3959 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17770 2022-06-30 18:11:00.000000 ocdskingfishercolab-0.3.9/tests/test_module.py
```

### Comparing `ocdskingfishercolab-0.3.8/LICENSE` & `ocdskingfishercolab-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ocdskingfishercolab-0.3.8/PKG-INFO` & `ocdskingfishercolab-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ocdskingfishercolab
-Version: 0.3.8
+Version: 0.3.9
 Summary: A set of utility functions for Google Colaboratory notebooks using OCDS data
 Home-page: https://github.com/open-contracting/kingfisher-colab
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
@@ -25,9 +24,7 @@
    :target: https://pypi.org/project/ocdskingfishercolab/
 .. |Build Status| image:: https://github.com/open-contracting/kingfisher-colab/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/kingfisher-colab/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/kingfisher-colab/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/kingfisher-colab?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdskingfishercolab.svg
    :target: https://pypi.org/project/ocdskingfishercolab/
-
-
```

### Comparing `ocdskingfishercolab-0.3.8/README.rst` & `ocdskingfishercolab-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `ocdskingfishercolab-0.3.8/docs/Makefile` & `ocdskingfishercolab-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ocdskingfishercolab-0.3.8/docs/changelog.rst` & `ocdskingfishercolab-0.3.9/docs/changelog.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,80 @@
 Changelog
 =========
 
+0.3.9 (Unreleased)
+------------------
+
+Changed
+~~~~~~~
+
+-  :func:`~ocdskingfishercolab.save_dataframe_to_sheet` and :func:`~ocdskingfishercolab.save_dataframe_to_spreadsheet` do nothing if the data frame is empty. :commit:`9b83348`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Rename keyword arguments from ``sql`` to ``print_sql`` and ``sql_only`` to ``return_sql``. :commit:`d706145`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Simplify the query if ``"ALL "`` is prefixed to a field that is not within an array. :commit:`869a9d0`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Raise an error if no ``fields`` are provided. :commit:`8896336`
+
+Fixed
+~~~~~
+
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Use the correct parent table if ``scope`` is not set. Previously, Kingfisher Colab would not use:
+
+   -  ``award_documents``
+   -  ``award_items``
+   -  ``award_suppliers``
+   -  ``contract_documents``
+   -  ``contract_items``
+   -  ``contract_milestones``
+   -  ``contract_implementation_documents``
+   -  ``contract_implementation_milestones``
+   -  ``contract_implementation_transactions``
+
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Construct correct conditions and warnings if a field is within nested arrays. :commit:`3dced1a`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Use the ``relatedprocesses_summary`` table for fields starting with ``relatedProcesses/``, where appropriate. :commit:`9e6cdb7`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: Prefix ``all_`` to the column if ``"ALL "`` is prefixed to the field, to avoid duplicate columns. :commit:`e9427b2`
+-  :func:`~ocdskingfishercolab.calculate_coverage`: No longer warn about ``address`` fields. :commit:`e2b8d72`
+
 0.3.8 (2022-04-27)
 ------------------
 
 Changed
--------
+~~~~~~~
 
 -  Removed dependency on `libcoveocds <https://pypi.org/project/libcoveocds/>`__ (GPL).
 
 0.3.7 (2022-03-11)
 ------------------
 
 Added
 ~~~~~
 
--  Add :meth:`~ocdskingfishercolab.calculate_coverage` to calculate the co-occurence coverage of a group of fields. 
+-  Add :func:`~ocdskingfishercolab.calculate_coverage` to calculate the co-occurence coverage of a group of fields.
 
 0.3.6 (2021-09-15)
 ------------------
 
 Changed
 -------
 
-- :meth:`~ocdskingfishercolab.list_collections`: `source_id` is now an optional argument. If omitted, all collections are returned.
+- :func:`~ocdskingfishercolab.list_collections`: `source_id` is now an optional argument. If omitted, all collections are returned.
 
 0.3.5 (2021-08-09)
 ------------------
 
 Added
 ~~~~~
 
--  Add :meth:`~ocdskingfishercolab.render_json` to render JSON into collapsible HTML. 
+-  Add :func:`~ocdskingfishercolab.render_json` to render JSON into collapsible HTML.
 
 0.3.4 (2021-04-16)
 ------------------
 
 Fixed
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.set_search_path` no longer outputs an error message.
+-  :func:`~ocdskingfishercolab.set_search_path` no longer outputs an error message.
 
 0.3.3 (2021-04-10)
 ------------------
 
 Added
 ~~~~~
 
@@ -74,80 +105,80 @@
 -  Refactor to build upon `ipython-sql <https://pypi.org/project/ipython-sql/>`__.
    Removes several functions that can be replaced with direct usage of ipython-sql magics in the notebook, and replace all remaining sql calls with calls to ipython-sql.
 
    Replacements (must run ``%load_ext sql`` first, and ``%config SqlMagic.autopandas = True`` to get a pandas ``DataFrame``):
 
    -  ``ocdskingfishercolab.create_connection`` — replaced by using an ipython-sql connection string, e.g. ``%sql postgresql://user:pass@host/db``
    -  ``ocdskingfishercolab.execute_statement``, ``ocdskingfishercolab.get_dataframe_from_cursor`` and ``ocdskingfishercolab.get_dataframe_from_query`` — replaced by ipython-sql's ``%sql`` magic, e.g. ``%sql SELECT a FROM b``
-   -  ``ocdskingfishercolab.get_list_from_query`` — replaced by :meth:`ocdskingfishercolab.get_ipython_sql_resultset_from_query`. This returns an `ipython-sql ResultSet <https://pypi.org/project/ipython-sql/#examples>`__, the type returned by the ``%sql%`` magic when ``autopandas`` is off. It behaves like a list, but with extra methods.
-   -  :meth:`ocdskingfishercolab.download_package_from_query` no longer takes a ``params`` argument, and instead uses variables from the local scope, to be consisent with the ipython-sql's ``%sql`` magic.
+   -  ``ocdskingfishercolab.get_list_from_query`` — replaced by :func:`ocdskingfishercolab.get_ipython_sql_resultset_from_query`. This returns an `ipython-sql ResultSet <https://pypi.org/project/ipython-sql/#examples>`__, the type returned by the ``%sql%`` magic when ``autopandas`` is off. It behaves like a list, but with extra methods.
+   -  :func:`ocdskingfishercolab.download_package_from_query` no longer takes a ``params`` argument, and instead uses variables from the local scope, to be consisent with the ipython-sql's ``%sql`` magic.
 
    There's a shared (but not public) `colab notebook of examples run against live kingfisher <https://colab.research.google.com/drive/1cUYY4on72831DPSiQ_JLxJEY2uGTfVrN#scrollTo=I-QPDbliMVXC>`__.
 
--  :meth:`~ocdskingfishercolab.create_connection` creates a new connection if the current connection is closed.
--  :meth:`~ocdskingfishercolab.download_package_from_ocid` orders packaged releases in reverse date order.
--  Remove :meth:`~ocdskingfishercolab.reset_connection`.
+-  :func:`~ocdskingfishercolab.create_connection` creates a new connection if the current connection is closed.
+-  :func:`~ocdskingfishercolab.download_package_from_ocid` orders packaged releases in reverse date order.
+-  Remove :func:`~ocdskingfishercolab.reset_connection`.
 
 Fixed
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.write_data_as_json` replaces path separators with underscores in filenames.
+-  :func:`~ocdskingfishercolab.write_data_as_json` replaces path separators with underscores in filenames.
 
 0.2.2 (2020-04-22)
 ------------------
 
 Added
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.set_search_path`
--  :meth:`~ocdskingfishercolab.get_list_from_query`
+-  :func:`~ocdskingfishercolab.set_search_path`
+-  :func:`~ocdskingfishercolab.get_list_from_query`
 
 Fixed
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.execute_statement` no longer has a mutable default argument value.
+-  :func:`~ocdskingfishercolab.execute_statement` no longer has a mutable default argument value.
 
 0.2.1 (2020-04-21)
 ------------------
 
 Fixed
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.execute_statement` no longer errors if given a ``psycopg2.sql.Composable``.
+-  :func:`~ocdskingfishercolab.execute_statement` no longer errors if given a ``psycopg2.sql.Composable``.
 
 0.2.0 (2020-04-21)
 ------------------
 
 **Upgrade instructions:**
 
 -  Upgrade to 0.1.x if you have not already, and address any deprecation warnings. Then, upgrade to 0.2.x.
 -  Install alembic and SQLAlchemy separately, if used in the notebook.
 
 Added
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.list_source_ids`
--  :meth:`~ocdskingfishercolab.list_collections`
--  :meth:`~ocdskingfishercolab.execute_statement`
--  :meth:`~ocdskingfishercolab.save_dataframe_to_spreadsheet`
--  :meth:`~ocdskingfishercolab.download_data_as_json`
--  :meth:`~ocdskingfishercolab.write_data_as_json`
+-  :func:`~ocdskingfishercolab.list_source_ids`
+-  :func:`~ocdskingfishercolab.list_collections`
+-  :func:`~ocdskingfishercolab.execute_statement`
+-  :func:`~ocdskingfishercolab.save_dataframe_to_spreadsheet`
+-  :func:`~ocdskingfishercolab.download_data_as_json`
+-  :func:`~ocdskingfishercolab.write_data_as_json`
 -  Add a comment to all SQL queries with a link to the notebook, for database administrators.
 
 Changed
 ~~~~~~~
 
 -  **Backwards-incompatible**: The methods deprecated in 0.1.x are removed.
 -  **Backwards-incompatible**: alembic and SQLAlchemy are no longer installed.
 
 Fixed
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.download_package_from_ocid` returns structurally correct records. Previously, the ``ocid`` field was at the package-level instead of the record-level.
--  :meth:`~ocdskingfishercolab.download_package_from_ocid` and :meth:`~ocdskingfishercolab.download_package_from_query` return structurally correct packages. Previously, required fields were omitted.
+-  :func:`~ocdskingfishercolab.download_package_from_ocid` returns structurally correct records. Previously, the ``ocid`` field was at the package-level instead of the record-level.
+-  :func:`~ocdskingfishercolab.download_package_from_ocid` and :func:`~ocdskingfishercolab.download_package_from_query` return structurally correct packages. Previously, required fields were omitted.
 
 0.1.1 (2020-04-20)
 ------------------
 
 Fixed
 ~~~~~
 
@@ -160,29 +191,29 @@
 
 -  Use ``pip install 'ocdskingfishercolab<0.2'`` instead of any previous ``pip install`` command.
 -  Import :mod:`ocdskingfishercolab` instead of ``kingfishercolab``.
 
 Added
 ~~~~~
 
--  :meth:`~ocdskingfishercolab.download_package_from_query`
+-  :func:`~ocdskingfishercolab.download_package_from_query`
 
 Changed
 ~~~~~~~
 
 -  **Backwards-incompatible**: Renamed package from kingfishercolab to ocdskingfishercolab.
 -  Renamed methods for consistent style. Old-style methods are deprecated:
 
-   - ``saveToSheets`` is now :meth:`~ocdskingfishercolab.save_dataframe_to_sheet`
-   - ``saveStraightToSheets`` is now :meth:`~ocdskingfishercolab.save_dataframe_to_sheet` with ``prompt=False``
-   - ``saveToCSV`` is now :meth:`~ocdskingfishercolab.download_dataframe_as_csv`
-   - ``downloadReleases`` is now :meth:`~ocdskingfishercolab.download_package_from_ocid`
-   - ``output_notebook`` is now :meth:`~ocdskingfishercolab.get_dataframe_from_query`
-   - ``getResults`` is now :meth:`~ocdskingfishercolab.get_dataframe_from_cursor`
+   - ``saveToSheets`` is now :func:`~ocdskingfishercolab.save_dataframe_to_sheet`
+   - ``saveStraightToSheets`` is now :func:`~ocdskingfishercolab.save_dataframe_to_sheet` with ``prompt=False``
+   - ``saveToCSV`` is now :func:`~ocdskingfishercolab.download_dataframe_as_csv`
+   - ``downloadReleases`` is now :func:`~ocdskingfishercolab.download_package_from_ocid`
+   - ``output_notebook`` is now :func:`~ocdskingfishercolab.get_dataframe_from_query`
+   - ``getResults`` is now :func:`~ocdskingfishercolab.get_dataframe_from_cursor`
 
--  :meth:`~ocdskingfishercolab.get_dataframe_from_query` raises an error instead of returning an error.
--  :meth:`~ocdskingfishercolab.download_package_from_ocid` raises an error instead of printing a message.
+-  :func:`~ocdskingfishercolab.get_dataframe_from_query` raises an error instead of returning an error.
+-  :func:`~ocdskingfishercolab.download_package_from_ocid` raises an error instead of printing a message.
 
 0.0.1 (2020-04-20)
 ------------------
 
 Initial release.
```

### Comparing `ocdskingfishercolab-0.3.8/docs/conf.py` & `ocdskingfishercolab-0.3.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "OCDS Kingfisher Colab"
 copyright = "2019, Open Contracting Partnership"
 author = "Open Contracting Partnership"
 
 # The short X.Y version
-version = "0.3.8"
+version = "0.3.9"
 # The full version, including alpha/beta/rc tags
 release = version
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
@@ -75,10 +75,11 @@
 autodoc_type_aliases = {}
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
 }
 
 extlinks = {
+    "commit": ("https://github.com/open-contracting/kingfisher-colab/commit/%s", "%s"),
     "ipython-sql": (
         "https://github.com/catherinedevlin/ipython-sql/blob/b24ac6e9410416eafde86ae22fd8d6f34acbe05d/%s", None),
 }
```

### Comparing `ocdskingfishercolab-0.3.8/docs/index.rst` & `ocdskingfishercolab-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ocdskingfishercolab-0.3.8/ocdskingfishercolab/__init__.py` & `ocdskingfishercolab-0.3.9/ocdskingfishercolab/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,53 +3,61 @@
 import textwrap
 import warnings
 from urllib.parse import urljoin
 
 import flattentool
 import google.auth
 import gspread
+import httplib2
 import requests
 import sql
+from gspread_dataframe import set_with_dataframe
+from IPython import get_ipython
+from IPython.display import HTML
+from notebook import notebookapp
+from oauth2client.client import GoogleCredentials
+from oauth2client.contrib.gce import AppAssertionCredentials
+from pydrive2.auth import GoogleAuth
+from pydrive2.drive import GoogleDrive
 from sqlalchemy.exc import ResourceClosedError
 
 try:
     from google.colab import auth, files
 except ImportError:
     # Assume we are in a testing environment.
     from unittest.mock import Mock
 
     files = Mock()
     files.download.return_value = None
 
-from gspread_dataframe import set_with_dataframe
-from IPython import get_ipython
-from IPython.display import HTML
-from notebook import notebookapp
-from oauth2client.client import GoogleCredentials
-from pydrive2.auth import GoogleAuth
-from pydrive2.drive import GoogleDrive
-
-# Monkeypatch ipython-sql's sql run function, to add a comment linking to the
-# colab notebook that it's run from
-# We monkeypatch run(), but don't call it directly below, as calling the magic
-# will handle connections for us.
+# Patch ipython-sql to add a comment to all SQL queries.
 old_run = sql.run.run
+# Patch PyDrive2 like at: https://github.com/googlecolab/colabtools/blob/main/google/colab/_import_hooks/_pydrive.py
+old_local_webserver_auth = GoogleAuth.LocalWebserverAuth
 
 
 def run(conn, _sql, *args, **kwargs):
     try:
         comment = f'/* https://colab.research.google.com/drive/{_notebook_id()} */'
     except KeyError:
         comment = "/* run from a notebook, but no colab id */"
     return old_run(conn, comment + _sql, *args, **kwargs)
 
 
-sql.run.run = run
+def LocalWebServerAuth(self, *args, **kwargs):
+    if isinstance(self.credentials, AppAssertionCredentials):
+        self.credentials.refresh(httplib2.Http())
+        return
+    return old_local_webserver_auth(self, *args, **kwargs)
+
 
+sql.run.run = run
+GoogleAuth.LocalWebserverAuth = LocalWebServerAuth
 
+# A global variable used in set_spreadsheet_name() and save_dataframe_to_sheet().
 spreadsheet_name = None
 
 # Use the same placeholder values as OCDS Kit.
 package_metadata = {
     'uri': 'placeholder:',
     'publisher': {
         'name': '',
@@ -159,15 +167,19 @@
 
     Use :meth:`ocdskingfishercolab.set_spreadsheet_name` to set the spreadsheet name.
 
     :param pandas.DataFrame dataframe: a data frame
     :param str sheetname: a sheet name
     :param bool prompt: whether to prompt the user
     """
-    if prompt is False or input('Save to Google Sheets? (y/N)') == 'y':
+    if dataframe.empty:
+        print('Data frame is empty.')
+        return
+
+    if not prompt or input('Save to Google Sheets? (y/N)') == 'y':
         gc = authenticate_gspread()
         try:
             sheet = gc.open(spreadsheet_name)
         except gspread.SpreadsheetNotFound:
             sheet = gc.create(spreadsheet_name)
 
         try:
@@ -183,14 +195,18 @@
     """
     Dumps the ``release_package`` column of a data frame to a JSON file, converts the JSON file to an Excel file,
     and uploads the Excel file to Google Drive.
 
     :param pandas.DataFrame dataframe: a data frame
     :param str name: the basename of the Excel file to write
     """
+    if dataframe.empty:
+        print('Data frame is empty.')
+        return
+
     write_data_as_json(dataframe['release_package'][0], 'release_package.json')
 
     with warnings.catch_warnings():
         warnings.filterwarnings('ignore')  # flattentool uses UserWarning, so we can't set a specific category
 
         flattentool.flatten(
             'release_package.json',
@@ -226,34 +242,30 @@
     :param data: JSON-serializable data
     :param str filename: a file name
     """
     write_data_as_json(data, filename)
     files.download(filename)
 
 
-def get_ipython_sql_resultset_from_query(sql):
+# We need to add the local variables from its callers, so that `run_line_magic` finds them among locals. This module's
+# local variables are prefixed with "_", to avoid shadowing local variables in the notebook's cells.
+def get_ipython_sql_resultset_from_query(sql, _collection_id=None, _ocid=None):
     """
     Executes a SQL statement and returns a ResultSet.
 
     Parameters are taken from the scope this function is called from (same behaviour as ipython-sql's ``%sql`` magic).
 
     :param str sql: a SQL statement
     :returns: the results as a :ipython-sql:`ResultSet<src/sql/run.py#L99>`
     :rtype: sql.run.ResultSet
     """
     ipython = get_ipython()
     autopandas = ipython.run_line_magic('config', 'SqlMagic.autopandas')
-    # Disable autopandas, so we know that the sql magic call will always return
-    # a ResultSet (rather than a pandas DataFrame). Since the DataFrame would
-    # be created from the ResultSet, it would be less efficient.
     if autopandas:
         ipython.run_line_magic('config', 'SqlMagic.autopandas = False')
-    # Use ipython.run_line_magic instead of ipython.magic here
-    # to get variables from the scope of the ipython cell,
-    # instead of the scope in this function.
     results = ipython.run_line_magic('sql', sql)
     if autopandas:
         ipython.run_line_magic('config', 'SqlMagic.autopandas = True')
     return results
 
 
 def download_package_from_query(sql, package_type=None):
@@ -264,15 +276,15 @@
     :param str sql: a SQL statement
     :param str package_type: "record" or "release"
     :raises UnknownPackageTypeError: when the provided package type is unknown
     """
     if package_type not in ('record', 'release'):
         raise UnknownPackageTypeError("package_type argument must be either 'release' or 'record'")
 
-    data = [row[0] for row in get_ipython_sql_resultset_from_query(sql)]
+    data = _pluck(sql)
 
     if package_type == 'record':
         package = {'records': data}
     elif package_type == 'release':
         package = {'releases': data}
 
     package.update(package_metadata)
@@ -292,31 +304,19 @@
     if package_type not in ('record', 'release'):
         raise UnknownPackageTypeError("package_type argument must be either 'release' or 'record'")
 
     sql = """
     SELECT data
     FROM data
     JOIN release ON data.id = release.data_id
-    WHERE collection_id = :collection_id AND ocid = :ocid
+    WHERE collection_id = :_collection_id AND ocid = :_ocid
     ORDER BY data->>'date' DESC
     """
 
-    ipython = get_ipython()
-    autopandas = ipython.run_line_magic('config', 'SqlMagic.autopandas')
-    # Disable autopandas, so we know that the sql magic call will always return
-    # a ResultSet (rather than a pandas DataFrame). Since the DataFrame would
-    # be created from the ResultSet, it would be less efficient.
-    if autopandas:
-        ipython.run_line_magic('config', 'SqlMagic.autopandas = False')
-    # This inspects locals to find `ocid` and `collection_id`.
-    results = ipython.run_line_magic('sql', sql)
-    if autopandas:
-        ipython.run_line_magic('config', 'SqlMagic.autopandas = True')
-
-    data = [row[0] for row in results]
+    data = _pluck(sql, _collection_id=collection_id, _ocid=ocid)
 
     if package_type == 'record':
         package = {'records': [{'ocid': ocid, 'releases': data}]}
     elif package_type == 'release':
         package = {'releases': data}
 
     package.update(package_metadata)
@@ -343,14 +343,27 @@
     drive = authenticate_pydrive()
     drive_file = drive.CreateFile(metadata)
     drive_file.SetContentFile(filename)
     drive_file.Upload()
     return drive_file
 
 
+def _pluck(sql, **kwargs):
+    return [row[0] for row in get_ipython_sql_resultset_from_query(sql, **kwargs)]
+
+
+def _all_tables():
+    tables = set()
+    for column, table in (('viewname', 'pg_views'), ('tablename', 'pg_tables')):
+        tables.update(_pluck(
+            f"SELECT {column} FROM pg_catalog.{table} WHERE schemaname = ANY(CURRENT_SCHEMAS(false))"
+        ))
+    return tables
+
+
 def render_json(json_string):
     """
     Renders JSON into collapsible HTML.
 
     :param json_string: JSON-deserializable string
     """
     if not isinstance(json_string, str):
@@ -363,179 +376,210 @@
         renderjson.set_show_to_level(1)
         document.body.appendChild(renderjson({json_string}))
         new ResizeObserver(google.colab.output.resizeIframeToContent).observe(document.body)
         </script>
         """)
 
 
-def calculate_coverage(fields, scope=None, sql=True, sql_only=False):
+def calculate_coverage(fields, scope=None, print_sql=True, return_sql=False):
     """
     Calculates the coverage of one or more fields using the summary tables produced by Kingfisher Summarize's
-    `--field-lists` option. Returns the coverage of each field and the co-occurrence coverage of all the fields.
+    ``--field-lists`` option. Returns the coverage of each field and the co-occurrence coverage of all fields.
 
-    `scope` is the Kingfisher Summarize table to measure coverage against, e.g. `awards_summary`.
-    The number of rows in this table is used as the denominator when calculating the coverage.
+    ``scope`` is the Kingfisher Summarize table to measure coverage against, e.g. ``"awards_summary"``.
+    Coverage is calculated using the number of rows in this table as the denominator.
 
-    `fields` is a list of fields to measure the coverage of, specified using JSON Pointer.
+    If ``scope`` is not set, it defaults to the parent table of the first field.
 
-    To specify fields that are children of the scope table, you can use either an absolute pointer or a relative
-    pointer prefixed with `:`, e.g. if `scope` is set to 'awards_summary', then `awards/value/amount` and
-    `:value/amount` refer to the same field. Coverage of such fields is measured against the number of rows
-    in the `scope` table.
+    ``fields`` is a list of fields to measure the coverage of, specified using JSON Pointer.
 
-    To specify fields that are not children of the scope table, use an absolute path,
-    e.g. `tender/procurementMethod`. Coverage of such fields is measured against the number of releases/records.
+    If a field isn't a child of the ``scope`` table, use an absolute pointer:
 
-    For arrays, a field is counted if it appears in **any** object in the array,
-    e.g. if `scope` is set to `awards_summary` and `field` is set to `:items/description`,
-    at least one item must have a description for the coverage to be non-zero.
+    .. code-block:: python
 
-    To specify that a field must appear in **all** objects in the array, prepend the field with `ALL `,
-    e.g. if `scope` is set to `awards_summary` and `field` is set to `ALL :items/description`,
-    all items must have a description for the coverage to be non-zero.
+       calculate_coverage(["tender/procurementMethod"], "awards_summary")
 
-    If `scope` is set to `awards_summary`, specify fields on related contracts by prefixing the path with
-    `:contracts/`, e.g. to measure how many awards have a value and a related contract with a period, set `scope`
-    to `awards` and `fields` to `[':value', ':contracts/period']`. Similarly, if `scope` is set to
-    `contracts_summary`, specify fields on related awards by prefixing the path with `:awards/`.
+    If a field is a child of the ``scope`` table, use either an absolute pointer:
 
+    .. code-block:: python
 
-    :param list fields: a list of fields as described above.
-    :param str scope: table name as described above; defaults to the parent table of the first item in the fields list.
-    :param bool sql: print the SQL query generated by the function.
+       calculate_coverage(["awards/value/amount"], "awards_summary")
 
-    :returns: the coverage of each field and the co-occurrence coverage of all the fields as a pandas DataFrame or an
-                  ipython-sql :ipython-sql:`ResultSet<src/sql/run.py#L99>`, depending on whether
-                  ``%config SqlMagic.autopandas`` is ``True`` or ``False`` respectively. This is the same behaviour as
-                  ipython-sql's ``%sql`` magic.
-    :rtype: pandas.DataFrame or sql.run.ResultSet
-    """
+    Or a relative pointer (prepend with ``":"``):
 
-    def get_all_tables():
-        views = get_ipython_sql_resultset_from_query(
-            "SELECT viewname FROM pg_catalog.pg_views WHERE schemaname = ANY (CURRENT_SCHEMAS(false))"
-        )
-        tables = get_ipython_sql_resultset_from_query(
-            "SELECT tablename FROM pg_catalog.pg_tables WHERE schemaname = ANY (CURRENT_SCHEMAS(false))"
-        )
-        return [x[0] for x in list(views) + list(tables)]
+    .. code-block:: python
 
-    def get_table_and_path(field, scope_table):
+       calculate_coverage([":value/amount"], "awards_summary")
 
-        if field.startswith(':'):
-            return scope_table, field[1:]
+    If a field is within an array, it counts if it appears in **any** object in the array.
 
-        path = field.split("/")
-        table_candidates = [
-            "_".join(path[:-i]) for i in reversed(range(1, len(path)))
-        ]
-        table = "release_summary"
+    .. code-block:: python
 
-        for num, table_candidate in enumerate(table_candidates):
-            if scope_table[:-8] == table_candidate:  # remove "_summary" from `scope_table`
-                path = path[num+1:]
-                table = scope_table
-                break
-        return table, "/".join(path)
+       calculate_coverage([":items/description"], "awards_summary")
 
-    def get_scope_table(field):
+    To require a field to appear in **all** objects in the array, prepend with ``"ALL "``:
 
-        all_tables = get_all_tables()
-        path = field.split("/")
-        table_candidates = {
-            "_".join(path[:-i]) for i in range(1, len(path))
-        }
-        table = "release"
-
-        for table_candidate in table_candidates:
-            if f"{table_candidate}_summary" in all_tables:
-                table = table_candidate
-        return f"{table}_summary"
-
-    def coverage_wrapper(condition, field):
-        field_name = field.replace("/", "_").replace(" ", "_").lower()
-        return f"ROUND(SUM(CASE WHEN {condition} THEN 1 ELSE 0 END) * 100.0 / count(*), 2) AS {field_name}_percentage"
-
-    def any_condition(field, current_scope_table):
-        return f"{current_scope_table}.field_list ? '{field}'"
-
-    def all_condition(field, current_scope_table):
-        split_field = field.split("/")
-        one_to_manys = [field for field in split_field[:-1] if field.endswith("s")]
+    .. code-block:: python
 
-        if not one_to_manys:
-            nearest_parent_one_to_many = split_field[0]
-        else:
-            nearest_parent_one_to_many = one_to_manys[-1]
+       calculate_coverage(["ALL :items/description"], "awards_summary")
+
+    .. note::
+
+       Nested arrays, like the ``"awards/items/description"`` field with a ``"release_summary"`` scope, will yield
+       inaccurate results, unless the initial arrays are present and one-to-one with the scope table (i.e. there is
+       always exactly one award for each release).
+
+    If ``scope`` is ``"awards_summary"``, you can specify fields on related contracts by prepending ``":contracts/"``:
+
+    .. code-block:: python
+
+       calculate_coverage([":value/amount", ":contracts/period"], "awards_summary")
+
+    If ``scope`` is ``"contracts_summary"``, you can specify fields on related awards by prepending ``":awards/"``:
+
+    .. code-block:: python
+
+       calculate_coverage([":value/amount", ":awards/date"], "contracts_summary")
 
-        if len(one_to_manys) > 1:
+    :param list fields: the fields to measure coverage of
+    :param str scope: the table to measure coverage against
+    :param bool print_sql: print the SQL query
+    :param bool return_sql: return the SQL query instead of executing the SQL query and returning the results
+
+    :returns: the results as a pandas DataFrame or an ipython-sql :ipython-sql:`ResultSet<src/sql/run.py#L99>`,
+              depending on whether ``%config SqlMagic.autopandas`` is ``True`` or ``False`` respectively. This is the
+              same behaviour as ipython-sql's ``%sql`` magic.
+    :rtype: pandas.DataFrame or sql.run.ResultSet
+    """
+
+    head_replacements = {
+        "awards": "award",
+        "contracts": "contract",
+    }
+
+    def get_table_and_pointer(tables, pointer):
+        parts = pointer.split("/")
+        table = "release_summary"
+
+        # Abbreviate absolute pointers to relative pointers if the pointer is on the scope table.
+        # For example: "awards/date" to "date" if the scope is "awards_summary."
+        for i in range(len(parts), 0, -1):
+            head = parts[0]
+            # Kingfisher Summarize uses the singular prefixes "award_" and "contract_".
+            if i > 1:
+                head = head_replacements.get(head, head)
+            # Kingfisher Summarize tables are lowercase.
+            candidate = f"{'_'.join([head] + parts[1:i])}_summary".lower()
+            if candidate in tables:
+                parts = parts[i:]
+                table = candidate
+                break
+
+        return table, "/".join(parts)
+
+    # https://www.postgresql.org/docs/11/functions-json.html
+    def get_condition(table, pointer, mode):
+        # Test for the presence of the field in any object.
+        if mode == "any":
+            return f"{table}.field_list ? '{pointer}'"
+
+        # The logic from here is for mode == "all".
+        parts = pointer.split("/")
+
+        # It would be more robust to analyze the release schema. That said, as of OCDS 1.1.5, all arrays of objects
+        # end in "s", and only one object ends in "s" ("address").
+        array_indices = [i for i, part in enumerate(parts[:-1]) if part.endswith("s") and part != "address"]
+
+        # If the field is not within an array, simplify the logic from ALL to ANY.
+        if not array_indices:
+            return f"{table}.field_list ? '{pointer}'"
+
+        # If arrays are nested, then the condition below can be satisfied for, e.g., awards/items/description, if there
+        # are 2 awards, only one of which sets items/description.
+        if len(array_indices) > 1:
             print(
-                f"""WARNING: The results of this query might be inacurate, you will need to check that
-                 `{', '.join(one_to_manys[:-1])}` fields are one to one with `{current_scope_table[:-8]}`
-                 and that `{', '.join(one_to_manys[:-1])}` exists for all `{current_scope_table[:-8]}` """
+                'WARNING: Results might be inaccurate due to nested arrays. Check that there is exactly one '
+                f"`{'/'.join(parts[:array_indices[-2] + 1])}` path per {table} row."
             )
 
-        return f"""coalesce({current_scope_table}.field_list ->> '{field}' =
-                  {current_scope_table}.field_list ->> '{nearest_parent_one_to_many}', false)"""
+        # Test whether the number of occurrences of the path and its closest enclosing array are equal.
+        return (
+            f"coalesce({table}.field_list->>'{pointer}' =\n"
+            f"                  {table}.field_list->>'{'/'.join(parts[:array_indices[-1] + 1])}', false)"
+        )
 
-    def release_summary_join(scope_table, join_to_release):
-        if not join_to_release:
-            return ""
-        return f"""JOIN
-        release_summary ON release_summary.id = {scope_table}.id"""
+    if not fields:
+        raise MissingFieldsError("You must provide a list of fields as the first argument to `calculate_coverage`.")
 
+    # Default to the parent table of the first field.
     if not scope:
-        field = fields[0].split()[-1]
-        scope = get_scope_table(field)
-
-    scope_table = scope
-
-    join_to_release = False
+        scope, _ = get_table_and_pointer(_all_tables(), fields[0].split()[-1])
 
+    columns = {}
     conditions = []
+    join = ""
+    for field in fields:
+        split = field.split()
+        pointer = split[-1]
 
-    query_parts = []
+        # If the first token isn't "ALL" or if there are more than 2, behave as if only the last token was provided.
+        if len(split) == 2 and split[0].lower() == "all":
+            mode = "all"
+        else:
+            mode = "any"
 
-    for field in fields:
-        split_field = field.split()
-        field_name = split_field[-1]
+        # Handle relative pointers. This includes `:awards` and `:contracts` (see Kingfisher Summarize).
+        if pointer.startswith(":"):
+            table, pointer = scope, pointer[1:]
+        # Handle absolute pointers.
+        else:
+            table, pointer = get_table_and_pointer({scope}, pointer)
 
-        table, path = get_table_and_path(field_name, scope)
+        condition = get_condition(table, pointer, mode)
 
-        if table == "release_summary" and scope_table != "release_summary":
-            join_to_release = True
+        # Add a JOIN clause for the release_summary table, unless it is already in the FROM clause.
+        if table == "release_summary" and scope != "release_summary":
+            join = f"JOIN\n            release_summary ON release_summary.id = {scope}.id"
 
-        if len(split_field) == 2 and split_field[0].lower() == "all":
-            condition = all_condition(path, table)
-        else:
-            condition = any_condition(path, table)
+        # Add the field coverage.
+        alias = pointer.replace("/", "_").lower()
+        if mode == "all":
+            alias = f"all_{alias}"
+        columns[alias] = condition
 
+        # Collect the conditions for co-occurrence coverage.
         conditions.append(condition)
-        query_parts.append(coverage_wrapper(condition, path))
 
-    query_parts.append(
-        coverage_wrapper(" AND \n              ".join(conditions), "total")
-    )
+    # Add the co-occurrence coverage.
+    columns["total"] = " AND\n                ".join(conditions)
 
-    select = ",\n            ".join(query_parts)
-    select = textwrap.dedent(f"""
+    select = ",\n            ".join(
+        f"ROUND(SUM(CASE WHEN {condition} THEN 1 ELSE 0 END) * 100.0 / count(*), 2) AS {alias}_percentage"
+        for alias, condition in columns.items()
+    )
+    sql = textwrap.dedent(f"""\
         SELECT
             count(*) AS total_{scope},
             {select}
-        FROM
-        {scope_table}
-        {release_summary_join(scope_table, join_to_release)}
+        FROM {scope}
+        {join}
     """)
 
-    if sql:
-        print(select)
-    if sql_only:
-        return select
-    return get_ipython().run_cell_magic("sql", "", select)
+    if print_sql:
+        print(sql)
+
+    if return_sql:
+        return sql
+
+    return get_ipython().run_cell_magic("sql", "", sql)
 
 
 class OCDSKingfisherColabError(Exception):
     """Base class for exceptions from within this package"""
 
 
 class UnknownPackageTypeError(OCDSKingfisherColabError, ValueError):
     """Raised when the provided package type is unknown"""
+
+
+class MissingFieldsError(OCDSKingfisherColabError):
+    """Raised when no fields are provided to a function"""
```

### Comparing `ocdskingfishercolab-0.3.8/ocdskingfishercolab.egg-info/PKG-INFO` & `ocdskingfishercolab-0.3.9/ocdskingfishercolab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: ocdskingfishercolab
-Version: 0.3.8
+Version: 0.3.9
 Summary: A set of utility functions for Google Colaboratory notebooks using OCDS data
 Home-page: https://github.com/open-contracting/kingfisher-colab
 Author: Open Contracting Partnership
 Author-email: data@open-contracting.org
 License: BSD
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE
@@ -25,9 +24,7 @@
    :target: https://pypi.org/project/ocdskingfishercolab/
 .. |Build Status| image:: https://github.com/open-contracting/kingfisher-colab/workflows/CI/badge.svg
    :target: https://github.com/open-contracting/kingfisher-colab/actions?query=workflow%3ACI
 .. |Coverage Status| image:: https://coveralls.io/repos/github/open-contracting/kingfisher-colab/badge.svg?branch=main
    :target: https://coveralls.io/github/open-contracting/kingfisher-colab?branch=main
 .. |Python Version| image:: https://img.shields.io/pypi/pyversions/ocdskingfishercolab.svg
    :target: https://pypi.org/project/ocdskingfishercolab/
-
-
```

### Comparing `ocdskingfishercolab-0.3.8/setup.py` & `ocdskingfishercolab-0.3.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='ocdskingfishercolab',
-    version='0.3.8',
+    version='0.3.9',
     author='Open Contracting Partnership',
     author_email='data@open-contracting.org',
     url='https://github.com/open-contracting/kingfisher-colab',
     description='A set of utility functions for Google Colaboratory notebooks using OCDS data',
     license='BSD',
     packages=find_packages(exclude=['tests', 'tests.*']),
     long_description=long_description,
@@ -17,14 +17,15 @@
     # google-colab on PyPI has different requirements than google-colab on Google Colaboratory. It's not possible to
     # list a set of requirements that pip can resolve in both environments.
     install_requires=[
         'flattentool',
         'google-auth',
         'gspread',
         'gspread-dataframe',
+        'httplib2',
         'ipython',
         'ipython-sql~=0.4.0',  # Google Colaboratory uses 0.3.x
         'notebook',
         'oauth2client',
         'pydrive2',
         'requests',
         'sqlalchemy',
```

### Comparing `ocdskingfishercolab-0.3.8/tests/conftest.py` & `ocdskingfishercolab-0.3.9/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,27 +57,29 @@
 
             cur.execute("INSERT INTO record VALUES (1, 1, 'ocds-213czf-2', 4)")
             cur.execute("""INSERT INTO data VALUES (4, '{"ocid":"ocds-213czf-2","""
                         """"releases":[{"ocid":"ocds-213czf-2"}]}'::jsonb)""")
 
             conn.commit()
 
-            get_ipython().run_line_magic('load_ext', 'sql')
-            get_ipython().run_line_magic('sql', created_database_url)
-            # Set autopandas, because we think most users will want it.
-            get_ipython().run_line_magic('config', 'SqlMagic.autopandas = True')
+            ipython = get_ipython()
+            ipython.run_line_magic('load_ext', 'sql')
+            ipython.run_line_magic('sql', created_database_url)
+            # Avoid "KeyError: 'DEFAULT'" in some test environments.
+            # https://github.com/catherinedevlin/ipython-sql/issues/129
+            ipython.run_line_magic('config', 'SqlMagic.style = "NONE"')
+            ipython.run_line_magic('config', 'SqlMagic.autopandas = True')
 
             yield cur
         finally:
             cur.close()
             conn.close()
     finally:
-        # Close ipython-sql's open connections, so that we can drop the database.
-        # We have to do this manually, because ipython-sql's own connection
-        # closing support is broken
+        # Close ipython-sql's open connections, to be able to drop the database.
+        # ipython-sql's own connection closing logic is broken.
         # https://github.com/catherinedevlin/ipython-sql/issues/170
         for ipython_sql_connection in sql.connection.Connection.connections.values():
             ipython_sql_connection.session.close()
             ipython_sql_connection.session.engine.dispose()
         sql.connection.Connection.connections = {}
 
         cursor.execute('DROP DATABASE ocdskingfishercolab_test')
```

