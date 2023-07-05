# Comparing `tmp/pyiron_base-0.6.1.tar.gz` & `tmp/pyiron_base-0.6.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron_base-0.6.1.tar", last modified: Fri Jun  9 04:58:54 2023, max compression
+gzip compressed data, was "pyiron_base-0.6.1.dev0.tar", last modified: Wed Jul  5 13:57:58 2023, max compression
```

## Comparing `pyiron_base-0.6.1.tar` & `pyiron_base-0.6.1.dev0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/pyiron_base/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/pyiron_base/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.635112 pyiron_base-0.6.1/pyiron_base/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/reloadfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/rm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/cli/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.639112 pyiron_base-0.6.1/pyiron_base/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/filetable.py
--rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/jobtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/performance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/database/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.643112 pyiron_base-0.6.1/pyiron_base/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/has_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/has_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/interfaces/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.643112 pyiron_base-0.6.1/pyiron_base/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.647112 pyiron_base-0.6.1/pyiron_base/jobs/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.647112 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/jobstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.651112 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/queuestatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/runmode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    55900 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/jobtype.py
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    20443 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/runfunction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/job/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.655112 pyiron_base-0.6.1/pyiron_base/jobs/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/flexible.py
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/list.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/master/submissionstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/jobs/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.655112 pyiron_base-0.6.1/pyiron_base/project/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.659112 pyiron_base-0.6.1/pyiron_base/project/archiving/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/export_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/import_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/archiving/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.659112 pyiron_base-0.6.1/pyiron_base/project/update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.663112 pyiron_base-0.6.1/pyiron_base/state/
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/queue_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/state/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/pyiron_base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/datacontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/filedata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/fileio.py
--rw-r--r--   0 runner    (1001) docker     (123)    38762 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/flattenedstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/has_stored_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/hdfio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/hdfstub.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/inputlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/storage/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/pyiron_base/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/jedi.py
--rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/safetar.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/pyiron_base/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.635112 pyiron_base-0.6.1/pyiron_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/pyiron_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-09 04:58:54.000000 pyiron_base-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/test_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.667112 pyiron_base-0.6.1/test_benchmarks/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/test_benchmarks/generic/test_filehdfio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 04:58:54.671112 pyiron_base-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/tests/test_testwithproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-09 04:58:50.000000 pyiron_base-0.6.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/pyiron_base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/pyiron_base/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.943146 pyiron_base-0.6.1.dev0/pyiron_base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/reloadfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/rm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/cli/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.943146 pyiron_base-0.6.1.dev0/pyiron_base/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25072 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/filetable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45395 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/jobtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/database/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.947146 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/interfaces/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.947146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27892 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.951146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36920 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.951146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/jobstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.955146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/queuestatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/runmode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55629 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13584 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/jobtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/runfunction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.955146 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/flexible.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/submissionstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16462 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/jobs/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/export_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/import_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68931 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.959146 pyiron_base-0.6.1.dev0/pyiron_base/project/update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/project/update/pyiron_base_03x_to_04x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.963146 pyiron_base-0.6.1.dev0/pyiron_base/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/queue_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25086 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/state/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.963146 pyiron_base-0.6.1.dev0/pyiron_base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32693 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/datacontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7321 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/filedata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39557 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/flattenedstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14165 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/has_stored_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50450 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfstub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/inputlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32625 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/storage/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/pyiron_base/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/jedi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29090 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/safetar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/pyiron_base/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.939146 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/pyiron_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-05 13:57:58.971146 pyiron_base-0.6.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-05 13:57:58.000000 pyiron_base-0.6.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/test_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/test_benchmarks/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/test_benchmarks/generic/test_filehdfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:57:58.967146 pyiron_base-0.6.1.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/tests/test_testwithproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-05 13:57:55.000000 pyiron_base-0.6.1.dev0/versioneer.py
```

### Comparing `pyiron_base-0.6.1/LICENSE` & `pyiron_base-0.6.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/PKG-INFO` & `pyiron_base-0.6.1.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron_base
-Version: 0.6.1
+Version: 0.6.1.dev0
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.1/README.rst` & `pyiron_base-0.6.1.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/__init__.py` & `pyiron_base-0.6.1.dev0/pyiron_base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/_tests.py` & `pyiron_base-0.6.1.dev0/pyiron_base/_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from io import StringIO
 import unittest
 import os
 from pyiron_base import PythonTemplateJob, state
 from pyiron_base.project.generic import Project
 from abc import ABC
 from inspect import getfile
