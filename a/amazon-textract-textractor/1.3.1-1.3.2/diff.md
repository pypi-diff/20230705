# Comparing `tmp/amazon-textract-textractor-1.3.1.tar.gz` & `tmp/amazon-textract-textractor-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-textractor-1.3.1.tar", last modified: Wed May 24 03:35:03 2023, max compression
+gzip compressed data, was "amazon-textract-textractor-1.3.2.tar", last modified: Wed Jul  5 19:39:16 2023, max compression
```

## Comparing `amazon-textract-textractor-1.3.1.tar` & `amazon-textract-textractor-1.3.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-05-24 03:34:55.000000 amazon-textract-textractor-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.892584 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 03:35:03.000000 amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.892584 amazon-textract-textractor-1.3.1/extras/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/pandas.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/pdf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/extras/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.896584 amazon-textract-textractor-1.3.1/textractor/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/document_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/expense_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/expense_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/identity_document.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/identity_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/key_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/lazy_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/line.py
--rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/selection_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/table_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/entities/word.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35542 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/parsers/response_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    37612 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/textractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/utils/search_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 03:35:03.900584 amazon-textract-textractor-1.3.1/textractor/visualizers/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/arial.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-05-24 03:34:56.000000 amazon-textract-textractor-1.3.1/textractor/visualizers/entitylist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.574718 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 19:39:16.000000 amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.574718 amazon-textract-textractor-1.3.2/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/extras/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/extras/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/extras/pandas.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/extras/pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/extras/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.574718 amazon-textract-textractor-1.3.2/textractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.574718 amazon-textract-textractor-1.3.2/textractor/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15145 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.574718 amazon-textract-textractor-1.3.2/textractor/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/textractor/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30720 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/document_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/expense_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/expense_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/identity_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/identity_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/key_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/lazy_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34524 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/selection_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23273 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11729 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/table_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/table_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/table_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/entities/word.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/textractor/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35602 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/parsers/response_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37684 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/textractor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/textractor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/utils/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/utils/search_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 19:39:16.578718 amazon-textract-textractor-1.3.2/textractor/visualizers/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/visualizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   367112 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/visualizers/arial.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    42343 2023-07-05 19:39:09.000000 amazon-textract-textractor-1.3.2/textractor/visualizers/entitylist.py
```

### Comparing `amazon-textract-textractor-1.3.1/LICENSE` & `amazon-textract-textractor-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/PKG-INFO` & `amazon-textract-textractor-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.3.1/README.md` & `amazon-textract-textractor-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/PKG-INFO` & `amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-textract-textractor
-Version: 1.3.1
+Version: 1.3.2
 Summary: A package to use AWS Textract services.
 Home-page: https://github.com/aws-samples/amazon-textract-textractor
 License: Apache 2.0
 Keywords: amazon textract aws ocr document
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/SOURCES.txt` & `amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/amazon_textract_textractor.egg-info/requires.txt` & `amazon-textract-textractor-1.3.2/amazon_textract_textractor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/setup.py` & `amazon-textract-textractor-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         requirements = [line for line in f.readlines()]
     return requirements
 
 
 setup(
     # include data files
     name="amazon-textract-textractor",
-    version="1.3.1",
+    version="1.3.2",
     license="Apache 2.0",
     description="A package to use AWS Textract services.",
     url="https://github.com/aws-samples/amazon-textract-textractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `amazon-textract-textractor-1.3.1/textractor/cli/cli.py` & `amazon-textract-textractor-1.3.2/textractor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/data/constants.py` & `amazon-textract-textractor-1.3.2/textractor/data/constants.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/bbox.py` & `amazon-textract-textractor-1.3.2/textractor/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/document.py` & `amazon-textract-textractor-1.3.2/textractor/entities/document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/document_entity.py` & `amazon-textract-textractor-1.3.2/textractor/entities/document_entity.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/expense_document.py` & `amazon-textract-textractor-1.3.2/textractor/entities/expense_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/expense_field.py` & `amazon-textract-textractor-1.3.2/textractor/entities/expense_field.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/identity_document.py` & `amazon-textract-textractor-1.3.2/textractor/entities/identity_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/key_value.py` & `amazon-textract-textractor-1.3.2/textractor/entities/key_value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/lazy_document.py` & `amazon-textract-textractor-1.3.2/textractor/entities/lazy_document.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/line.py` & `amazon-textract-textractor-1.3.2/textractor/entities/line.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/page.py` & `amazon-textract-textractor-1.3.2/textractor/entities/page.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/query.py` & `amazon-textract-textractor-1.3.2/textractor/entities/query.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/query_result.py` & `amazon-textract-textractor-1.3.2/textractor/entities/query_result.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/selection_element.py` & `amazon-textract-textractor-1.3.2/textractor/entities/selection_element.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/signature.py` & `amazon-textract-textractor-1.3.2/textractor/entities/signature.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/table.py` & `amazon-textract-textractor-1.3.2/textractor/entities/table.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/table_cell.py` & `amazon-textract-textractor-1.3.2/textractor/entities/table_cell.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/table_footer.py` & `amazon-textract-textractor-1.3.2/textractor/entities/table_footer.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/table_title.py` & `amazon-textract-textractor-1.3.2/textractor/entities/table_title.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/value.py` & `amazon-textract-textractor-1.3.2/textractor/entities/value.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/entities/word.py` & `amazon-textract-textractor-1.3.2/textractor/entities/word.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/exceptions.py` & `amazon-textract-textractor-1.3.2/textractor/exceptions.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/parsers/response_parser.py` & `amazon-textract-textractor-1.3.2/textractor/parsers/response_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,14 +934,16 @@
             line_item_rows = []
             for i, line_item in enumerate(line_items_group["LineItems"]):
                 row_expenses = []
                 for line_item_field in line_item["LineItemExpenseFields"]:
                     row_expenses.append(create_expense_from_field(line_item_field, page))
                     row_expenses[-1].raw_object = line_item_field
                 line_item_rows.append(LineItemRow(index=i, line_item_expense_fields=row_expenses, page=page.page_num))
+            if not line_item_rows:
+                continue
             line_items_groups.append(LineItemGroup(index=line_items_group["LineItemGroupIndex"], line_item_rows=line_item_rows, page=page.page_num))
 
         bbox = BoundingBox.enclosing_bbox(bboxes=[s.bbox for s in summary_fields] + [g.bbox for g in line_items_groups], spatial_object=page)
         expense_document = ExpenseDocument(
             summary_fields=summary_fields, line_items_groups=line_items_groups, bounding_box=bbox, page=page.page_num
         )
         expense_document.raw_object = doc
```

### Comparing `amazon-textract-textractor-1.3.1/textractor/textractor.py` & `amazon-textract-textractor-1.3.2/textractor/textractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
             or isinstance(file_source, Image.Image)
         ):
             raise InputError(
                 f"file_source needs to be of type str, bytes or PIL Image, not {type(file_source)}"
             )
 
         # If the file is not already in S3