+import numpy as np
 
 
 __author__ = "Liam Huber"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
     "Computational Materials Design (CM) Department"
 )
@@ -26,17 +27,32 @@
 __status__ = "development"
 __date__ = "Mar 23, 2021"
 
 
 class PyironTestCase(unittest.TestCase, ABC):
 
     """
-    Tests that also include testing the docstrings in the specified modules
+    Base class for all pyiron unit tets.
+
+    Registers utility type equality functions:
+        - np.testing.assert_array_equal
+
+    Optionally includes testing the docstrings in the specified module by
+    overloading :attr:`~.docstring_module`.
     """
 
+    def setUp(self):
+        self.addTypeEqualityFunc(np.ndarray, self._assert_equal_numpy)
+
+    def _assert_equal_numpy(self, a, b, msg=None):
+        try:
+            np.testing.assert_array_equal(a, b, err_msg=msg)
+        except AssertionError as e:
+            raise self.failureException(*e.args) from None
+
     @classmethod
     def setUpClass(cls):
         cls._initial_settings_configuration = state.settings.configuration.copy()
         if any([cls is c for c in _TO_SKIP]):
             raise unittest.SkipTest(f"{cls.__name__} tests, it's a base class")
         super().setUpClass()
```

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/control.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/control.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/install.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/ls.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/ls.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/reloadfile.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/reloadfile.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/rm.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/rm.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/cli/wrapper.py` & `pyiron_base-0.6.1.dev0/pyiron_base/cli/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/database/filetable.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/filetable.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,17 +530,23 @@
                 *[
                     [project + subjob[1:] + ".h5", project + subjob[1:] + "_hdf5"]
                     for project, subjob in zip(
                         self._job_table.project.values, self._job_table.subjob.values
                     )
                 ]
             )
+            sanitized_paths = self._fileindex.dataframe.path.str.replace("\\", "/")
+            # The files_list is generated using project path values
+            # In pyiron, these are all forced to be posix-like with /
+            # But _fileindex is of type PyFileIndex, which does _not_ modify paths
+            # so to get the two compatible for an isin check, we need to sanitize the
+            # _fileindex.dataframe.path results
             df_new = self._fileindex.dataframe[
                 ~self._fileindex.dataframe.is_directory
-                & ~self._fileindex.dataframe.path.isin(files_lst)
+                & ~sanitized_paths.isin(files_lst)
             ]
         else:
             files_lst, working_dir_lst = [], []
             df_new = self._fileindex.dataframe[~self._fileindex.dataframe.is_directory]
         if len(df_new) > 0:
             job_lst = self.init_table(
                 fileindex=df_new, working_dir_lst=list(working_dir_lst)
@@ -561,15 +567,19 @@
         time = datetime.datetime.fromtimestamp(mtime)
         return_dict = table_columns.copy()
         return_dict.update(
             {
                 "status": get_job_status_from_file(hdf5_file=path, job_name=job),
                 "job": job,
                 "subjob": "/" + job,
-                "project": os.path.dirname(path) + "/",
+                "project": os.path.dirname(path).replace("\\", "/") + "/",
+                # pyiron Project paths are forced to be posix-like with / instead of \
+                # in order for the contains and endswith tests down in _get_job_table
+                # to work on windows, we need to make sure that the file table obeys
+                # this conversion
                 "timestart": time,
                 "timestop": time,
                 "totalcputime": 0.0,
                 "hamilton": get_hamilton_from_file(hdf5_file=path, job_name=job),
                 "hamversion": get_hamilton_version_from_file(
                     hdf5_file=path, job_name=job
                 ),
```

### Comparing `pyiron_base-0.6.1/pyiron_base/database/generic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/database/jobtable.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/jobtable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/database/manager.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/manager.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/database/performance.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/performance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/database/tables.py` & `pyiron_base-0.6.1.dev0/pyiron_base/database/tables.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/interfaces/factory.py` & `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/interfaces/has_groups.py` & `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_groups.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/interfaces/has_hdf.py` & `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/has_hdf.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/interfaces/object.py` & `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/object.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/interfaces/singleton.py` & `pyiron_base-0.6.1.dev0/pyiron_base/interfaces/singleton.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/datamining.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/datamining.py`

 * *Files 2% similar despite different names*

```diff
@@ -679,22 +679,27 @@
             group_name:
         """
         super(TableJob, self).from_hdf(hdf=hdf, group_name=group_name)
         hdf_version = self.project_hdf5.get("HDF_VERSION", "0.1.0")
         with self.project_hdf5.open("input") as hdf5_input:
             if "project" in hdf5_input.list_nodes():
                 project_dict = hdf5_input["project"]
-                project = self.project.__class__(
-                    path=project_dict["path"],
-                    user=project_dict["user"],
-                    sql_query=project_dict["sql_query"],
-                )
-                project._filter = project_dict["filter"]
-                project._inspect_mode = project_dict["inspect_mode"]
-                self.analysis_project = project
+                if os.path.exists(project_dict["path"]):
+                    project = self.project.__class__(
+                        path=project_dict["path"],
+                        user=project_dict["user"],
+                        sql_query=project_dict["sql_query"],
+                    )
+                    project._filter = project_dict["filter"]
+                    project._inspect_mode = project_dict["inspect_mode"]
+                    self.analysis_project = project
+                else:
+                    self._logger.warning(
+                        f"Could not instantiate analysis_project, no such path {project_dict['path']}."
+                    )
             if "filter" in hdf5_input.list_nodes():
                 if hdf_version == "0.1.0":
                     self.pyiron_table._filter_function_str = hdf5_input["filter"]
                     self.pyiron_table.filter_function = get_function_from_string(
                         hdf5_input["filter"]
                     )
                 else:
```

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/dynamic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/dynamic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/core.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/core.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/executable.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/jobstatus.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/jobstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/generic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
         threads=1,
         gpus=None,
         run_mode="modal",
         new_hdf=True,
     ):
         self._cores = cores
         self._threads = threads
-        self._gpus = None
+        self._active_queue = None
+        self._gpus = gpus
         self._run_time = None
         self._memory_limit = None
         self._host = self._init_host(host=host)
         self._run_mode = Runmode()
 
         self.queue = queue
 
@@ -460,15 +461,15 @@
         hdf_dict["structure_id"] = self.structure_id
         hdf_dict["run_time"] = self.run_time
         hdf_dict["memory_limit"] = self.memory_limit
         hdf_dict["accept_crash"] = self.accept_crash
         if len(self.additional_arguments) > 0:
             hdf_dict["additional_arguments"] = self.additional_arguments
         if self._gpus is not None:
-            hdf_dict["accept_crash"] = self._gpus
+            hdf_dict["gpus"] = self._gpus
 
         if group_name is not None:
             with hdf.open(group_name) as hdf_group:
                 hdf_group["server"] = hdf_dict
         else:
             hdf["server"] = hdf_dict
 
@@ -505,15 +506,15 @@
         if "accept_crash" in hdf_dict.keys():
             self._accept_crash = hdf_dict["accept_crash"] == 1
         if "threads" in hdf_dict.keys():
             self._threads = hdf_dict["threads"]
         if "additional_arguments" in hdf_dict.keys():
             self.additional_arguments = hdf_dict["additional_arguments"]
         if "gpus" in hdf_dict.keys():
-            self._gpus = hdf_dict["accept_crash"]
+            self._gpus = hdf_dict["gpus"]
         self._new_hdf = hdf_dict["new_h5"] == 1
 
     def db_entry(self):
         """
         connect all the info regarding the server into a single word that can be used e.g. as entry in a database
 
         Returns:
```

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/queuestatus.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/queuestatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/extension/server/runmode.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/extension/server/runmode.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     "modal",
     "non_modal",
     "queue",
     "manual",
     "thread",
     "worker",
     "srun",
-    "flux",
     "interactive",
     "interactive_non_modal",
 ]
 
 
 class Runmode(object):
     """