-        if not file_source.startswith("s3://"):
+        if not isinstance(file_source, str) or not file_source.startswith("s3://"):
             # Check if the user has given us a bucket to upload to
             if not s3_upload_path:
                 raise InputError(
                     f"For files not in S3, an S3 upload path must be provided"
                 )
 
             s3_file_path = os.path.join(s3_upload_path, str(uuid.uuid4()))
@@ -756,15 +756,15 @@
             or isinstance(file_source, Image.Image)
         ):
             raise InputError(
                 f"file_source needs to be of type str, bytes or PIL Image, not {type(file_source)}"
             )
 
         # If the file is not already in S3
-        if not file_source.startswith("s3://"):
+        if not isinstance(file_source, str) or not file_source.startswith("s3://"):
             # Check if the user has given us a bucket to upload to
             if not s3_upload_path:
                 raise InputError(
                     f"For files not in S3, an S3 upload path must be provided"
                 )
 
             s3_file_path = os.path.join(s3_upload_path, str(uuid.uuid4()))
```

### Comparing `amazon-textract-textractor-1.3.1/textractor/utils/geometry_util.py` & `amazon-textract-textractor-1.3.2/textractor/utils/geometry_util.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/utils/s3_utils.py` & `amazon-textract-textractor-1.3.2/textractor/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/utils/search_utils.py` & `amazon-textract-textractor-1.3.2/textractor/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/visualizers/arial.ttf` & `amazon-textract-textractor-1.3.2/textractor/visualizers/arial.ttf`

 * *Files identical despite different names*

### Comparing `amazon-textract-textractor-1.3.1/textractor/visualizers/entitylist.py` & `amazon-textract-textractor-1.3.2/textractor/visualizers/entitylist.py`

 * *Files identical despite different names*