```

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/factory.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/generic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,14 @@
         self._restart_file_dict = dict()
         self._exclude_nodes_hdf = list()
         self._exclude_groups_hdf = list()
         self._process = None
         self._compress_by_default = False
         self._python_only_job = False
         self._write_work_dir_warnings = True
-        self._flux_executor = None
         self.interactive_cache = None
         self.error = GenericError(job=self)
 
     @property
     def version(self):
         """
         Get the version of the hamiltonian, which is also the version of the executable unless a custom executable is
@@ -207,23 +206,14 @@
         Args:
             exe (str): executable path, if no valid path is provided an executable is chosen based on version.
         """
         self._executable_activate()
         self._executable.executable_path = exe
 
     @property
-    def flux_executor(self):
-        return self._flux_executor
-
-    @flux_executor.setter
-    def flux_executor(self, exe):
-        self.server.run_mode.flux = True
-        self._flux_executor = exe
-
-    @property
     def server(self):
         """
         Get the server object to handle the execution environment for the job.
 
         Returns:
             Server: server object
         """
@@ -696,17 +686,17 @@
                     self.server.run_mode = run_mode
                 if delete_existing_job:
                     status = "initialized"
                     self.remove_and_reset_id(_protect_childs=False)
                 if repair and self.job_id and not self.status.finished:
                     self._run_if_repair()
                 elif status == "initialized":
-                    return self._run_if_new(debug=debug)
+                    self._run_if_new(debug=debug)
                 elif status == "created":
-                    return self._run_if_created()
+                    self._run_if_created()
                 elif status == "submitted":
                     run_job_with_status_submitted(job=self)
                 elif status == "running":
                     self._run_if_running()
                 elif status == "collect":
                     self._run_if_collect()
                 elif status == "suspend":
@@ -1197,15 +1187,15 @@
         """
         Internal helper function the run if new function is called when the job status is 'initialized'. It prepares
         the hdf5 file and the corresponding directory structure.
 
         Args:
             debug (bool): Debug Mode
         """
-        return run_job_with_status_initialized(job=self, debug=debug)
+        run_job_with_status_initialized(job=self, debug=debug)
 
     def _run_if_created(self):
         """
         Internal helper function the run if created function is called when the job status is 'created'. It executes
         the simulation, either in modal mode, meaning waiting for the simulation to finish, manually, or submits the
         simulation to the que.
```

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/interactive.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/jobtype.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/jobtype.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/path.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/runfunction.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/runfunction.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,18 @@
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 from datetime import datetime
 import multiprocessing
 import os
 import posixpath
 import subprocess
 
-from jinja2 import Template
-
 from pyiron_base.utils.deprecate import deprecate
 from pyiron_base.jobs.job.wrapper import JobWrapper
 from pyiron_base.state import state
 
-try:
-    import flux.job
-
-    flux_available = True
-except ImportError:
-    flux_available = False
-
 
 """
 The function job.run() inside pyiron is executed differently depending on the status of the job object. This module 
 introduces the most general run functions and how they are selected. 
 
 If an additional parameter is provided, then a specific run function is executed: 
     repair: run_job_with_parameter_repair
@@ -44,15 +35,14 @@
     manual: run_job_with_runmode_manually
     modal: run_job_with_runmode_modal
     non_modal: run_job_with_runmode_non_modal
     interactive: run_job_with_runmode_interactive
     interactive_non_modal: run_job_with_runmode_interactive_non_modal
     queue: run_job_with_runmode_queue
     srun: run_job_with_runmode_srun
-    flux: run_job_with_runmode_flux
     thread: only affects children of a GenericMaster 
     worker: only affects children of a GenericMaster 
     
 Finally for jobs which call an external executable the execution is implemented in an function as well: 
     execute_job_with_external_executable
 """
 
@@ -82,15 +72,15 @@
     job.validate_ready_to_run()
     if job.server.run_mode.queue:
         job.check_setup()
     if job.check_if_job_exists():
         print("job exists already and therefore was not created!")
     else:
         job.save()
-        return job.run()
+        job.run()
 
 
 def run_job_with_status_created(job):
     """
     Internal helper function the run if created function is called when the job status is 'created'. It executes
     the simulation, either in modal mode, meaning waiting for the simulation to finish, manually, or submits the
     simulation to the que.
@@ -108,24 +98,14 @@
         run_job_with_runmode_manually(job=job, _manually_print=True)
     elif job.server.run_mode.worker:
         run_job_with_runmode_manually(job=job, _manually_print=True)
     elif job.server.run_mode.modal:
         job.run_static()
     elif job.server.run_mode.srun:
         run_job_with_runmode_srun(job=job)
-    elif job.server.run_mode.flux:
-        if job.server.gpus is not None:
-            gpus_per_slot = int(job.server.gpus / job.server.cores)
-        else:
-            gpus_per_slot = None
-        return run_job_with_runmode_flux(
-            job=job,
-            executor=job.flux_executor,
-            gpus_per_slot=gpus_per_slot,
-        )
     elif (
         job.server.run_mode.non_modal
         or job.server.run_mode.thread
         or job.server.run_mode.worker
     ):
         run_job_with_runmode_non_modal(job=job)
     elif job.server.run_mode.queue:
@@ -447,59 +427,14 @@
         shell=True,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         universal_newlines=True,
     )
 
 
-def run_job_with_runmode_flux(job, executor, gpus_per_slot=None):
-    if not flux_available:
-        raise ModuleNotFoundError(
-            "No module named 'flux'. No linux you can install flux via conda."
-            + "'conda install -c conda-forge flux'"
-        )
-    if not state.database.database_is_disabled:
-        executable_template = Template(
-            """\
-#!/bin/bash
-python -m pyiron_base.cli wrapper -p {{working_directory}} -j {{job_id}}
-"""
-        )
-        exeuctable_str = executable_template.render(
-            working_directory=job.working_directory,
-            job_id=str(job.job_id),
-        )
-        job_name = "pi_" + str(job.job_id)
-    else:
-        executable_template = Template(
-            """\
-#!/bin/bash
-python -m pyiron_base.cli wrapper -p {{working_directory}} -f {{file_name}}{{h5_path}}
-"""
-        )
-        exeuctable_str = executable_template.render(
-            working_directory=job.working_directory,
-            file_name=job.project_hdf5.file_name,
-            h5_path=job.project_hdf5.h5_path,
-        )
-        job_name = "pi_" + job.job_name
-
-    jobspec = flux.job.JobspecV1.from_batch_command(
-        jobname=job_name,
-        script=exeuctable_str,
-        num_nodes=1,
-        cores_per_slot=1,
-        gpus_per_slot=gpus_per_slot,
-        num_slots=job.server.cores,
-    )
-    jobspec.cwd = job.project_hdf5.working_directory
-    jobspec.environment = dict(os.environ)
-    return executor.submit(jobspec)
-
-
 def run_time_decorator(func):
     def wrapper(job):
         if not state.database.database_is_disabled and job.job_id is not None:
             job.project.db.item_update({"timestart": datetime.now()}, job.job_id)
             func(job)
             job.project.db.item_update(job._runtime(), job.job_id)
         else:
```

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/template.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/template.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/toolkit.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/util.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/util.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/job/wrapper.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/job/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/flexible.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/flexible.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/generic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/interactivewrapper.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/list.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/list.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/parallel.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/serial.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/master/submissionstatus.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/master/submissionstatus.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/script.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/script.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/jobs/worker.py` & `pyiron_base-0.6.1.dev0/pyiron_base/jobs/worker.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/archiving/export_archive.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/export_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/archiving/import_archive.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/archiving/import_archive.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/data.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/data.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/external.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/external.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 """
 Load input parameters for jupyter notebooks from external HDF5 or JSON file
 """
 
 import json
-from pathlib2 import Path
+from pathlib import Path
 import warnings
 from pyiron_base.storage.hdfio import FileHDFio
 from pyiron_base.storage.datacontainer import DataContainer
 
 __author__ = "Osamu Waseda"
 __copyright__ = (
     "Copyright 2020, Max-Planck-Institut für Eisenforschung GmbH - "
```

### Comparing `pyiron_base-0.6.1/pyiron_base/project/generic.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/gui.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/gui.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/maintenance.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/maintenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                             (eg. status="finished"). Asterisk can be used to denote a wildcard, for zero or more
                             instances of any character
         """
         for job in self._project.iter_jobs(
             recursive=recursive, progress=progress, convert_to_object=False, **kwargs
         ):
             hdf = job.project_hdf5
-            hdf.rewrite_hdf(job.name)
+            hdf.rewrite_hdf5(job.name)
 
 
 class UpdateMaintenance:
     def __init__(self, project):
         self._project = project
 
     def base_to_current(self, start_version: str, project=None):
@@ -115,17 +115,17 @@
             project(None/project/list/str): The project(s) to be converted from 0.3 to 0.4 ; default: current project
                 One may provide a pyiron Project, a list of pyiron Projects, or a string containing "all" or a valid
                 path.
                 If "all" is provided, pyiron tries to find all projects using the PROJECT_PATHS defined in the
                 configuration.
         """
         mayor, minor = start_version.split(".")[0:2]
-        if mayor != 0:
+        if int(mayor) != 0:
             raise ValueError("Updates to version >0.x.y is not possible.")
-        if minor < 4:
+        if int(minor) < 4:
             self.base_v0_3_to_v0_4(project)
 
     def base_v0_3_to_v0_4(self, project=None):
         """Update hdf files written with pyiron_base-0.3.x to pyiron_base-0.4.x
 
         pyiron_base<=0.3.9 has a bug that writes all arrays with dtype=object even
         numeric ones.  As a fix pyiron_base=0.4.0 introduces a conversion when reading
```

### Comparing `pyiron_base-0.6.1/pyiron_base/project/path.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/path.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/project/update/pyiron_base_03x_to_04x.py` & `pyiron_base-0.6.1.dev0/pyiron_base/project/update/pyiron_base_03x_to_04x.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/__init__.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/install.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/install.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/logger.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/logger.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/publications.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/publications.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/queue_adapter.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/queue_adapter.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/settings.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/settings.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/signal.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/signal.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/state/update.py` & `pyiron_base-0.6.1.dev0/pyiron_base/state/update.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/datacontainer.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/datacontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/filedata.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/filedata.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/fileio.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/flattenedstorage.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/flattenedstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,26 +542,50 @@
                 self._per_chunk_arrays[name] = _ensure_str_array_size(
                     self._per_chunk_arrays[name], strlen
                 )
             self._per_chunk_arrays[name][frame] = value
         else:
             raise KeyError(f"no array named {name}")
 
+    def del_array(self, name: str, ignore_missing: bool = False):
+        """
+        Remove an array.
+
+        Works with both per chunk and per element arrays.
+
+        Args:
+            name (str): name of the array
+            ignore_missing (bool): if given do not raise an error if no array
+                                   of the given `name` exists
+
+        Raises:
+            KeyError: if no array with given `name` exists and `ignore_missing` is not given
+        """
+        if name in self._per_element_arrays:
+            del self._per_element_arrays[name]
+        elif name in self._per_chunk_arrays:
+            del self._per_chunk_arrays[name]
+        elif not ignore_missing:
+            raise KeyError(name)
+
     def __getitem__(self, index):
         if isinstance(index, tuple) and len(index) == 2:
             return self.get_array(index[0], index[1])
         else:
             return self.get_array(index)
 
     def __setitem__(self, index, value):
         if isinstance(index, tuple) and len(index) == 2:
             self.set_array(index[0], index[1], value)
         else:
             raise IndexError("Must specify chunk index.")
 
+    def __delitem__(self, index):
+        self.del_array(index)
+
     def has_array(self, name):
         """
         Checks whether an array of the given name exists and returns meta data given to :method:`.add_array()`.
 
         >>> container.has_array("energy")
         {'shape': (), 'dtype': np.float64, 'per': 'chunk'}
         >>> container.has_array("fnorble")
```

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/has_stored_traits.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/has_stored_traits.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/hdfio.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/hdfstub.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/hdfstub.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/helper_functions.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/storage/parameters.py` & `pyiron_base-0.6.1.dev0/pyiron_base/storage/parameters.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/deprecate.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/error.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/error.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/instance.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/instance.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/jedi.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/jedi.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/parser.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/parser.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/safetar.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/safetar.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base/utils/units.py` & `pyiron_base-0.6.1.dev0/pyiron_base/utils/units.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/pyiron_base.egg-info/PKG-INFO` & `pyiron_base-0.6.1.dev0/pyiron_base.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-base
-Version: 0.6.1
+Version: 0.6.1.dev0
 Summary: pyiron_base - an integrated development environment (IDE) for computational science.
 Home-page: https://github.com/pyiron/pyiron_base
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron_base-0.6.1/pyiron_base.egg-info/SOURCES.txt` & `pyiron_base-0.6.1.dev0/pyiron_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/setup.py` & `pyiron_base-0.6.1.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,22 @@
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
         'dill>=0.3.6',
         'gitpython>=3.1.31',
         'h5io>=0.1.7',
-        'h5py>=3.8.0',
+        'h5py>=3.9.0',
         'numpy>=1.24.3',
-        'pandas>=2.0.2',
-        'pathlib2>=2.3.7.post1',
+        'pandas>=2.0.3',
         'pint>=0.22',
         'psutil>=5.9.5',
         'pyfileindex>=0.0.11',
         'pysqa>=0.0.25',
-        'sqlalchemy>=2.0.15',
+        'sqlalchemy>=2.0.17',
         'tables>=3.8.0',
         'tqdm>=4.65.0',
         'traitlets>=5.9.0',
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     entry_points={
```

### Comparing `pyiron_base-0.6.1/test_benchmarks/generic/test_filehdfio.py` & `pyiron_base-0.6.1.dev0/test_benchmarks/generic/test_filehdfio.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/tests/test_testwithproject.py` & `pyiron_base-0.6.1.dev0/tests/test_testwithproject.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/tests/test_toolkit.py` & `pyiron_base-0.6.1.dev0/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron_base-0.6.1/versioneer.py` & `pyiron_base-0.6.1.dev0/versioneer.py`

 * *Files identical despite different names*

