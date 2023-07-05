# Comparing `tmp/projectal-4.0.1.tar.gz` & `tmp/projectal-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "projectal-4.0.1.tar", last modified: Wed Jun 14 06:22:58 2023, max compression
+gzip compressed data, was "projectal-4.0.2.tar", last modified: Wed Jul  5 06:06:20 2023, max compression
```

## Comparing `projectal-4.0.1.tar` & `projectal-4.0.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.0.1/LICENSE
--rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.0.1/MANIFEST.in
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 06:22:58.541076 projectal-4.0.1/PKG-INFO
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.533076 projectal-4.0.1/docs/
--rw-rw-r--   0 luked     (1003) luked     (1003)      140 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/index.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.537076 projectal-4.0.1/docs/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)   123963 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/api.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.537076 projectal-4.0.1/docs/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)    44886 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/access_policy.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    48388 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/activity.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    43819 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/booking.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76700 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/calendar.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    78998 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/company.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    60445 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/contact.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    47063 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/customer.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    72006 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/department.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   112784 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/file.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    79391 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/folder.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    67125 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/location.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    73862 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/note.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    51453 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/permission.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76122 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/project.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    53421 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/project_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    46200 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/rebate.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    46469 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/resource.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    45789 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/skill.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   138305 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/staff.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    44760 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/stage.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    42248 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/tag.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   167963 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/task.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    81669 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/task_template.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    82639 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/user.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    76578 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities/webhook.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    42661 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entities.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   660878 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/entity.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    81307 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/enums.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   107022 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/errors.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   260261 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/linkers.html
--rw-rw-r--   0 luked     (1003) luked     (1003)    57589 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal/profile.html
--rw-rw-r--   0 luked     (1003) luked     (1003)   113364 2023-06-14 06:22:04.000000 projectal-4.0.1/docs/projectal.html
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/examples/
--rw-rw-r--   0 luked     (1003) luked     (1003)     3154 2022-11-17 04:31:31.000000 projectal-4.0.1/examples/linking.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      811 2022-11-17 04:31:31.000000 projectal-4.0.1/examples/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1064 2022-12-01 02:53:21.000000 projectal-4.0.1/examples/webhook.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal/
--rw-rw-r--   0 luked     (1003) luked     (1003)    17172 2023-06-14 06:18:47.000000 projectal-4.0.1/projectal/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     9133 2023-03-09 04:46:05.000000 projectal-4.0.1/projectal/api.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal/entities/
--rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.0.1/projectal/entities/__init__.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/access_policy.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      485 2023-05-16 05:57:07.000000 projectal-4.0.1/projectal/entities/activity.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      303 2023-05-16 05:57:12.000000 projectal-4.0.1/projectal/entities/booking.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2233 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/calendar.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1935 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/company.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      982 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/contact.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      460 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/customer.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1855 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/department.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3171 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/file.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1732 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/folder.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1305 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/location.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1939 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/note.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      613 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/permission.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1655 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/project.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      709 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/project_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      426 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/rebate.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      434 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/resource.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/skill.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     4678 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/staff.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      344 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/stage.py
--rw-rw-r--   0 luked     (1003) luked     (1003)      230 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/tag.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     6359 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/task.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1833 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/task_template.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1978 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/entities/user.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     1668 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/entities/webhook.py
--rw-rw-r--   0 luked     (1003) luked     (1003)    40482 2023-03-09 04:46:05.000000 projectal-4.0.1/projectal/entity.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2152 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/enums.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     3564 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/errors.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     8657 2022-12-21 23:38:50.000000 projectal-4.0.1/projectal/linkers.py
--rw-rw-r--   0 luked     (1003) luked     (1003)     2382 2022-11-17 04:31:31.000000 projectal-4.0.1/projectal/profile.py
-drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-06-14 06:22:58.541076 projectal-4.0.1/projectal.egg-info/
--rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/PKG-INFO
--rw-rw-r--   0 luked     (1003) luked     (1003)     2336 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/SOURCES.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)        1 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/dependency_links.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/requires.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-06-14 06:22:58.000000 projectal-4.0.1/projectal.egg-info/top_level.txt
--rw-rw-r--   0 luked     (1003) luked     (1003)       38 2023-06-14 06:22:58.541076 projectal-4.0.1/setup.cfg
--rw-rw-r--   0 luked     (1003) luked     (1003)      757 2023-06-14 06:15:07.000000 projectal-4.0.1/setup.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.344832 projectal-4.0.2/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1074 2022-11-17 04:31:31.000000 projectal-4.0.2/LICENSE
+-rw-rw-r--   0 luked     (1003) luked     (1003)       30 2022-11-17 04:31:31.000000 projectal-4.0.2/MANIFEST.in
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-07-05 06:06:20.344832 projectal-4.0.2/PKG-INFO
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.336832 projectal-4.0.2/docs/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      140 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/index.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.340832 projectal-4.0.2/docs/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)   123963 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/api.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.340832 projectal-4.0.2/docs/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44886 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/access_policy.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    50589 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/activity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   116129 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/booking.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76700 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/calendar.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    78998 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/company.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    60445 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/contact.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    47063 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/customer.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    72006 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/department.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   112784 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/file.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    79391 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/folder.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    67125 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/location.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    73862 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/note.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    51453 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/permission.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76122 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/project.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    53421 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/project_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46200 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/rebate.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    46469 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/resource.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    45789 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/skill.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   138305 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/staff.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    44760 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/stage.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42248 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/tag.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   167963 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/task.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81669 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/task_template.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    82639 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/user.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    76578 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities/webhook.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    42661 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal/entities.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   660868 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/projectal/entity.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    81307 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/projectal/enums.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   107022 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/projectal/errors.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   279057 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/projectal/linkers.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)    57589 2023-07-05 06:03:46.000000 projectal-4.0.2/docs/projectal/profile.html
+-rw-rw-r--   0 luked     (1003) luked     (1003)   115089 2023-07-05 06:03:45.000000 projectal-4.0.2/docs/projectal.html
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.340832 projectal-4.0.2/examples/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3154 2022-11-17 04:31:31.000000 projectal-4.0.2/examples/linking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      811 2022-11-17 04:31:31.000000 projectal-4.0.2/examples/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1064 2022-12-01 02:53:21.000000 projectal-4.0.2/examples/webhook.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.344832 projectal-4.0.2/projectal/
+-rw-rw-r--   0 luked     (1003) luked     (1003)    17530 2023-07-05 05:35:31.000000 projectal-4.0.2/projectal/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9133 2023-03-09 04:46:05.000000 projectal-4.0.2/projectal/api.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.344832 projectal-4.0.2/projectal/entities/
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1298 2023-05-16 05:22:36.000000 projectal-4.0.2/projectal/entities/__init__.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/access_policy.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      593 2023-07-05 03:55:16.000000 projectal-4.0.2/projectal/entities/activity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4688 2023-07-05 05:27:31.000000 projectal-4.0.2/projectal/entities/booking.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2233 2022-12-21 23:38:50.000000 projectal-4.0.2/projectal/entities/calendar.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1935 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/company.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      982 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/contact.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      460 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/customer.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1855 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/department.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3171 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/file.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1732 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/folder.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1305 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/location.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1939 2022-12-21 23:38:50.000000 projectal-4.0.2/projectal/entities/note.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      613 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/permission.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1655 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/project.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      709 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/project_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      426 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/rebate.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      434 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/resource.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      395 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/skill.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     4678 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/staff.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      344 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/stage.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)      230 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/tag.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     6359 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/task.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1833 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/task_template.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1978 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/entities/user.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     1668 2022-12-21 23:38:50.000000 projectal-4.0.2/projectal/entities/webhook.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)    40479 2023-07-04 07:22:47.000000 projectal-4.0.2/projectal/entity.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2152 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/enums.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     3564 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/errors.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     9209 2023-07-05 05:01:23.000000 projectal-4.0.2/projectal/linkers.py
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2382 2022-11-17 04:31:31.000000 projectal-4.0.2/projectal/profile.py
+drwxrwxr-x   0 luked     (1003) luked     (1003)        0 2023-07-05 06:06:20.344832 projectal-4.0.2/projectal.egg-info/
+-rw-rw-r--   0 luked     (1003) luked     (1003)      573 2023-07-05 06:06:20.000000 projectal-4.0.2/projectal.egg-info/PKG-INFO
+-rw-rw-r--   0 luked     (1003) luked     (1003)     2336 2023-07-05 06:06:20.000000 projectal-4.0.2/projectal.egg-info/SOURCES.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)        1 2023-07-05 06:06:20.000000 projectal-4.0.2/projectal.egg-info/dependency_links.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-07-05 06:06:20.000000 projectal-4.0.2/projectal.egg-info/requires.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       19 2023-07-05 06:06:20.000000 projectal-4.0.2/projectal.egg-info/top_level.txt
+-rw-rw-r--   0 luked     (1003) luked     (1003)       38 2023-07-05 06:06:20.344832 projectal-4.0.2/setup.cfg
+-rw-rw-r--   0 luked     (1003) luked     (1003)      757 2023-07-05 05:53:17.000000 projectal-4.0.2/setup.py
```

### Comparing `projectal-4.0.1/LICENSE` & `projectal-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/PKG-INFO` & `projectal-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 4.0.1
+Version: 4.0.2
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-4.0.1/docs/projectal/api.html` & `projectal-4.0.2/docs/projectal/api.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/access_policy.html` & `projectal-4.0.2/docs/projectal/entities/access_policy.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/activity.html` & `projectal-4.0.2/docs/projectal/entities/activity.html`

 * *Files 4% similar despite different names*

```diff
@@ -58,47 +58,51 @@
 
                         <label class="view-source-button" for="mod-activity-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">from</span> <span class="nn">projectal.entity</span> <span class="kn">import</span> <span class="n">Entity</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">from</span> <span class="nn">projectal.linkers</span> <span class="kn">import</span> <span class="o">*</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Activity</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>               <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/Activity) API.</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span>
-</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>              <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Activity</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">BookingLinker</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">NoteLinker</span><span class="p">,</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>               <span class="n">FileLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span> <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a>               <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="sd">    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/Activity) API.</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">BookingLinker</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">NoteLinker</span><span class="p">,</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a>              <span class="n">FileLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span> <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a>              <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
             </section>
                 <section id="Activity">
                             <input id="Activity-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
-    <span class="name">Activity</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#ContactLinker">projectal.linkers.ContactLinker</a></span>, <span class="base"><a href="../linkers.html#LocationLinker">projectal.linkers.LocationLinker</a></span>, <span class="base"><a href="../linkers.html#RebateLinker">projectal.linkers.RebateLinker</a></span>, <span class="base"><a href="../linkers.html#ResourceLinker">projectal.linkers.ResourceLinker</a></span>, <span class="base"><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></span>, <span class="base"><a href="../linkers.html#StageLinker">projectal.linkers.StageLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
+    <span class="name">Activity</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#BookingLinker">projectal.linkers.BookingLinker</a></span>, <span class="base"><a href="../linkers.html#ContactLinker">projectal.linkers.ContactLinker</a></span>, <span class="base"><a href="../linkers.html#LocationLinker">projectal.linkers.LocationLinker</a></span>, <span class="base"><a href="../linkers.html#NoteLinker">projectal.linkers.NoteLinker</a></span>, <span class="base"><a href="../linkers.html#FileLinker">projectal.linkers.FileLinker</a></span>, <span class="base"><a href="../linkers.html#RebateLinker">projectal.linkers.RebateLinker</a></span>, <span class="base"><a href="../linkers.html#ResourceLinker">projectal.linkers.ResourceLinker</a></span>, <span class="base"><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></span>, <span class="base"><a href="../linkers.html#StageLinker">projectal.linkers.StageLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
 
                 <label class="view-source-button" for="Activity-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#Activity"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Activity-6"><a href="#Activity-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Activity</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span>
-</span><span id="Activity-7"><a href="#Activity-7"><span class="linenos"> 7</span></a>               <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="Activity-8"><a href="#Activity-8"><span class="linenos"> 8</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Activity-9"><a href="#Activity-9"><span class="linenos"> 9</span></a><span class="sd">    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/Activity) API.</span>
-</span><span id="Activity-10"><a href="#Activity-10"><span class="linenos">10</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Activity-11"><a href="#Activity-11"><span class="linenos">11</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
-</span><span id="Activity-12"><a href="#Activity-12"><span class="linenos">12</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
-</span><span id="Activity-13"><a href="#Activity-13"><span class="linenos">13</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span>
-</span><span id="Activity-14"><a href="#Activity-14"><span class="linenos">14</span></a>              <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Activity-6"><a href="#Activity-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Activity</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">BookingLinker</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">NoteLinker</span><span class="p">,</span>
+</span><span id="Activity-7"><a href="#Activity-7"><span class="linenos"> 7</span></a>               <span class="n">FileLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span> <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span>
+</span><span id="Activity-8"><a href="#Activity-8"><span class="linenos"> 8</span></a>               <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="Activity-9"><a href="#Activity-9"><span class="linenos"> 9</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Activity-10"><a href="#Activity-10"><span class="linenos">10</span></a><span class="sd">    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/Activity) API.</span>
+</span><span id="Activity-11"><a href="#Activity-11"><span class="linenos">11</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Activity-12"><a href="#Activity-12"><span class="linenos">12</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="Activity-13"><a href="#Activity-13"><span class="linenos">13</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="Activity-14"><a href="#Activity-14"><span class="linenos">14</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">BookingLinker</span><span class="p">,</span> <span class="n">ContactLinker</span><span class="p">,</span> <span class="n">LocationLinker</span><span class="p">,</span> <span class="n">NoteLinker</span><span class="p">,</span>
+</span><span id="Activity-15"><a href="#Activity-15"><span class="linenos">15</span></a>              <span class="n">FileLinker</span><span class="p">,</span> <span class="n">RebateLinker</span><span class="p">,</span> <span class="n">ResourceLinker</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span>
+</span><span id="Activity-16"><a href="#Activity-16"><span class="linenos">16</span></a>              <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Activity">Activity</a> API.</p>
 </div>
 
 
@@ -126,24 +130,34 @@
                 <dd id="Activity.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
                 <dd id="Activity.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
                 <dd id="Activity.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
                 <dd id="Activity.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
                 <dd id="Activity.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
 
             </div>
+            <div><dt><a href="../linkers.html#BookingLinker">projectal.linkers.BookingLinker</a></dt>
+                                <dd id="Activity.link_booking" class="function"><a href="../linkers.html#BookingLinker.link_booking">link_booking</a></dd>
+                <dd id="Activity.unlink_booking" class="function"><a href="../linkers.html#BookingLinker.unlink_booking">unlink_booking</a></dd>
+
+            </div>
             <div><dt><a href="../linkers.html#ContactLinker">projectal.linkers.ContactLinker</a></dt>
                                 <dd id="Activity.link_contact" class="function"><a href="../linkers.html#ContactLinker.link_contact">link_contact</a></dd>
                 <dd id="Activity.unlink_contact" class="function"><a href="../linkers.html#ContactLinker.unlink_contact">unlink_contact</a></dd>
 
             </div>
             <div><dt><a href="../linkers.html#LocationLinker">projectal.linkers.LocationLinker</a></dt>
                                 <dd id="Activity.link_location" class="function"><a href="../linkers.html#LocationLinker.link_location">link_location</a></dd>
                 <dd id="Activity.unlink_location" class="function"><a href="../linkers.html#LocationLinker.unlink_location">unlink_location</a></dd>
 
             </div>
+            <div><dt><a href="../linkers.html#FileLinker">projectal.linkers.FileLinker</a></dt>
+                                <dd id="Activity.link_file" class="function"><a href="../linkers.html#FileLinker.link_file">link_file</a></dd>
+                <dd id="Activity.unlink_file" class="function"><a href="../linkers.html#FileLinker.unlink_file">unlink_file</a></dd>
+
+            </div>
             <div><dt><a href="../linkers.html#RebateLinker">projectal.linkers.RebateLinker</a></dt>
                                 <dd id="Activity.link_rebate" class="function"><a href="../linkers.html#RebateLinker.link_rebate">link_rebate</a></dd>
                 <dd id="Activity.unlink_rebate" class="function"><a href="../linkers.html#RebateLinker.unlink_rebate">unlink_rebate</a></dd>
 
             </div>
             <div><dt><a href="../linkers.html#ResourceLinker">projectal.linkers.ResourceLinker</a></dt>
                                 <dd id="Activity.link_resource" class="function"><a href="../linkers.html#ResourceLinker.link_resource">link_resource</a></dd>
```

#### html2text {}

```diff
@@ -8,35 +8,45 @@
 
 ****** projectal.entities.activity ******
 ⁰ View Source
 _1from projectal.entity import Entity
 _2from projectal.linkers import *
 _3
 _4
-_5class Activity(Entity, ContactLinker, LocationLinker, RebateLinker,
-_6               ResourceLinker, StaffLinker, StageLinker, TagLinker):
-_7    """
-_8    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/
-Activity) API.
-_9    """
-10    _path = 'activity'
-11    _name = 'activity'
-12    _links = [ContactLinker, LocationLinker, RebateLinker,
-13              ResourceLinker, StaffLinker, StageLinker, TagLinker]
-  ⁰
-class Activity(projectal.entity.Entity, projectal.linkers.ContactLinker,
-projectal.linkers.LocationLinker, projectal.linkers.RebateLinker,
-projectal.linkers.ResourceLinker, projectal.linkers.StaffLinker,
-projectal.linkers.StageLinker, projectal.linkers.TagLinker): View Source
-_6class Activity(Entity, ContactLinker, LocationLinker, RebateLinker,
-_7               ResourceLinker, StaffLinker, StageLinker, TagLinker):
+_5class Activity(Entity, BookingLinker, ContactLinker, LocationLinker,
+NoteLinker,
+_6               FileLinker, RebateLinker, ResourceLinker, StaffLinker,
+StageLinker,
+_7               TagLinker):
 _8    """
 _9    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/
 Activity) API.
 10    """
 11    _path = 'activity'
 12    _name = 'activity'
-13    _links = [ContactLinker, LocationLinker, RebateLinker,
-14              ResourceLinker, StaffLinker, StageLinker, TagLinker]
+13    _links = [BookingLinker, ContactLinker, LocationLinker, NoteLinker,
+14              FileLinker, RebateLinker, ResourceLinker, StaffLinker,
+15              StageLinker, TagLinker]
+  ⁰
+class Activity(projectal.entity.Entity, projectal.linkers.BookingLinker,
+projectal.linkers.ContactLinker, projectal.linkers.LocationLinker,
+projectal.linkers.NoteLinker, projectal.linkers.FileLinker,
+projectal.linkers.RebateLinker, projectal.linkers.ResourceLinker,
+projectal.linkers.StaffLinker, projectal.linkers.StageLinker,
+projectal.linkers.TagLinker): View Source
+_6class Activity(Entity, BookingLinker, ContactLinker, LocationLinker,
+NoteLinker,
+_7               FileLinker, RebateLinker, ResourceLinker, StaffLinker,
+StageLinker,
+_8               TagLinker):
+_9    """
+10    Implementation of the [Activity](https://projectal.com/docs/latest/#tag/
+Activity) API.
+11    """
+12    _path = 'activity'
+13    _name = 'activity'
+14    _links = [BookingLinker, ContactLinker, LocationLinker, NoteLinker,
+15              FileLinker, RebateLinker, ResourceLinker, StaffLinker,
+16              StageLinker, TagLinker]
 Implementation of the Activity API.
 ** Inherited Members **
```

### Comparing `projectal-4.0.1/docs/projectal/entities/booking.html` & `projectal-4.0.2/docs/projectal/entities/skill.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <meta name="generator" content="pdoc 12.3.0"/>
-    <title>projectal.entities.booking API documentation</title>
+    <title>projectal.entities.skill API documentation</title>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
     <style>/*! custom.css */</style></head>
@@ -28,15 +28,15 @@
                    pattern=".+" required>
 
 
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
-                    <a class="class" href="#Booking">Booking</a>
+                    <a class="class" href="#Skill">Skill</a>
                             <ul class="memberlist">
                 </ul>
 
             </li>
     </ul>
 
 
@@ -47,109 +47,122 @@
                 src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20role%3D%22img%22%20aria-label%3D%22pdoc%20logo%22%20width%3D%22300%22%20height%3D%22150%22%20viewBox%3D%22-1%200%2060%2030%22%3E%3Ctitle%3Epdoc%3C/title%3E%3Cpath%20d%3D%22M29.621%2021.293c-.011-.273-.214-.475-.511-.481a.5.5%200%200%200-.489.503l-.044%201.393c-.097.551-.695%201.215-1.566%201.704-.577.428-1.306.486-2.193.182-1.426-.617-2.467-1.654-3.304-2.487l-.173-.172a3.43%203.43%200%200%200-.365-.306.49.49%200%200%200-.286-.196c-1.718-1.06-4.931-1.47-7.353.191l-.219.15c-1.707%201.187-3.413%202.131-4.328%201.03-.02-.027-.49-.685-.141-1.763.233-.721.546-2.408.772-4.076.042-.09.067-.187.046-.288.166-1.347.277-2.625.241-3.351%201.378-1.008%202.271-2.586%202.271-4.362%200-.976-.272-1.935-.788-2.774-.057-.094-.122-.18-.184-.268.033-.167.052-.339.052-.516%200-1.477-1.202-2.679-2.679-2.679-.791%200-1.496.352-1.987.9a6.3%206.3%200%200%200-1.001.029c-.492-.564-1.207-.929-2.012-.929-1.477%200-2.679%201.202-2.679%202.679A2.65%202.65%200%200%200%20.97%206.554c-.383.747-.595%201.572-.595%202.41%200%202.311%201.507%204.29%203.635%205.107-.037.699-.147%202.27-.423%203.294l-.137.461c-.622%202.042-2.515%208.257%201.727%2010.643%201.614.908%203.06%201.248%204.317%201.248%202.665%200%204.492-1.524%205.322-2.401%201.476-1.559%202.886-1.854%206.491.82%201.877%201.393%203.514%201.753%204.861%201.068%202.223-1.713%202.811-3.867%203.399-6.374.077-.846.056-1.469.054-1.537zm-4.835%204.313c-.054.305-.156.586-.242.629-.034-.007-.131-.022-.307-.157-.145-.111-.314-.478-.456-.908.221.121.432.25.675.355.115.039.219.051.33.081zm-2.251-1.238c-.05.33-.158.648-.252.694-.022.001-.125-.018-.307-.157-.217-.166-.488-.906-.639-1.573.358.344.754.693%201.198%201.036zm-3.887-2.337c-.006-.116-.018-.231-.041-.342.635.145%201.189.368%201.599.625.097.231.166.481.174.642-.03.049-.055.101-.067.158-.046.013-.128.026-.298.004-.278-.037-.901-.57-1.367-1.087zm-1.127-.497c.116.306.176.625.12.71-.019.014-.117.045-.345.016-.206-.027-.604-.332-.986-.695.41-.051.816-.056%201.211-.031zm-4.535%201.535c.209.22.379.47.358.598-.006.041-.088.138-.351.234-.144.055-.539-.063-.979-.259a11.66%2011.66%200%200%200%20.972-.573zm.983-.664c.359-.237.738-.418%201.126-.554.25.237.479.548.457.694-.006.042-.087.138-.351.235-.174.064-.694-.105-1.232-.375zm-3.381%201.794c-.022.145-.061.29-.149.401-.133.166-.358.248-.69.251h-.002c-.133%200-.306-.26-.45-.621.417.091.854.07%201.291-.031zm-2.066-8.077a4.78%204.78%200%200%201-.775-.584c.172-.115.505-.254.88-.378l-.105.962zm-.331%202.302a10.32%2010.32%200%200%201-.828-.502c.202-.143.576-.328.984-.49l-.156.992zm-.45%202.157l-.701-.403c.214-.115.536-.249.891-.376a11.57%2011.57%200%200%201-.19.779zm-.181%201.716c.064.398.194.702.298.893-.194-.051-.435-.162-.736-.398.061-.119.224-.3.438-.495zM8.87%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zm-.735-.389a1.15%201.15%200%200%200-.314.783%201.16%201.16%200%200%200%201.162%201.162c.457%200%20.842-.27%201.032-.653.026.117.042.238.042.362a1.68%201.68%200%200%201-1.679%201.679%201.68%201.68%200%200%201-1.679-1.679c0-.843.626-1.535%201.436-1.654zM5.059%205.406A1.68%201.68%200%200%201%203.38%207.085a1.68%201.68%200%200%201-1.679-1.679c0-.037.009-.072.011-.109.21.3.541.508.935.508a1.16%201.16%200%200%200%201.162-1.162%201.14%201.14%200%200%200-.474-.912c.015%200%20.03-.005.045-.005.926.001%201.679.754%201.679%201.68zM3.198%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zM1.375%208.964c0-.52.103-1.035.288-1.52.466.394%201.06.64%201.717.64%201.144%200%202.116-.725%202.499-1.738.383%201.012%201.355%201.738%202.499%201.738.867%200%201.631-.421%202.121-1.062.307.605.478%201.267.478%201.942%200%202.486-2.153%204.51-4.801%204.51s-4.801-2.023-4.801-4.51zm24.342%2019.349c-.985.498-2.267.168-3.813-.979-3.073-2.281-5.453-3.199-7.813-.705-1.315%201.391-4.163%203.365-8.423.97-3.174-1.786-2.239-6.266-1.261-9.479l.146-.492c.276-1.02.395-2.457.444-3.268a6.11%206.11%200%200%200%201.18.115%206.01%206.01%200%200%200%202.536-.562l-.006.175c-.802.215-1.848.612-2.021%201.25-.079.295.021.601.274.837.219.203.415.364.598.501-.667.304-1.243.698-1.311%201.179-.02.144-.022.507.393.787.213.144.395.26.564.365-1.285.521-1.361.96-1.381%201.126-.018.142-.011.496.427.746l.854.489c-.473.389-.971.914-.999%201.429-.018.278.095.532.316.713.675.556%201.231.721%201.653.721.059%200%20.104-.014.158-.02.207.707.641%201.64%201.513%201.64h.013c.8-.008%201.236-.345%201.462-.626.173-.216.268-.457.325-.692.424.195.93.374%201.372.374.151%200%20.294-.021.423-.068.732-.27.944-.704.993-1.021.009-.061.003-.119.002-.179.266.086.538.147.789.147.15%200%20.294-.021.423-.069.542-.2.797-.489.914-.754.237.147.478.258.704.288.106.014.205.021.296.021.356%200%20.595-.101.767-.229.438.435%201.094.992%201.656%201.067.106.014.205.021.296.021a1.56%201.56%200%200%200%20.323-.035c.17.575.453%201.289.866%201.605.358.273.665.362.914.362a.99.99%200%200%200%20.421-.093%201.03%201.03%200%200%200%20.245-.164c.168.428.39.846.68%201.068.358.273.665.362.913.362a.99.99%200%200%200%20.421-.093c.317-.148.512-.448.639-.762.251.157.495.257.726.257.127%200%20.25-.024.37-.071.427-.17.706-.617.841-1.314.022-.015.047-.022.068-.038.067-.051.133-.104.196-.159-.443%201.486-1.107%202.761-2.086%203.257zM8.66%209.925a.5.5%200%201%200-1%200c0%20.653-.818%201.205-1.787%201.205s-1.787-.552-1.787-1.205a.5.5%200%201%200-1%200c0%201.216%201.25%202.205%202.787%202.205s2.787-.989%202.787-2.205zm4.4%2015.965l-.208.097c-2.661%201.258-4.708%201.436-6.086.527-1.542-1.017-1.88-3.19-1.844-4.198a.4.4%200%200%200-.385-.414c-.242-.029-.406.164-.414.385-.046%201.249.367%203.686%202.202%204.896.708.467%201.547.7%202.51.7%201.248%200%202.706-.392%204.362-1.174l.185-.086a.4.4%200%200%200%20.205-.527c-.089-.204-.326-.291-.527-.206zM9.547%202.292c.093.077.205.114.317.114a.5.5%200%200%200%20.318-.886L8.817.397a.5.5%200%200%200-.703.068.5.5%200%200%200%20.069.703l1.364%201.124zm-7.661-.065c.086%200%20.173-.022.253-.068l1.523-.893a.5.5%200%200%200-.506-.863l-1.523.892a.5.5%200%200%200-.179.685c.094.158.261.247.432.247z%22%20transform%3D%22matrix%28-1%200%200%201%2058%200%29%22%20fill%3D%22%233bb300%22/%3E%3Cpath%20d%3D%22M.3%2021.86V10.18q0-.46.02-.68.04-.22.18-.5.28-.54%201.34-.54%201.06%200%201.42.28.38.26.44.78.76-1.04%202.38-1.04%201.64%200%203.1%201.54%201.46%201.54%201.46%203.58%200%202.04-1.46%203.58-1.44%201.54-3.08%201.54-1.64%200-2.38-.92v4.04q0%20.46-.04.68-.02.22-.18.5-.14.3-.5.42-.36.12-.98.12-.62%200-1-.12-.36-.12-.52-.4-.14-.28-.18-.5-.02-.22-.02-.68zm3.96-9.42q-.46.54-.46%201.18%200%20.64.46%201.18.48.52%201.2.52.74%200%201.24-.52.52-.52.52-1.18%200-.66-.48-1.18-.48-.54-1.26-.54-.76%200-1.22.54zm14.741-8.36q.16-.3.54-.42.38-.12%201-.12.64%200%201.02.12.38.12.52.42.16.3.18.54.04.22.04.68v11.94q0%20.46-.04.7-.02.22-.18.5-.3.54-1.7.54-1.38%200-1.54-.98-.84.96-2.34.96-1.8%200-3.28-1.56-1.48-1.58-1.48-3.66%200-2.1%201.48-3.68%201.5-1.58%203.28-1.58%201.48%200%202.3%201v-4.2q0-.46.02-.68.04-.24.18-.52zm-3.24%2010.86q.52.54%201.26.54.74%200%201.22-.54.5-.54.5-1.18%200-.66-.48-1.22-.46-.56-1.26-.56-.8%200-1.28.56-.48.54-.48%201.2%200%20.66.52%201.2zm7.833-1.2q0-2.4%201.68-3.96%201.68-1.56%203.84-1.56%202.16%200%203.82%201.56%201.66%201.54%201.66%203.94%200%201.66-.86%202.96-.86%201.28-2.1%201.9-1.22.6-2.54.6-1.32%200-2.56-.64-1.24-.66-2.1-1.92-.84-1.28-.84-2.88zm4.18%201.44q.64.48%201.3.48.66%200%201.32-.5.66-.5.66-1.48%200-.98-.62-1.46-.62-.48-1.34-.48-.72%200-1.34.5-.62.5-.62%201.48%200%20.96.64%201.46zm11.412-1.44q0%20.84.56%201.32.56.46%201.18.46.64%200%201.18-.36.56-.38.9-.38.6%200%201.46%201.06.46.58.46%201.04%200%20.76-1.1%201.42-1.14.8-2.8.8-1.86%200-3.58-1.34-.82-.64-1.34-1.7-.52-1.08-.52-2.36%200-1.3.52-2.34.52-1.06%201.34-1.7%201.66-1.32%203.54-1.32.76%200%201.48.22.72.2%201.06.4l.32.2q.36.24.56.38.52.4.52.92%200%20.5-.42%201.14-.72%201.1-1.38%201.1-.38%200-1.08-.44-.36-.34-1.04-.34-.66%200-1.24.48-.58.48-.58%201.34z%22%20fill%3D%22green%22/%3E%3C/svg%3E"/>
         </a>
 </div>
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
-<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.booking    </h1>
+<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.skill    </h1>
 
                 
-                        <input id="mod-booking-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                        <input id="mod-skill-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
-                        <label class="view-source-button" for="mod-booking-view-source"><span>View Source</span></label>
+                        <label class="view-source-button" for="mod-skill-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">from</span> <span class="nn">projectal.entity</span> <span class="kn">import</span> <span class="n">Entity</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">from</span> <span class="nn">projectal.linkers</span> <span class="kn">import</span> <span class="o">*</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Booking</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Skill</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Booking](https://projectal.com/docs/latest/#tag/Booking) API.</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/Skill) API.</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>  <span class="c1"># TODO: note?</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
             </section>
-                <section id="Booking">
-                            <input id="Booking-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="Skill">
+                            <input id="Skill-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
-    <span class="name">Booking</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#StageLinker">projectal.linkers.StageLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
+    <span class="name">Skill</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></span>, <span class="base"><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></span>, <span class="base"><a href="../linkers.html#TaskTemplateLinker">projectal.linkers.TaskTemplateLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
 
-                <label class="view-source-button" for="Booking-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Skill-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Booking"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Booking-6"><a href="#Booking-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Booking</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="Booking-7"><a href="#Booking-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Booking-8"><a href="#Booking-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Booking](https://projectal.com/docs/latest/#tag/Booking) API.</span>
-</span><span id="Booking-9"><a href="#Booking-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Booking-10"><a href="#Booking-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
-</span><span id="Booking-11"><a href="#Booking-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
-</span><span id="Booking-12"><a href="#Booking-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">StageLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">]</span>
+    <a class="headerlink" href="#Skill"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Skill-6"><a href="#Skill-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Skill</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="Skill-7"><a href="#Skill-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Skill-8"><a href="#Skill-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/Skill) API.</span>
+</span><span id="Skill-9"><a href="#Skill-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Skill-10"><a href="#Skill-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="Skill-11"><a href="#Skill-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="Skill-12"><a href="#Skill-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>  <span class="c1"># TODO: note?</span>
+</span><span id="Skill-13"><a href="#Skill-13"><span class="linenos">13</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Booking">Booking</a> API.</p>
+            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Skill">Skill</a> API.</p>
 </div>
 
 
                             <div class="inherited">
                                 <h5>Inherited Members</h5>
                                 <dl>
                                     <div><dt><a href="../entity.html#Entity">projectal.entity.Entity</a></dt>
-                                <dd id="Booking.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
-                <dd id="Booking.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
-                <dd id="Booking.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
-                <dd id="Booking.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
-                <dd id="Booking.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
-                <dd id="Booking.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
-                <dd id="Booking.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
-                <dd id="Booking.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
-                <dd id="Booking.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
-                <dd id="Booking.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
-                <dd id="Booking.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
-                <dd id="Booking.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
-                <dd id="Booking.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
-                <dd id="Booking.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
-                <dd id="Booking.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
-                <dd id="Booking.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
-                <dd id="Booking.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
-                <dd id="Booking.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
-                <dd id="Booking.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
-                <dd id="Booking.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
-                <dd id="Booking.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
-                <dd id="Booking.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#StageLinker">projectal.linkers.StageLinker</a></dt>
-                                <dd id="Booking.link_stage" class="function"><a href="../linkers.html#StageLinker.link_stage">link_stage</a></dd>
-                <dd id="Booking.unlink_stage" class="function"><a href="../linkers.html#StageLinker.unlink_stage">unlink_stage</a></dd>
+                                <dd id="Skill.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
+                <dd id="Skill.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
+                <dd id="Skill.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
+                <dd id="Skill.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
+                <dd id="Skill.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
+                <dd id="Skill.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
+                <dd id="Skill.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
+                <dd id="Skill.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
+                <dd id="Skill.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
+                <dd id="Skill.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
+                <dd id="Skill.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
+                <dd id="Skill.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
+                <dd id="Skill.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
+                <dd id="Skill.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
+                <dd id="Skill.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
+                <dd id="Skill.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
+                <dd id="Skill.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
+                <dd id="Skill.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
+                <dd id="Skill.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
+                <dd id="Skill.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
+                <dd id="Skill.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
+                <dd id="Skill.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
+
+            </div>
+            <div><dt><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></dt>
+                                <dd id="Skill.link_staff" class="function"><a href="../linkers.html#StaffLinker.link_staff">link_staff</a></dd>
+                <dd id="Skill.relink_staff" class="function"><a href="../linkers.html#StaffLinker.relink_staff">relink_staff</a></dd>
+                <dd id="Skill.unlink_staff" class="function"><a href="../linkers.html#StaffLinker.unlink_staff">unlink_staff</a></dd>
+
+            </div>
+            <div><dt><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></dt>
+                                <dd id="Skill.link_task" class="function"><a href="../linkers.html#TaskLinker.link_task">link_task</a></dd>
+                <dd id="Skill.unlink_task" class="function"><a href="../linkers.html#TaskLinker.unlink_task">unlink_task</a></dd>
+
+            </div>
+            <div><dt><a href="../linkers.html#TaskTemplateLinker">projectal.linkers.TaskTemplateLinker</a></dt>
+                                <dd id="Skill.link_task_template" class="function"><a href="../linkers.html#TaskTemplateLinker.link_task_template">link_task_template</a></dd>
+                <dd id="Skill.unlink_task_template" class="function"><a href="../linkers.html#TaskTemplateLinker.unlink_task_template">unlink_task_template</a></dd>
 
             </div>
             <div><dt><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></dt>
-                                <dd id="Booking.link_tag" class="function"><a href="../linkers.html#TagLinker.link_tag">link_tag</a></dd>
-                <dd id="Booking.unlink_tag" class="function"><a href="../linkers.html#TagLinker.unlink_tag">unlink_tag</a></dd>
+                                <dd id="Skill.link_tag" class="function"><a href="../linkers.html#TagLinker.link_tag">link_tag</a></dd>
+                <dd id="Skill.unlink_tag" class="function"><a href="../linkers.html#TagLinker.unlink_tag">unlink_tag</a></dd>
 
             </div>
             <div><dt>builtins.dict</dt>
-                                <dd id="Booking.setdefault" class="function">setdefault</dd>
-                <dd id="Booking.pop" class="function">pop</dd>
-                <dd id="Booking.popitem" class="function">popitem</dd>
-                <dd id="Booking.keys" class="function">keys</dd>
-                <dd id="Booking.items" class="function">items</dd>
-                <dd id="Booking.values" class="function">values</dd>
-                <dd id="Booking.fromkeys" class="function">fromkeys</dd>
-                <dd id="Booking.clear" class="function">clear</dd>
-                <dd id="Booking.copy" class="function">copy</dd>
+                                <dd id="Skill.setdefault" class="function">setdefault</dd>
+                <dd id="Skill.pop" class="function">pop</dd>
+                <dd id="Skill.popitem" class="function">popitem</dd>
+                <dd id="Skill.keys" class="function">keys</dd>
+                <dd id="Skill.items" class="function">items</dd>
+                <dd id="Skill.values" class="function">values</dd>
+                <dd id="Skill.fromkeys" class="function">fromkeys</dd>
+                <dd id="Skill.clear" class="function">clear</dd>
+                <dd id="Skill.copy" class="function">copy</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -1,36 +1,39 @@
 
 
   ⁰
 ____ projectal.entities [project logo] [Unknown INPUT type]
 ***** API Documentation *****
-    * Booking
+    * Skill
 built_with_pdoc[pdoc_logo]
 
-****** projectal.entities.booking ******
+****** projectal.entities.skill ******
 ⁰ View Source
 _1from projectal.entity import Entity
 _2from projectal.linkers import *
 _3
 _4
-_5class Booking(Entity, StageLinker, TagLinker):
+_5class Skill(Entity, StaffLinker, TaskLinker, TaskTemplateLinker, TagLinker):
 _6    """
-_7    Implementation of the [Booking](https://projectal.com/docs/latest/#tag/
-Booking) API.
+_7    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/
+Skill) API.
 _8    """
-_9    _path = 'booking'
-10    _name = 'booking'
-11    _links = [StageLinker, TagLinker]
+_9    _path = 'skill'
+10    _name = 'skill'
+11    _links = [TagLinker]  # TODO: note?
+12    _links_reverse = [StaffLinker, TaskLinker, TaskTemplateLinker]
   ⁰
-class Booking(projectal.entity.Entity, projectal.linkers.StageLinker,
+class Skill(projectal.entity.Entity, projectal.linkers.StaffLinker,
+projectal.linkers.TaskLinker, projectal.linkers.TaskTemplateLinker,
 projectal.linkers.TagLinker): View Source
-_6class Booking(Entity, StageLinker, TagLinker):
+_6class Skill(Entity, StaffLinker, TaskLinker, TaskTemplateLinker, TagLinker):
 _7    """
-_8    Implementation of the [Booking](https://projectal.com/docs/latest/#tag/
-Booking) API.
+_8    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/
+Skill) API.
 _9    """
-10    _path = 'booking'
-11    _name = 'booking'
-12    _links = [StageLinker, TagLinker]
-Implementation of the Booking API.
+10    _path = 'skill'
+11    _name = 'skill'
+12    _links = [TagLinker]  # TODO: note?
+13    _links_reverse = [StaffLinker, TaskLinker, TaskTemplateLinker]
+Implementation of the Skill API.
 ** Inherited Members **
```

### Comparing `projectal-4.0.1/docs/projectal/entities/calendar.html` & `projectal-4.0.2/docs/projectal/entities/calendar.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/company.html` & `projectal-4.0.2/docs/projectal/entities/company.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/contact.html` & `projectal-4.0.2/docs/projectal/entities/contact.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/customer.html` & `projectal-4.0.2/docs/projectal/entities/customer.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/department.html` & `projectal-4.0.2/docs/projectal/entities/department.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/file.html` & `projectal-4.0.2/docs/projectal/entities/file.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/folder.html` & `projectal-4.0.2/docs/projectal/entities/folder.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/location.html` & `projectal-4.0.2/docs/projectal/entities/location.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/note.html` & `projectal-4.0.2/docs/projectal/entities/note.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/permission.html` & `projectal-4.0.2/docs/projectal/entities/permission.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/project.html` & `projectal-4.0.2/docs/projectal/entities/project.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/project_template.html` & `projectal-4.0.2/docs/projectal/entities/project_template.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/rebate.html` & `projectal-4.0.2/docs/projectal/entities/rebate.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/resource.html` & `projectal-4.0.2/docs/projectal/entities/resource.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/skill.html` & `projectal-4.0.2/docs/projectal/entities/stage.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <meta name="generator" content="pdoc 12.3.0"/>
-    <title>projectal.entities.skill API documentation</title>
+    <title>projectal.entities.stage API documentation</title>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
     <style>/*! custom.css */</style></head>
@@ -28,15 +28,15 @@
                    pattern=".+" required>
 
 
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
-                    <a class="class" href="#Skill">Skill</a>
+                    <a class="class" href="#Stage">Stage</a>
                             <ul class="memberlist">
                 </ul>
 
             </li>
     </ul>
 
 
@@ -47,122 +47,116 @@
                 src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20role%3D%22img%22%20aria-label%3D%22pdoc%20logo%22%20width%3D%22300%22%20height%3D%22150%22%20viewBox%3D%22-1%200%2060%2030%22%3E%3Ctitle%3Epdoc%3C/title%3E%3Cpath%20d%3D%22M29.621%2021.293c-.011-.273-.214-.475-.511-.481a.5.5%200%200%200-.489.503l-.044%201.393c-.097.551-.695%201.215-1.566%201.704-.577.428-1.306.486-2.193.182-1.426-.617-2.467-1.654-3.304-2.487l-.173-.172a3.43%203.43%200%200%200-.365-.306.49.49%200%200%200-.286-.196c-1.718-1.06-4.931-1.47-7.353.191l-.219.15c-1.707%201.187-3.413%202.131-4.328%201.03-.02-.027-.49-.685-.141-1.763.233-.721.546-2.408.772-4.076.042-.09.067-.187.046-.288.166-1.347.277-2.625.241-3.351%201.378-1.008%202.271-2.586%202.271-4.362%200-.976-.272-1.935-.788-2.774-.057-.094-.122-.18-.184-.268.033-.167.052-.339.052-.516%200-1.477-1.202-2.679-2.679-2.679-.791%200-1.496.352-1.987.9a6.3%206.3%200%200%200-1.001.029c-.492-.564-1.207-.929-2.012-.929-1.477%200-2.679%201.202-2.679%202.679A2.65%202.65%200%200%200%20.97%206.554c-.383.747-.595%201.572-.595%202.41%200%202.311%201.507%204.29%203.635%205.107-.037.699-.147%202.27-.423%203.294l-.137.461c-.622%202.042-2.515%208.257%201.727%2010.643%201.614.908%203.06%201.248%204.317%201.248%202.665%200%204.492-1.524%205.322-2.401%201.476-1.559%202.886-1.854%206.491.82%201.877%201.393%203.514%201.753%204.861%201.068%202.223-1.713%202.811-3.867%203.399-6.374.077-.846.056-1.469.054-1.537zm-4.835%204.313c-.054.305-.156.586-.242.629-.034-.007-.131-.022-.307-.157-.145-.111-.314-.478-.456-.908.221.121.432.25.675.355.115.039.219.051.33.081zm-2.251-1.238c-.05.33-.158.648-.252.694-.022.001-.125-.018-.307-.157-.217-.166-.488-.906-.639-1.573.358.344.754.693%201.198%201.036zm-3.887-2.337c-.006-.116-.018-.231-.041-.342.635.145%201.189.368%201.599.625.097.231.166.481.174.642-.03.049-.055.101-.067.158-.046.013-.128.026-.298.004-.278-.037-.901-.57-1.367-1.087zm-1.127-.497c.116.306.176.625.12.71-.019.014-.117.045-.345.016-.206-.027-.604-.332-.986-.695.41-.051.816-.056%201.211-.031zm-4.535%201.535c.209.22.379.47.358.598-.006.041-.088.138-.351.234-.144.055-.539-.063-.979-.259a11.66%2011.66%200%200%200%20.972-.573zm.983-.664c.359-.237.738-.418%201.126-.554.25.237.479.548.457.694-.006.042-.087.138-.351.235-.174.064-.694-.105-1.232-.375zm-3.381%201.794c-.022.145-.061.29-.149.401-.133.166-.358.248-.69.251h-.002c-.133%200-.306-.26-.45-.621.417.091.854.07%201.291-.031zm-2.066-8.077a4.78%204.78%200%200%201-.775-.584c.172-.115.505-.254.88-.378l-.105.962zm-.331%202.302a10.32%2010.32%200%200%201-.828-.502c.202-.143.576-.328.984-.49l-.156.992zm-.45%202.157l-.701-.403c.214-.115.536-.249.891-.376a11.57%2011.57%200%200%201-.19.779zm-.181%201.716c.064.398.194.702.298.893-.194-.051-.435-.162-.736-.398.061-.119.224-.3.438-.495zM8.87%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zm-.735-.389a1.15%201.15%200%200%200-.314.783%201.16%201.16%200%200%200%201.162%201.162c.457%200%20.842-.27%201.032-.653.026.117.042.238.042.362a1.68%201.68%200%200%201-1.679%201.679%201.68%201.68%200%200%201-1.679-1.679c0-.843.626-1.535%201.436-1.654zM5.059%205.406A1.68%201.68%200%200%201%203.38%207.085a1.68%201.68%200%200%201-1.679-1.679c0-.037.009-.072.011-.109.21.3.541.508.935.508a1.16%201.16%200%200%200%201.162-1.162%201.14%201.14%200%200%200-.474-.912c.015%200%20.03-.005.045-.005.926.001%201.679.754%201.679%201.68zM3.198%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zM1.375%208.964c0-.52.103-1.035.288-1.52.466.394%201.06.64%201.717.64%201.144%200%202.116-.725%202.499-1.738.383%201.012%201.355%201.738%202.499%201.738.867%200%201.631-.421%202.121-1.062.307.605.478%201.267.478%201.942%200%202.486-2.153%204.51-4.801%204.51s-4.801-2.023-4.801-4.51zm24.342%2019.349c-.985.498-2.267.168-3.813-.979-3.073-2.281-5.453-3.199-7.813-.705-1.315%201.391-4.163%203.365-8.423.97-3.174-1.786-2.239-6.266-1.261-9.479l.146-.492c.276-1.02.395-2.457.444-3.268a6.11%206.11%200%200%200%201.18.115%206.01%206.01%200%200%200%202.536-.562l-.006.175c-.802.215-1.848.612-2.021%201.25-.079.295.021.601.274.837.219.203.415.364.598.501-.667.304-1.243.698-1.311%201.179-.02.144-.022.507.393.787.213.144.395.26.564.365-1.285.521-1.361.96-1.381%201.126-.018.142-.011.496.427.746l.854.489c-.473.389-.971.914-.999%201.429-.018.278.095.532.316.713.675.556%201.231.721%201.653.721.059%200%20.104-.014.158-.02.207.707.641%201.64%201.513%201.64h.013c.8-.008%201.236-.345%201.462-.626.173-.216.268-.457.325-.692.424.195.93.374%201.372.374.151%200%20.294-.021.423-.068.732-.27.944-.704.993-1.021.009-.061.003-.119.002-.179.266.086.538.147.789.147.15%200%20.294-.021.423-.069.542-.2.797-.489.914-.754.237.147.478.258.704.288.106.014.205.021.296.021.356%200%20.595-.101.767-.229.438.435%201.094.992%201.656%201.067.106.014.205.021.296.021a1.56%201.56%200%200%200%20.323-.035c.17.575.453%201.289.866%201.605.358.273.665.362.914.362a.99.99%200%200%200%20.421-.093%201.03%201.03%200%200%200%20.245-.164c.168.428.39.846.68%201.068.358.273.665.362.913.362a.99.99%200%200%200%20.421-.093c.317-.148.512-.448.639-.762.251.157.495.257.726.257.127%200%20.25-.024.37-.071.427-.17.706-.617.841-1.314.022-.015.047-.022.068-.038.067-.051.133-.104.196-.159-.443%201.486-1.107%202.761-2.086%203.257zM8.66%209.925a.5.5%200%201%200-1%200c0%20.653-.818%201.205-1.787%201.205s-1.787-.552-1.787-1.205a.5.5%200%201%200-1%200c0%201.216%201.25%202.205%202.787%202.205s2.787-.989%202.787-2.205zm4.4%2015.965l-.208.097c-2.661%201.258-4.708%201.436-6.086.527-1.542-1.017-1.88-3.19-1.844-4.198a.4.4%200%200%200-.385-.414c-.242-.029-.406.164-.414.385-.046%201.249.367%203.686%202.202%204.896.708.467%201.547.7%202.51.7%201.248%200%202.706-.392%204.362-1.174l.185-.086a.4.4%200%200%200%20.205-.527c-.089-.204-.326-.291-.527-.206zM9.547%202.292c.093.077.205.114.317.114a.5.5%200%200%200%20.318-.886L8.817.397a.5.5%200%200%200-.703.068.5.5%200%200%200%20.069.703l1.364%201.124zm-7.661-.065c.086%200%20.173-.022.253-.068l1.523-.893a.5.5%200%200%200-.506-.863l-1.523.892a.5.5%200%200%200-.179.685c.094.158.261.247.432.247z%22%20transform%3D%22matrix%28-1%200%200%201%2058%200%29%22%20fill%3D%22%233bb300%22/%3E%3Cpath%20d%3D%22M.3%2021.86V10.18q0-.46.02-.68.04-.22.18-.5.28-.54%201.34-.54%201.06%200%201.42.28.38.26.44.78.76-1.04%202.38-1.04%201.64%200%203.1%201.54%201.46%201.54%201.46%203.58%200%202.04-1.46%203.58-1.44%201.54-3.08%201.54-1.64%200-2.38-.92v4.04q0%20.46-.04.68-.02.22-.18.5-.14.3-.5.42-.36.12-.98.12-.62%200-1-.12-.36-.12-.52-.4-.14-.28-.18-.5-.02-.22-.02-.68zm3.96-9.42q-.46.54-.46%201.18%200%20.64.46%201.18.48.52%201.2.52.74%200%201.24-.52.52-.52.52-1.18%200-.66-.48-1.18-.48-.54-1.26-.54-.76%200-1.22.54zm14.741-8.36q.16-.3.54-.42.38-.12%201-.12.64%200%201.02.12.38.12.52.42.16.3.18.54.04.22.04.68v11.94q0%20.46-.04.7-.02.22-.18.5-.3.54-1.7.54-1.38%200-1.54-.98-.84.96-2.34.96-1.8%200-3.28-1.56-1.48-1.58-1.48-3.66%200-2.1%201.48-3.68%201.5-1.58%203.28-1.58%201.48%200%202.3%201v-4.2q0-.46.02-.68.04-.24.18-.52zm-3.24%2010.86q.52.54%201.26.54.74%200%201.22-.54.5-.54.5-1.18%200-.66-.48-1.22-.46-.56-1.26-.56-.8%200-1.28.56-.48.54-.48%201.2%200%20.66.52%201.2zm7.833-1.2q0-2.4%201.68-3.96%201.68-1.56%203.84-1.56%202.16%200%203.82%201.56%201.66%201.54%201.66%203.94%200%201.66-.86%202.96-.86%201.28-2.1%201.9-1.22.6-2.54.6-1.32%200-2.56-.64-1.24-.66-2.1-1.92-.84-1.28-.84-2.88zm4.18%201.44q.64.48%201.3.48.66%200%201.32-.5.66-.5.66-1.48%200-.98-.62-1.46-.62-.48-1.34-.48-.72%200-1.34.5-.62.5-.62%201.48%200%20.96.64%201.46zm11.412-1.44q0%20.84.56%201.32.56.46%201.18.46.64%200%201.18-.36.56-.38.9-.38.6%200%201.46%201.06.46.58.46%201.04%200%20.76-1.1%201.42-1.14.8-2.8.8-1.86%200-3.58-1.34-.82-.64-1.34-1.7-.52-1.08-.52-2.36%200-1.3.52-2.34.52-1.06%201.34-1.7%201.66-1.32%203.54-1.32.76%200%201.48.22.72.2%201.06.4l.32.2q.36.24.56.38.52.4.52.92%200%20.5-.42%201.14-.72%201.1-1.38%201.1-.38%200-1.08-.44-.36-.34-1.04-.34-.66%200-1.24.48-.58.48-.58%201.34z%22%20fill%3D%22green%22/%3E%3C/svg%3E"/>
         </a>
 </div>
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
-<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.skill    </h1>
+<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.stage    </h1>
 
                 
-                        <input id="mod-skill-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                        <input id="mod-stage-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
-                        <label class="view-source-button" for="mod-skill-view-source"><span>View Source</span></label>
+                        <label class="view-source-button" for="mod-stage-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">from</span> <span class="nn">projectal.entity</span> <span class="kn">import</span> <span class="n">Entity</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">from</span> <span class="nn">projectal.linkers</span> <span class="kn">import</span> <span class="o">*</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
 </span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Skill</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Stage</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/Skill) API.</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/Stage) API.</span>
 </span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>  <span class="c1"># TODO: note?</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">]</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
             </section>
-                <section id="Skill">
-                            <input id="Skill-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="Stage">
+                            <input id="Stage-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
-    <span class="name">Skill</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></span>, <span class="base"><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></span>, <span class="base"><a href="../linkers.html#TaskTemplateLinker">projectal.linkers.TaskTemplateLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
+    <span class="name">Stage</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#ProjectLinker">projectal.linkers.ProjectLinker</a></span>, <span class="base"><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
 
-                <label class="view-source-button" for="Skill-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Stage-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Skill"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Skill-6"><a href="#Skill-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Skill</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="Skill-7"><a href="#Skill-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Skill-8"><a href="#Skill-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/Skill) API.</span>
-</span><span id="Skill-9"><a href="#Skill-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Skill-10"><a href="#Skill-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="Skill-11"><a href="#Skill-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="Skill-12"><a href="#Skill-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>  <span class="c1"># TODO: note?</span>
-</span><span id="Skill-13"><a href="#Skill-13"><span class="linenos">13</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">StaffLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TaskTemplateLinker</span><span class="p">]</span>
+    <a class="headerlink" href="#Stage"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Stage-6"><a href="#Stage-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Stage</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
+</span><span id="Stage-7"><a href="#Stage-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Stage-8"><a href="#Stage-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/Stage) API.</span>
+</span><span id="Stage-9"><a href="#Stage-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Stage-10"><a href="#Stage-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="Stage-11"><a href="#Stage-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="Stage-12"><a href="#Stage-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>
+</span><span id="Stage-13"><a href="#Stage-13"><span class="linenos">13</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">]</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Skill">Skill</a> API.</p>
+            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Stage">Stage</a> API.</p>
 </div>
 
 
                             <div class="inherited">
                                 <h5>Inherited Members</h5>
                                 <dl>
                                     <div><dt><a href="../entity.html#Entity">projectal.entity.Entity</a></dt>
-                                <dd id="Skill.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
-                <dd id="Skill.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
-                <dd id="Skill.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
-                <dd id="Skill.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
-                <dd id="Skill.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
-                <dd id="Skill.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
-                <dd id="Skill.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
-                <dd id="Skill.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
-                <dd id="Skill.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
-                <dd id="Skill.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
-                <dd id="Skill.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
-                <dd id="Skill.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
-                <dd id="Skill.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
-                <dd id="Skill.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
-                <dd id="Skill.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
-                <dd id="Skill.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
-                <dd id="Skill.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
-                <dd id="Skill.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
-                <dd id="Skill.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
-                <dd id="Skill.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
-                <dd id="Skill.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
-                <dd id="Skill.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#StaffLinker">projectal.linkers.StaffLinker</a></dt>
-                                <dd id="Skill.link_staff" class="function"><a href="../linkers.html#StaffLinker.link_staff">link_staff</a></dd>
-                <dd id="Skill.relink_staff" class="function"><a href="../linkers.html#StaffLinker.relink_staff">relink_staff</a></dd>
-                <dd id="Skill.unlink_staff" class="function"><a href="../linkers.html#StaffLinker.unlink_staff">unlink_staff</a></dd>
+                                <dd id="Stage.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
+                <dd id="Stage.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
+                <dd id="Stage.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
+                <dd id="Stage.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
+                <dd id="Stage.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
+                <dd id="Stage.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
+                <dd id="Stage.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
+                <dd id="Stage.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
+                <dd id="Stage.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
+                <dd id="Stage.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
+                <dd id="Stage.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
+                <dd id="Stage.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
+                <dd id="Stage.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
+                <dd id="Stage.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
+                <dd id="Stage.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
+                <dd id="Stage.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
+                <dd id="Stage.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
+                <dd id="Stage.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
+                <dd id="Stage.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
+                <dd id="Stage.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
+                <dd id="Stage.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
+                <dd id="Stage.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
+
+            </div>
+            <div><dt><a href="../linkers.html#ProjectLinker">projectal.linkers.ProjectLinker</a></dt>
+                                <dd id="Stage.link_project" class="function"><a href="../linkers.html#ProjectLinker.link_project">link_project</a></dd>
+                <dd id="Stage.unlink_project" class="function"><a href="../linkers.html#ProjectLinker.unlink_project">unlink_project</a></dd>
 
             </div>
             <div><dt><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></dt>
-                                <dd id="Skill.link_task" class="function"><a href="../linkers.html#TaskLinker.link_task">link_task</a></dd>
-                <dd id="Skill.unlink_task" class="function"><a href="../linkers.html#TaskLinker.unlink_task">unlink_task</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#TaskTemplateLinker">projectal.linkers.TaskTemplateLinker</a></dt>
-                                <dd id="Skill.link_task_template" class="function"><a href="../linkers.html#TaskTemplateLinker.link_task_template">link_task_template</a></dd>
-                <dd id="Skill.unlink_task_template" class="function"><a href="../linkers.html#TaskTemplateLinker.unlink_task_template">unlink_task_template</a></dd>
+                                <dd id="Stage.link_task" class="function"><a href="../linkers.html#TaskLinker.link_task">link_task</a></dd>
+                <dd id="Stage.unlink_task" class="function"><a href="../linkers.html#TaskLinker.unlink_task">unlink_task</a></dd>
 
             </div>
             <div><dt><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></dt>
-                                <dd id="Skill.link_tag" class="function"><a href="../linkers.html#TagLinker.link_tag">link_tag</a></dd>
-                <dd id="Skill.unlink_tag" class="function"><a href="../linkers.html#TagLinker.unlink_tag">unlink_tag</a></dd>
+                                <dd id="Stage.link_tag" class="function"><a href="../linkers.html#TagLinker.link_tag">link_tag</a></dd>
+                <dd id="Stage.unlink_tag" class="function"><a href="../linkers.html#TagLinker.unlink_tag">unlink_tag</a></dd>
 
             </div>
             <div><dt>builtins.dict</dt>
-                                <dd id="Skill.setdefault" class="function">setdefault</dd>
-                <dd id="Skill.pop" class="function">pop</dd>
-                <dd id="Skill.popitem" class="function">popitem</dd>
-                <dd id="Skill.keys" class="function">keys</dd>
-                <dd id="Skill.items" class="function">items</dd>
-                <dd id="Skill.values" class="function">values</dd>
-                <dd id="Skill.fromkeys" class="function">fromkeys</dd>
-                <dd id="Skill.clear" class="function">clear</dd>
-                <dd id="Skill.copy" class="function">copy</dd>
+                                <dd id="Stage.setdefault" class="function">setdefault</dd>
+                <dd id="Stage.pop" class="function">pop</dd>
+                <dd id="Stage.popitem" class="function">popitem</dd>
+                <dd id="Stage.keys" class="function">keys</dd>
+                <dd id="Stage.items" class="function">items</dd>
+                <dd id="Stage.values" class="function">values</dd>
+                <dd id="Stage.fromkeys" class="function">fromkeys</dd>
+                <dd id="Stage.clear" class="function">clear</dd>
+                <dd id="Stage.copy" class="function">copy</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -1,39 +1,38 @@
 
 
   ⁰
 ____ projectal.entities [project logo] [Unknown INPUT type]
 ***** API Documentation *****
-    * Skill
+    * Stage
 built_with_pdoc[pdoc_logo]
 
-****** projectal.entities.skill ******
+****** projectal.entities.stage ******
 ⁰ View Source
 _1from projectal.entity import Entity
 _2from projectal.linkers import *
 _3
 _4
-_5class Skill(Entity, StaffLinker, TaskLinker, TaskTemplateLinker, TagLinker):
+_5class Stage(Entity, ProjectLinker, TaskLinker, TagLinker):
 _6    """
-_7    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/
-Skill) API.
+_7    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/
+Stage) API.
 _8    """
-_9    _path = 'skill'
-10    _name = 'skill'
-11    _links = [TagLinker]  # TODO: note?
-12    _links_reverse = [StaffLinker, TaskLinker, TaskTemplateLinker]
+_9    _path = 'stage'
+10    _name = 'stage'
+11    _links = [TagLinker]
+12    _links_reverse = [ProjectLinker, TaskLinker]
   ⁰
-class Skill(projectal.entity.Entity, projectal.linkers.StaffLinker,
-projectal.linkers.TaskLinker, projectal.linkers.TaskTemplateLinker,
-projectal.linkers.TagLinker): View Source
-_6class Skill(Entity, StaffLinker, TaskLinker, TaskTemplateLinker, TagLinker):
+class Stage(projectal.entity.Entity, projectal.linkers.ProjectLinker,
+projectal.linkers.TaskLinker, projectal.linkers.TagLinker): View Source
+_6class Stage(Entity, ProjectLinker, TaskLinker, TagLinker):
 _7    """
-_8    Implementation of the [Skill](https://projectal.com/docs/latest/#tag/
-Skill) API.
+_8    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/
+Stage) API.
 _9    """
-10    _path = 'skill'
-11    _name = 'skill'
-12    _links = [TagLinker]  # TODO: note?
-13    _links_reverse = [StaffLinker, TaskLinker, TaskTemplateLinker]
-Implementation of the Skill API.
+10    _path = 'stage'
+11    _name = 'stage'
+12    _links = [TagLinker]
+13    _links_reverse = [ProjectLinker, TaskLinker]
+Implementation of the Stage API.
 ** Inherited Members **
```

### Comparing `projectal-4.0.1/docs/projectal/entities/staff.html` & `projectal-4.0.2/docs/projectal/entities/staff.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/stage.html` & `projectal-4.0.2/docs/projectal/entities/tag.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <meta name="generator" content="pdoc 12.3.0"/>
-    <title>projectal.entities.stage API documentation</title>
+    <title>projectal.entities.tag API documentation</title>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
     <style>/*! custom.css */</style></head>
@@ -28,15 +28,15 @@
                    pattern=".+" required>
 
 
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
-                    <a class="class" href="#Stage">Stage</a>
+                    <a class="class" href="#Tag">Tag</a>
                             <ul class="memberlist">
                 </ul>
 
             </li>
     </ul>
 
 
@@ -47,116 +47,100 @@
                 src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20role%3D%22img%22%20aria-label%3D%22pdoc%20logo%22%20width%3D%22300%22%20height%3D%22150%22%20viewBox%3D%22-1%200%2060%2030%22%3E%3Ctitle%3Epdoc%3C/title%3E%3Cpath%20d%3D%22M29.621%2021.293c-.011-.273-.214-.475-.511-.481a.5.5%200%200%200-.489.503l-.044%201.393c-.097.551-.695%201.215-1.566%201.704-.577.428-1.306.486-2.193.182-1.426-.617-2.467-1.654-3.304-2.487l-.173-.172a3.43%203.43%200%200%200-.365-.306.49.49%200%200%200-.286-.196c-1.718-1.06-4.931-1.47-7.353.191l-.219.15c-1.707%201.187-3.413%202.131-4.328%201.03-.02-.027-.49-.685-.141-1.763.233-.721.546-2.408.772-4.076.042-.09.067-.187.046-.288.166-1.347.277-2.625.241-3.351%201.378-1.008%202.271-2.586%202.271-4.362%200-.976-.272-1.935-.788-2.774-.057-.094-.122-.18-.184-.268.033-.167.052-.339.052-.516%200-1.477-1.202-2.679-2.679-2.679-.791%200-1.496.352-1.987.9a6.3%206.3%200%200%200-1.001.029c-.492-.564-1.207-.929-2.012-.929-1.477%200-2.679%201.202-2.679%202.679A2.65%202.65%200%200%200%20.97%206.554c-.383.747-.595%201.572-.595%202.41%200%202.311%201.507%204.29%203.635%205.107-.037.699-.147%202.27-.423%203.294l-.137.461c-.622%202.042-2.515%208.257%201.727%2010.643%201.614.908%203.06%201.248%204.317%201.248%202.665%200%204.492-1.524%205.322-2.401%201.476-1.559%202.886-1.854%206.491.82%201.877%201.393%203.514%201.753%204.861%201.068%202.223-1.713%202.811-3.867%203.399-6.374.077-.846.056-1.469.054-1.537zm-4.835%204.313c-.054.305-.156.586-.242.629-.034-.007-.131-.022-.307-.157-.145-.111-.314-.478-.456-.908.221.121.432.25.675.355.115.039.219.051.33.081zm-2.251-1.238c-.05.33-.158.648-.252.694-.022.001-.125-.018-.307-.157-.217-.166-.488-.906-.639-1.573.358.344.754.693%201.198%201.036zm-3.887-2.337c-.006-.116-.018-.231-.041-.342.635.145%201.189.368%201.599.625.097.231.166.481.174.642-.03.049-.055.101-.067.158-.046.013-.128.026-.298.004-.278-.037-.901-.57-1.367-1.087zm-1.127-.497c.116.306.176.625.12.71-.019.014-.117.045-.345.016-.206-.027-.604-.332-.986-.695.41-.051.816-.056%201.211-.031zm-4.535%201.535c.209.22.379.47.358.598-.006.041-.088.138-.351.234-.144.055-.539-.063-.979-.259a11.66%2011.66%200%200%200%20.972-.573zm.983-.664c.359-.237.738-.418%201.126-.554.25.237.479.548.457.694-.006.042-.087.138-.351.235-.174.064-.694-.105-1.232-.375zm-3.381%201.794c-.022.145-.061.29-.149.401-.133.166-.358.248-.69.251h-.002c-.133%200-.306-.26-.45-.621.417.091.854.07%201.291-.031zm-2.066-8.077a4.78%204.78%200%200%201-.775-.584c.172-.115.505-.254.88-.378l-.105.962zm-.331%202.302a10.32%2010.32%200%200%201-.828-.502c.202-.143.576-.328.984-.49l-.156.992zm-.45%202.157l-.701-.403c.214-.115.536-.249.891-.376a11.57%2011.57%200%200%201-.19.779zm-.181%201.716c.064.398.194.702.298.893-.194-.051-.435-.162-.736-.398.061-.119.224-.3.438-.495zM8.87%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zm-.735-.389a1.15%201.15%200%200%200-.314.783%201.16%201.16%200%200%200%201.162%201.162c.457%200%20.842-.27%201.032-.653.026.117.042.238.042.362a1.68%201.68%200%200%201-1.679%201.679%201.68%201.68%200%200%201-1.679-1.679c0-.843.626-1.535%201.436-1.654zM5.059%205.406A1.68%201.68%200%200%201%203.38%207.085a1.68%201.68%200%200%201-1.679-1.679c0-.037.009-.072.011-.109.21.3.541.508.935.508a1.16%201.16%200%200%200%201.162-1.162%201.14%201.14%200%200%200-.474-.912c.015%200%20.03-.005.045-.005.926.001%201.679.754%201.679%201.68zM3.198%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zM1.375%208.964c0-.52.103-1.035.288-1.52.466.394%201.06.64%201.717.64%201.144%200%202.116-.725%202.499-1.738.383%201.012%201.355%201.738%202.499%201.738.867%200%201.631-.421%202.121-1.062.307.605.478%201.267.478%201.942%200%202.486-2.153%204.51-4.801%204.51s-4.801-2.023-4.801-4.51zm24.342%2019.349c-.985.498-2.267.168-3.813-.979-3.073-2.281-5.453-3.199-7.813-.705-1.315%201.391-4.163%203.365-8.423.97-3.174-1.786-2.239-6.266-1.261-9.479l.146-.492c.276-1.02.395-2.457.444-3.268a6.11%206.11%200%200%200%201.18.115%206.01%206.01%200%200%200%202.536-.562l-.006.175c-.802.215-1.848.612-2.021%201.25-.079.295.021.601.274.837.219.203.415.364.598.501-.667.304-1.243.698-1.311%201.179-.02.144-.022.507.393.787.213.144.395.26.564.365-1.285.521-1.361.96-1.381%201.126-.018.142-.011.496.427.746l.854.489c-.473.389-.971.914-.999%201.429-.018.278.095.532.316.713.675.556%201.231.721%201.653.721.059%200%20.104-.014.158-.02.207.707.641%201.64%201.513%201.64h.013c.8-.008%201.236-.345%201.462-.626.173-.216.268-.457.325-.692.424.195.93.374%201.372.374.151%200%20.294-.021.423-.068.732-.27.944-.704.993-1.021.009-.061.003-.119.002-.179.266.086.538.147.789.147.15%200%20.294-.021.423-.069.542-.2.797-.489.914-.754.237.147.478.258.704.288.106.014.205.021.296.021.356%200%20.595-.101.767-.229.438.435%201.094.992%201.656%201.067.106.014.205.021.296.021a1.56%201.56%200%200%200%20.323-.035c.17.575.453%201.289.866%201.605.358.273.665.362.914.362a.99.99%200%200%200%20.421-.093%201.03%201.03%200%200%200%20.245-.164c.168.428.39.846.68%201.068.358.273.665.362.913.362a.99.99%200%200%200%20.421-.093c.317-.148.512-.448.639-.762.251.157.495.257.726.257.127%200%20.25-.024.37-.071.427-.17.706-.617.841-1.314.022-.015.047-.022.068-.038.067-.051.133-.104.196-.159-.443%201.486-1.107%202.761-2.086%203.257zM8.66%209.925a.5.5%200%201%200-1%200c0%20.653-.818%201.205-1.787%201.205s-1.787-.552-1.787-1.205a.5.5%200%201%200-1%200c0%201.216%201.25%202.205%202.787%202.205s2.787-.989%202.787-2.205zm4.4%2015.965l-.208.097c-2.661%201.258-4.708%201.436-6.086.527-1.542-1.017-1.88-3.19-1.844-4.198a.4.4%200%200%200-.385-.414c-.242-.029-.406.164-.414.385-.046%201.249.367%203.686%202.202%204.896.708.467%201.547.7%202.51.7%201.248%200%202.706-.392%204.362-1.174l.185-.086a.4.4%200%200%200%20.205-.527c-.089-.204-.326-.291-.527-.206zM9.547%202.292c.093.077.205.114.317.114a.5.5%200%200%200%20.318-.886L8.817.397a.5.5%200%200%200-.703.068.5.5%200%200%200%20.069.703l1.364%201.124zm-7.661-.065c.086%200%20.173-.022.253-.068l1.523-.893a.5.5%200%200%200-.506-.863l-1.523.892a.5.5%200%200%200-.179.685c.094.158.261.247.432.247z%22%20transform%3D%22matrix%28-1%200%200%201%2058%200%29%22%20fill%3D%22%233bb300%22/%3E%3Cpath%20d%3D%22M.3%2021.86V10.18q0-.46.02-.68.04-.22.18-.5.28-.54%201.34-.54%201.06%200%201.42.28.38.26.44.78.76-1.04%202.38-1.04%201.64%200%203.1%201.54%201.46%201.54%201.46%203.58%200%202.04-1.46%203.58-1.44%201.54-3.08%201.54-1.64%200-2.38-.92v4.04q0%20.46-.04.68-.02.22-.18.5-.14.3-.5.42-.36.12-.98.12-.62%200-1-.12-.36-.12-.52-.4-.14-.28-.18-.5-.02-.22-.02-.68zm3.96-9.42q-.46.54-.46%201.18%200%20.64.46%201.18.48.52%201.2.52.74%200%201.24-.52.52-.52.52-1.18%200-.66-.48-1.18-.48-.54-1.26-.54-.76%200-1.22.54zm14.741-8.36q.16-.3.54-.42.38-.12%201-.12.64%200%201.02.12.38.12.52.42.16.3.18.54.04.22.04.68v11.94q0%20.46-.04.7-.02.22-.18.5-.3.54-1.7.54-1.38%200-1.54-.98-.84.96-2.34.96-1.8%200-3.28-1.56-1.48-1.58-1.48-3.66%200-2.1%201.48-3.68%201.5-1.58%203.28-1.58%201.48%200%202.3%201v-4.2q0-.46.02-.68.04-.24.18-.52zm-3.24%2010.86q.52.54%201.26.54.74%200%201.22-.54.5-.54.5-1.18%200-.66-.48-1.22-.46-.56-1.26-.56-.8%200-1.28.56-.48.54-.48%201.2%200%20.66.52%201.2zm7.833-1.2q0-2.4%201.68-3.96%201.68-1.56%203.84-1.56%202.16%200%203.82%201.56%201.66%201.54%201.66%203.94%200%201.66-.86%202.96-.86%201.28-2.1%201.9-1.22.6-2.54.6-1.32%200-2.56-.64-1.24-.66-2.1-1.92-.84-1.28-.84-2.88zm4.18%201.44q.64.48%201.3.48.66%200%201.32-.5.66-.5.66-1.48%200-.98-.62-1.46-.62-.48-1.34-.48-.72%200-1.34.5-.62.5-.62%201.48%200%20.96.64%201.46zm11.412-1.44q0%20.84.56%201.32.56.46%201.18.46.64%200%201.18-.36.56-.38.9-.38.6%200%201.46%201.06.46.58.46%201.04%200%20.76-1.1%201.42-1.14.8-2.8.8-1.86%200-3.58-1.34-.82-.64-1.34-1.7-.52-1.08-.52-2.36%200-1.3.52-2.34.52-1.06%201.34-1.7%201.66-1.32%203.54-1.32.76%200%201.48.22.72.2%201.06.4l.32.2q.36.24.56.38.52.4.52.92%200%20.5-.42%201.14-.72%201.1-1.38%201.1-.38%200-1.08-.44-.36-.34-1.04-.34-.66%200-1.24.48-.58.48-.58%201.34z%22%20fill%3D%22green%22/%3E%3C/svg%3E"/>
         </a>
 </div>
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
-<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.stage    </h1>
+<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.tag    </h1>
 
                 
-                        <input id="mod-stage-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                        <input id="mod-tag-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
-                        <label class="view-source-button" for="mod-stage-view-source"><span>View Source</span></label>
+                        <label class="view-source-button" for="mod-tag-view-source"><span>View Source</span></label>
 
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">from</span> <span class="nn">projectal.entity</span> <span class="kn">import</span> <span class="n">Entity</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="kn">from</span> <span class="nn">projectal.linkers</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a>
 </span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Stage</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/Stage) API.</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>
-</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">]</span>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="k">class</span> <span class="nc">Tag</span><span class="p">(</span><span class="n">Entity</span><span class="p">):</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag) API.</span>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[]</span>
 </span></pre></div>
 
 
             </section>
-                <section id="Stage">
-                            <input id="Stage-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="Tag">
+                            <input id="Tag-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
             
     <span class="def">class</span>
-    <span class="name">Stage</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>, <span class="base"><a href="../linkers.html#ProjectLinker">projectal.linkers.ProjectLinker</a></span>, <span class="base"><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></span>, <span class="base"><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></span>):
+    <span class="name">Tag</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>):
 
-                <label class="view-source-button" for="Stage-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="Tag-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#Stage"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Stage-6"><a href="#Stage-6"><span class="linenos"> 6</span></a><span class="k">class</span> <span class="nc">Stage</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">,</span> <span class="n">TagLinker</span><span class="p">):</span>
-</span><span id="Stage-7"><a href="#Stage-7"><span class="linenos"> 7</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Stage-8"><a href="#Stage-8"><span class="linenos"> 8</span></a><span class="sd">    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/Stage) API.</span>
-</span><span id="Stage-9"><a href="#Stage-9"><span class="linenos"> 9</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Stage-10"><a href="#Stage-10"><span class="linenos">10</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="Stage-11"><a href="#Stage-11"><span class="linenos">11</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="Stage-12"><a href="#Stage-12"><span class="linenos">12</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[</span><span class="n">TagLinker</span><span class="p">]</span>
-</span><span id="Stage-13"><a href="#Stage-13"><span class="linenos">13</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[</span><span class="n">ProjectLinker</span><span class="p">,</span> <span class="n">TaskLinker</span><span class="p">]</span>
+    <a class="headerlink" href="#Tag"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="Tag-5"><a href="#Tag-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Tag</span><span class="p">(</span><span class="n">Entity</span><span class="p">):</span>
+</span><span id="Tag-6"><a href="#Tag-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;</span>
+</span><span id="Tag-7"><a href="#Tag-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag) API.</span>
+</span><span id="Tag-8"><a href="#Tag-8"><span class="linenos"> 8</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="Tag-9"><a href="#Tag-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="Tag-10"><a href="#Tag-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="Tag-11"><a href="#Tag-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="Tag-12"><a href="#Tag-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[]</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Stage">Stage</a> API.</p>
+            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Tag">Tag</a> API.</p>
 </div>
 
 
                             <div class="inherited">
                                 <h5>Inherited Members</h5>
                                 <dl>
                                     <div><dt><a href="../entity.html#Entity">projectal.entity.Entity</a></dt>
-                                <dd id="Stage.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
-                <dd id="Stage.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
-                <dd id="Stage.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
-                <dd id="Stage.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
-                <dd id="Stage.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
-                <dd id="Stage.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
-                <dd id="Stage.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
-                <dd id="Stage.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
-                <dd id="Stage.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
-                <dd id="Stage.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
-                <dd id="Stage.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
-                <dd id="Stage.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
-                <dd id="Stage.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
-                <dd id="Stage.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
-                <dd id="Stage.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
-                <dd id="Stage.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
-                <dd id="Stage.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
-                <dd id="Stage.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
-                <dd id="Stage.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
-                <dd id="Stage.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
-                <dd id="Stage.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
-                <dd id="Stage.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#ProjectLinker">projectal.linkers.ProjectLinker</a></dt>
-                                <dd id="Stage.link_project" class="function"><a href="../linkers.html#ProjectLinker.link_project">link_project</a></dd>
-                <dd id="Stage.unlink_project" class="function"><a href="../linkers.html#ProjectLinker.unlink_project">unlink_project</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#TaskLinker">projectal.linkers.TaskLinker</a></dt>
-                                <dd id="Stage.link_task" class="function"><a href="../linkers.html#TaskLinker.link_task">link_task</a></dd>
-                <dd id="Stage.unlink_task" class="function"><a href="../linkers.html#TaskLinker.unlink_task">unlink_task</a></dd>
-
-            </div>
-            <div><dt><a href="../linkers.html#TagLinker">projectal.linkers.TagLinker</a></dt>
-                                <dd id="Stage.link_tag" class="function"><a href="../linkers.html#TagLinker.link_tag">link_tag</a></dd>
-                <dd id="Stage.unlink_tag" class="function"><a href="../linkers.html#TagLinker.unlink_tag">unlink_tag</a></dd>
+                                <dd id="Tag.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
+                <dd id="Tag.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
+                <dd id="Tag.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
+                <dd id="Tag.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
+                <dd id="Tag.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
+                <dd id="Tag.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
+                <dd id="Tag.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
+                <dd id="Tag.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
+                <dd id="Tag.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
+                <dd id="Tag.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
+                <dd id="Tag.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
+                <dd id="Tag.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
+                <dd id="Tag.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
+                <dd id="Tag.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
+                <dd id="Tag.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
+                <dd id="Tag.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
+                <dd id="Tag.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
+                <dd id="Tag.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
+                <dd id="Tag.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
+                <dd id="Tag.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
+                <dd id="Tag.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
+                <dd id="Tag.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
 
             </div>
             <div><dt>builtins.dict</dt>
-                                <dd id="Stage.setdefault" class="function">setdefault</dd>
-                <dd id="Stage.pop" class="function">pop</dd>
-                <dd id="Stage.popitem" class="function">popitem</dd>
-                <dd id="Stage.keys" class="function">keys</dd>
-                <dd id="Stage.items" class="function">items</dd>
-                <dd id="Stage.values" class="function">values</dd>
-                <dd id="Stage.fromkeys" class="function">fromkeys</dd>
-                <dd id="Stage.clear" class="function">clear</dd>
-                <dd id="Stage.copy" class="function">copy</dd>
+                                <dd id="Tag.setdefault" class="function">setdefault</dd>
+                <dd id="Tag.pop" class="function">pop</dd>
+                <dd id="Tag.popitem" class="function">popitem</dd>
+                <dd id="Tag.keys" class="function">keys</dd>
+                <dd id="Tag.items" class="function">items</dd>
+                <dd id="Tag.values" class="function">values</dd>
+                <dd id="Tag.fromkeys" class="function">fromkeys</dd>
+                <dd id="Tag.clear" class="function">clear</dd>
+                <dd id="Tag.copy" class="function">copy</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
     </main>
 <script>
```

#### html2text {}

```diff
@@ -1,38 +1,36 @@
 
 
   ⁰
 ____ projectal.entities [project logo] [Unknown INPUT type]
 ***** API Documentation *****
-    * Stage
+    * Tag
 built_with_pdoc[pdoc_logo]
 
-****** projectal.entities.stage ******
+****** projectal.entities.tag ******
 ⁰ View Source
 _1from projectal.entity import Entity
-_2from projectal.linkers import *
+_2
 _3
-_4
-_5class Stage(Entity, ProjectLinker, TaskLinker, TagLinker):
+_4class Tag(Entity):
+_5    """
+_6    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag)
+API.
+_7    """
+_8    _path = 'tag'
+_9    _name = 'tag'
+10    _links = []
+11    _links_reverse = []
+  ⁰
+class Tag(projectal.entity.Entity): View Source
+_5class Tag(Entity):
 _6    """
-_7    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/
-Stage) API.
+_7    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag)
+API.
 _8    """
-_9    _path = 'stage'
-10    _name = 'stage'
-11    _links = [TagLinker]
-12    _links_reverse = [ProjectLinker, TaskLinker]
-  ⁰
-class Stage(projectal.entity.Entity, projectal.linkers.ProjectLinker,
-projectal.linkers.TaskLinker, projectal.linkers.TagLinker): View Source
-_6class Stage(Entity, ProjectLinker, TaskLinker, TagLinker):
-_7    """
-_8    Implementation of the [Stage](https://projectal.com/docs/latest/#tag/
-Stage) API.
-_9    """
-10    _path = 'stage'
-11    _name = 'stage'
-12    _links = [TagLinker]
-13    _links_reverse = [ProjectLinker, TaskLinker]
-Implementation of the Stage API.
+_9    _path = 'tag'
+10    _name = 'tag'
+11    _links = []
+12    _links_reverse = []
+Implementation of the Tag API.
 ** Inherited Members **
```

### Comparing `projectal-4.0.1/docs/projectal/entities/tag.html` & `projectal-4.0.2/docs/projectal/entities.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,151 +1,124 @@
 <!doctype html>
 <html lang="en">
 <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <meta name="generator" content="pdoc 12.3.0"/>
-    <title>projectal.entities.tag API documentation</title>
+    <title>projectal.entities API documentation</title>
 
     <style>/*! * Bootstrap Reboot v5.0.0 (https://getbootstrap.com/) * Copyright 2011-2021 The Bootstrap Authors * Copyright 2011-2021 Twitter, Inc. * Licensed under MIT (https://github.com/twbs/bootstrap/blob/main/LICENSE) * Forked from Normalize.css, licensed MIT (https://github.com/necolas/normalize.css/blob/master/LICENSE.md) */*,::after,::before{box-sizing:border-box}@media (prefers-reduced-motion:no-preference){:root{scroll-behavior:smooth}}body{margin:0;font-family:system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial,"Noto Sans","Liberation Sans",sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol","Noto Color Emoji";font-size:1rem;font-weight:400;line-height:1.5;color:#212529;background-color:#fff;-webkit-text-size-adjust:100%;-webkit-tap-highlight-color:transparent}hr{margin:1rem 0;color:inherit;background-color:currentColor;border:0;opacity:.25}hr:not([size]){height:1px}h1,h2,h3,h4,h5,h6{margin-top:0;margin-bottom:.5rem;font-weight:500;line-height:1.2}h1{font-size:calc(1.375rem + 1.5vw)}@media (min-width:1200px){h1{font-size:2.5rem}}h2{font-size:calc(1.325rem + .9vw)}@media (min-width:1200px){h2{font-size:2rem}}h3{font-size:calc(1.3rem + .6vw)}@media (min-width:1200px){h3{font-size:1.75rem}}h4{font-size:calc(1.275rem + .3vw)}@media (min-width:1200px){h4{font-size:1.5rem}}h5{font-size:1.25rem}h6{font-size:1rem}p{margin-top:0;margin-bottom:1rem}abbr[data-bs-original-title],abbr[title]{-webkit-text-decoration:underline dotted;text-decoration:underline dotted;cursor:help;-webkit-text-decoration-skip-ink:none;text-decoration-skip-ink:none}address{margin-bottom:1rem;font-style:normal;line-height:inherit}ol,ul{padding-left:2rem}dl,ol,ul{margin-top:0;margin-bottom:1rem}ol ol,ol ul,ul ol,ul ul{margin-bottom:0}dt{font-weight:700}dd{margin-bottom:.5rem;margin-left:0}blockquote{margin:0 0 1rem}b,strong{font-weight:bolder}small{font-size:.875em}mark{padding:.2em;background-color:#fcf8e3}sub,sup{position:relative;font-size:.75em;line-height:0;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}a{color:#0d6efd;text-decoration:underline}a:hover{color:#0a58ca}a:not([href]):not([class]),a:not([href]):not([class]):hover{color:inherit;text-decoration:none}code,kbd,pre,samp{font-family:SFMono-Regular,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:1em;direction:ltr;unicode-bidi:bidi-override}pre{display:block;margin-top:0;margin-bottom:1rem;overflow:auto;font-size:.875em}pre code{font-size:inherit;color:inherit;word-break:normal}code{font-size:.875em;color:#d63384;word-wrap:break-word}a>code{color:inherit}kbd{padding:.2rem .4rem;font-size:.875em;color:#fff;background-color:#212529;border-radius:.2rem}kbd kbd{padding:0;font-size:1em;font-weight:700}figure{margin:0 0 1rem}img,svg{vertical-align:middle}table{caption-side:bottom;border-collapse:collapse}caption{padding-top:.5rem;padding-bottom:.5rem;color:#6c757d;text-align:left}th{text-align:inherit;text-align:-webkit-match-parent}tbody,td,tfoot,th,thead,tr{border-color:inherit;border-style:solid;border-width:0}label{display:inline-block}button{border-radius:0}button:focus:not(:focus-visible){outline:0}button,input,optgroup,select,textarea{margin:0;font-family:inherit;font-size:inherit;line-height:inherit}button,select{text-transform:none}[role=button]{cursor:pointer}select{word-wrap:normal}select:disabled{opacity:1}[list]::-webkit-calendar-picker-indicator{display:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button}[type=button]:not(:disabled),[type=reset]:not(:disabled),[type=submit]:not(:disabled),button:not(:disabled){cursor:pointer}::-moz-focus-inner{padding:0;border-style:none}textarea{resize:vertical}fieldset{min-width:0;padding:0;margin:0;border:0}legend{float:left;width:100%;padding:0;margin-bottom:.5rem;font-size:calc(1.275rem + .3vw);line-height:inherit}@media (min-width:1200px){legend{font-size:1.5rem}}legend+*{clear:left}::-webkit-datetime-edit-day-field,::-webkit-datetime-edit-fields-wrapper,::-webkit-datetime-edit-hour-field,::-webkit-datetime-edit-minute,::-webkit-datetime-edit-month-field,::-webkit-datetime-edit-text,::-webkit-datetime-edit-year-field{padding:0}::-webkit-inner-spin-button{height:auto}[type=search]{outline-offset:-2px;-webkit-appearance:textfield}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-color-swatch-wrapper{padding:0}::file-selector-button{font:inherit}::-webkit-file-upload-button{font:inherit;-webkit-appearance:button}output{display:inline-block}iframe{border:0}summary{display:list-item;cursor:pointer}progress{vertical-align:baseline}[hidden]{display:none!important}</style>
     <style>/*! syntax-highlighting.css */pre{line-height:125%;}span.linenos{color:inherit; background-color:transparent; padding-left:5px; padding-right:20px;}.pdoc-code .hll{background-color:#ffffcc}.pdoc-code{background:#f8f8f8;}.pdoc-code .c{color:#3D7B7B; font-style:italic}.pdoc-code .err{border:1px solid #FF0000}.pdoc-code .k{color:#008000; font-weight:bold}.pdoc-code .o{color:#666666}.pdoc-code .ch{color:#3D7B7B; font-style:italic}.pdoc-code .cm{color:#3D7B7B; font-style:italic}.pdoc-code .cp{color:#9C6500}.pdoc-code .cpf{color:#3D7B7B; font-style:italic}.pdoc-code .c1{color:#3D7B7B; font-style:italic}.pdoc-code .cs{color:#3D7B7B; font-style:italic}.pdoc-code .gd{color:#A00000}.pdoc-code .ge{font-style:italic}.pdoc-code .gr{color:#E40000}.pdoc-code .gh{color:#000080; font-weight:bold}.pdoc-code .gi{color:#008400}.pdoc-code .go{color:#717171}.pdoc-code .gp{color:#000080; font-weight:bold}.pdoc-code .gs{font-weight:bold}.pdoc-code .gu{color:#800080; font-weight:bold}.pdoc-code .gt{color:#0044DD}.pdoc-code .kc{color:#008000; font-weight:bold}.pdoc-code .kd{color:#008000; font-weight:bold}.pdoc-code .kn{color:#008000; font-weight:bold}.pdoc-code .kp{color:#008000}.pdoc-code .kr{color:#008000; font-weight:bold}.pdoc-code .kt{color:#B00040}.pdoc-code .m{color:#666666}.pdoc-code .s{color:#BA2121}.pdoc-code .na{color:#687822}.pdoc-code .nb{color:#008000}.pdoc-code .nc{color:#0000FF; font-weight:bold}.pdoc-code .no{color:#880000}.pdoc-code .nd{color:#AA22FF}.pdoc-code .ni{color:#717171; font-weight:bold}.pdoc-code .ne{color:#CB3F38; font-weight:bold}.pdoc-code .nf{color:#0000FF}.pdoc-code .nl{color:#767600}.pdoc-code .nn{color:#0000FF; font-weight:bold}.pdoc-code .nt{color:#008000; font-weight:bold}.pdoc-code .nv{color:#19177C}.pdoc-code .ow{color:#AA22FF; font-weight:bold}.pdoc-code .w{color:#bbbbbb}.pdoc-code .mb{color:#666666}.pdoc-code .mf{color:#666666}.pdoc-code .mh{color:#666666}.pdoc-code .mi{color:#666666}.pdoc-code .mo{color:#666666}.pdoc-code .sa{color:#BA2121}.pdoc-code .sb{color:#BA2121}.pdoc-code .sc{color:#BA2121}.pdoc-code .dl{color:#BA2121}.pdoc-code .sd{color:#BA2121; font-style:italic}.pdoc-code .s2{color:#BA2121}.pdoc-code .se{color:#AA5D1F; font-weight:bold}.pdoc-code .sh{color:#BA2121}.pdoc-code .si{color:#A45A77; font-weight:bold}.pdoc-code .sx{color:#008000}.pdoc-code .sr{color:#A45A77}.pdoc-code .s1{color:#BA2121}.pdoc-code .ss{color:#19177C}.pdoc-code .bp{color:#008000}.pdoc-code .fm{color:#0000FF}.pdoc-code .vc{color:#19177C}.pdoc-code .vg{color:#19177C}.pdoc-code .vi{color:#19177C}.pdoc-code .vm{color:#19177C}.pdoc-code .il{color:#666666}</style>
     <style>/*! theme.css */:root{--pdoc-background:#fff;}.pdoc{--text:#212529;--muted:#6c757d;--link:#3660a5;--link-hover:#1659c5;--code:#f8f8f8;--active:#fff598;--accent:#eee;--accent2:#c1c1c1;--nav-hover:rgba(255, 255, 255, 0.5);--name:#0066BB;--def:#008800;--annotation:#007020;}</style>
     <style>/*! layout.css */html, body{width:100%;height:100%;}html, main{scroll-behavior:smooth;}body{background-color:var(--pdoc-background);}@media (max-width:769px){#navtoggle{cursor:pointer;position:absolute;width:50px;height:40px;top:1rem;right:1rem;border-color:var(--text);color:var(--text);display:flex;opacity:0.8;}#navtoggle:hover{opacity:1;}#togglestate + div{display:none;}#togglestate:checked + div{display:inherit;}main, header{padding:2rem 3vw;}header + main{margin-top:-3rem;}.git-button{display:none !important;}nav input[type="search"]{max-width:77%;}nav input[type="search"]:first-child{margin-top:-6px;}nav input[type="search"]:valid ~ *{display:none !important;}}@media (min-width:770px){:root{--sidebar-width:clamp(12.5rem, 28vw, 22rem);}nav{position:fixed;overflow:auto;height:100vh;width:var(--sidebar-width);}main, header{padding:3rem 2rem 3rem calc(var(--sidebar-width) + 3rem);width:calc(54rem + var(--sidebar-width));max-width:100%;}header + main{margin-top:-4rem;}#navtoggle{display:none;}}#togglestate{position:absolute;height:0;opacity:0;}nav.pdoc{--pad:clamp(0.5rem, 2vw, 1.75rem);--indent:1.5rem;background-color:var(--accent);border-right:1px solid var(--accent2);box-shadow:0 0 20px rgba(50, 50, 50, .2) inset;padding:0 0 0 var(--pad);overflow-wrap:anywhere;scrollbar-width:thin; scrollbar-color:var(--accent2) transparent }nav.pdoc::-webkit-scrollbar{width:.4rem; }nav.pdoc::-webkit-scrollbar-thumb{background-color:var(--accent2); }nav.pdoc > div{padding:var(--pad) 0;}nav.pdoc .module-list-button{display:inline-flex;align-items:center;color:var(--text);border-color:var(--muted);margin-bottom:1rem;}nav.pdoc .module-list-button:hover{border-color:var(--text);}nav.pdoc input[type=search]{display:block;outline-offset:0;width:calc(100% - var(--pad));}nav.pdoc .logo{max-width:calc(100% - var(--pad));max-height:35vh;display:block;margin:0 auto 1rem;transform:translate(calc(-.5 * var(--pad)), 0);}nav.pdoc ul{list-style:none;padding-left:0;}nav.pdoc > div > ul{margin-left:calc(0px - var(--pad));}nav.pdoc li a{padding:.2rem 0 .2rem calc(var(--pad) + var(--indent));}nav.pdoc > div > ul > li > a{padding-left:var(--pad);}nav.pdoc li{transition:all 100ms;}nav.pdoc li:hover{background-color:var(--nav-hover);}nav.pdoc a, nav.pdoc a:hover{color:var(--text);}nav.pdoc a{display:block;}nav.pdoc > h2:first-of-type{margin-top:1.5rem;}nav.pdoc .class:before{content:"class ";color:var(--muted);}nav.pdoc .function:after{content:"()";color:var(--muted);}nav.pdoc footer:before{content:"";display:block;width:calc(100% - var(--pad));border-top:solid var(--accent2) 1px;margin-top:1.5rem;padding-top:.5rem;}nav.pdoc footer{font-size:small;}</style>
     <style>/*! content.css */.pdoc{color:var(--text);box-sizing:border-box;line-height:1.5;background:none;}.pdoc .pdoc-button{display:inline-block;border:solid black 1px;border-radius:2px;font-size:.75rem;padding:calc(0.5em - 1px) 1em;transition:100ms all;}.pdoc .pdoc-alert{padding:1rem 1rem 1rem calc(1.5rem + 24px);border:1px solid transparent;border-radius:.25rem;background-repeat:no-repeat;background-position:1rem center;margin-bottom:1rem;}.pdoc .pdoc-alert > *:last-child{margin-bottom:0;}.pdoc .pdoc-alert-note {color:#084298;background-color:#cfe2ff;border-color:#b6d4fe;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23084298%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8%2016A8%208%200%201%200%208%200a8%208%200%200%200%200%2016zm.93-9.412-1%204.705c-.07.34.029.533.304.533.194%200%20.487-.07.686-.246l-.088.416c-.287.346-.92.598-1.465.598-.703%200-1.002-.422-.808-1.319l.738-3.468c.064-.293.006-.399-.287-.47l-.451-.081.082-.381%202.29-.287zM8%205.5a1%201%200%201%201%200-2%201%201%200%200%201%200%202z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-warning{color:#664d03;background-color:#fff3cd;border-color:#ffecb5;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23664d03%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M8.982%201.566a1.13%201.13%200%200%200-1.96%200L.165%2013.233c-.457.778.091%201.767.98%201.767h13.713c.889%200%201.438-.99.98-1.767L8.982%201.566zM8%205c.535%200%20.954.462.9.995l-.35%203.507a.552.552%200%200%201-1.1%200L7.1%205.995A.905.905%200%200%201%208%205zm.002%206a1%201%200%201%201%200%202%201%201%200%200%201%200-2z%22/%3E%3C/svg%3E");}.pdoc .pdoc-alert-danger{color:#842029;background-color:#f8d7da;border-color:#f5c2c7;background-image:url("data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20width%3D%2224%22%20height%3D%2224%22%20fill%3D%22%23842029%22%20viewBox%3D%220%200%2016%2016%22%3E%3Cpath%20d%3D%22M5.52.359A.5.5%200%200%201%206%200h4a.5.5%200%200%201%20.474.658L8.694%206H12.5a.5.5%200%200%201%20.395.807l-7%209a.5.5%200%200%201-.873-.454L6.823%209.5H3.5a.5.5%200%200%201-.48-.641l2.5-8.5z%22/%3E%3C/svg%3E");}.pdoc .visually-hidden{position:absolute !important;width:1px !important;height:1px !important;padding:0 !important;margin:-1px !important;overflow:hidden !important;clip:rect(0, 0, 0, 0) !important;white-space:nowrap !important;border:0 !important;}.pdoc h1, .pdoc h2, .pdoc h3{font-weight:300;margin:.3em 0;padding:.2em 0;}.pdoc > section:not(.module-info) h1{font-size:1.5rem;font-weight:500;}.pdoc > section:not(.module-info) h2{font-size:1.4rem;font-weight:500;}.pdoc > section:not(.module-info) h3{font-size:1.3rem;font-weight:500;}.pdoc > section:not(.module-info) h4{font-size:1.2rem;}.pdoc > section:not(.module-info) h5{font-size:1.1rem;}.pdoc a{text-decoration:none;color:var(--link);}.pdoc a:hover{color:var(--link-hover);}.pdoc blockquote{margin-left:2rem;}.pdoc pre{border-top:1px solid var(--accent2);border-bottom:1px solid var(--accent2);margin-top:0;margin-bottom:1em;padding:.5rem 0 .5rem .5rem;overflow-x:auto;background-color:var(--code);}.pdoc code{color:var(--text);padding:.2em .4em;margin:0;font-size:85%;background-color:var(--code);border-radius:6px;}.pdoc a > code{color:inherit;}.pdoc pre > code{display:inline-block;font-size:inherit;background:none;border:none;padding:0;}.pdoc > section:not(.module-info){margin-bottom:1.5rem;}.pdoc .modulename{margin-top:0;font-weight:bold;}.pdoc .modulename a{color:var(--link);transition:100ms all;}.pdoc .git-button{float:right;border:solid var(--link) 1px;}.pdoc .git-button:hover{background-color:var(--link);color:var(--pdoc-background);}.view-source-toggle-state,.view-source-toggle-state ~ .pdoc-code{display:none;}.view-source-toggle-state:checked ~ .pdoc-code{display:block;}.view-source-button{display:inline-block;float:right;font-size:.75rem;line-height:1.5rem;color:var(--muted);padding:0 .4rem 0 1.3rem;cursor:pointer;text-indent:-2px;}.view-source-button > span{visibility:hidden;}.module-info .view-source-button{float:none;display:flex;justify-content:flex-end;margin:-1.2rem .4rem -.2rem 0;}.view-source-button::before{position:absolute;content:"View Source";display:list-item;list-style-type:disclosure-closed;}.view-source-toggle-state:checked ~ .attr .view-source-button::before,.view-source-toggle-state:checked ~ .view-source-button::before{list-style-type:disclosure-open;}.pdoc .docstring{margin-bottom:1.5rem;}.pdoc section:not(.module-info) .docstring{margin-left:clamp(0rem, 5vw - 2rem, 1rem);}.pdoc .docstring .pdoc-code{margin-left:1em;margin-right:1em;}.pdoc h1:target,.pdoc h2:target,.pdoc h3:target,.pdoc h4:target,.pdoc h5:target,.pdoc h6:target,.pdoc .pdoc-code > pre > span:target{background-color:var(--active);box-shadow:-1rem 0 0 0 var(--active);}.pdoc .pdoc-code > pre > span:target{display:block;}.pdoc div:target > .attr,.pdoc section:target > .attr,.pdoc dd:target > a{background-color:var(--active);}.pdoc *{scroll-margin:2rem;}.pdoc .pdoc-code .linenos{user-select:none;}.pdoc .attr:hover{filter:contrast(0.95);}.pdoc section, .pdoc .classattr{position:relative;}.pdoc .headerlink{--width:clamp(1rem, 3vw, 2rem);position:absolute;top:0;left:calc(0rem - var(--width));transition:all 100ms ease-in-out;opacity:0;}.pdoc .headerlink::before{content:"#";display:block;text-align:center;width:var(--width);height:2.3rem;line-height:2.3rem;font-size:1.5rem;}.pdoc .attr:hover ~ .headerlink,.pdoc *:target > .headerlink,.pdoc .headerlink:hover{opacity:1;}.pdoc .attr{display:block;margin:.5rem 0 .5rem;padding:.4rem .4rem .4rem 1rem;background-color:var(--accent);overflow-x:auto;}.pdoc .classattr{margin-left:2rem;}.pdoc .name{color:var(--name);font-weight:bold;}.pdoc .def{color:var(--def);font-weight:bold;}.pdoc .signature{background-color:transparent;}.pdoc .param, .pdoc .return-annotation{white-space:pre;}.pdoc .signature.multiline .param{display:block;}.pdoc .signature.condensed .param{display:inline-block;}.pdoc .annotation{color:var(--annotation);}.pdoc .inherited{margin-left:2rem;}.pdoc .inherited dt{font-weight:700;}.pdoc .inherited dt, .pdoc .inherited dd{display:inline;margin-left:0;margin-bottom:.5rem;}.pdoc .inherited dd:not(:last-child):after{content:", ";}.pdoc .inherited .class:before{content:"class ";}.pdoc .inherited .function a:after{content:"()";}.pdoc .search-result .docstring{overflow:auto;max-height:25vh;}.pdoc .search-result.focused > .attr{background-color:var(--active);}.pdoc .attribution{margin-top:2rem;display:block;opacity:0.5;transition:all 200ms;filter:grayscale(100%);}.pdoc .attribution:hover{opacity:1;filter:grayscale(0%);}.pdoc .attribution img{margin-left:5px;height:35px;vertical-align:middle;width:70px;transition:all 200ms;}.pdoc table{display:block;width:max-content;max-width:100%;overflow:auto;margin-bottom:1rem;}.pdoc table th{font-weight:600;}.pdoc table th, .pdoc table td{padding:6px 13px;border:1px solid var(--accent2);}</style>
     <style>/*! custom.css */</style></head>
 <body>
     <nav class="pdoc">
         <label id="navtoggle" for="togglestate" class="pdoc-button"><svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 30 30'><path stroke-linecap='round' stroke="currentColor" stroke-miterlimit='10' stroke-width='2' d='M4 7h22M4 15h22M4 23h22'/></svg></label>
         <input id="togglestate" type="checkbox" aria-hidden="true" tabindex="-1">
-        <div>            <a class="pdoc-button module-list-button" href="../entities.html">
+        <div>            <a class="pdoc-button module-list-button" href="../projectal.html">
 <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-left" viewBox="0 0 16 16">
   <path fill-rule="evenodd" d="M10 3.5a.5.5 0 0 0-.5-.5h-8a.5.5 0 0 0-.5.5v9a.5.5 0 0 0 .5.5h8a.5.5 0 0 0 .5-.5v-2a.5.5 0 0 1 1 0v2A1.5 1.5 0 0 1 9.5 14h-8A1.5 1.5 0 0 1 0 12.5v-9A1.5 1.5 0 0 1 1.5 2h8A1.5 1.5 0 0 1 11 3.5v2a.5.5 0 0 1-1 0v-2z"/>
   <path fill-rule="evenodd" d="M4.146 8.354a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5H14.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3z"/>
-</svg>                &nbsp;projectal.entities</a>
+</svg>                &nbsp;projectal</a>
 
             <img src="https://projectal.com/img/logos/projectal-logo-icon-text-blue.svg" class="logo" alt="project logo"/>
 
             <input type="search" placeholder="Search..." role="searchbox" aria-label="search"
                    pattern=".+" required>
 
 
-
-        <h2>API Documentation</h2>
-            <ul class="memberlist">
-            <li>
-                    <a class="class" href="#Tag">Tag</a>
-                            <ul class="memberlist">
-                </ul>
-
-            </li>
-    </ul>
+        <h2>Submodules</h2>
+        <ul>
+                <li><a href="entities/access_policy.html">access_policy</a></li>
+                <li><a href="entities/activity.html">activity</a></li>
+                <li><a href="entities/booking.html">booking</a></li>
+                <li><a href="entities/calendar.html">calendar</a></li>
+                <li><a href="entities/company.html">company</a></li>
+                <li><a href="entities/contact.html">contact</a></li>
+                <li><a href="entities/customer.html">customer</a></li>
+                <li><a href="entities/department.html">department</a></li>
+                <li><a href="entities/file.html">file</a></li>
+                <li><a href="entities/folder.html">folder</a></li>
+                <li><a href="entities/location.html">location</a></li>
+                <li><a href="entities/note.html">note</a></li>
+                <li><a href="entities/permission.html">permission</a></li>
+                <li><a href="entities/project.html">project</a></li>
+                <li><a href="entities/project_template.html">project_template</a></li>
+                <li><a href="entities/rebate.html">rebate</a></li>
+                <li><a href="entities/resource.html">resource</a></li>
+                <li><a href="entities/skill.html">skill</a></li>
+                <li><a href="entities/staff.html">staff</a></li>
+                <li><a href="entities/stage.html">stage</a></li>
+                <li><a href="entities/tag.html">tag</a></li>
+                <li><a href="entities/task.html">task</a></li>
+                <li><a href="entities/task_template.html">task_template</a></li>
+                <li><a href="entities/user.html">user</a></li>
+                <li><a href="entities/webhook.html">webhook</a></li>
+        </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
                 src="data:image/svg+xml,%3Csvg%20xmlns%3D%22http%3A//www.w3.org/2000/svg%22%20role%3D%22img%22%20aria-label%3D%22pdoc%20logo%22%20width%3D%22300%22%20height%3D%22150%22%20viewBox%3D%22-1%200%2060%2030%22%3E%3Ctitle%3Epdoc%3C/title%3E%3Cpath%20d%3D%22M29.621%2021.293c-.011-.273-.214-.475-.511-.481a.5.5%200%200%200-.489.503l-.044%201.393c-.097.551-.695%201.215-1.566%201.704-.577.428-1.306.486-2.193.182-1.426-.617-2.467-1.654-3.304-2.487l-.173-.172a3.43%203.43%200%200%200-.365-.306.49.49%200%200%200-.286-.196c-1.718-1.06-4.931-1.47-7.353.191l-.219.15c-1.707%201.187-3.413%202.131-4.328%201.03-.02-.027-.49-.685-.141-1.763.233-.721.546-2.408.772-4.076.042-.09.067-.187.046-.288.166-1.347.277-2.625.241-3.351%201.378-1.008%202.271-2.586%202.271-4.362%200-.976-.272-1.935-.788-2.774-.057-.094-.122-.18-.184-.268.033-.167.052-.339.052-.516%200-1.477-1.202-2.679-2.679-2.679-.791%200-1.496.352-1.987.9a6.3%206.3%200%200%200-1.001.029c-.492-.564-1.207-.929-2.012-.929-1.477%200-2.679%201.202-2.679%202.679A2.65%202.65%200%200%200%20.97%206.554c-.383.747-.595%201.572-.595%202.41%200%202.311%201.507%204.29%203.635%205.107-.037.699-.147%202.27-.423%203.294l-.137.461c-.622%202.042-2.515%208.257%201.727%2010.643%201.614.908%203.06%201.248%204.317%201.248%202.665%200%204.492-1.524%205.322-2.401%201.476-1.559%202.886-1.854%206.491.82%201.877%201.393%203.514%201.753%204.861%201.068%202.223-1.713%202.811-3.867%203.399-6.374.077-.846.056-1.469.054-1.537zm-4.835%204.313c-.054.305-.156.586-.242.629-.034-.007-.131-.022-.307-.157-.145-.111-.314-.478-.456-.908.221.121.432.25.675.355.115.039.219.051.33.081zm-2.251-1.238c-.05.33-.158.648-.252.694-.022.001-.125-.018-.307-.157-.217-.166-.488-.906-.639-1.573.358.344.754.693%201.198%201.036zm-3.887-2.337c-.006-.116-.018-.231-.041-.342.635.145%201.189.368%201.599.625.097.231.166.481.174.642-.03.049-.055.101-.067.158-.046.013-.128.026-.298.004-.278-.037-.901-.57-1.367-1.087zm-1.127-.497c.116.306.176.625.12.71-.019.014-.117.045-.345.016-.206-.027-.604-.332-.986-.695.41-.051.816-.056%201.211-.031zm-4.535%201.535c.209.22.379.47.358.598-.006.041-.088.138-.351.234-.144.055-.539-.063-.979-.259a11.66%2011.66%200%200%200%20.972-.573zm.983-.664c.359-.237.738-.418%201.126-.554.25.237.479.548.457.694-.006.042-.087.138-.351.235-.174.064-.694-.105-1.232-.375zm-3.381%201.794c-.022.145-.061.29-.149.401-.133.166-.358.248-.69.251h-.002c-.133%200-.306-.26-.45-.621.417.091.854.07%201.291-.031zm-2.066-8.077a4.78%204.78%200%200%201-.775-.584c.172-.115.505-.254.88-.378l-.105.962zm-.331%202.302a10.32%2010.32%200%200%201-.828-.502c.202-.143.576-.328.984-.49l-.156.992zm-.45%202.157l-.701-.403c.214-.115.536-.249.891-.376a11.57%2011.57%200%200%201-.19.779zm-.181%201.716c.064.398.194.702.298.893-.194-.051-.435-.162-.736-.398.061-.119.224-.3.438-.495zM8.87%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zm-.735-.389a1.15%201.15%200%200%200-.314.783%201.16%201.16%200%200%200%201.162%201.162c.457%200%20.842-.27%201.032-.653.026.117.042.238.042.362a1.68%201.68%200%200%201-1.679%201.679%201.68%201.68%200%200%201-1.679-1.679c0-.843.626-1.535%201.436-1.654zM5.059%205.406A1.68%201.68%200%200%201%203.38%207.085a1.68%201.68%200%200%201-1.679-1.679c0-.037.009-.072.011-.109.21.3.541.508.935.508a1.16%201.16%200%200%200%201.162-1.162%201.14%201.14%200%200%200-.474-.912c.015%200%20.03-.005.045-.005.926.001%201.679.754%201.679%201.68zM3.198%204.141c0%20.152-.123.276-.276.276s-.275-.124-.275-.276.123-.276.276-.276.275.124.275.276zM1.375%208.964c0-.52.103-1.035.288-1.52.466.394%201.06.64%201.717.64%201.144%200%202.116-.725%202.499-1.738.383%201.012%201.355%201.738%202.499%201.738.867%200%201.631-.421%202.121-1.062.307.605.478%201.267.478%201.942%200%202.486-2.153%204.51-4.801%204.51s-4.801-2.023-4.801-4.51zm24.342%2019.349c-.985.498-2.267.168-3.813-.979-3.073-2.281-5.453-3.199-7.813-.705-1.315%201.391-4.163%203.365-8.423.97-3.174-1.786-2.239-6.266-1.261-9.479l.146-.492c.276-1.02.395-2.457.444-3.268a6.11%206.11%200%200%200%201.18.115%206.01%206.01%200%200%200%202.536-.562l-.006.175c-.802.215-1.848.612-2.021%201.25-.079.295.021.601.274.837.219.203.415.364.598.501-.667.304-1.243.698-1.311%201.179-.02.144-.022.507.393.787.213.144.395.26.564.365-1.285.521-1.361.96-1.381%201.126-.018.142-.011.496.427.746l.854.489c-.473.389-.971.914-.999%201.429-.018.278.095.532.316.713.675.556%201.231.721%201.653.721.059%200%20.104-.014.158-.02.207.707.641%201.64%201.513%201.64h.013c.8-.008%201.236-.345%201.462-.626.173-.216.268-.457.325-.692.424.195.93.374%201.372.374.151%200%20.294-.021.423-.068.732-.27.944-.704.993-1.021.009-.061.003-.119.002-.179.266.086.538.147.789.147.15%200%20.294-.021.423-.069.542-.2.797-.489.914-.754.237.147.478.258.704.288.106.014.205.021.296.021.356%200%20.595-.101.767-.229.438.435%201.094.992%201.656%201.067.106.014.205.021.296.021a1.56%201.56%200%200%200%20.323-.035c.17.575.453%201.289.866%201.605.358.273.665.362.914.362a.99.99%200%200%200%20.421-.093%201.03%201.03%200%200%200%20.245-.164c.168.428.39.846.68%201.068.358.273.665.362.913.362a.99.99%200%200%200%20.421-.093c.317-.148.512-.448.639-.762.251.157.495.257.726.257.127%200%20.25-.024.37-.071.427-.17.706-.617.841-1.314.022-.015.047-.022.068-.038.067-.051.133-.104.196-.159-.443%201.486-1.107%202.761-2.086%203.257zM8.66%209.925a.5.5%200%201%200-1%200c0%20.653-.818%201.205-1.787%201.205s-1.787-.552-1.787-1.205a.5.5%200%201%200-1%200c0%201.216%201.25%202.205%202.787%202.205s2.787-.989%202.787-2.205zm4.4%2015.965l-.208.097c-2.661%201.258-4.708%201.436-6.086.527-1.542-1.017-1.88-3.19-1.844-4.198a.4.4%200%200%200-.385-.414c-.242-.029-.406.164-.414.385-.046%201.249.367%203.686%202.202%204.896.708.467%201.547.7%202.51.7%201.248%200%202.706-.392%204.362-1.174l.185-.086a.4.4%200%200%200%20.205-.527c-.089-.204-.326-.291-.527-.206zM9.547%202.292c.093.077.205.114.317.114a.5.5%200%200%200%20.318-.886L8.817.397a.5.5%200%200%200-.703.068.5.5%200%200%200%20.069.703l1.364%201.124zm-7.661-.065c.086%200%20.173-.022.253-.068l1.523-.893a.5.5%200%200%200-.506-.863l-1.523.892a.5.5%200%200%200-.179.685c.094.158.261.247.432.247z%22%20transform%3D%22matrix%28-1%200%200%201%2058%200%29%22%20fill%3D%22%233bb300%22/%3E%3Cpath%20d%3D%22M.3%2021.86V10.18q0-.46.02-.68.04-.22.18-.5.28-.54%201.34-.54%201.06%200%201.42.28.38.26.44.78.76-1.04%202.38-1.04%201.64%200%203.1%201.54%201.46%201.54%201.46%203.58%200%202.04-1.46%203.58-1.44%201.54-3.08%201.54-1.64%200-2.38-.92v4.04q0%20.46-.04.68-.02.22-.18.5-.14.3-.5.42-.36.12-.98.12-.62%200-1-.12-.36-.12-.52-.4-.14-.28-.18-.5-.02-.22-.02-.68zm3.96-9.42q-.46.54-.46%201.18%200%20.64.46%201.18.48.52%201.2.52.74%200%201.24-.52.52-.52.52-1.18%200-.66-.48-1.18-.48-.54-1.26-.54-.76%200-1.22.54zm14.741-8.36q.16-.3.54-.42.38-.12%201-.12.64%200%201.02.12.38.12.52.42.16.3.18.54.04.22.04.68v11.94q0%20.46-.04.7-.02.22-.18.5-.3.54-1.7.54-1.38%200-1.54-.98-.84.96-2.34.96-1.8%200-3.28-1.56-1.48-1.58-1.48-3.66%200-2.1%201.48-3.68%201.5-1.58%203.28-1.58%201.48%200%202.3%201v-4.2q0-.46.02-.68.04-.24.18-.52zm-3.24%2010.86q.52.54%201.26.54.74%200%201.22-.54.5-.54.5-1.18%200-.66-.48-1.22-.46-.56-1.26-.56-.8%200-1.28.56-.48.54-.48%201.2%200%20.66.52%201.2zm7.833-1.2q0-2.4%201.68-3.96%201.68-1.56%203.84-1.56%202.16%200%203.82%201.56%201.66%201.54%201.66%203.94%200%201.66-.86%202.96-.86%201.28-2.1%201.9-1.22.6-2.54.6-1.32%200-2.56-.64-1.24-.66-2.1-1.92-.84-1.28-.84-2.88zm4.18%201.44q.64.48%201.3.48.66%200%201.32-.5.66-.5.66-1.48%200-.98-.62-1.46-.62-.48-1.34-.48-.72%200-1.34.5-.62.5-.62%201.48%200%20.96.64%201.46zm11.412-1.44q0%20.84.56%201.32.56.46%201.18.46.64%200%201.18-.36.56-.38.9-.38.6%200%201.46%201.06.46.58.46%201.04%200%20.76-1.1%201.42-1.14.8-2.8.8-1.86%200-3.58-1.34-.82-.64-1.34-1.7-.52-1.08-.52-2.36%200-1.3.52-2.34.52-1.06%201.34-1.7%201.66-1.32%203.54-1.32.76%200%201.48.22.72.2%201.06.4l.32.2q.36.24.56.38.52.4.52.92%200%20.5-.42%201.14-.72%201.1-1.38%201.1-.38%200-1.08-.44-.36-.34-1.04-.34-.66%200-1.24.48-.58.48-.58%201.34z%22%20fill%3D%22green%22/%3E%3C/svg%3E"/>
         </a>
 </div>
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
-<a href="./../../projectal.html">projectal</a><wbr>.<a href="./../entities.html">entities</a><wbr>.tag    </h1>
+<a href="./../projectal.html">projectal</a><wbr>.entities    </h1>
 
-                
-                        <input id="mod-tag-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                        <div class="docstring"><p>Implementations of all Projectal entities.</p>
 
-                        <label class="view-source-button" for="mod-tag-view-source"><span>View Source</span></label>
+<p>All classes here inherit from <code><a href="entity.html#Entity">projectal.entity.Entity</a></code>.</p>
+</div>
 
-                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="kn">from</span> <span class="nn">projectal.entity</span> <span class="kn">import</span> <span class="n">Entity</span>
-</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a>
-</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
-</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="k">class</span> <span class="nc">Tag</span><span class="p">(</span><span class="n">Entity</span><span class="p">):</span>
-</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a><span class="sd">    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag) API.</span>
-</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[]</span>
-</span></pre></div>
+                        <input id="mod-entities-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 
+                        <label class="view-source-button" for="mod-entities-view-source"><span>View Source</span></label>
 
-            </section>
-                <section id="Tag">
-                            <input id="Tag-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
-<div class="attr class">
-            
-    <span class="def">class</span>
-    <span class="name">Tag</span><wbr>(<span class="base"><a href="../entity.html#Entity">projectal.entity.Entity</a></span>):
-
-                <label class="view-source-button" for="Tag-view-source"><span>View Source</span></label>
-
-    </div>
-    <a class="headerlink" href="#Tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="Tag-5"><a href="#Tag-5"><span class="linenos"> 5</span></a><span class="k">class</span> <span class="nc">Tag</span><span class="p">(</span><span class="n">Entity</span><span class="p">):</span>
-</span><span id="Tag-6"><a href="#Tag-6"><span class="linenos"> 6</span></a>    <span class="sd">&quot;&quot;&quot;</span>
-</span><span id="Tag-7"><a href="#Tag-7"><span class="linenos"> 7</span></a><span class="sd">    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag) API.</span>
-</span><span id="Tag-8"><a href="#Tag-8"><span class="linenos"> 8</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="Tag-9"><a href="#Tag-9"><span class="linenos"> 9</span></a>    <span class="n">_path</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
-</span><span id="Tag-10"><a href="#Tag-10"><span class="linenos">10</span></a>    <span class="n">_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
-</span><span id="Tag-11"><a href="#Tag-11"><span class="linenos">11</span></a>    <span class="n">_links</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="Tag-12"><a href="#Tag-12"><span class="linenos">12</span></a>    <span class="n">_links_reverse</span> <span class="o">=</span> <span class="p">[]</span>
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos"> 1</span></a><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-2"><a href="#L-2"><span class="linenos"> 2</span></a><span class="sd">Implementations of all Projectal entities.</span>
+</span><span id="L-3"><a href="#L-3"><span class="linenos"> 3</span></a>
+</span><span id="L-4"><a href="#L-4"><span class="linenos"> 4</span></a><span class="sd">All classes here inherit from `projectal.entity.Entity`.</span>
+</span><span id="L-5"><a href="#L-5"><span class="linenos"> 5</span></a><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-6"><a href="#L-6"><span class="linenos"> 6</span></a>
+</span><span id="L-7"><a href="#L-7"><span class="linenos"> 7</span></a><span class="kn">from</span> <span class="nn">projectal.entities.access_policy</span> <span class="kn">import</span> <span class="n">AccessPolicy</span>
+</span><span id="L-8"><a href="#L-8"><span class="linenos"> 8</span></a><span class="kn">from</span> <span class="nn">projectal.entities.activity</span> <span class="kn">import</span> <span class="n">Activity</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos"> 9</span></a><span class="kn">from</span> <span class="nn">projectal.entities.booking</span> <span class="kn">import</span> <span class="n">Booking</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos">10</span></a><span class="kn">from</span> <span class="nn">projectal.entities.calendar</span> <span class="kn">import</span> <span class="n">Calendar</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos">11</span></a><span class="kn">from</span> <span class="nn">projectal.entities.company</span> <span class="kn">import</span> <span class="n">Company</span>
+</span><span id="L-12"><a href="#L-12"><span class="linenos">12</span></a><span class="kn">from</span> <span class="nn">projectal.entities.contact</span> <span class="kn">import</span> <span class="n">Contact</span>
+</span><span id="L-13"><a href="#L-13"><span class="linenos">13</span></a><span class="kn">from</span> <span class="nn">projectal.entities.customer</span> <span class="kn">import</span> <span class="n">Customer</span>
+</span><span id="L-14"><a href="#L-14"><span class="linenos">14</span></a><span class="kn">from</span> <span class="nn">projectal.entities.department</span> <span class="kn">import</span> <span class="n">Department</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos">15</span></a><span class="kn">from</span> <span class="nn">projectal.entities.file</span> <span class="kn">import</span> <span class="n">File</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos">16</span></a><span class="kn">from</span> <span class="nn">projectal.entities.folder</span> <span class="kn">import</span> <span class="n">Folder</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a><span class="kn">from</span> <span class="nn">projectal.entities.location</span> <span class="kn">import</span> <span class="n">Location</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a><span class="kn">from</span> <span class="nn">projectal.entities.note</span> <span class="kn">import</span> <span class="n">Note</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a><span class="kn">from</span> <span class="nn">projectal.entities.permission</span> <span class="kn">import</span> <span class="n">Permission</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project</span> <span class="kn">import</span> <span class="n">Project</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a><span class="kn">from</span> <span class="nn">projectal.entities.project_template</span> <span class="kn">import</span> <span class="n">ProjectTemplate</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a><span class="kn">from</span> <span class="nn">projectal.entities.rebate</span> <span class="kn">import</span> <span class="n">Rebate</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a><span class="kn">from</span> <span class="nn">projectal.entities.resource</span> <span class="kn">import</span> <span class="n">Resource</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a><span class="kn">from</span> <span class="nn">projectal.entities.skill</span> <span class="kn">import</span> <span class="n">Skill</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a><span class="kn">from</span> <span class="nn">projectal.entities.staff</span> <span class="kn">import</span> <span class="n">Staff</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a><span class="kn">from</span> <span class="nn">projectal.entities.stage</span> <span class="kn">import</span> <span class="n">Stage</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="kn">from</span> <span class="nn">projectal.entities.tag</span> <span class="kn">import</span> <span class="n">Tag</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task</span> <span class="kn">import</span> <span class="n">Task</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a><span class="kn">from</span> <span class="nn">projectal.entities.task_template</span> <span class="kn">import</span> <span class="n">TaskTemplate</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a><span class="kn">from</span> <span class="nn">projectal.entities.user</span> <span class="kn">import</span> <span class="n">User</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a><span class="kn">from</span> <span class="nn">projectal.entities.webhook</span> <span class="kn">import</span> <span class="n">Webhook</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Implementation of the <a href="https://projectal.com/docs/latest/#tag/Tag">Tag</a> API.</p>
-</div>
-
-
-                            <div class="inherited">
-                                <h5>Inherited Members</h5>
-                                <dl>
-                                    <div><dt><a href="../entity.html#Entity">projectal.entity.Entity</a></dt>
-                                <dd id="Tag.get" class="function"><a href="../entity.html#Entity.get">get</a></dd>
-                <dd id="Tag.update" class="function"><a href="../entity.html#Entity.update">update</a></dd>
-                <dd id="Tag.delete" class="function"><a href="../entity.html#Entity.delete">delete</a></dd>
-                <dd id="Tag.history" class="function"><a href="../entity.html#Entity.history">history</a></dd>
-                <dd id="Tag.create" class="function"><a href="../entity.html#Entity.create">create</a></dd>
-                <dd id="Tag.save" class="function"><a href="../entity.html#Entity.save">save</a></dd>
-                <dd id="Tag.clone" class="function"><a href="../entity.html#Entity.clone">clone</a></dd>
-                <dd id="Tag.list" class="function"><a href="../entity.html#Entity.list">list</a></dd>
-                <dd id="Tag.match" class="function"><a href="../entity.html#Entity.match">match</a></dd>
-                <dd id="Tag.match_startswith" class="function"><a href="../entity.html#Entity.match_startswith">match_startswith</a></dd>
-                <dd id="Tag.match_endswith" class="function"><a href="../entity.html#Entity.match_endswith">match_endswith</a></dd>
-                <dd id="Tag.match_one" class="function"><a href="../entity.html#Entity.match_one">match_one</a></dd>
-                <dd id="Tag.match_startswith_one" class="function"><a href="../entity.html#Entity.match_startswith_one">match_startswith_one</a></dd>
-                <dd id="Tag.match_endswith_one" class="function"><a href="../entity.html#Entity.match_endswith_one">match_endswith_one</a></dd>
-                <dd id="Tag.search" class="function"><a href="../entity.html#Entity.search">search</a></dd>
-                <dd id="Tag.query" class="function"><a href="../entity.html#Entity.query">query</a></dd>
-                <dd id="Tag.profile_get" class="function"><a href="../entity.html#Entity.profile_get">profile_get</a></dd>
-                <dd id="Tag.profile_set" class="function"><a href="../entity.html#Entity.profile_set">profile_set</a></dd>
-                <dd id="Tag.changes" class="function"><a href="../entity.html#Entity.changes">changes</a></dd>
-                <dd id="Tag.set_readonly" class="function"><a href="../entity.html#Entity.set_readonly">set_readonly</a></dd>
-                <dd id="Tag.get_link_definitions" class="function"><a href="../entity.html#Entity.get_link_definitions">get_link_definitions</a></dd>
-                <dd id="Tag.entity_name" class="function"><a href="../entity.html#Entity.entity_name">entity_name</a></dd>
-
-            </div>
-            <div><dt>builtins.dict</dt>
-                                <dd id="Tag.setdefault" class="function">setdefault</dd>
-                <dd id="Tag.pop" class="function">pop</dd>
-                <dd id="Tag.popitem" class="function">popitem</dd>
-                <dd id="Tag.keys" class="function">keys</dd>
-                <dd id="Tag.items" class="function">items</dd>
-                <dd id="Tag.values" class="function">values</dd>
-                <dd id="Tag.fromkeys" class="function">fromkeys</dd>
-                <dd id="Tag.clear" class="function">clear</dd>
-                <dd id="Tag.copy" class="function">copy</dd>
-
-            </div>
-                                </dl>
-                            </div>
-                </section>
+            </section>
     </main>
 <script>
     function escapeHTML(html) {
         return document.createElement('div').appendChild(document.createTextNode(html)).parentNode.innerHTML;
     }
 
     const originalContent = document.querySelector("main.pdoc");
@@ -191,15 +164,15 @@
         try {
             search = await new Promise((resolve, reject) => {
                 const script = document.createElement("script");
                 script.type = "text/javascript";
                 script.async = true;
                 script.onload = () => resolve(window.pdocSearch);
                 script.onerror = (e) => reject(e);
-                script.src = "../../search.js";
+                script.src = "../search.js";
                 document.getElementsByTagName("head")[0].appendChild(script);
             });
         } catch (e) {
             console.error("Cannot fetch pdoc search index");
             searchErr = "Cannot fetch search index.";
         }
         onInput();
@@ -233,15 +206,15 @@
             if (results.length === 0) {
                 html = `No search results for '${escapeHTML(term)}'.`
             } else {
                 html = `<h4>${results.length} search result${results.length > 1 ? "s" : ""} for '${escapeHTML(term)}'.</h4>`;
             }
             for (let result of results.slice(0, 10)) {
                 let doc = result.doc;
-                let url = `../../${doc.modulename.replaceAll(".", "/")}.html`;
+                let url = `../${doc.modulename.replaceAll(".", "/")}.html`;
                 if (doc.qualname) {
                     url += `#${doc.qualname}`;
                 }
 
                 let heading;
                 switch (result.doc.kind) {
                     case "function":
```

#### html2text {}

```diff
@@ -1,36 +1,68 @@
 
 
   ⁰
-____ projectal.entities [project logo] [Unknown INPUT type]
-***** API Documentation *****
-    * Tag
+____ projectal [project logo] [Unknown INPUT type]
+***** Submodules *****
+    * access_policy
+    * activity
+    * booking
+    * calendar
+    * company
+    * contact
+    * customer
+    * department
+    * file
+    * folder
+    * location
+    * note
+    * permission
+    * project
+    * project_template
+    * rebate
+    * resource
+    * skill
+    * staff
+    * stage
+    * tag
+    * task
+    * task_template
+    * user
+    * webhook
 built_with_pdoc[pdoc_logo]
 
-****** projectal.entities.tag ******
+****** projectal.entities ******
+Implementations of all Projectal entities.
+All classes here inherit from projectal.entity.Entity.
 ⁰ View Source
-_1from projectal.entity import Entity
-_2
+_1"""
+_2Implementations of all Projectal entities.
 _3
-_4class Tag(Entity):
-_5    """
-_6    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag)
-API.
-_7    """
-_8    _path = 'tag'
-_9    _name = 'tag'
-10    _links = []
-11    _links_reverse = []
-  ⁰
-class Tag(projectal.entity.Entity): View Source
-_5class Tag(Entity):
-_6    """
-_7    Implementation of the [Tag](https://projectal.com/docs/latest/#tag/Tag)
-API.
-_8    """
-_9    _path = 'tag'
-10    _name = 'tag'
-11    _links = []
-12    _links_reverse = []
-Implementation of the Tag API.
-** Inherited Members **
+_4All classes here inherit from `projectal.entity.Entity`.
+_5"""
+_6
+_7from projectal.entities.access_policy import AccessPolicy
+_8from projectal.entities.activity import Activity
+_9from projectal.entities.booking import Booking
+10from projectal.entities.calendar import Calendar
+11from projectal.entities.company import Company
+12from projectal.entities.contact import Contact
+13from projectal.entities.customer import Customer
+14from projectal.entities.department import Department
+15from projectal.entities.file import File
+16from projectal.entities.folder import Folder
+17from projectal.entities.location import Location
+18from projectal.entities.note import Note
+19from projectal.entities.permission import Permission
+20from projectal.entities.project import Project
+21from projectal.entities.project_template import ProjectTemplate
+22from projectal.entities.rebate import Rebate
+23from projectal.entities.resource import Resource
+24from projectal.entities.skill import Skill
+25from projectal.entities.staff import Staff
+26from projectal.entities.stage import Stage
+27from projectal.entities.tag import Tag
+28from projectal.entities.task import Task
+29from projectal.entities.task_template import TaskTemplate
+30from projectal.entities.user import User
+31from projectal.entities.webhook import Webhook
```

### Comparing `projectal-4.0.1/docs/projectal/entities/task.html` & `projectal-4.0.2/docs/projectal/entities/task.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/task_template.html` & `projectal-4.0.2/docs/projectal/entities/task_template.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/user.html` & `projectal-4.0.2/docs/projectal/entities/user.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entities/webhook.html` & `projectal-4.0.2/docs/projectal/entities/webhook.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/entity.html` & `projectal-4.0.2/docs/projectal/entity.html`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
 </span><span id="L-85"><a href="#L-85"><span class="linenos">  85</span></a>        <span class="p">}</span>
 </span><span id="L-86"><a href="#L-86"><span class="linenos">  86</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link_def_by_key</span><span class="p">[</span><span class="n">d</span><span class="p">[</span><span class="s1">&#39;link_key&#39;</span><span class="p">]]</span> <span class="o">=</span> <span class="n">d</span>
 </span><span id="L-87"><a href="#L-87"><span class="linenos">  87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link_def_by_name</span><span class="p">[</span><span class="n">d</span><span class="p">[</span><span class="s1">&#39;name&#39;</span><span class="p">]]</span> <span class="o">=</span> <span class="n">d</span>
 </span><span id="L-88"><a href="#L-88"><span class="linenos">  88</span></a>
 </span><span id="L-89"><a href="#L-89"><span class="linenos">  89</span></a>    <span class="k">def</span> <span class="nf">_add_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="L-90"><a href="#L-90"><span class="linenos">  90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;add&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="L-91"><a href="#L-91"><span class="linenos">  91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos">  92</span></a>    <span class="k">def</span> <span class="nf">_update_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos">  92</span></a>    <span class="k">def</span> <span class="nf">_update_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="L-93"><a href="#L-93"><span class="linenos">  93</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;update&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="L-94"><a href="#L-94"><span class="linenos">  94</span></a>
 </span><span id="L-95"><a href="#L-95"><span class="linenos">  95</span></a>    <span class="k">def</span> <span class="nf">_delete_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="L-96"><a href="#L-96"><span class="linenos">  96</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;delete&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="L-97"><a href="#L-97"><span class="linenos">  97</span></a>
 </span><span id="L-98"><a href="#L-98"><span class="linenos">  98</span></a>    <span class="k">def</span> <span class="nf">_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="n">operation</span><span class="p">,</span> <span class="n">update_cache</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">True</span><span class="p">):</span>
 </span><span id="L-99"><a href="#L-99"><span class="linenos">  99</span></a>        <span class="sd">&quot;&quot;&quot;</span>
@@ -446,16 +446,16 @@
 </span><span id="L-318"><a href="#L-318"><span class="linenos"> 318</span></a>        <span class="c1"># API requests</span>
 </span><span id="L-319"><a href="#L-319"><span class="linenos"> 319</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-320"><a href="#L-320"><span class="linenos"> 320</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="L-321"><a href="#L-321"><span class="linenos"> 321</span></a>            <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="L-322"><a href="#L-322"><span class="linenos"> 322</span></a>            <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="L-323"><a href="#L-323"><span class="linenos"> 323</span></a>
 </span><span id="L-324"><a href="#L-324"><span class="linenos"> 324</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="L-325"><a href="#L-325"><span class="linenos"> 325</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos"> 326</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos"> 325</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="L-326"><a href="#L-326"><span class="linenos"> 326</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="L-327"><a href="#L-327"><span class="linenos"> 327</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="L-328"><a href="#L-328"><span class="linenos"> 328</span></a>
 </span><span id="L-329"><a href="#L-329"><span class="linenos"> 329</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">entities</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
 </span><span id="L-330"><a href="#L-330"><span class="linenos"> 330</span></a>            <span class="k">return</span> <span class="n">objects</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="L-331"><a href="#L-331"><span class="linenos"> 331</span></a>        <span class="k">return</span> <span class="n">objects</span>
 </span><span id="L-332"><a href="#L-332"><span class="linenos"> 332</span></a>
 </span><span id="L-333"><a href="#L-333"><span class="linenos"> 333</span></a>    <span class="nd">@classmethod</span>
@@ -639,16 +639,16 @@
 </span><span id="L-511"><a href="#L-511"><span class="linenos"> 511</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="L-512"><a href="#L-512"><span class="linenos"> 512</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="L-513"><a href="#L-513"><span class="linenos"> 513</span></a>            <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">e</span><span class="p">,</span> <span class="n">Entity</span><span class="p">):</span>
 </span><span id="L-514"><a href="#L-514"><span class="linenos"> 514</span></a>                <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="L-515"><a href="#L-515"><span class="linenos"> 515</span></a>                <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="L-516"><a href="#L-516"><span class="linenos"> 516</span></a>
 </span><span id="L-517"><a href="#L-517"><span class="linenos"> 517</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="L-518"><a href="#L-518"><span class="linenos"> 518</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="L-519"><a href="#L-519"><span class="linenos"> 519</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="L-518"><a href="#L-518"><span class="linenos"> 518</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="L-519"><a href="#L-519"><span class="linenos"> 519</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="L-520"><a href="#L-520"><span class="linenos"> 520</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="L-521"><a href="#L-521"><span class="linenos"> 521</span></a>
 </span><span id="L-522"><a href="#L-522"><span class="linenos"> 522</span></a>        <span class="k">return</span> <span class="kc">True</span>
 </span><span id="L-523"><a href="#L-523"><span class="linenos"> 523</span></a>
 </span><span id="L-524"><a href="#L-524"><span class="linenos"> 524</span></a>    <span class="k">def</span> <span class="nf">__update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
 </span><span id="L-525"><a href="#L-525"><span class="linenos"> 525</span></a>        <span class="sd">&quot;&quot;&quot;Use the dict update for instances.&quot;&quot;&quot;</span>
 </span><span id="L-526"><a href="#L-526"><span class="linenos"> 526</span></a>        <span class="k">return</span> <span class="nb">super</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="bp">self</span><span class="p">)</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
@@ -1239,15 +1239,15 @@
 </span><span id="Entity-86"><a href="#Entity-86"><span class="linenos">  86</span></a>        <span class="p">}</span>
 </span><span id="Entity-87"><a href="#Entity-87"><span class="linenos">  87</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link_def_by_key</span><span class="p">[</span><span class="n">d</span><span class="p">[</span><span class="s1">&#39;link_key&#39;</span><span class="p">]]</span> <span class="o">=</span> <span class="n">d</span>
 </span><span id="Entity-88"><a href="#Entity-88"><span class="linenos">  88</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link_def_by_name</span><span class="p">[</span><span class="n">d</span><span class="p">[</span><span class="s1">&#39;name&#39;</span><span class="p">]]</span> <span class="o">=</span> <span class="n">d</span>
 </span><span id="Entity-89"><a href="#Entity-89"><span class="linenos">  89</span></a>
 </span><span id="Entity-90"><a href="#Entity-90"><span class="linenos">  90</span></a>    <span class="k">def</span> <span class="nf">_add_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="Entity-91"><a href="#Entity-91"><span class="linenos">  91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;add&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="Entity-92"><a href="#Entity-92"><span class="linenos">  92</span></a>
-</span><span id="Entity-93"><a href="#Entity-93"><span class="linenos">  93</span></a>    <span class="k">def</span> <span class="nf">_update_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
+</span><span id="Entity-93"><a href="#Entity-93"><span class="linenos">  93</span></a>    <span class="k">def</span> <span class="nf">_update_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="Entity-94"><a href="#Entity-94"><span class="linenos">  94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;update&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="Entity-95"><a href="#Entity-95"><span class="linenos">  95</span></a>
 </span><span id="Entity-96"><a href="#Entity-96"><span class="linenos">  96</span></a>    <span class="k">def</span> <span class="nf">_delete_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">):</span>
 </span><span id="Entity-97"><a href="#Entity-97"><span class="linenos">  97</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_link</span><span class="p">(</span><span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="s1">&#39;delete&#39;</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
 </span><span id="Entity-98"><a href="#Entity-98"><span class="linenos">  98</span></a>
 </span><span id="Entity-99"><a href="#Entity-99"><span class="linenos">  99</span></a>    <span class="k">def</span> <span class="nf">_link</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">to_entity_name</span><span class="p">,</span> <span class="n">to_link</span><span class="p">,</span> <span class="n">operation</span><span class="p">,</span> <span class="n">update_cache</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">batch_linking</span><span class="o">=</span><span class="kc">True</span><span class="p">):</span>
 </span><span id="Entity-100"><a href="#Entity-100"><span class="linenos"> 100</span></a>        <span class="sd">&quot;&quot;&quot;</span>
@@ -1472,16 +1472,16 @@
 </span><span id="Entity-319"><a href="#Entity-319"><span class="linenos"> 319</span></a>        <span class="c1"># API requests</span>
 </span><span id="Entity-320"><a href="#Entity-320"><span class="linenos"> 320</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="Entity-321"><a href="#Entity-321"><span class="linenos"> 321</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="Entity-322"><a href="#Entity-322"><span class="linenos"> 322</span></a>            <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="Entity-323"><a href="#Entity-323"><span class="linenos"> 323</span></a>            <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="Entity-324"><a href="#Entity-324"><span class="linenos"> 324</span></a>
 </span><span id="Entity-325"><a href="#Entity-325"><span class="linenos"> 325</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="Entity-326"><a href="#Entity-326"><span class="linenos"> 326</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="Entity-327"><a href="#Entity-327"><span class="linenos"> 327</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="Entity-326"><a href="#Entity-326"><span class="linenos"> 326</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="Entity-327"><a href="#Entity-327"><span class="linenos"> 327</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="Entity-328"><a href="#Entity-328"><span class="linenos"> 328</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="Entity-329"><a href="#Entity-329"><span class="linenos"> 329</span></a>
 </span><span id="Entity-330"><a href="#Entity-330"><span class="linenos"> 330</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">entities</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
 </span><span id="Entity-331"><a href="#Entity-331"><span class="linenos"> 331</span></a>            <span class="k">return</span> <span class="n">objects</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="Entity-332"><a href="#Entity-332"><span class="linenos"> 332</span></a>        <span class="k">return</span> <span class="n">objects</span>
 </span><span id="Entity-333"><a href="#Entity-333"><span class="linenos"> 333</span></a>
 </span><span id="Entity-334"><a href="#Entity-334"><span class="linenos"> 334</span></a>    <span class="nd">@classmethod</span>
@@ -1665,16 +1665,16 @@
 </span><span id="Entity-512"><a href="#Entity-512"><span class="linenos"> 512</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="Entity-513"><a href="#Entity-513"><span class="linenos"> 513</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="Entity-514"><a href="#Entity-514"><span class="linenos"> 514</span></a>            <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">e</span><span class="p">,</span> <span class="n">Entity</span><span class="p">):</span>
 </span><span id="Entity-515"><a href="#Entity-515"><span class="linenos"> 515</span></a>                <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="Entity-516"><a href="#Entity-516"><span class="linenos"> 516</span></a>                <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="Entity-517"><a href="#Entity-517"><span class="linenos"> 517</span></a>
 </span><span id="Entity-518"><a href="#Entity-518"><span class="linenos"> 518</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="Entity-519"><a href="#Entity-519"><span class="linenos"> 519</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="Entity-520"><a href="#Entity-520"><span class="linenos"> 520</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="Entity-519"><a href="#Entity-519"><span class="linenos"> 519</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="Entity-520"><a href="#Entity-520"><span class="linenos"> 520</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="Entity-521"><a href="#Entity-521"><span class="linenos"> 521</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="Entity-522"><a href="#Entity-522"><span class="linenos"> 522</span></a>
 </span><span id="Entity-523"><a href="#Entity-523"><span class="linenos"> 523</span></a>        <span class="k">return</span> <span class="kc">True</span>
 </span><span id="Entity-524"><a href="#Entity-524"><span class="linenos"> 524</span></a>
 </span><span id="Entity-525"><a href="#Entity-525"><span class="linenos"> 525</span></a>    <span class="k">def</span> <span class="nf">__update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">):</span>
 </span><span id="Entity-526"><a href="#Entity-526"><span class="linenos"> 526</span></a>        <span class="sd">&quot;&quot;&quot;Use the dict update for instances.&quot;&quot;&quot;</span>
 </span><span id="Entity-527"><a href="#Entity-527"><span class="linenos"> 527</span></a>        <span class="k">return</span> <span class="nb">super</span><span class="p">(</span><span class="n">Entity</span><span class="p">,</span> <span class="bp">self</span><span class="p">)</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="o">*</span><span class="n">args</span><span class="p">,</span> <span class="o">**</span><span class="n">kwargs</span><span class="p">)</span>
@@ -2432,16 +2432,16 @@
 </span><span id="Entity.update-512"><a href="#Entity.update-512"><span class="linenos">512</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="Entity.update-513"><a href="#Entity.update-513"><span class="linenos">513</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="Entity.update-514"><a href="#Entity.update-514"><span class="linenos">514</span></a>            <span class="k">if</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">e</span><span class="p">,</span> <span class="n">Entity</span><span class="p">):</span>
 </span><span id="Entity.update-515"><a href="#Entity.update-515"><span class="linenos">515</span></a>                <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="Entity.update-516"><a href="#Entity.update-516"><span class="linenos">516</span></a>                <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="Entity.update-517"><a href="#Entity.update-517"><span class="linenos">517</span></a>
 </span><span id="Entity.update-518"><a href="#Entity.update-518"><span class="linenos">518</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="Entity.update-519"><a href="#Entity.update-519"><span class="linenos">519</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="Entity.update-520"><a href="#Entity.update-520"><span class="linenos">520</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="Entity.update-519"><a href="#Entity.update-519"><span class="linenos">519</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="Entity.update-520"><a href="#Entity.update-520"><span class="linenos">520</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="Entity.update-521"><a href="#Entity.update-521"><span class="linenos">521</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="Entity.update-522"><a href="#Entity.update-522"><span class="linenos">522</span></a>
 </span><span id="Entity.update-523"><a href="#Entity.update-523"><span class="linenos">523</span></a>        <span class="k">return</span> <span class="kc">True</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Save one or more entities of the same type. The entity
@@ -2691,16 +2691,16 @@
 </span><span id="Entity.create-319"><a href="#Entity.create-319"><span class="linenos">319</span></a>        <span class="c1"># API requests</span>
 </span><span id="Entity.create-320"><a href="#Entity.create-320"><span class="linenos">320</span></a>        <span class="n">link_request_batch</span> <span class="o">=</span> <span class="p">[]</span>
 </span><span id="Entity.create-321"><a href="#Entity.create-321"><span class="linenos">321</span></a>        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="n">e_list</span><span class="p">:</span>
 </span><span id="Entity.create-322"><a href="#Entity.create-322"><span class="linenos">322</span></a>            <span class="n">requests</span> <span class="o">=</span> <span class="n">e</span><span class="o">.</span><span class="n">__apply_link_changes</span><span class="p">(</span><span class="n">batch_linking</span><span class="o">=</span><span class="n">batch_linking</span><span class="p">)</span>
 </span><span id="Entity.create-323"><a href="#Entity.create-323"><span class="linenos">323</span></a>            <span class="n">link_request_batch</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">requests</span><span class="p">)</span>
 </span><span id="Entity.create-324"><a href="#Entity.create-324"><span class="linenos">324</span></a>
 </span><span id="Entity.create-325"><a href="#Entity.create-325"><span class="linenos">325</span></a>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span> <span class="ow">and</span> <span class="n">batch_linking</span><span class="p">:</span>
-</span><span id="Entity.create-326"><a href="#Entity.create-326"><span class="linenos">326</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">1000</span><span class="p">):</span>
-</span><span id="Entity.create-327"><a href="#Entity.create-327"><span class="linenos">327</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">1000</span><span class="p">]</span>
+</span><span id="Entity.create-326"><a href="#Entity.create-326"><span class="linenos">326</span></a>            <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">link_request_batch</span><span class="p">),</span> <span class="mi">100</span><span class="p">):</span>
+</span><span id="Entity.create-327"><a href="#Entity.create-327"><span class="linenos">327</span></a>                <span class="n">chunk</span> <span class="o">=</span> <span class="n">link_request_batch</span><span class="p">[</span><span class="n">i</span><span class="p">:</span><span class="n">i</span> <span class="o">+</span> <span class="mi">100</span><span class="p">]</span>
 </span><span id="Entity.create-328"><a href="#Entity.create-328"><span class="linenos">328</span></a>                <span class="n">api</span><span class="o">.</span><span class="n">post</span><span class="p">(</span><span class="s1">&#39;/api/composite&#39;</span><span class="p">,</span> <span class="n">chunk</span><span class="p">)</span>
 </span><span id="Entity.create-329"><a href="#Entity.create-329"><span class="linenos">329</span></a>
 </span><span id="Entity.create-330"><a href="#Entity.create-330"><span class="linenos">330</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">entities</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
 </span><span id="Entity.create-331"><a href="#Entity.create-331"><span class="linenos">331</span></a>            <span class="k">return</span> <span class="n">objects</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
 </span><span id="Entity.create-332"><a href="#Entity.create-332"><span class="linenos">332</span></a>        <span class="k">return</span> <span class="n">objects</span>
 </span></pre></div>
```

#### html2text {}

```diff
@@ -118,15 +118,15 @@
 __85        }
 __86        self._link_def_by_key[d['link_key']] = d
 __87        self._link_def_by_name[d['name']] = d
 __88
 __89    def _add_link(self, to_entity_name, to_link):
 __90        self._link(to_entity_name, to_link, 'add', batch_linking=False)
 __91
-__92    def _update_link(self,to_entity_name, to_link):
+__92    def _update_link(self, to_entity_name, to_link):
 __93        self._link(to_entity_name, to_link, 'update', batch_linking=False)
 __94
 __95    def _delete_link(self, to_entity_name, to_link):
 __96        self._link(to_entity_name, to_link, 'delete', batch_linking=False)
 __97
 __98    def _link(self, to_entity_name, to_link, operation, update_cache=True,
 batch_linking=True):
@@ -369,16 +369,16 @@
 _318        # API requests
 _319        link_request_batch = []
 _320        for e in e_list:
 _321            requests = e.__apply_link_changes(batch_linking=batch_linking)
 _322            link_request_batch.extend(requests)
 _323
 _324        if len(link_request_batch) > 0 and batch_linking:
-_325            for i in range(0, len(link_request_batch), 1000):
-_326                chunk = link_request_batch[i:i + 1000]
+_325            for i in range(0, len(link_request_batch), 100):
+_326                chunk = link_request_batch[i:i + 100]
 _327                api.post('/api/composite', chunk)
 _328
 _329        if not isinstance(entities, list):
 _330            return objects[0]
 _331        return objects
 _332
 _333    @classmethod
@@ -575,16 +575,16 @@
 _512        for e in e_list:
 _513            if isinstance(e, Entity):
 _514                requests = e.__apply_link_changes
 (batch_linking=batch_linking)
 _515                link_request_batch.extend(requests)
 _516
 _517        if len(link_request_batch) > 0 and batch_linking:
-_518            for i in range(0, len(link_request_batch), 1000):
-_519                chunk = link_request_batch[i:i + 1000]
+_518            for i in range(0, len(link_request_batch), 100):
+_519                chunk = link_request_batch[i:i + 100]
 _520                api.post('/api/composite', chunk)
 _521
 _522        return True
 _523
 _524    def __update(self, *args, **kwargs):
 _525        """Use the dict update for instances."""
 _526        return super(Entity, self).update(*args, **kwargs)
@@ -1210,15 +1210,15 @@
 __86        }
 __87        self._link_def_by_key[d['link_key']] = d
 __88        self._link_def_by_name[d['name']] = d
 __89
 __90    def _add_link(self, to_entity_name, to_link):
 __91        self._link(to_entity_name, to_link, 'add', batch_linking=False)
 __92
-__93    def _update_link(self,to_entity_name, to_link):
+__93    def _update_link(self, to_entity_name, to_link):
 __94        self._link(to_entity_name, to_link, 'update', batch_linking=False)
 __95
 __96    def _delete_link(self, to_entity_name, to_link):
 __97        self._link(to_entity_name, to_link, 'delete', batch_linking=False)
 __98
 __99    def _link(self, to_entity_name, to_link, operation, update_cache=True,
 batch_linking=True):
@@ -1461,16 +1461,16 @@
 _319        # API requests
 _320        link_request_batch = []
 _321        for e in e_list:
 _322            requests = e.__apply_link_changes(batch_linking=batch_linking)
 _323            link_request_batch.extend(requests)
 _324
 _325        if len(link_request_batch) > 0 and batch_linking:
-_326            for i in range(0, len(link_request_batch), 1000):
-_327                chunk = link_request_batch[i:i + 1000]
+_326            for i in range(0, len(link_request_batch), 100):
+_327                chunk = link_request_batch[i:i + 100]
 _328                api.post('/api/composite', chunk)
 _329
 _330        if not isinstance(entities, list):
 _331            return objects[0]
 _332        return objects
 _333
 _334    @classmethod
@@ -1667,16 +1667,16 @@
 _513        for e in e_list:
 _514            if isinstance(e, Entity):
 _515                requests = e.__apply_link_changes
 (batch_linking=batch_linking)
 _516                link_request_batch.extend(requests)
 _517
 _518        if len(link_request_batch) > 0 and batch_linking:
-_519            for i in range(0, len(link_request_batch), 1000):
-_520                chunk = link_request_batch[i:i + 1000]
+_519            for i in range(0, len(link_request_batch), 100):
+_520                chunk = link_request_batch[i:i + 100]
 _521                api.post('/api/composite', chunk)
 _522
 _523        return True
 _524
 _525    def __update(self, *args, **kwargs):
 _526        """Use the dict update for instances."""
 _527        return super(Entity, self).update(*args, **kwargs)
@@ -2442,16 +2442,16 @@
 513        for e in e_list:
 514            if isinstance(e, Entity):
 515                requests = e.__apply_link_changes
 (batch_linking=batch_linking)
 516                link_request_batch.extend(requests)
 517
 518        if len(link_request_batch) > 0 and batch_linking:
-519            for i in range(0, len(link_request_batch), 1000):
-520                chunk = link_request_batch[i:i + 1000]
+519            for i in range(0, len(link_request_batch), 100):
+520                chunk = link_request_batch[i:i + 100]
 521                api.post('/api/composite', chunk)
 522
 523        return True
 Save one or more entities of the same type. The entity type is determined by
 the subclass calling this method. Only the fields that have been modifier will
 be sent to the server as part of the request.
 entities: Can be a dict to update a single entity, or a list of dicts to update
@@ -2640,16 +2640,16 @@
 319        # API requests
 320        link_request_batch = []
 321        for e in e_list:
 322            requests = e.__apply_link_changes(batch_linking=batch_linking)
 323            link_request_batch.extend(requests)
 324
 325        if len(link_request_batch) > 0 and batch_linking:
-326            for i in range(0, len(link_request_batch), 1000):
-327                chunk = link_request_batch[i:i + 1000]
+326            for i in range(0, len(link_request_batch), 100):
+327                chunk = link_request_batch[i:i + 100]
 328                api.post('/api/composite', chunk)
 329
 330        if not isinstance(entities, list):
 331            return objects[0]
 332        return objects
 Create one or more entities of the same type. The entity type is determined by
 the subclass calling this method.
```

### Comparing `projectal-4.0.1/docs/projectal/enums.html` & `projectal-4.0.2/docs/projectal/enums.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/errors.html` & `projectal-4.0.2/docs/projectal/errors.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal/linkers.html` & `projectal-4.0.2/docs/projectal/linkers.html`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,44 @@
                         <li>
                                 <a class="function" href="#AccessPolicyLinker.unlink_access_policy">unlink_access_policy</a>
                         </li>
                 </ul>
 
             </li>
             <li>
+                    <a class="class" href="#ActivityLinker">ActivityLinker</a>
+                            <ul class="memberlist">
+                        <li>
+                                <a class="function" href="#ActivityLinker.__init__">ActivityLinker</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#ActivityLinker.link_activity">link_activity</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#ActivityLinker.unlink_activity">unlink_activity</a>
+                        </li>
+                </ul>
+
+            </li>
+            <li>
+                    <a class="class" href="#BookingLinker">BookingLinker</a>
+                            <ul class="memberlist">
+                        <li>
+                                <a class="function" href="#BookingLinker.__init__">BookingLinker</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#BookingLinker.link_booking">link_booking</a>
+                        </li>
+                        <li>
+                                <a class="function" href="#BookingLinker.unlink_booking">unlink_booking</a>
+                        </li>
+                </ul>
+
+            </li>
+            <li>
                     <a class="class" href="#CompanyLinker">CompanyLinker</a>
                             <ul class="memberlist">
                         <li>
                                 <a class="function" href="#CompanyLinker.__init__">CompanyLinker</a>
                         </li>
                         <li>
                                 <a class="function" href="#CompanyLinker.link_company">link_company</a>
@@ -450,290 +480,314 @@
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="sd">task.link_staff(staff)</span>
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">```</span>
 </span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="sd">&quot;&quot;&quot;</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a><span class="kn">from</span> <span class="nn">projectal</span> <span class="kn">import</span> <span class="n">api</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a><span class="k">class</span> <span class="nc">BaseLinker</span><span class="p">:</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="c1"># _link_name is the link name (usually the entity name)</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="c1"># _link_key is the key within the source object that points to the</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="c1"># links. E.g., &#39;skillList&#39;</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="c1"># _link_data_name is the key within the linked (target) object that points</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="c1"># to a store of custom values within that link. E.g, Skill objects,</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="c1"># when linked, have a &#39;skillLink&#39; property that holds data about</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="c1"># the link.</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="c1"># _link_type is the data type of the value in entity[link_key]. This is</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="c1"># usually a list since most links appear as &#39;skillList&#39;, &#39;staffList&#39;,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="c1"># etc. But some links are single-entity only and appear as dicts like</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="c1"># project[stage] = Stage.</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">list</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="c1"># _link_entity is the string name (capitalized, like Stage) of the Entity</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="c1"># class within this library that fetched links will be converted to.</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="c1"># This is useful when the name of the list differs from the entity</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="c1"># name. E.g: stage_list needs to be converted to Stage.</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="k">class</span> <span class="nc">AccessPolicyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Access Policies&quot;&quot;&quot;</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;access_policy&#39;</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;accessPolicyList&#39;</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;AccessPolicy&#39;</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="k">class</span> <span class="nc">CompanyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Companies&quot;&quot;&quot;</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;company&#39;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="k">class</span> <span class="nc">ContactLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Contacts&quot;&quot;&quot;</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;contact&#39;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="k">class</span> <span class="nc">CustomerLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Customers&quot;&quot;&quot;</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;customer&#39;</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="k">class</span> <span class="nc">DepartmentLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Departments&quot;&quot;&quot;</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;department&#39;</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="k">class</span> <span class="nc">FileLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Files&quot;&quot;&quot;</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;file&#39;</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;storageFileList&#39;</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">class</span> <span class="nc">BaseLinker</span><span class="p">:</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="c1"># _link_name is the link name (usually the entity name)</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="c1"># _link_key is the key within the source object that points to the</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>    <span class="c1"># links. E.g., &#39;skillList&#39;</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="c1"># _link_data_name is the key within the linked (target) object that points</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="c1"># to a store of custom values within that link. E.g, Skill objects,</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="c1"># when linked, have a &#39;skillLink&#39; property that holds data about</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="c1"># the link.</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="c1"># _link_type is the data type of the value in entity[link_key]. This is</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="c1"># usually a list since most links appear as &#39;skillList&#39;, &#39;staffList&#39;,</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="c1"># etc. But some links are single-entity only and appear as dicts like</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="c1"># project[stage] = Stage.</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">list</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="c1"># _link_entity is the string name (capitalized, like Stage) of the Entity</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="c1"># class within this library that fetched links will be converted to.</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>    <span class="c1"># This is useful when the name of the list differs from the entity</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>    <span class="c1"># name. E.g: stage_list needs to be converted to Stage.</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="k">class</span> <span class="nc">AccessPolicyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Access Policies&quot;&quot;&quot;</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;access_policy&#39;</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;accessPolicyList&#39;</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;AccessPolicy&#39;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="k">class</span> <span class="nc">ActivityLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Activities&quot;&quot;&quot;</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="k">def</span> <span class="nf">link_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="k">def</span> <span class="nf">unlink_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="k">class</span> <span class="nc">BookingLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Bookings&quot;&quot;&quot;</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="k">def</span> <span class="nf">link_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="k">def</span> <span class="nf">unlink_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="k">class</span> <span class="nc">CompanyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Companies&quot;&quot;&quot;</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;company&#39;</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="k">class</span> <span class="nc">ContactLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Contacts&quot;&quot;&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;contact&#39;</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="k">class</span> <span class="nc">CustomerLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Customers&quot;&quot;&quot;</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;customer&#39;</span>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
 </span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="k">class</span> <span class="nc">FolderLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Folders&quot;&quot;&quot;</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;folder&#39;</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;folders&#39;</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">class</span> <span class="nc">DepartmentLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Departments&quot;&quot;&quot;</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;department&#39;</span>
 </span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
 </span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
 </span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
 </span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="k">class</span> <span class="nc">LocationLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Locations&quot;&quot;&quot;</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;location&#39;</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="k">class</span> <span class="nc">FileLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Files&quot;&quot;&quot;</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;file&#39;</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;storageFileList&#39;</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
 </span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a><span class="k">class</span> <span class="nc">PermissionLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Permissions&quot;&quot;&quot;</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;permission&#39;</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">class</span> <span class="nc">ProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Projects&quot;&quot;&quot;</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;project&#39;</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="k">class</span> <span class="nc">RebateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Rebates&quot;&quot;&quot;</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;rebate&#39;</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a><span class="k">class</span> <span class="nc">ResourceLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Resources&quot;&quot;&quot;</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;resource&#39;</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="k">class</span> <span class="nc">SkillLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Skills&quot;&quot;&quot;</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;skillLink&#39;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="k">class</span> <span class="nc">FolderLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Folders&quot;&quot;&quot;</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;folder&#39;</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;folders&#39;</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="k">class</span> <span class="nc">LocationLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Locations&quot;&quot;&quot;</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;location&#39;</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="k">class</span> <span class="nc">PermissionLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Permissions&quot;&quot;&quot;</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;permission&#39;</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="k">class</span> <span class="nc">ProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Projects&quot;&quot;&quot;</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;project&#39;</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="k">class</span> <span class="nc">RebateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Rebates&quot;&quot;&quot;</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;rebate&#39;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
 </span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
 </span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="k">class</span> <span class="nc">ResourceLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Resources&quot;&quot;&quot;</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;resource&#39;</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
 </span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="k">class</span> <span class="nc">StaffLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Staff&quot;&quot;&quot;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;staff&#39;</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="k">class</span> <span class="nc">SkillLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Skills&quot;&quot;&quot;</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;skillLink&#39;</span>
 </span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a><span class="k">class</span> <span class="nc">StageLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stages&quot;&quot;&quot;</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">dict</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
 </span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="k">class</span> <span class="nc">StageListLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stage List&quot;&quot;&quot;</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage_list&#39;</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stageList&#39;</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;Stage&#39;</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="k">class</span> <span class="nc">StaffLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Staff&quot;&quot;&quot;</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;staff&#39;</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>
 </span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="k">class</span> <span class="nc">StageLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stages&quot;&quot;&quot;</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">dict</span>
 </span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="k">class</span> <span class="nc">UserLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;user&#39;</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
 </span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="k">class</span> <span class="nc">TaskLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task&#39;</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="k">class</span> <span class="nc">TaskTemplateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task_template&#39;</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;TaskTemplate&#39;</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="k">class</span> <span class="nc">StageListLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stage List&quot;&quot;&quot;</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage_list&#39;</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stageList&#39;</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;Stage&#39;</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>
 </span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="k">class</span> <span class="nc">UserLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;user&#39;</span>
 </span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
 </span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="k">class</span> <span class="nc">TagLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
 </span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="k">class</span> <span class="nc">NoteLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;note&#39;</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="k">class</span> <span class="nc">CalendarLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;calendar&#39;</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="c1"># Projects have a list of tasks that we can fetch using the links=</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="c1"># method, but they have no linker methods available.</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="k">class</span> <span class="nc">TaskInProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s2">&quot;task&quot;</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="k">class</span> <span class="nc">TaskLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task&#39;</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="k">class</span> <span class="nc">TaskTemplateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task_template&#39;</span>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;TaskTemplate&#39;</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="k">class</span> <span class="nc">TagLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a><span class="k">class</span> <span class="nc">NoteLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;note&#39;</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a><span class="k">class</span> <span class="nc">CalendarLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;calendar&#39;</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a><span class="c1"># Projects have a list of tasks that we can fetch using the links=</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a><span class="c1"># method, but they have no linker methods available.</span>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="k">class</span> <span class="nc">TaskInProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s2">&quot;task&quot;</span>
 </span></pre></div>
 
 
             </section>
                 <section id="BaseLinker">
                             <input id="BaseLinker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -741,39 +795,39 @@
     <span class="def">class</span>
     <span class="name">BaseLinker</span>:
 
                 <label class="view-source-button" for="BaseLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#BaseLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="BaseLinker-34"><a href="#BaseLinker-34"><span class="linenos">34</span></a><span class="k">class</span> <span class="nc">BaseLinker</span><span class="p">:</span>
-</span><span id="BaseLinker-35"><a href="#BaseLinker-35"><span class="linenos">35</span></a>    <span class="c1"># _link_name is the link name (usually the entity name)</span>
-</span><span id="BaseLinker-36"><a href="#BaseLinker-36"><span class="linenos">36</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="BaseLinker-37"><a href="#BaseLinker-37"><span class="linenos">37</span></a>
-</span><span id="BaseLinker-38"><a href="#BaseLinker-38"><span class="linenos">38</span></a>    <span class="c1"># _link_key is the key within the source object that points to the</span>
-</span><span id="BaseLinker-39"><a href="#BaseLinker-39"><span class="linenos">39</span></a>    <span class="c1"># links. E.g., &#39;skillList&#39;</span>
-</span><span id="BaseLinker-40"><a href="#BaseLinker-40"><span class="linenos">40</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="BaseLinker-41"><a href="#BaseLinker-41"><span class="linenos">41</span></a>
-</span><span id="BaseLinker-42"><a href="#BaseLinker-42"><span class="linenos">42</span></a>    <span class="c1"># _link_data_name is the key within the linked (target) object that points</span>
-</span><span id="BaseLinker-43"><a href="#BaseLinker-43"><span class="linenos">43</span></a>    <span class="c1"># to a store of custom values within that link. E.g, Skill objects,</span>
-</span><span id="BaseLinker-44"><a href="#BaseLinker-44"><span class="linenos">44</span></a>    <span class="c1"># when linked, have a &#39;skillLink&#39; property that holds data about</span>
-</span><span id="BaseLinker-45"><a href="#BaseLinker-45"><span class="linenos">45</span></a>    <span class="c1"># the link.</span>
-</span><span id="BaseLinker-46"><a href="#BaseLinker-46"><span class="linenos">46</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="BaseLinker-47"><a href="#BaseLinker-47"><span class="linenos">47</span></a>
-</span><span id="BaseLinker-48"><a href="#BaseLinker-48"><span class="linenos">48</span></a>    <span class="c1"># _link_type is the data type of the value in entity[link_key]. This is</span>
-</span><span id="BaseLinker-49"><a href="#BaseLinker-49"><span class="linenos">49</span></a>    <span class="c1"># usually a list since most links appear as &#39;skillList&#39;, &#39;staffList&#39;,</span>
-</span><span id="BaseLinker-50"><a href="#BaseLinker-50"><span class="linenos">50</span></a>    <span class="c1"># etc. But some links are single-entity only and appear as dicts like</span>
-</span><span id="BaseLinker-51"><a href="#BaseLinker-51"><span class="linenos">51</span></a>    <span class="c1"># project[stage] = Stage.</span>
-</span><span id="BaseLinker-52"><a href="#BaseLinker-52"><span class="linenos">52</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">list</span>
-</span><span id="BaseLinker-53"><a href="#BaseLinker-53"><span class="linenos">53</span></a>
-</span><span id="BaseLinker-54"><a href="#BaseLinker-54"><span class="linenos">54</span></a>    <span class="c1"># _link_entity is the string name (capitalized, like Stage) of the Entity</span>
-</span><span id="BaseLinker-55"><a href="#BaseLinker-55"><span class="linenos">55</span></a>    <span class="c1"># class within this library that fetched links will be converted to.</span>
-</span><span id="BaseLinker-56"><a href="#BaseLinker-56"><span class="linenos">56</span></a>    <span class="c1"># This is useful when the name of the list differs from the entity</span>
-</span><span id="BaseLinker-57"><a href="#BaseLinker-57"><span class="linenos">57</span></a>    <span class="c1"># name. E.g: stage_list needs to be converted to Stage.</span>
-</span><span id="BaseLinker-58"><a href="#BaseLinker-58"><span class="linenos">58</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="kc">None</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BaseLinker-35"><a href="#BaseLinker-35"><span class="linenos">35</span></a><span class="k">class</span> <span class="nc">BaseLinker</span><span class="p">:</span>
+</span><span id="BaseLinker-36"><a href="#BaseLinker-36"><span class="linenos">36</span></a>    <span class="c1"># _link_name is the link name (usually the entity name)</span>
+</span><span id="BaseLinker-37"><a href="#BaseLinker-37"><span class="linenos">37</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="BaseLinker-38"><a href="#BaseLinker-38"><span class="linenos">38</span></a>
+</span><span id="BaseLinker-39"><a href="#BaseLinker-39"><span class="linenos">39</span></a>    <span class="c1"># _link_key is the key within the source object that points to the</span>
+</span><span id="BaseLinker-40"><a href="#BaseLinker-40"><span class="linenos">40</span></a>    <span class="c1"># links. E.g., &#39;skillList&#39;</span>
+</span><span id="BaseLinker-41"><a href="#BaseLinker-41"><span class="linenos">41</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="BaseLinker-42"><a href="#BaseLinker-42"><span class="linenos">42</span></a>
+</span><span id="BaseLinker-43"><a href="#BaseLinker-43"><span class="linenos">43</span></a>    <span class="c1"># _link_data_name is the key within the linked (target) object that points</span>
+</span><span id="BaseLinker-44"><a href="#BaseLinker-44"><span class="linenos">44</span></a>    <span class="c1"># to a store of custom values within that link. E.g, Skill objects,</span>
+</span><span id="BaseLinker-45"><a href="#BaseLinker-45"><span class="linenos">45</span></a>    <span class="c1"># when linked, have a &#39;skillLink&#39; property that holds data about</span>
+</span><span id="BaseLinker-46"><a href="#BaseLinker-46"><span class="linenos">46</span></a>    <span class="c1"># the link.</span>
+</span><span id="BaseLinker-47"><a href="#BaseLinker-47"><span class="linenos">47</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="BaseLinker-48"><a href="#BaseLinker-48"><span class="linenos">48</span></a>
+</span><span id="BaseLinker-49"><a href="#BaseLinker-49"><span class="linenos">49</span></a>    <span class="c1"># _link_type is the data type of the value in entity[link_key]. This is</span>
+</span><span id="BaseLinker-50"><a href="#BaseLinker-50"><span class="linenos">50</span></a>    <span class="c1"># usually a list since most links appear as &#39;skillList&#39;, &#39;staffList&#39;,</span>
+</span><span id="BaseLinker-51"><a href="#BaseLinker-51"><span class="linenos">51</span></a>    <span class="c1"># etc. But some links are single-entity only and appear as dicts like</span>
+</span><span id="BaseLinker-52"><a href="#BaseLinker-52"><span class="linenos">52</span></a>    <span class="c1"># project[stage] = Stage.</span>
+</span><span id="BaseLinker-53"><a href="#BaseLinker-53"><span class="linenos">53</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">list</span>
+</span><span id="BaseLinker-54"><a href="#BaseLinker-54"><span class="linenos">54</span></a>
+</span><span id="BaseLinker-55"><a href="#BaseLinker-55"><span class="linenos">55</span></a>    <span class="c1"># _link_entity is the string name (capitalized, like Stage) of the Entity</span>
+</span><span id="BaseLinker-56"><a href="#BaseLinker-56"><span class="linenos">56</span></a>    <span class="c1"># class within this library that fetched links will be converted to.</span>
+</span><span id="BaseLinker-57"><a href="#BaseLinker-57"><span class="linenos">57</span></a>    <span class="c1"># This is useful when the name of the list differs from the entity</span>
+</span><span id="BaseLinker-58"><a href="#BaseLinker-58"><span class="linenos">58</span></a>    <span class="c1"># name. E.g: stage_list needs to be converted to Stage.</span>
+</span><span id="BaseLinker-59"><a href="#BaseLinker-59"><span class="linenos">59</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="kc">None</span>
 </span></pre></div>
 
 
     
 
                             <div id="BaseLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -795,25 +849,25 @@
     <span class="def">class</span>
     <span class="name">AccessPolicyLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="AccessPolicyLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AccessPolicyLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker-60"><a href="#AccessPolicyLinker-60"><span class="linenos">60</span></a><span class="k">class</span> <span class="nc">AccessPolicyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="AccessPolicyLinker-61"><a href="#AccessPolicyLinker-61"><span class="linenos">61</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Access Policies&quot;&quot;&quot;</span>
-</span><span id="AccessPolicyLinker-62"><a href="#AccessPolicyLinker-62"><span class="linenos">62</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;access_policy&#39;</span>
-</span><span id="AccessPolicyLinker-63"><a href="#AccessPolicyLinker-63"><span class="linenos">63</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;accessPolicyList&#39;</span>
-</span><span id="AccessPolicyLinker-64"><a href="#AccessPolicyLinker-64"><span class="linenos">64</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;AccessPolicy&#39;</span>
-</span><span id="AccessPolicyLinker-65"><a href="#AccessPolicyLinker-65"><span class="linenos">65</span></a>
-</span><span id="AccessPolicyLinker-66"><a href="#AccessPolicyLinker-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="AccessPolicyLinker-67"><a href="#AccessPolicyLinker-67"><span class="linenos">67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
-</span><span id="AccessPolicyLinker-68"><a href="#AccessPolicyLinker-68"><span class="linenos">68</span></a>
-</span><span id="AccessPolicyLinker-69"><a href="#AccessPolicyLinker-69"><span class="linenos">69</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="AccessPolicyLinker-70"><a href="#AccessPolicyLinker-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker-62"><a href="#AccessPolicyLinker-62"><span class="linenos">62</span></a><span class="k">class</span> <span class="nc">AccessPolicyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="AccessPolicyLinker-63"><a href="#AccessPolicyLinker-63"><span class="linenos">63</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Access Policies&quot;&quot;&quot;</span>
+</span><span id="AccessPolicyLinker-64"><a href="#AccessPolicyLinker-64"><span class="linenos">64</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;access_policy&#39;</span>
+</span><span id="AccessPolicyLinker-65"><a href="#AccessPolicyLinker-65"><span class="linenos">65</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;accessPolicyList&#39;</span>
+</span><span id="AccessPolicyLinker-66"><a href="#AccessPolicyLinker-66"><span class="linenos">66</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;AccessPolicy&#39;</span>
+</span><span id="AccessPolicyLinker-67"><a href="#AccessPolicyLinker-67"><span class="linenos">67</span></a>
+</span><span id="AccessPolicyLinker-68"><a href="#AccessPolicyLinker-68"><span class="linenos">68</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="AccessPolicyLinker-69"><a href="#AccessPolicyLinker-69"><span class="linenos">69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+</span><span id="AccessPolicyLinker-70"><a href="#AccessPolicyLinker-70"><span class="linenos">70</span></a>
+</span><span id="AccessPolicyLinker-71"><a href="#AccessPolicyLinker-71"><span class="linenos">71</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="AccessPolicyLinker-72"><a href="#AccessPolicyLinker-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Access Policies</p>
 </div>
 
 
@@ -836,16 +890,16 @@
         <span class="def">def</span>
         <span class="name">link_access_policy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">access_policies</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="AccessPolicyLinker.link_access_policy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AccessPolicyLinker.link_access_policy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker.link_access_policy-66"><a href="#AccessPolicyLinker.link_access_policy-66"><span class="linenos">66</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="AccessPolicyLinker.link_access_policy-67"><a href="#AccessPolicyLinker.link_access_policy-67"><span class="linenos">67</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker.link_access_policy-68"><a href="#AccessPolicyLinker.link_access_policy-68"><span class="linenos">68</span></a>    <span class="k">def</span> <span class="nf">link_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="AccessPolicyLinker.link_access_policy-69"><a href="#AccessPolicyLinker.link_access_policy-69"><span class="linenos">69</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="AccessPolicyLinker.unlink_access_policy" class="classattr">
@@ -855,16 +909,172 @@
         <span class="def">def</span>
         <span class="name">unlink_access_policy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">access_policies</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="AccessPolicyLinker.unlink_access_policy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#AccessPolicyLinker.unlink_access_policy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker.unlink_access_policy-69"><a href="#AccessPolicyLinker.unlink_access_policy-69"><span class="linenos">69</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
-</span><span id="AccessPolicyLinker.unlink_access_policy-70"><a href="#AccessPolicyLinker.unlink_access_policy-70"><span class="linenos">70</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="AccessPolicyLinker.unlink_access_policy-71"><a href="#AccessPolicyLinker.unlink_access_policy-71"><span class="linenos">71</span></a>    <span class="k">def</span> <span class="nf">unlink_access_policy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">):</span>
+</span><span id="AccessPolicyLinker.unlink_access_policy-72"><a href="#AccessPolicyLinker.unlink_access_policy-72"><span class="linenos">72</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;access_policy&#39;</span><span class="p">,</span> <span class="n">access_policies</span><span class="p">)</span>
+</span></pre></div>
+
+
+    
+
+                            </div>
+                </section>
+                <section id="ActivityLinker">
+                            <input id="ActivityLinker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr class">
+            
+    <span class="def">class</span>
+    <span class="name">ActivityLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
+
+                <label class="view-source-button" for="ActivityLinker-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#ActivityLinker"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ActivityLinker-75"><a href="#ActivityLinker-75"><span class="linenos">75</span></a><span class="k">class</span> <span class="nc">ActivityLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="ActivityLinker-76"><a href="#ActivityLinker-76"><span class="linenos">76</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Activities&quot;&quot;&quot;</span>
+</span><span id="ActivityLinker-77"><a href="#ActivityLinker-77"><span class="linenos">77</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;activity&#39;</span>
+</span><span id="ActivityLinker-78"><a href="#ActivityLinker-78"><span class="linenos">78</span></a>
+</span><span id="ActivityLinker-79"><a href="#ActivityLinker-79"><span class="linenos">79</span></a>    <span class="k">def</span> <span class="nf">link_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="ActivityLinker-80"><a href="#ActivityLinker-80"><span class="linenos">80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span><span id="ActivityLinker-81"><a href="#ActivityLinker-81"><span class="linenos">81</span></a>
+</span><span id="ActivityLinker-82"><a href="#ActivityLinker-82"><span class="linenos">82</span></a>    <span class="k">def</span> <span class="nf">unlink_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="ActivityLinker-83"><a href="#ActivityLinker-83"><span class="linenos">83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Subclass can link to Activities</p>
+</div>
+
+
+                            <div id="ActivityLinker.__init__" class="classattr">
+                                <div class="attr function">
+            
+        <span class="name">ActivityLinker</span><span class="signature pdoc-code condensed">()</span>
+
+        
+    </div>
+    <a class="headerlink" href="#ActivityLinker.__init__"></a>
+    
+    
+
+                            </div>
+                            <div id="ActivityLinker.link_activity" class="classattr">
+                                        <input id="ActivityLinker.link_activity-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">link_activity</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">activity</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="ActivityLinker.link_activity-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#ActivityLinker.link_activity"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ActivityLinker.link_activity-79"><a href="#ActivityLinker.link_activity-79"><span class="linenos">79</span></a>    <span class="k">def</span> <span class="nf">link_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="ActivityLinker.link_activity-80"><a href="#ActivityLinker.link_activity-80"><span class="linenos">80</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span></pre></div>
+
+
+    
+
+                            </div>
+                            <div id="ActivityLinker.unlink_activity" class="classattr">
+                                        <input id="ActivityLinker.unlink_activity-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">unlink_activity</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">activity</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="ActivityLinker.unlink_activity-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#ActivityLinker.unlink_activity"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ActivityLinker.unlink_activity-82"><a href="#ActivityLinker.unlink_activity-82"><span class="linenos">82</span></a>    <span class="k">def</span> <span class="nf">unlink_activity</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">activity</span><span class="p">):</span>
+</span><span id="ActivityLinker.unlink_activity-83"><a href="#ActivityLinker.unlink_activity-83"><span class="linenos">83</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;activity&#39;</span><span class="p">,</span> <span class="n">activity</span><span class="p">)</span>
+</span></pre></div>
+
+
+    
+
+                            </div>
+                </section>
+                <section id="BookingLinker">
+                            <input id="BookingLinker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr class">
+            
+    <span class="def">class</span>
+    <span class="name">BookingLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
+
+                <label class="view-source-button" for="BookingLinker-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#BookingLinker"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BookingLinker-86"><a href="#BookingLinker-86"><span class="linenos">86</span></a><span class="k">class</span> <span class="nc">BookingLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="BookingLinker-87"><a href="#BookingLinker-87"><span class="linenos">87</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Bookings&quot;&quot;&quot;</span>
+</span><span id="BookingLinker-88"><a href="#BookingLinker-88"><span class="linenos">88</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;booking&#39;</span>
+</span><span id="BookingLinker-89"><a href="#BookingLinker-89"><span class="linenos">89</span></a>
+</span><span id="BookingLinker-90"><a href="#BookingLinker-90"><span class="linenos">90</span></a>    <span class="k">def</span> <span class="nf">link_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="BookingLinker-91"><a href="#BookingLinker-91"><span class="linenos">91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
+</span><span id="BookingLinker-92"><a href="#BookingLinker-92"><span class="linenos">92</span></a>
+</span><span id="BookingLinker-93"><a href="#BookingLinker-93"><span class="linenos">93</span></a>    <span class="k">def</span> <span class="nf">unlink_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="BookingLinker-94"><a href="#BookingLinker-94"><span class="linenos">94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Subclass can link to Bookings</p>
+</div>
+
+
+                            <div id="BookingLinker.__init__" class="classattr">
+                                <div class="attr function">
+            
+        <span class="name">BookingLinker</span><span class="signature pdoc-code condensed">()</span>
+
+        
+    </div>
+    <a class="headerlink" href="#BookingLinker.__init__"></a>
+    
+    
+
+                            </div>
+                            <div id="BookingLinker.link_booking" class="classattr">
+                                        <input id="BookingLinker.link_booking-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">link_booking</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">booking</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="BookingLinker.link_booking-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#BookingLinker.link_booking"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BookingLinker.link_booking-90"><a href="#BookingLinker.link_booking-90"><span class="linenos">90</span></a>    <span class="k">def</span> <span class="nf">link_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="BookingLinker.link_booking-91"><a href="#BookingLinker.link_booking-91"><span class="linenos">91</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
+</span></pre></div>
+
+
+    
+
+                            </div>
+                            <div id="BookingLinker.unlink_booking" class="classattr">
+                                        <input id="BookingLinker.unlink_booking-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">unlink_booking</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">booking</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="BookingLinker.unlink_booking-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#BookingLinker.unlink_booking"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="BookingLinker.unlink_booking-93"><a href="#BookingLinker.unlink_booking-93"><span class="linenos">93</span></a>    <span class="k">def</span> <span class="nf">unlink_booking</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">booking</span><span class="p">):</span>
+</span><span id="BookingLinker.unlink_booking-94"><a href="#BookingLinker.unlink_booking-94"><span class="linenos">94</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;booking&#39;</span><span class="p">,</span> <span class="n">booking</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -875,23 +1085,23 @@
     <span class="def">class</span>
     <span class="name">CompanyLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="CompanyLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CompanyLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker-73"><a href="#CompanyLinker-73"><span class="linenos">73</span></a><span class="k">class</span> <span class="nc">CompanyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="CompanyLinker-74"><a href="#CompanyLinker-74"><span class="linenos">74</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Companies&quot;&quot;&quot;</span>
-</span><span id="CompanyLinker-75"><a href="#CompanyLinker-75"><span class="linenos">75</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;company&#39;</span>
-</span><span id="CompanyLinker-76"><a href="#CompanyLinker-76"><span class="linenos">76</span></a>
-</span><span id="CompanyLinker-77"><a href="#CompanyLinker-77"><span class="linenos">77</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="CompanyLinker-78"><a href="#CompanyLinker-78"><span class="linenos">78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
-</span><span id="CompanyLinker-79"><a href="#CompanyLinker-79"><span class="linenos">79</span></a>
-</span><span id="CompanyLinker-80"><a href="#CompanyLinker-80"><span class="linenos">80</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="CompanyLinker-81"><a href="#CompanyLinker-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker-97"><a href="#CompanyLinker-97"><span class="linenos"> 97</span></a><span class="k">class</span> <span class="nc">CompanyLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="CompanyLinker-98"><a href="#CompanyLinker-98"><span class="linenos"> 98</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Companies&quot;&quot;&quot;</span>
+</span><span id="CompanyLinker-99"><a href="#CompanyLinker-99"><span class="linenos"> 99</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;company&#39;</span>
+</span><span id="CompanyLinker-100"><a href="#CompanyLinker-100"><span class="linenos">100</span></a>
+</span><span id="CompanyLinker-101"><a href="#CompanyLinker-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="CompanyLinker-102"><a href="#CompanyLinker-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+</span><span id="CompanyLinker-103"><a href="#CompanyLinker-103"><span class="linenos">103</span></a>
+</span><span id="CompanyLinker-104"><a href="#CompanyLinker-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="CompanyLinker-105"><a href="#CompanyLinker-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Companies</p>
 </div>
 
 
@@ -914,16 +1124,16 @@
         <span class="def">def</span>
         <span class="name">link_company</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">companies</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="CompanyLinker.link_company-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CompanyLinker.link_company"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker.link_company-77"><a href="#CompanyLinker.link_company-77"><span class="linenos">77</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="CompanyLinker.link_company-78"><a href="#CompanyLinker.link_company-78"><span class="linenos">78</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker.link_company-101"><a href="#CompanyLinker.link_company-101"><span class="linenos">101</span></a>    <span class="k">def</span> <span class="nf">link_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="CompanyLinker.link_company-102"><a href="#CompanyLinker.link_company-102"><span class="linenos">102</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="CompanyLinker.unlink_company" class="classattr">
@@ -933,16 +1143,16 @@
         <span class="def">def</span>
         <span class="name">unlink_company</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">companies</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="CompanyLinker.unlink_company-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CompanyLinker.unlink_company"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker.unlink_company-80"><a href="#CompanyLinker.unlink_company-80"><span class="linenos">80</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
-</span><span id="CompanyLinker.unlink_company-81"><a href="#CompanyLinker.unlink_company-81"><span class="linenos">81</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CompanyLinker.unlink_company-104"><a href="#CompanyLinker.unlink_company-104"><span class="linenos">104</span></a>    <span class="k">def</span> <span class="nf">unlink_company</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">companies</span><span class="p">):</span>
+</span><span id="CompanyLinker.unlink_company-105"><a href="#CompanyLinker.unlink_company-105"><span class="linenos">105</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;company&#39;</span><span class="p">,</span> <span class="n">companies</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -953,23 +1163,23 @@
     <span class="def">class</span>
     <span class="name">ContactLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="ContactLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ContactLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker-84"><a href="#ContactLinker-84"><span class="linenos">84</span></a><span class="k">class</span> <span class="nc">ContactLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="ContactLinker-85"><a href="#ContactLinker-85"><span class="linenos">85</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Contacts&quot;&quot;&quot;</span>
-</span><span id="ContactLinker-86"><a href="#ContactLinker-86"><span class="linenos">86</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;contact&#39;</span>
-</span><span id="ContactLinker-87"><a href="#ContactLinker-87"><span class="linenos">87</span></a>
-</span><span id="ContactLinker-88"><a href="#ContactLinker-88"><span class="linenos">88</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="ContactLinker-89"><a href="#ContactLinker-89"><span class="linenos">89</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
-</span><span id="ContactLinker-90"><a href="#ContactLinker-90"><span class="linenos">90</span></a>
-</span><span id="ContactLinker-91"><a href="#ContactLinker-91"><span class="linenos">91</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="ContactLinker-92"><a href="#ContactLinker-92"><span class="linenos">92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker-108"><a href="#ContactLinker-108"><span class="linenos">108</span></a><span class="k">class</span> <span class="nc">ContactLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="ContactLinker-109"><a href="#ContactLinker-109"><span class="linenos">109</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Contacts&quot;&quot;&quot;</span>
+</span><span id="ContactLinker-110"><a href="#ContactLinker-110"><span class="linenos">110</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;contact&#39;</span>
+</span><span id="ContactLinker-111"><a href="#ContactLinker-111"><span class="linenos">111</span></a>
+</span><span id="ContactLinker-112"><a href="#ContactLinker-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="ContactLinker-113"><a href="#ContactLinker-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+</span><span id="ContactLinker-114"><a href="#ContactLinker-114"><span class="linenos">114</span></a>
+</span><span id="ContactLinker-115"><a href="#ContactLinker-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="ContactLinker-116"><a href="#ContactLinker-116"><span class="linenos">116</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Contacts</p>
 </div>
 
 
@@ -992,16 +1202,16 @@
         <span class="def">def</span>
         <span class="name">link_contact</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">contacts</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ContactLinker.link_contact-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ContactLinker.link_contact"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker.link_contact-88"><a href="#ContactLinker.link_contact-88"><span class="linenos">88</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="ContactLinker.link_contact-89"><a href="#ContactLinker.link_contact-89"><span class="linenos">89</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker.link_contact-112"><a href="#ContactLinker.link_contact-112"><span class="linenos">112</span></a>    <span class="k">def</span> <span class="nf">link_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="ContactLinker.link_contact-113"><a href="#ContactLinker.link_contact-113"><span class="linenos">113</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ContactLinker.unlink_contact" class="classattr">
@@ -1011,16 +1221,16 @@
         <span class="def">def</span>
         <span class="name">unlink_contact</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">contacts</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ContactLinker.unlink_contact-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ContactLinker.unlink_contact"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker.unlink_contact-91"><a href="#ContactLinker.unlink_contact-91"><span class="linenos">91</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
-</span><span id="ContactLinker.unlink_contact-92"><a href="#ContactLinker.unlink_contact-92"><span class="linenos">92</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ContactLinker.unlink_contact-115"><a href="#ContactLinker.unlink_contact-115"><span class="linenos">115</span></a>    <span class="k">def</span> <span class="nf">unlink_contact</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">contacts</span><span class="p">):</span>
+</span><span id="ContactLinker.unlink_contact-116"><a href="#ContactLinker.unlink_contact-116"><span class="linenos">116</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;contact&#39;</span><span class="p">,</span> <span class="n">contacts</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1031,23 +1241,23 @@
     <span class="def">class</span>
     <span class="name">CustomerLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="CustomerLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CustomerLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker-95"><a href="#CustomerLinker-95"><span class="linenos"> 95</span></a><span class="k">class</span> <span class="nc">CustomerLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="CustomerLinker-96"><a href="#CustomerLinker-96"><span class="linenos"> 96</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Customers&quot;&quot;&quot;</span>
-</span><span id="CustomerLinker-97"><a href="#CustomerLinker-97"><span class="linenos"> 97</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;customer&#39;</span>
-</span><span id="CustomerLinker-98"><a href="#CustomerLinker-98"><span class="linenos"> 98</span></a>
-</span><span id="CustomerLinker-99"><a href="#CustomerLinker-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="CustomerLinker-100"><a href="#CustomerLinker-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
-</span><span id="CustomerLinker-101"><a href="#CustomerLinker-101"><span class="linenos">101</span></a>
-</span><span id="CustomerLinker-102"><a href="#CustomerLinker-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="CustomerLinker-103"><a href="#CustomerLinker-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker-119"><a href="#CustomerLinker-119"><span class="linenos">119</span></a><span class="k">class</span> <span class="nc">CustomerLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="CustomerLinker-120"><a href="#CustomerLinker-120"><span class="linenos">120</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Customers&quot;&quot;&quot;</span>
+</span><span id="CustomerLinker-121"><a href="#CustomerLinker-121"><span class="linenos">121</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;customer&#39;</span>
+</span><span id="CustomerLinker-122"><a href="#CustomerLinker-122"><span class="linenos">122</span></a>
+</span><span id="CustomerLinker-123"><a href="#CustomerLinker-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="CustomerLinker-124"><a href="#CustomerLinker-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
+</span><span id="CustomerLinker-125"><a href="#CustomerLinker-125"><span class="linenos">125</span></a>
+</span><span id="CustomerLinker-126"><a href="#CustomerLinker-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="CustomerLinker-127"><a href="#CustomerLinker-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Customers</p>
 </div>
 
 
@@ -1070,16 +1280,16 @@
         <span class="def">def</span>
         <span class="name">link_customer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">customers</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="CustomerLinker.link_customer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CustomerLinker.link_customer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker.link_customer-99"><a href="#CustomerLinker.link_customer-99"><span class="linenos"> 99</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="CustomerLinker.link_customer-100"><a href="#CustomerLinker.link_customer-100"><span class="linenos">100</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker.link_customer-123"><a href="#CustomerLinker.link_customer-123"><span class="linenos">123</span></a>    <span class="k">def</span> <span class="nf">link_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="CustomerLinker.link_customer-124"><a href="#CustomerLinker.link_customer-124"><span class="linenos">124</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="CustomerLinker.unlink_customer" class="classattr">
@@ -1089,16 +1299,16 @@
         <span class="def">def</span>
         <span class="name">unlink_customer</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">customers</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="CustomerLinker.unlink_customer-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CustomerLinker.unlink_customer"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker.unlink_customer-102"><a href="#CustomerLinker.unlink_customer-102"><span class="linenos">102</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
-</span><span id="CustomerLinker.unlink_customer-103"><a href="#CustomerLinker.unlink_customer-103"><span class="linenos">103</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CustomerLinker.unlink_customer-126"><a href="#CustomerLinker.unlink_customer-126"><span class="linenos">126</span></a>    <span class="k">def</span> <span class="nf">unlink_customer</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">customers</span><span class="p">):</span>
+</span><span id="CustomerLinker.unlink_customer-127"><a href="#CustomerLinker.unlink_customer-127"><span class="linenos">127</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;customer&#39;</span><span class="p">,</span> <span class="n">customers</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1109,23 +1319,23 @@
     <span class="def">class</span>
     <span class="name">DepartmentLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="DepartmentLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DepartmentLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker-106"><a href="#DepartmentLinker-106"><span class="linenos">106</span></a><span class="k">class</span> <span class="nc">DepartmentLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="DepartmentLinker-107"><a href="#DepartmentLinker-107"><span class="linenos">107</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Departments&quot;&quot;&quot;</span>
-</span><span id="DepartmentLinker-108"><a href="#DepartmentLinker-108"><span class="linenos">108</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;department&#39;</span>
-</span><span id="DepartmentLinker-109"><a href="#DepartmentLinker-109"><span class="linenos">109</span></a>
-</span><span id="DepartmentLinker-110"><a href="#DepartmentLinker-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="DepartmentLinker-111"><a href="#DepartmentLinker-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
-</span><span id="DepartmentLinker-112"><a href="#DepartmentLinker-112"><span class="linenos">112</span></a>
-</span><span id="DepartmentLinker-113"><a href="#DepartmentLinker-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="DepartmentLinker-114"><a href="#DepartmentLinker-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker-130"><a href="#DepartmentLinker-130"><span class="linenos">130</span></a><span class="k">class</span> <span class="nc">DepartmentLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="DepartmentLinker-131"><a href="#DepartmentLinker-131"><span class="linenos">131</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Departments&quot;&quot;&quot;</span>
+</span><span id="DepartmentLinker-132"><a href="#DepartmentLinker-132"><span class="linenos">132</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;department&#39;</span>
+</span><span id="DepartmentLinker-133"><a href="#DepartmentLinker-133"><span class="linenos">133</span></a>
+</span><span id="DepartmentLinker-134"><a href="#DepartmentLinker-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="DepartmentLinker-135"><a href="#DepartmentLinker-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
+</span><span id="DepartmentLinker-136"><a href="#DepartmentLinker-136"><span class="linenos">136</span></a>
+</span><span id="DepartmentLinker-137"><a href="#DepartmentLinker-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="DepartmentLinker-138"><a href="#DepartmentLinker-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Departments</p>
 </div>
 
 
@@ -1148,16 +1358,16 @@
         <span class="def">def</span>
         <span class="name">link_department</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">departments</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DepartmentLinker.link_department-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DepartmentLinker.link_department"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker.link_department-110"><a href="#DepartmentLinker.link_department-110"><span class="linenos">110</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="DepartmentLinker.link_department-111"><a href="#DepartmentLinker.link_department-111"><span class="linenos">111</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker.link_department-134"><a href="#DepartmentLinker.link_department-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">link_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="DepartmentLinker.link_department-135"><a href="#DepartmentLinker.link_department-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="DepartmentLinker.unlink_department" class="classattr">
@@ -1167,16 +1377,16 @@
         <span class="def">def</span>
         <span class="name">unlink_department</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">departments</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DepartmentLinker.unlink_department-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DepartmentLinker.unlink_department"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker.unlink_department-113"><a href="#DepartmentLinker.unlink_department-113"><span class="linenos">113</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
-</span><span id="DepartmentLinker.unlink_department-114"><a href="#DepartmentLinker.unlink_department-114"><span class="linenos">114</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DepartmentLinker.unlink_department-137"><a href="#DepartmentLinker.unlink_department-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">unlink_department</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">departments</span><span class="p">):</span>
+</span><span id="DepartmentLinker.unlink_department-138"><a href="#DepartmentLinker.unlink_department-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;department&#39;</span><span class="p">,</span> <span class="n">departments</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1187,24 +1397,24 @@
     <span class="def">class</span>
     <span class="name">FileLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="FileLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FileLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker-117"><a href="#FileLinker-117"><span class="linenos">117</span></a><span class="k">class</span> <span class="nc">FileLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="FileLinker-118"><a href="#FileLinker-118"><span class="linenos">118</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Files&quot;&quot;&quot;</span>
-</span><span id="FileLinker-119"><a href="#FileLinker-119"><span class="linenos">119</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;file&#39;</span>
-</span><span id="FileLinker-120"><a href="#FileLinker-120"><span class="linenos">120</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;storageFileList&#39;</span>
-</span><span id="FileLinker-121"><a href="#FileLinker-121"><span class="linenos">121</span></a>
-</span><span id="FileLinker-122"><a href="#FileLinker-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="FileLinker-123"><a href="#FileLinker-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
-</span><span id="FileLinker-124"><a href="#FileLinker-124"><span class="linenos">124</span></a>
-</span><span id="FileLinker-125"><a href="#FileLinker-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="FileLinker-126"><a href="#FileLinker-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker-141"><a href="#FileLinker-141"><span class="linenos">141</span></a><span class="k">class</span> <span class="nc">FileLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="FileLinker-142"><a href="#FileLinker-142"><span class="linenos">142</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Files&quot;&quot;&quot;</span>
+</span><span id="FileLinker-143"><a href="#FileLinker-143"><span class="linenos">143</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;file&#39;</span>
+</span><span id="FileLinker-144"><a href="#FileLinker-144"><span class="linenos">144</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;storageFileList&#39;</span>
+</span><span id="FileLinker-145"><a href="#FileLinker-145"><span class="linenos">145</span></a>
+</span><span id="FileLinker-146"><a href="#FileLinker-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="FileLinker-147"><a href="#FileLinker-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
+</span><span id="FileLinker-148"><a href="#FileLinker-148"><span class="linenos">148</span></a>
+</span><span id="FileLinker-149"><a href="#FileLinker-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="FileLinker-150"><a href="#FileLinker-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Files</p>
 </div>
 
 
@@ -1227,16 +1437,16 @@
         <span class="def">def</span>
         <span class="name">link_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">files</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="FileLinker.link_file-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FileLinker.link_file"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker.link_file-122"><a href="#FileLinker.link_file-122"><span class="linenos">122</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="FileLinker.link_file-123"><a href="#FileLinker.link_file-123"><span class="linenos">123</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker.link_file-146"><a href="#FileLinker.link_file-146"><span class="linenos">146</span></a>    <span class="k">def</span> <span class="nf">link_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="FileLinker.link_file-147"><a href="#FileLinker.link_file-147"><span class="linenos">147</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="FileLinker.unlink_file" class="classattr">
@@ -1246,16 +1456,16 @@
         <span class="def">def</span>
         <span class="name">unlink_file</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">files</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="FileLinker.unlink_file-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FileLinker.unlink_file"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker.unlink_file-125"><a href="#FileLinker.unlink_file-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
-</span><span id="FileLinker.unlink_file-126"><a href="#FileLinker.unlink_file-126"><span class="linenos">126</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FileLinker.unlink_file-149"><a href="#FileLinker.unlink_file-149"><span class="linenos">149</span></a>    <span class="k">def</span> <span class="nf">unlink_file</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">files</span><span class="p">):</span>
+</span><span id="FileLinker.unlink_file-150"><a href="#FileLinker.unlink_file-150"><span class="linenos">150</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;file&#39;</span><span class="p">,</span> <span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1266,24 +1476,24 @@
     <span class="def">class</span>
     <span class="name">FolderLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="FolderLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FolderLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker-129"><a href="#FolderLinker-129"><span class="linenos">129</span></a><span class="k">class</span> <span class="nc">FolderLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="FolderLinker-130"><a href="#FolderLinker-130"><span class="linenos">130</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Folders&quot;&quot;&quot;</span>
-</span><span id="FolderLinker-131"><a href="#FolderLinker-131"><span class="linenos">131</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;folder&#39;</span>
-</span><span id="FolderLinker-132"><a href="#FolderLinker-132"><span class="linenos">132</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;folders&#39;</span>
-</span><span id="FolderLinker-133"><a href="#FolderLinker-133"><span class="linenos">133</span></a>
-</span><span id="FolderLinker-134"><a href="#FolderLinker-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="FolderLinker-135"><a href="#FolderLinker-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
-</span><span id="FolderLinker-136"><a href="#FolderLinker-136"><span class="linenos">136</span></a>
-</span><span id="FolderLinker-137"><a href="#FolderLinker-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="FolderLinker-138"><a href="#FolderLinker-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker-153"><a href="#FolderLinker-153"><span class="linenos">153</span></a><span class="k">class</span> <span class="nc">FolderLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="FolderLinker-154"><a href="#FolderLinker-154"><span class="linenos">154</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Folders&quot;&quot;&quot;</span>
+</span><span id="FolderLinker-155"><a href="#FolderLinker-155"><span class="linenos">155</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;folder&#39;</span>
+</span><span id="FolderLinker-156"><a href="#FolderLinker-156"><span class="linenos">156</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;folders&#39;</span>
+</span><span id="FolderLinker-157"><a href="#FolderLinker-157"><span class="linenos">157</span></a>
+</span><span id="FolderLinker-158"><a href="#FolderLinker-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="FolderLinker-159"><a href="#FolderLinker-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+</span><span id="FolderLinker-160"><a href="#FolderLinker-160"><span class="linenos">160</span></a>
+</span><span id="FolderLinker-161"><a href="#FolderLinker-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="FolderLinker-162"><a href="#FolderLinker-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Folders</p>
 </div>
 
 
@@ -1306,16 +1516,16 @@
         <span class="def">def</span>
         <span class="name">link_folder</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">folders</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="FolderLinker.link_folder-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FolderLinker.link_folder"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker.link_folder-134"><a href="#FolderLinker.link_folder-134"><span class="linenos">134</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="FolderLinker.link_folder-135"><a href="#FolderLinker.link_folder-135"><span class="linenos">135</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker.link_folder-158"><a href="#FolderLinker.link_folder-158"><span class="linenos">158</span></a>    <span class="k">def</span> <span class="nf">link_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="FolderLinker.link_folder-159"><a href="#FolderLinker.link_folder-159"><span class="linenos">159</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="FolderLinker.unlink_folder" class="classattr">
@@ -1325,16 +1535,16 @@
         <span class="def">def</span>
         <span class="name">unlink_folder</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">folders</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="FolderLinker.unlink_folder-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#FolderLinker.unlink_folder"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker.unlink_folder-137"><a href="#FolderLinker.unlink_folder-137"><span class="linenos">137</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
-</span><span id="FolderLinker.unlink_folder-138"><a href="#FolderLinker.unlink_folder-138"><span class="linenos">138</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="FolderLinker.unlink_folder-161"><a href="#FolderLinker.unlink_folder-161"><span class="linenos">161</span></a>    <span class="k">def</span> <span class="nf">unlink_folder</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">folders</span><span class="p">):</span>
+</span><span id="FolderLinker.unlink_folder-162"><a href="#FolderLinker.unlink_folder-162"><span class="linenos">162</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;folder&#39;</span><span class="p">,</span> <span class="n">folders</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1345,23 +1555,23 @@
     <span class="def">class</span>
     <span class="name">LocationLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="LocationLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#LocationLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker-141"><a href="#LocationLinker-141"><span class="linenos">141</span></a><span class="k">class</span> <span class="nc">LocationLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="LocationLinker-142"><a href="#LocationLinker-142"><span class="linenos">142</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Locations&quot;&quot;&quot;</span>
-</span><span id="LocationLinker-143"><a href="#LocationLinker-143"><span class="linenos">143</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;location&#39;</span>
-</span><span id="LocationLinker-144"><a href="#LocationLinker-144"><span class="linenos">144</span></a>
-</span><span id="LocationLinker-145"><a href="#LocationLinker-145"><span class="linenos">145</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="LocationLinker-146"><a href="#LocationLinker-146"><span class="linenos">146</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
-</span><span id="LocationLinker-147"><a href="#LocationLinker-147"><span class="linenos">147</span></a>
-</span><span id="LocationLinker-148"><a href="#LocationLinker-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="LocationLinker-149"><a href="#LocationLinker-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker-165"><a href="#LocationLinker-165"><span class="linenos">165</span></a><span class="k">class</span> <span class="nc">LocationLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="LocationLinker-166"><a href="#LocationLinker-166"><span class="linenos">166</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Locations&quot;&quot;&quot;</span>
+</span><span id="LocationLinker-167"><a href="#LocationLinker-167"><span class="linenos">167</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;location&#39;</span>
+</span><span id="LocationLinker-168"><a href="#LocationLinker-168"><span class="linenos">168</span></a>
+</span><span id="LocationLinker-169"><a href="#LocationLinker-169"><span class="linenos">169</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="LocationLinker-170"><a href="#LocationLinker-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+</span><span id="LocationLinker-171"><a href="#LocationLinker-171"><span class="linenos">171</span></a>
+</span><span id="LocationLinker-172"><a href="#LocationLinker-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="LocationLinker-173"><a href="#LocationLinker-173"><span class="linenos">173</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Locations</p>
 </div>
 
 
@@ -1384,16 +1594,16 @@
         <span class="def">def</span>
         <span class="name">link_location</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">locations</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="LocationLinker.link_location-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#LocationLinker.link_location"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker.link_location-145"><a href="#LocationLinker.link_location-145"><span class="linenos">145</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="LocationLinker.link_location-146"><a href="#LocationLinker.link_location-146"><span class="linenos">146</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker.link_location-169"><a href="#LocationLinker.link_location-169"><span class="linenos">169</span></a>    <span class="k">def</span> <span class="nf">link_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="LocationLinker.link_location-170"><a href="#LocationLinker.link_location-170"><span class="linenos">170</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="LocationLinker.unlink_location" class="classattr">
@@ -1403,16 +1613,16 @@
         <span class="def">def</span>
         <span class="name">unlink_location</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">locations</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="LocationLinker.unlink_location-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#LocationLinker.unlink_location"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker.unlink_location-148"><a href="#LocationLinker.unlink_location-148"><span class="linenos">148</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
-</span><span id="LocationLinker.unlink_location-149"><a href="#LocationLinker.unlink_location-149"><span class="linenos">149</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="LocationLinker.unlink_location-172"><a href="#LocationLinker.unlink_location-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">unlink_location</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">locations</span><span class="p">):</span>
+</span><span id="LocationLinker.unlink_location-173"><a href="#LocationLinker.unlink_location-173"><span class="linenos">173</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;location&#39;</span><span class="p">,</span> <span class="n">locations</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1423,23 +1633,23 @@
     <span class="def">class</span>
     <span class="name">PermissionLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="PermissionLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#PermissionLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker-152"><a href="#PermissionLinker-152"><span class="linenos">152</span></a><span class="k">class</span> <span class="nc">PermissionLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="PermissionLinker-153"><a href="#PermissionLinker-153"><span class="linenos">153</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Permissions&quot;&quot;&quot;</span>
-</span><span id="PermissionLinker-154"><a href="#PermissionLinker-154"><span class="linenos">154</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;permission&#39;</span>
-</span><span id="PermissionLinker-155"><a href="#PermissionLinker-155"><span class="linenos">155</span></a>
-</span><span id="PermissionLinker-156"><a href="#PermissionLinker-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="PermissionLinker-157"><a href="#PermissionLinker-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
-</span><span id="PermissionLinker-158"><a href="#PermissionLinker-158"><span class="linenos">158</span></a>
-</span><span id="PermissionLinker-159"><a href="#PermissionLinker-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="PermissionLinker-160"><a href="#PermissionLinker-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker-176"><a href="#PermissionLinker-176"><span class="linenos">176</span></a><span class="k">class</span> <span class="nc">PermissionLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="PermissionLinker-177"><a href="#PermissionLinker-177"><span class="linenos">177</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Permissions&quot;&quot;&quot;</span>
+</span><span id="PermissionLinker-178"><a href="#PermissionLinker-178"><span class="linenos">178</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;permission&#39;</span>
+</span><span id="PermissionLinker-179"><a href="#PermissionLinker-179"><span class="linenos">179</span></a>
+</span><span id="PermissionLinker-180"><a href="#PermissionLinker-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="PermissionLinker-181"><a href="#PermissionLinker-181"><span class="linenos">181</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+</span><span id="PermissionLinker-182"><a href="#PermissionLinker-182"><span class="linenos">182</span></a>
+</span><span id="PermissionLinker-183"><a href="#PermissionLinker-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="PermissionLinker-184"><a href="#PermissionLinker-184"><span class="linenos">184</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Permissions</p>
 </div>
 
 
@@ -1462,16 +1672,16 @@
         <span class="def">def</span>
         <span class="name">link_permission</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">permissions</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="PermissionLinker.link_permission-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#PermissionLinker.link_permission"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker.link_permission-156"><a href="#PermissionLinker.link_permission-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="PermissionLinker.link_permission-157"><a href="#PermissionLinker.link_permission-157"><span class="linenos">157</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker.link_permission-180"><a href="#PermissionLinker.link_permission-180"><span class="linenos">180</span></a>    <span class="k">def</span> <span class="nf">link_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="PermissionLinker.link_permission-181"><a href="#PermissionLinker.link_permission-181"><span class="linenos">181</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="PermissionLinker.unlink_permission" class="classattr">
@@ -1481,16 +1691,16 @@
         <span class="def">def</span>
         <span class="name">unlink_permission</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">permissions</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="PermissionLinker.unlink_permission-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#PermissionLinker.unlink_permission"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker.unlink_permission-159"><a href="#PermissionLinker.unlink_permission-159"><span class="linenos">159</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
-</span><span id="PermissionLinker.unlink_permission-160"><a href="#PermissionLinker.unlink_permission-160"><span class="linenos">160</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="PermissionLinker.unlink_permission-183"><a href="#PermissionLinker.unlink_permission-183"><span class="linenos">183</span></a>    <span class="k">def</span> <span class="nf">unlink_permission</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">permissions</span><span class="p">):</span>
+</span><span id="PermissionLinker.unlink_permission-184"><a href="#PermissionLinker.unlink_permission-184"><span class="linenos">184</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;permission&#39;</span><span class="p">,</span> <span class="n">permissions</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1501,23 +1711,23 @@
     <span class="def">class</span>
     <span class="name">ProjectLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="ProjectLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProjectLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker-163"><a href="#ProjectLinker-163"><span class="linenos">163</span></a><span class="k">class</span> <span class="nc">ProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="ProjectLinker-164"><a href="#ProjectLinker-164"><span class="linenos">164</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Projects&quot;&quot;&quot;</span>
-</span><span id="ProjectLinker-165"><a href="#ProjectLinker-165"><span class="linenos">165</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;project&#39;</span>
-</span><span id="ProjectLinker-166"><a href="#ProjectLinker-166"><span class="linenos">166</span></a>
-</span><span id="ProjectLinker-167"><a href="#ProjectLinker-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="ProjectLinker-168"><a href="#ProjectLinker-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
-</span><span id="ProjectLinker-169"><a href="#ProjectLinker-169"><span class="linenos">169</span></a>
-</span><span id="ProjectLinker-170"><a href="#ProjectLinker-170"><span class="linenos">170</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="ProjectLinker-171"><a href="#ProjectLinker-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker-187"><a href="#ProjectLinker-187"><span class="linenos">187</span></a><span class="k">class</span> <span class="nc">ProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="ProjectLinker-188"><a href="#ProjectLinker-188"><span class="linenos">188</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Projects&quot;&quot;&quot;</span>
+</span><span id="ProjectLinker-189"><a href="#ProjectLinker-189"><span class="linenos">189</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;project&#39;</span>
+</span><span id="ProjectLinker-190"><a href="#ProjectLinker-190"><span class="linenos">190</span></a>
+</span><span id="ProjectLinker-191"><a href="#ProjectLinker-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="ProjectLinker-192"><a href="#ProjectLinker-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+</span><span id="ProjectLinker-193"><a href="#ProjectLinker-193"><span class="linenos">193</span></a>
+</span><span id="ProjectLinker-194"><a href="#ProjectLinker-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="ProjectLinker-195"><a href="#ProjectLinker-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Projects</p>
 </div>
 
 
@@ -1540,16 +1750,16 @@
         <span class="def">def</span>
         <span class="name">link_project</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">projects</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProjectLinker.link_project-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProjectLinker.link_project"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker.link_project-167"><a href="#ProjectLinker.link_project-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="ProjectLinker.link_project-168"><a href="#ProjectLinker.link_project-168"><span class="linenos">168</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker.link_project-191"><a href="#ProjectLinker.link_project-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">link_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="ProjectLinker.link_project-192"><a href="#ProjectLinker.link_project-192"><span class="linenos">192</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ProjectLinker.unlink_project" class="classattr">
@@ -1559,16 +1769,16 @@
         <span class="def">def</span>
         <span class="name">unlink_project</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">projects</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ProjectLinker.unlink_project-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ProjectLinker.unlink_project"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker.unlink_project-170"><a href="#ProjectLinker.unlink_project-170"><span class="linenos">170</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
-</span><span id="ProjectLinker.unlink_project-171"><a href="#ProjectLinker.unlink_project-171"><span class="linenos">171</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ProjectLinker.unlink_project-194"><a href="#ProjectLinker.unlink_project-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">unlink_project</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">projects</span><span class="p">):</span>
+</span><span id="ProjectLinker.unlink_project-195"><a href="#ProjectLinker.unlink_project-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;project&#39;</span><span class="p">,</span> <span class="n">projects</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1579,23 +1789,23 @@
     <span class="def">class</span>
     <span class="name">RebateLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="RebateLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#RebateLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker-174"><a href="#RebateLinker-174"><span class="linenos">174</span></a><span class="k">class</span> <span class="nc">RebateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="RebateLinker-175"><a href="#RebateLinker-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Rebates&quot;&quot;&quot;</span>
-</span><span id="RebateLinker-176"><a href="#RebateLinker-176"><span class="linenos">176</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;rebate&#39;</span>
-</span><span id="RebateLinker-177"><a href="#RebateLinker-177"><span class="linenos">177</span></a>
-</span><span id="RebateLinker-178"><a href="#RebateLinker-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="RebateLinker-179"><a href="#RebateLinker-179"><span class="linenos">179</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
-</span><span id="RebateLinker-180"><a href="#RebateLinker-180"><span class="linenos">180</span></a>
-</span><span id="RebateLinker-181"><a href="#RebateLinker-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="RebateLinker-182"><a href="#RebateLinker-182"><span class="linenos">182</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker-198"><a href="#RebateLinker-198"><span class="linenos">198</span></a><span class="k">class</span> <span class="nc">RebateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="RebateLinker-199"><a href="#RebateLinker-199"><span class="linenos">199</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Rebates&quot;&quot;&quot;</span>
+</span><span id="RebateLinker-200"><a href="#RebateLinker-200"><span class="linenos">200</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;rebate&#39;</span>
+</span><span id="RebateLinker-201"><a href="#RebateLinker-201"><span class="linenos">201</span></a>
+</span><span id="RebateLinker-202"><a href="#RebateLinker-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="RebateLinker-203"><a href="#RebateLinker-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
+</span><span id="RebateLinker-204"><a href="#RebateLinker-204"><span class="linenos">204</span></a>
+</span><span id="RebateLinker-205"><a href="#RebateLinker-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="RebateLinker-206"><a href="#RebateLinker-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Rebates</p>
 </div>
 
 
@@ -1618,16 +1828,16 @@
         <span class="def">def</span>
         <span class="name">link_rebate</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">rebates</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="RebateLinker.link_rebate-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#RebateLinker.link_rebate"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker.link_rebate-178"><a href="#RebateLinker.link_rebate-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="RebateLinker.link_rebate-179"><a href="#RebateLinker.link_rebate-179"><span class="linenos">179</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker.link_rebate-202"><a href="#RebateLinker.link_rebate-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">link_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="RebateLinker.link_rebate-203"><a href="#RebateLinker.link_rebate-203"><span class="linenos">203</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="RebateLinker.unlink_rebate" class="classattr">
@@ -1637,16 +1847,16 @@
         <span class="def">def</span>
         <span class="name">unlink_rebate</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">rebates</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="RebateLinker.unlink_rebate-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#RebateLinker.unlink_rebate"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker.unlink_rebate-181"><a href="#RebateLinker.unlink_rebate-181"><span class="linenos">181</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
-</span><span id="RebateLinker.unlink_rebate-182"><a href="#RebateLinker.unlink_rebate-182"><span class="linenos">182</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="RebateLinker.unlink_rebate-205"><a href="#RebateLinker.unlink_rebate-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">unlink_rebate</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rebates</span><span class="p">):</span>
+</span><span id="RebateLinker.unlink_rebate-206"><a href="#RebateLinker.unlink_rebate-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;rebate&#39;</span><span class="p">,</span> <span class="n">rebates</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1657,27 +1867,27 @@
     <span class="def">class</span>
     <span class="name">ResourceLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="ResourceLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ResourceLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker-185"><a href="#ResourceLinker-185"><span class="linenos">185</span></a><span class="k">class</span> <span class="nc">ResourceLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="ResourceLinker-186"><a href="#ResourceLinker-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Resources&quot;&quot;&quot;</span>
-</span><span id="ResourceLinker-187"><a href="#ResourceLinker-187"><span class="linenos">187</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;resource&#39;</span>
-</span><span id="ResourceLinker-188"><a href="#ResourceLinker-188"><span class="linenos">188</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
-</span><span id="ResourceLinker-189"><a href="#ResourceLinker-189"><span class="linenos">189</span></a>
-</span><span id="ResourceLinker-190"><a href="#ResourceLinker-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker-191"><a href="#ResourceLinker-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
-</span><span id="ResourceLinker-192"><a href="#ResourceLinker-192"><span class="linenos">192</span></a>
-</span><span id="ResourceLinker-193"><a href="#ResourceLinker-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker-194"><a href="#ResourceLinker-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
-</span><span id="ResourceLinker-195"><a href="#ResourceLinker-195"><span class="linenos">195</span></a>
-</span><span id="ResourceLinker-196"><a href="#ResourceLinker-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker-197"><a href="#ResourceLinker-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker-209"><a href="#ResourceLinker-209"><span class="linenos">209</span></a><span class="k">class</span> <span class="nc">ResourceLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="ResourceLinker-210"><a href="#ResourceLinker-210"><span class="linenos">210</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Resources&quot;&quot;&quot;</span>
+</span><span id="ResourceLinker-211"><a href="#ResourceLinker-211"><span class="linenos">211</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;resource&#39;</span>
+</span><span id="ResourceLinker-212"><a href="#ResourceLinker-212"><span class="linenos">212</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
+</span><span id="ResourceLinker-213"><a href="#ResourceLinker-213"><span class="linenos">213</span></a>
+</span><span id="ResourceLinker-214"><a href="#ResourceLinker-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker-215"><a href="#ResourceLinker-215"><span class="linenos">215</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+</span><span id="ResourceLinker-216"><a href="#ResourceLinker-216"><span class="linenos">216</span></a>
+</span><span id="ResourceLinker-217"><a href="#ResourceLinker-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker-218"><a href="#ResourceLinker-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+</span><span id="ResourceLinker-219"><a href="#ResourceLinker-219"><span class="linenos">219</span></a>
+</span><span id="ResourceLinker-220"><a href="#ResourceLinker-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker-221"><a href="#ResourceLinker-221"><span class="linenos">221</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Resources</p>
 </div>
 
 
@@ -1700,16 +1910,16 @@
         <span class="def">def</span>
         <span class="name">link_resource</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">resources</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ResourceLinker.link_resource-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ResourceLinker.link_resource"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.link_resource-190"><a href="#ResourceLinker.link_resource-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker.link_resource-191"><a href="#ResourceLinker.link_resource-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.link_resource-214"><a href="#ResourceLinker.link_resource-214"><span class="linenos">214</span></a>    <span class="k">def</span> <span class="nf">link_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker.link_resource-215"><a href="#ResourceLinker.link_resource-215"><span class="linenos">215</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ResourceLinker.relink_resource" class="classattr">
@@ -1719,16 +1929,16 @@
         <span class="def">def</span>
         <span class="name">relink_resource</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">resources</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ResourceLinker.relink_resource-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ResourceLinker.relink_resource"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.relink_resource-193"><a href="#ResourceLinker.relink_resource-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker.relink_resource-194"><a href="#ResourceLinker.relink_resource-194"><span class="linenos">194</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.relink_resource-217"><a href="#ResourceLinker.relink_resource-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">relink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker.relink_resource-218"><a href="#ResourceLinker.relink_resource-218"><span class="linenos">218</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="ResourceLinker.unlink_resource" class="classattr">
@@ -1738,16 +1948,16 @@
         <span class="def">def</span>
         <span class="name">unlink_resource</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">resources</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="ResourceLinker.unlink_resource-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#ResourceLinker.unlink_resource"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.unlink_resource-196"><a href="#ResourceLinker.unlink_resource-196"><span class="linenos">196</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
-</span><span id="ResourceLinker.unlink_resource-197"><a href="#ResourceLinker.unlink_resource-197"><span class="linenos">197</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="ResourceLinker.unlink_resource-220"><a href="#ResourceLinker.unlink_resource-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">unlink_resource</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">resources</span><span class="p">):</span>
+</span><span id="ResourceLinker.unlink_resource-221"><a href="#ResourceLinker.unlink_resource-221"><span class="linenos">221</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;resource&#39;</span><span class="p">,</span> <span class="n">resources</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1758,27 +1968,27 @@
     <span class="def">class</span>
     <span class="name">SkillLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="SkillLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#SkillLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker-200"><a href="#SkillLinker-200"><span class="linenos">200</span></a><span class="k">class</span> <span class="nc">SkillLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="SkillLinker-201"><a href="#SkillLinker-201"><span class="linenos">201</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Skills&quot;&quot;&quot;</span>
-</span><span id="SkillLinker-202"><a href="#SkillLinker-202"><span class="linenos">202</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
-</span><span id="SkillLinker-203"><a href="#SkillLinker-203"><span class="linenos">203</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;skillLink&#39;</span>
-</span><span id="SkillLinker-204"><a href="#SkillLinker-204"><span class="linenos">204</span></a>
-</span><span id="SkillLinker-205"><a href="#SkillLinker-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker-206"><a href="#SkillLinker-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
-</span><span id="SkillLinker-207"><a href="#SkillLinker-207"><span class="linenos">207</span></a>
-</span><span id="SkillLinker-208"><a href="#SkillLinker-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker-209"><a href="#SkillLinker-209"><span class="linenos">209</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
-</span><span id="SkillLinker-210"><a href="#SkillLinker-210"><span class="linenos">210</span></a>
-</span><span id="SkillLinker-211"><a href="#SkillLinker-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker-212"><a href="#SkillLinker-212"><span class="linenos">212</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker-224"><a href="#SkillLinker-224"><span class="linenos">224</span></a><span class="k">class</span> <span class="nc">SkillLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="SkillLinker-225"><a href="#SkillLinker-225"><span class="linenos">225</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Skills&quot;&quot;&quot;</span>
+</span><span id="SkillLinker-226"><a href="#SkillLinker-226"><span class="linenos">226</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;skill&#39;</span>
+</span><span id="SkillLinker-227"><a href="#SkillLinker-227"><span class="linenos">227</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;skillLink&#39;</span>
+</span><span id="SkillLinker-228"><a href="#SkillLinker-228"><span class="linenos">228</span></a>
+</span><span id="SkillLinker-229"><a href="#SkillLinker-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker-230"><a href="#SkillLinker-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="SkillLinker-231"><a href="#SkillLinker-231"><span class="linenos">231</span></a>
+</span><span id="SkillLinker-232"><a href="#SkillLinker-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker-233"><a href="#SkillLinker-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+</span><span id="SkillLinker-234"><a href="#SkillLinker-234"><span class="linenos">234</span></a>
+</span><span id="SkillLinker-235"><a href="#SkillLinker-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker-236"><a href="#SkillLinker-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Skills</p>
 </div>
 
 
@@ -1801,16 +2011,16 @@
         <span class="def">def</span>
         <span class="name">link_skill</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">skills</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="SkillLinker.link_skill-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#SkillLinker.link_skill"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.link_skill-205"><a href="#SkillLinker.link_skill-205"><span class="linenos">205</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker.link_skill-206"><a href="#SkillLinker.link_skill-206"><span class="linenos">206</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.link_skill-229"><a href="#SkillLinker.link_skill-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">link_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker.link_skill-230"><a href="#SkillLinker.link_skill-230"><span class="linenos">230</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="SkillLinker.relink_skill" class="classattr">
@@ -1820,16 +2030,16 @@
         <span class="def">def</span>
         <span class="name">relink_skill</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">skills</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="SkillLinker.relink_skill-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#SkillLinker.relink_skill"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.relink_skill-208"><a href="#SkillLinker.relink_skill-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker.relink_skill-209"><a href="#SkillLinker.relink_skill-209"><span class="linenos">209</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.relink_skill-232"><a href="#SkillLinker.relink_skill-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">relink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker.relink_skill-233"><a href="#SkillLinker.relink_skill-233"><span class="linenos">233</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="SkillLinker.unlink_skill" class="classattr">
@@ -1839,16 +2049,16 @@
         <span class="def">def</span>
         <span class="name">unlink_skill</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">skills</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="SkillLinker.unlink_skill-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#SkillLinker.unlink_skill"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.unlink_skill-211"><a href="#SkillLinker.unlink_skill-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
-</span><span id="SkillLinker.unlink_skill-212"><a href="#SkillLinker.unlink_skill-212"><span class="linenos">212</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="SkillLinker.unlink_skill-235"><a href="#SkillLinker.unlink_skill-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">unlink_skill</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">skills</span><span class="p">):</span>
+</span><span id="SkillLinker.unlink_skill-236"><a href="#SkillLinker.unlink_skill-236"><span class="linenos">236</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;skill&#39;</span><span class="p">,</span> <span class="n">skills</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1859,27 +2069,27 @@
     <span class="def">class</span>
     <span class="name">StaffLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="StaffLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StaffLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker-215"><a href="#StaffLinker-215"><span class="linenos">215</span></a><span class="k">class</span> <span class="nc">StaffLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="StaffLinker-216"><a href="#StaffLinker-216"><span class="linenos">216</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Staff&quot;&quot;&quot;</span>
-</span><span id="StaffLinker-217"><a href="#StaffLinker-217"><span class="linenos">217</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;staff&#39;</span>
-</span><span id="StaffLinker-218"><a href="#StaffLinker-218"><span class="linenos">218</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
-</span><span id="StaffLinker-219"><a href="#StaffLinker-219"><span class="linenos">219</span></a>
-</span><span id="StaffLinker-220"><a href="#StaffLinker-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker-221"><a href="#StaffLinker-221"><span class="linenos">221</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
-</span><span id="StaffLinker-222"><a href="#StaffLinker-222"><span class="linenos">222</span></a>
-</span><span id="StaffLinker-223"><a href="#StaffLinker-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker-224"><a href="#StaffLinker-224"><span class="linenos">224</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
-</span><span id="StaffLinker-225"><a href="#StaffLinker-225"><span class="linenos">225</span></a>
-</span><span id="StaffLinker-226"><a href="#StaffLinker-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker-227"><a href="#StaffLinker-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker-239"><a href="#StaffLinker-239"><span class="linenos">239</span></a><span class="k">class</span> <span class="nc">StaffLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="StaffLinker-240"><a href="#StaffLinker-240"><span class="linenos">240</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Staff&quot;&quot;&quot;</span>
+</span><span id="StaffLinker-241"><a href="#StaffLinker-241"><span class="linenos">241</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;staff&#39;</span>
+</span><span id="StaffLinker-242"><a href="#StaffLinker-242"><span class="linenos">242</span></a>    <span class="n">_link_data_name</span> <span class="o">=</span> <span class="s1">&#39;resourceLink&#39;</span>
+</span><span id="StaffLinker-243"><a href="#StaffLinker-243"><span class="linenos">243</span></a>
+</span><span id="StaffLinker-244"><a href="#StaffLinker-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker-245"><a href="#StaffLinker-245"><span class="linenos">245</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="StaffLinker-246"><a href="#StaffLinker-246"><span class="linenos">246</span></a>
+</span><span id="StaffLinker-247"><a href="#StaffLinker-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker-248"><a href="#StaffLinker-248"><span class="linenos">248</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+</span><span id="StaffLinker-249"><a href="#StaffLinker-249"><span class="linenos">249</span></a>
+</span><span id="StaffLinker-250"><a href="#StaffLinker-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker-251"><a href="#StaffLinker-251"><span class="linenos">251</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Staff</p>
 </div>
 
 
@@ -1902,16 +2112,16 @@
         <span class="def">def</span>
         <span class="name">link_staff</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">staffs</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StaffLinker.link_staff-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StaffLinker.link_staff"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.link_staff-220"><a href="#StaffLinker.link_staff-220"><span class="linenos">220</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker.link_staff-221"><a href="#StaffLinker.link_staff-221"><span class="linenos">221</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.link_staff-244"><a href="#StaffLinker.link_staff-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">link_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker.link_staff-245"><a href="#StaffLinker.link_staff-245"><span class="linenos">245</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="StaffLinker.relink_staff" class="classattr">
@@ -1921,16 +2131,16 @@
         <span class="def">def</span>
         <span class="name">relink_staff</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">staffs</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StaffLinker.relink_staff-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StaffLinker.relink_staff"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.relink_staff-223"><a href="#StaffLinker.relink_staff-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker.relink_staff-224"><a href="#StaffLinker.relink_staff-224"><span class="linenos">224</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.relink_staff-247"><a href="#StaffLinker.relink_staff-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">relink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker.relink_staff-248"><a href="#StaffLinker.relink_staff-248"><span class="linenos">248</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_update_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="StaffLinker.unlink_staff" class="classattr">
@@ -1940,16 +2150,16 @@
         <span class="def">def</span>
         <span class="name">unlink_staff</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">staffs</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StaffLinker.unlink_staff-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StaffLinker.unlink_staff"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.unlink_staff-226"><a href="#StaffLinker.unlink_staff-226"><span class="linenos">226</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
-</span><span id="StaffLinker.unlink_staff-227"><a href="#StaffLinker.unlink_staff-227"><span class="linenos">227</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StaffLinker.unlink_staff-250"><a href="#StaffLinker.unlink_staff-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">unlink_staff</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">staffs</span><span class="p">):</span>
+</span><span id="StaffLinker.unlink_staff-251"><a href="#StaffLinker.unlink_staff-251"><span class="linenos">251</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;staff&#39;</span><span class="p">,</span> <span class="n">staffs</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -1960,25 +2170,25 @@
     <span class="def">class</span>
     <span class="name">StageLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="StageLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker-230"><a href="#StageLinker-230"><span class="linenos">230</span></a><span class="k">class</span> <span class="nc">StageLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="StageLinker-231"><a href="#StageLinker-231"><span class="linenos">231</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stages&quot;&quot;&quot;</span>
-</span><span id="StageLinker-232"><a href="#StageLinker-232"><span class="linenos">232</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="StageLinker-233"><a href="#StageLinker-233"><span class="linenos">233</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
-</span><span id="StageLinker-234"><a href="#StageLinker-234"><span class="linenos">234</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">dict</span>
-</span><span id="StageLinker-235"><a href="#StageLinker-235"><span class="linenos">235</span></a>
-</span><span id="StageLinker-236"><a href="#StageLinker-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageLinker-237"><a href="#StageLinker-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
-</span><span id="StageLinker-238"><a href="#StageLinker-238"><span class="linenos">238</span></a>
-</span><span id="StageLinker-239"><a href="#StageLinker-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageLinker-240"><a href="#StageLinker-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker-254"><a href="#StageLinker-254"><span class="linenos">254</span></a><span class="k">class</span> <span class="nc">StageLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="StageLinker-255"><a href="#StageLinker-255"><span class="linenos">255</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stages&quot;&quot;&quot;</span>
+</span><span id="StageLinker-256"><a href="#StageLinker-256"><span class="linenos">256</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="StageLinker-257"><a href="#StageLinker-257"><span class="linenos">257</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stage&#39;</span>
+</span><span id="StageLinker-258"><a href="#StageLinker-258"><span class="linenos">258</span></a>    <span class="n">_link_type</span> <span class="o">=</span> <span class="nb">dict</span>
+</span><span id="StageLinker-259"><a href="#StageLinker-259"><span class="linenos">259</span></a>
+</span><span id="StageLinker-260"><a href="#StageLinker-260"><span class="linenos">260</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageLinker-261"><a href="#StageLinker-261"><span class="linenos">261</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="StageLinker-262"><a href="#StageLinker-262"><span class="linenos">262</span></a>
+</span><span id="StageLinker-263"><a href="#StageLinker-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageLinker-264"><a href="#StageLinker-264"><span class="linenos">264</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Stages</p>
 </div>
 
 
@@ -2001,16 +2211,16 @@
         <span class="def">def</span>
         <span class="name">link_stage</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">stages</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StageLinker.link_stage-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageLinker.link_stage"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker.link_stage-236"><a href="#StageLinker.link_stage-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageLinker.link_stage-237"><a href="#StageLinker.link_stage-237"><span class="linenos">237</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker.link_stage-260"><a href="#StageLinker.link_stage-260"><span class="linenos">260</span></a>    <span class="k">def</span> <span class="nf">link_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageLinker.link_stage-261"><a href="#StageLinker.link_stage-261"><span class="linenos">261</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="StageLinker.unlink_stage" class="classattr">
@@ -2020,16 +2230,16 @@
         <span class="def">def</span>
         <span class="name">unlink_stage</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">stages</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StageLinker.unlink_stage-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageLinker.unlink_stage"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker.unlink_stage-239"><a href="#StageLinker.unlink_stage-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageLinker.unlink_stage-240"><a href="#StageLinker.unlink_stage-240"><span class="linenos">240</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageLinker.unlink_stage-263"><a href="#StageLinker.unlink_stage-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">unlink_stage</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageLinker.unlink_stage-264"><a href="#StageLinker.unlink_stage-264"><span class="linenos">264</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2040,30 +2250,30 @@
     <span class="def">class</span>
     <span class="name">StageListLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="StageListLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageListLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker-243"><a href="#StageListLinker-243"><span class="linenos">243</span></a><span class="k">class</span> <span class="nc">StageListLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="StageListLinker-244"><a href="#StageListLinker-244"><span class="linenos">244</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stage List&quot;&quot;&quot;</span>
-</span><span id="StageListLinker-245"><a href="#StageListLinker-245"><span class="linenos">245</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage_list&#39;</span>
-</span><span id="StageListLinker-246"><a href="#StageListLinker-246"><span class="linenos">246</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stageList&#39;</span>
-</span><span id="StageListLinker-247"><a href="#StageListLinker-247"><span class="linenos">247</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;Stage&#39;</span>
-</span><span id="StageListLinker-248"><a href="#StageListLinker-248"><span class="linenos">248</span></a>
-</span><span id="StageListLinker-249"><a href="#StageListLinker-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageListLinker-250"><a href="#StageListLinker-250"><span class="linenos">250</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="StageListLinker-251"><a href="#StageListLinker-251"><span class="linenos">251</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
-</span><span id="StageListLinker-252"><a href="#StageListLinker-252"><span class="linenos">252</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
-</span><span id="StageListLinker-253"><a href="#StageListLinker-253"><span class="linenos">253</span></a>
-</span><span id="StageListLinker-254"><a href="#StageListLinker-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageListLinker-255"><a href="#StageListLinker-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="StageListLinker-256"><a href="#StageListLinker-256"><span class="linenos">256</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
-</span><span id="StageListLinker-257"><a href="#StageListLinker-257"><span class="linenos">257</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
-</span><span id="StageListLinker-258"><a href="#StageListLinker-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker-267"><a href="#StageListLinker-267"><span class="linenos">267</span></a><span class="k">class</span> <span class="nc">StageListLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="StageListLinker-268"><a href="#StageListLinker-268"><span class="linenos">268</span></a>    <span class="sd">&quot;&quot;&quot;Subclass can link to Stage List&quot;&quot;&quot;</span>
+</span><span id="StageListLinker-269"><a href="#StageListLinker-269"><span class="linenos">269</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;stage_list&#39;</span>
+</span><span id="StageListLinker-270"><a href="#StageListLinker-270"><span class="linenos">270</span></a>    <span class="n">_link_key</span> <span class="o">=</span> <span class="s1">&#39;stageList&#39;</span>
+</span><span id="StageListLinker-271"><a href="#StageListLinker-271"><span class="linenos">271</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;Stage&#39;</span>
+</span><span id="StageListLinker-272"><a href="#StageListLinker-272"><span class="linenos">272</span></a>
+</span><span id="StageListLinker-273"><a href="#StageListLinker-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageListLinker-274"><a href="#StageListLinker-274"><span class="linenos">274</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="StageListLinker-275"><a href="#StageListLinker-275"><span class="linenos">275</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
+</span><span id="StageListLinker-276"><a href="#StageListLinker-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+</span><span id="StageListLinker-277"><a href="#StageListLinker-277"><span class="linenos">277</span></a>
+</span><span id="StageListLinker-278"><a href="#StageListLinker-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageListLinker-279"><a href="#StageListLinker-279"><span class="linenos">279</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="StageListLinker-280"><a href="#StageListLinker-280"><span class="linenos">280</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
+</span><span id="StageListLinker-281"><a href="#StageListLinker-281"><span class="linenos">281</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
+</span><span id="StageListLinker-282"><a href="#StageListLinker-282"><span class="linenos">282</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass can link to Stage List</p>
 </div>
 
 
@@ -2086,18 +2296,18 @@
         <span class="def">def</span>
         <span class="name">link_stage_list</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">stages</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StageListLinker.link_stage_list-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageListLinker.link_stage_list"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker.link_stage_list-249"><a href="#StageListLinker.link_stage_list-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageListLinker.link_stage_list-250"><a href="#StageListLinker.link_stage_list-250"><span class="linenos">250</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="StageListLinker.link_stage_list-251"><a href="#StageListLinker.link_stage_list-251"><span class="linenos">251</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
-</span><span id="StageListLinker.link_stage_list-252"><a href="#StageListLinker.link_stage_list-252"><span class="linenos">252</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker.link_stage_list-273"><a href="#StageListLinker.link_stage_list-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">link_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageListLinker.link_stage_list-274"><a href="#StageListLinker.link_stage_list-274"><span class="linenos">274</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="StageListLinker.link_stage_list-275"><a href="#StageListLinker.link_stage_list-275"><span class="linenos">275</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list link must be a list&#39;</span><span class="p">)</span>
+</span><span id="StageListLinker.link_stage_list-276"><a href="#StageListLinker.link_stage_list-276"><span class="linenos">276</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="StageListLinker.unlink_stage_list" class="classattr">
@@ -2107,19 +2317,19 @@
         <span class="def">def</span>
         <span class="name">unlink_stage_list</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">stages</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="StageListLinker.unlink_stage_list-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#StageListLinker.unlink_stage_list"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker.unlink_stage_list-254"><a href="#StageListLinker.unlink_stage_list-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
-</span><span id="StageListLinker.unlink_stage_list-255"><a href="#StageListLinker.unlink_stage_list-255"><span class="linenos">255</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
-</span><span id="StageListLinker.unlink_stage_list-256"><a href="#StageListLinker.unlink_stage_list-256"><span class="linenos">256</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
-</span><span id="StageListLinker.unlink_stage_list-257"><a href="#StageListLinker.unlink_stage_list-257"><span class="linenos">257</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
-</span><span id="StageListLinker.unlink_stage_list-258"><a href="#StageListLinker.unlink_stage_list-258"><span class="linenos">258</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="StageListLinker.unlink_stage_list-278"><a href="#StageListLinker.unlink_stage_list-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">unlink_stage_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">stages</span><span class="p">):</span>
+</span><span id="StageListLinker.unlink_stage_list-279"><a href="#StageListLinker.unlink_stage_list-279"><span class="linenos">279</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">stages</span><span class="p">,</span> <span class="nb">list</span><span class="p">):</span>
+</span><span id="StageListLinker.unlink_stage_list-280"><a href="#StageListLinker.unlink_stage_list-280"><span class="linenos">280</span></a>            <span class="k">raise</span> <span class="n">api</span><span class="o">.</span><span class="n">UsageException</span><span class="p">(</span><span class="s1">&#39;Stage list unlink must be a list&#39;</span><span class="p">)</span>
+</span><span id="StageListLinker.unlink_stage_list-281"><a href="#StageListLinker.unlink_stage_list-281"><span class="linenos">281</span></a>        <span class="n">stages</span> <span class="o">=</span> <span class="p">[{</span><span class="s1">&#39;uuId&#39;</span><span class="p">:</span> <span class="n">s</span><span class="p">[</span><span class="s1">&#39;uuId&#39;</span><span class="p">]}</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">stages</span><span class="p">]</span>
+</span><span id="StageListLinker.unlink_stage_list-282"><a href="#StageListLinker.unlink_stage_list-282"><span class="linenos">282</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;stage_list&#39;</span><span class="p">,</span> <span class="n">stages</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2130,22 +2340,22 @@
     <span class="def">class</span>
     <span class="name">UserLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="UserLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#UserLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker-261"><a href="#UserLinker-261"><span class="linenos">261</span></a><span class="k">class</span> <span class="nc">UserLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="UserLinker-262"><a href="#UserLinker-262"><span class="linenos">262</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;user&#39;</span>
-</span><span id="UserLinker-263"><a href="#UserLinker-263"><span class="linenos">263</span></a>
-</span><span id="UserLinker-264"><a href="#UserLinker-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="UserLinker-265"><a href="#UserLinker-265"><span class="linenos">265</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
-</span><span id="UserLinker-266"><a href="#UserLinker-266"><span class="linenos">266</span></a>
-</span><span id="UserLinker-267"><a href="#UserLinker-267"><span class="linenos">267</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="UserLinker-268"><a href="#UserLinker-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker-285"><a href="#UserLinker-285"><span class="linenos">285</span></a><span class="k">class</span> <span class="nc">UserLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="UserLinker-286"><a href="#UserLinker-286"><span class="linenos">286</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;user&#39;</span>
+</span><span id="UserLinker-287"><a href="#UserLinker-287"><span class="linenos">287</span></a>
+</span><span id="UserLinker-288"><a href="#UserLinker-288"><span class="linenos">288</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="UserLinker-289"><a href="#UserLinker-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
+</span><span id="UserLinker-290"><a href="#UserLinker-290"><span class="linenos">290</span></a>
+</span><span id="UserLinker-291"><a href="#UserLinker-291"><span class="linenos">291</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="UserLinker-292"><a href="#UserLinker-292"><span class="linenos">292</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="UserLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2166,16 +2376,16 @@
         <span class="def">def</span>
         <span class="name">link_user</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">users</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="UserLinker.link_user-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#UserLinker.link_user"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker.link_user-264"><a href="#UserLinker.link_user-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="UserLinker.link_user-265"><a href="#UserLinker.link_user-265"><span class="linenos">265</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker.link_user-288"><a href="#UserLinker.link_user-288"><span class="linenos">288</span></a>    <span class="k">def</span> <span class="nf">link_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="UserLinker.link_user-289"><a href="#UserLinker.link_user-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="UserLinker.unlink_user" class="classattr">
@@ -2185,16 +2395,16 @@
         <span class="def">def</span>
         <span class="name">unlink_user</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">users</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="UserLinker.unlink_user-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#UserLinker.unlink_user"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker.unlink_user-267"><a href="#UserLinker.unlink_user-267"><span class="linenos">267</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
-</span><span id="UserLinker.unlink_user-268"><a href="#UserLinker.unlink_user-268"><span class="linenos">268</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="UserLinker.unlink_user-291"><a href="#UserLinker.unlink_user-291"><span class="linenos">291</span></a>    <span class="k">def</span> <span class="nf">unlink_user</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">users</span><span class="p">):</span>
+</span><span id="UserLinker.unlink_user-292"><a href="#UserLinker.unlink_user-292"><span class="linenos">292</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;user&#39;</span><span class="p">,</span> <span class="n">users</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2205,22 +2415,22 @@
     <span class="def">class</span>
     <span class="name">TaskLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="TaskLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker-271"><a href="#TaskLinker-271"><span class="linenos">271</span></a><span class="k">class</span> <span class="nc">TaskLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="TaskLinker-272"><a href="#TaskLinker-272"><span class="linenos">272</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task&#39;</span>
-</span><span id="TaskLinker-273"><a href="#TaskLinker-273"><span class="linenos">273</span></a>
-</span><span id="TaskLinker-274"><a href="#TaskLinker-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="TaskLinker-275"><a href="#TaskLinker-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
-</span><span id="TaskLinker-276"><a href="#TaskLinker-276"><span class="linenos">276</span></a>
-</span><span id="TaskLinker-277"><a href="#TaskLinker-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="TaskLinker-278"><a href="#TaskLinker-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker-295"><a href="#TaskLinker-295"><span class="linenos">295</span></a><span class="k">class</span> <span class="nc">TaskLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="TaskLinker-296"><a href="#TaskLinker-296"><span class="linenos">296</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task&#39;</span>
+</span><span id="TaskLinker-297"><a href="#TaskLinker-297"><span class="linenos">297</span></a>
+</span><span id="TaskLinker-298"><a href="#TaskLinker-298"><span class="linenos">298</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="TaskLinker-299"><a href="#TaskLinker-299"><span class="linenos">299</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+</span><span id="TaskLinker-300"><a href="#TaskLinker-300"><span class="linenos">300</span></a>
+</span><span id="TaskLinker-301"><a href="#TaskLinker-301"><span class="linenos">301</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="TaskLinker-302"><a href="#TaskLinker-302"><span class="linenos">302</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="TaskLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2241,16 +2451,16 @@
         <span class="def">def</span>
         <span class="name">link_task</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tasks</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TaskLinker.link_task-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskLinker.link_task"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker.link_task-274"><a href="#TaskLinker.link_task-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="TaskLinker.link_task-275"><a href="#TaskLinker.link_task-275"><span class="linenos">275</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker.link_task-298"><a href="#TaskLinker.link_task-298"><span class="linenos">298</span></a>    <span class="k">def</span> <span class="nf">link_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="TaskLinker.link_task-299"><a href="#TaskLinker.link_task-299"><span class="linenos">299</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="TaskLinker.unlink_task" class="classattr">
@@ -2260,16 +2470,16 @@
         <span class="def">def</span>
         <span class="name">unlink_task</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tasks</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TaskLinker.unlink_task-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskLinker.unlink_task"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker.unlink_task-277"><a href="#TaskLinker.unlink_task-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
-</span><span id="TaskLinker.unlink_task-278"><a href="#TaskLinker.unlink_task-278"><span class="linenos">278</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskLinker.unlink_task-301"><a href="#TaskLinker.unlink_task-301"><span class="linenos">301</span></a>    <span class="k">def</span> <span class="nf">unlink_task</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tasks</span><span class="p">):</span>
+</span><span id="TaskLinker.unlink_task-302"><a href="#TaskLinker.unlink_task-302"><span class="linenos">302</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task&#39;</span><span class="p">,</span> <span class="n">tasks</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2280,23 +2490,23 @@
     <span class="def">class</span>
     <span class="name">TaskTemplateLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="TaskTemplateLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskTemplateLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker-281"><a href="#TaskTemplateLinker-281"><span class="linenos">281</span></a><span class="k">class</span> <span class="nc">TaskTemplateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="TaskTemplateLinker-282"><a href="#TaskTemplateLinker-282"><span class="linenos">282</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task_template&#39;</span>
-</span><span id="TaskTemplateLinker-283"><a href="#TaskTemplateLinker-283"><span class="linenos">283</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;TaskTemplate&#39;</span>
-</span><span id="TaskTemplateLinker-284"><a href="#TaskTemplateLinker-284"><span class="linenos">284</span></a>
-</span><span id="TaskTemplateLinker-285"><a href="#TaskTemplateLinker-285"><span class="linenos">285</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="TaskTemplateLinker-286"><a href="#TaskTemplateLinker-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
-</span><span id="TaskTemplateLinker-287"><a href="#TaskTemplateLinker-287"><span class="linenos">287</span></a>
-</span><span id="TaskTemplateLinker-288"><a href="#TaskTemplateLinker-288"><span class="linenos">288</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="TaskTemplateLinker-289"><a href="#TaskTemplateLinker-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker-305"><a href="#TaskTemplateLinker-305"><span class="linenos">305</span></a><span class="k">class</span> <span class="nc">TaskTemplateLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="TaskTemplateLinker-306"><a href="#TaskTemplateLinker-306"><span class="linenos">306</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;task_template&#39;</span>
+</span><span id="TaskTemplateLinker-307"><a href="#TaskTemplateLinker-307"><span class="linenos">307</span></a>    <span class="n">_link_entity</span> <span class="o">=</span> <span class="s1">&#39;TaskTemplate&#39;</span>
+</span><span id="TaskTemplateLinker-308"><a href="#TaskTemplateLinker-308"><span class="linenos">308</span></a>
+</span><span id="TaskTemplateLinker-309"><a href="#TaskTemplateLinker-309"><span class="linenos">309</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="TaskTemplateLinker-310"><a href="#TaskTemplateLinker-310"><span class="linenos">310</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+</span><span id="TaskTemplateLinker-311"><a href="#TaskTemplateLinker-311"><span class="linenos">311</span></a>
+</span><span id="TaskTemplateLinker-312"><a href="#TaskTemplateLinker-312"><span class="linenos">312</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="TaskTemplateLinker-313"><a href="#TaskTemplateLinker-313"><span class="linenos">313</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="TaskTemplateLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2317,16 +2527,16 @@
         <span class="def">def</span>
         <span class="name">link_task_template</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">task_templates</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TaskTemplateLinker.link_task_template-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskTemplateLinker.link_task_template"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker.link_task_template-285"><a href="#TaskTemplateLinker.link_task_template-285"><span class="linenos">285</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="TaskTemplateLinker.link_task_template-286"><a href="#TaskTemplateLinker.link_task_template-286"><span class="linenos">286</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker.link_task_template-309"><a href="#TaskTemplateLinker.link_task_template-309"><span class="linenos">309</span></a>    <span class="k">def</span> <span class="nf">link_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="TaskTemplateLinker.link_task_template-310"><a href="#TaskTemplateLinker.link_task_template-310"><span class="linenos">310</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="TaskTemplateLinker.unlink_task_template" class="classattr">
@@ -2336,16 +2546,16 @@
         <span class="def">def</span>
         <span class="name">unlink_task_template</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">task_templates</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TaskTemplateLinker.unlink_task_template-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskTemplateLinker.unlink_task_template"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker.unlink_task_template-288"><a href="#TaskTemplateLinker.unlink_task_template-288"><span class="linenos">288</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
-</span><span id="TaskTemplateLinker.unlink_task_template-289"><a href="#TaskTemplateLinker.unlink_task_template-289"><span class="linenos">289</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskTemplateLinker.unlink_task_template-312"><a href="#TaskTemplateLinker.unlink_task_template-312"><span class="linenos">312</span></a>    <span class="k">def</span> <span class="nf">unlink_task_template</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">):</span>
+</span><span id="TaskTemplateLinker.unlink_task_template-313"><a href="#TaskTemplateLinker.unlink_task_template-313"><span class="linenos">313</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;task_template&#39;</span><span class="p">,</span> <span class="n">task_templates</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2356,22 +2566,22 @@
     <span class="def">class</span>
     <span class="name">TagLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="TagLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TagLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker-291"><a href="#TagLinker-291"><span class="linenos">291</span></a><span class="k">class</span> <span class="nc">TagLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="TagLinker-292"><a href="#TagLinker-292"><span class="linenos">292</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
-</span><span id="TagLinker-293"><a href="#TagLinker-293"><span class="linenos">293</span></a>
-</span><span id="TagLinker-294"><a href="#TagLinker-294"><span class="linenos">294</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="TagLinker-295"><a href="#TagLinker-295"><span class="linenos">295</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
-</span><span id="TagLinker-296"><a href="#TagLinker-296"><span class="linenos">296</span></a>
-</span><span id="TagLinker-297"><a href="#TagLinker-297"><span class="linenos">297</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="TagLinker-298"><a href="#TagLinker-298"><span class="linenos">298</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker-315"><a href="#TagLinker-315"><span class="linenos">315</span></a><span class="k">class</span> <span class="nc">TagLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="TagLinker-316"><a href="#TagLinker-316"><span class="linenos">316</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;tag&#39;</span>
+</span><span id="TagLinker-317"><a href="#TagLinker-317"><span class="linenos">317</span></a>
+</span><span id="TagLinker-318"><a href="#TagLinker-318"><span class="linenos">318</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="TagLinker-319"><a href="#TagLinker-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+</span><span id="TagLinker-320"><a href="#TagLinker-320"><span class="linenos">320</span></a>
+</span><span id="TagLinker-321"><a href="#TagLinker-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="TagLinker-322"><a href="#TagLinker-322"><span class="linenos">322</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             <div id="TagLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2392,16 +2602,16 @@
         <span class="def">def</span>
         <span class="name">link_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tags</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TagLinker.link_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TagLinker.link_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker.link_tag-294"><a href="#TagLinker.link_tag-294"><span class="linenos">294</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="TagLinker.link_tag-295"><a href="#TagLinker.link_tag-295"><span class="linenos">295</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker.link_tag-318"><a href="#TagLinker.link_tag-318"><span class="linenos">318</span></a>    <span class="k">def</span> <span class="nf">link_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="TagLinker.link_tag-319"><a href="#TagLinker.link_tag-319"><span class="linenos">319</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_add_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                             <div id="TagLinker.unlink_tag" class="classattr">
@@ -2411,16 +2621,16 @@
         <span class="def">def</span>
         <span class="name">unlink_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tags</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="TagLinker.unlink_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TagLinker.unlink_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker.unlink_tag-297"><a href="#TagLinker.unlink_tag-297"><span class="linenos">297</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
-</span><span id="TagLinker.unlink_tag-298"><a href="#TagLinker.unlink_tag-298"><span class="linenos">298</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TagLinker.unlink_tag-321"><a href="#TagLinker.unlink_tag-321"><span class="linenos">321</span></a>    <span class="k">def</span> <span class="nf">unlink_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tags</span><span class="p">):</span>
+</span><span id="TagLinker.unlink_tag-322"><a href="#TagLinker.unlink_tag-322"><span class="linenos">322</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">_delete_link</span><span class="p">(</span><span class="s1">&#39;tag&#39;</span><span class="p">,</span> <span class="n">tags</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                             </div>
                 </section>
@@ -2431,16 +2641,16 @@
     <span class="def">class</span>
     <span class="name">NoteLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="NoteLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#NoteLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="NoteLinker-300"><a href="#NoteLinker-300"><span class="linenos">300</span></a><span class="k">class</span> <span class="nc">NoteLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="NoteLinker-301"><a href="#NoteLinker-301"><span class="linenos">301</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;note&#39;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="NoteLinker-324"><a href="#NoteLinker-324"><span class="linenos">324</span></a><span class="k">class</span> <span class="nc">NoteLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="NoteLinker-325"><a href="#NoteLinker-325"><span class="linenos">325</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;note&#39;</span>
 </span></pre></div>
 
 
     
 
                             <div id="NoteLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2462,16 +2672,16 @@
     <span class="def">class</span>
     <span class="name">CalendarLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="CalendarLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#CalendarLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="CalendarLinker-303"><a href="#CalendarLinker-303"><span class="linenos">303</span></a><span class="k">class</span> <span class="nc">CalendarLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="CalendarLinker-304"><a href="#CalendarLinker-304"><span class="linenos">304</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;calendar&#39;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="CalendarLinker-327"><a href="#CalendarLinker-327"><span class="linenos">327</span></a><span class="k">class</span> <span class="nc">CalendarLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="CalendarLinker-328"><a href="#CalendarLinker-328"><span class="linenos">328</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s1">&#39;calendar&#39;</span>
 </span></pre></div>
 
 
     
 
                             <div id="CalendarLinker.__init__" class="classattr">
                                 <div class="attr function">
@@ -2493,16 +2703,16 @@
     <span class="def">class</span>
     <span class="name">TaskInProjectLinker</span><wbr>(<span class="base"><a href="#BaseLinker">BaseLinker</a></span>):
 
                 <label class="view-source-button" for="TaskInProjectLinker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#TaskInProjectLinker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskInProjectLinker-308"><a href="#TaskInProjectLinker-308"><span class="linenos">308</span></a><span class="k">class</span> <span class="nc">TaskInProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
-</span><span id="TaskInProjectLinker-309"><a href="#TaskInProjectLinker-309"><span class="linenos">309</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s2">&quot;task&quot;</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="TaskInProjectLinker-332"><a href="#TaskInProjectLinker-332"><span class="linenos">332</span></a><span class="k">class</span> <span class="nc">TaskInProjectLinker</span><span class="p">(</span><span class="n">BaseLinker</span><span class="p">):</span>
+</span><span id="TaskInProjectLinker-333"><a href="#TaskInProjectLinker-333"><span class="linenos">333</span></a>    <span class="n">_link_name</span> <span class="o">=</span> <span class="s2">&quot;task&quot;</span>
 </span></pre></div>
 
 
     
 
                             <div id="TaskInProjectLinker.__init__" class="classattr">
                                 <div class="attr function">
```

#### html2text {}

```diff
@@ -5,14 +5,22 @@
 ***** API Documentation *****
     * BaseLinker
           o BaseLinker
     * AccessPolicyLinker
           o AccessPolicyLinker
           o link_access_policy
           o unlink_access_policy
+    * ActivityLinker
+          o ActivityLinker
+          o link_activity
+          o unlink_activity
+    * BookingLinker
+          o BookingLinker
+          o link_booking
+          o unlink_booking
     * CompanyLinker
           o CompanyLinker
           o link_company
           o unlink_company
     * ContactLinker
           o ContactLinker
           o link_contact
@@ -146,785 +154,851 @@
 _26task.link_staff(staff)
 _27```
 _28
 _29"""
 _30
 _31from projectal import api
 _32
-_33class BaseLinker:
-_34    # _link_name is the link name (usually the entity name)
-_35    _link_name = None
-_36
-_37    # _link_key is the key within the source object that points to the
-_38    # links. E.g., 'skillList'
-_39    _link_key = None
-_40
-_41    # _link_data_name is the key within the linked (target) object that
+_33
+_34class BaseLinker:
+_35    # _link_name is the link name (usually the entity name)
+_36    _link_name = None
+_37
+_38    # _link_key is the key within the source object that points to the
+_39    # links. E.g., 'skillList'
+_40    _link_key = None
+_41
+_42    # _link_data_name is the key within the linked (target) object that
 points
-_42    # to a store of custom values within that link. E.g, Skill objects,
-_43    # when linked, have a 'skillLink' property that holds data about
-_44    # the link.
-_45    _link_data_name = None
-_46
-_47    # _link_type is the data type of the value in entity[link_key]. This is
-_48    # usually a list since most links appear as 'skillList', 'staffList',
-_49    # etc. But some links are single-entity only and appear as dicts like
-_50    # project[stage] = Stage.
-_51    _link_type = list
-_52
-_53    # _link_entity is the string name (capitalized, like Stage) of the
+_43    # to a store of custom values within that link. E.g, Skill objects,
+_44    # when linked, have a 'skillLink' property that holds data about
+_45    # the link.
+_46    _link_data_name = None
+_47
+_48    # _link_type is the data type of the value in entity[link_key]. This is
+_49    # usually a list since most links appear as 'skillList', 'staffList',
+_50    # etc. But some links are single-entity only and appear as dicts like
+_51    # project[stage] = Stage.
+_52    _link_type = list
+_53
+_54    # _link_entity is the string name (capitalized, like Stage) of the
 Entity
-_54    # class within this library that fetched links will be converted to.
-_55    # This is useful when the name of the list differs from the entity
-_56    # name. E.g: stage_list needs to be converted to Stage.
-_57    _link_entity = None
-_58
-_59class AccessPolicyLinker(BaseLinker):
-_60    """Subclass can link to Access Policies"""
-_61    _link_name = 'access_policy'
-_62    _link_key = 'accessPolicyList'
-_63    _link_entity = 'AccessPolicy'
-_64
-_65    def link_access_policy(self, access_policies):
-_66        self._add_link('access_policy', access_policies)
-_67
-_68    def unlink_access_policy(self, access_policies):
-_69        self._delete_link('access_policy', access_policies)
-_70
-_71
-_72class CompanyLinker(BaseLinker):
-_73    """Subclass can link to Companies"""
-_74    _link_name = 'company'
-_75
-_76    def link_company(self, companies):
-_77        self._add_link('company', companies)
-_78
-_79    def unlink_company(self, companies):
-_80        self._delete_link('company', companies)
-_81
-_82
-_83class ContactLinker(BaseLinker):
-_84    """Subclass can link to Contacts"""
-_85    _link_name = 'contact'
-_86
-_87    def link_contact(self, contacts):
-_88        self._add_link('contact', contacts)
-_89
-_90    def unlink_contact(self, contacts):
-_91        self._delete_link('contact', contacts)
-_92
-_93
-_94class CustomerLinker(BaseLinker):
-_95    """Subclass can link to Customers"""
-_96    _link_name = 'customer'
-_97
-_98    def link_customer(self, customers):
-_99        self._add_link('customer', customers)
-100
-101    def unlink_customer(self, customers):
-102        self._delete_link('customer', customers)
-103
-104
-105class DepartmentLinker(BaseLinker):
-106    """Subclass can link to Departments"""
-107    _link_name = 'department'
-108
-109    def link_department(self, departments):
-110        self._add_link('department', departments)
-111
-112    def unlink_department(self, departments):
-113        self._delete_link('department', departments)
-114
-115
-116class FileLinker(BaseLinker):
-117    """Subclass can link to Files"""
-118    _link_name = 'file'
-119    _link_key = 'storageFileList'
-120
-121    def link_file(self, files):
-122        self._add_link('file', files)
-123
-124    def unlink_file(self, files):
-125        self._delete_link('file', files)
-126
+_55    # class within this library that fetched links will be converted to.
+_56    # This is useful when the name of the list differs from the entity
+_57    # name. E.g: stage_list needs to be converted to Stage.
+_58    _link_entity = None
+_59
+_60
+_61class AccessPolicyLinker(BaseLinker):
+_62    """Subclass can link to Access Policies"""
+_63    _link_name = 'access_policy'
+_64    _link_key = 'accessPolicyList'
+_65    _link_entity = 'AccessPolicy'
+_66
+_67    def link_access_policy(self, access_policies):
+_68        self._add_link('access_policy', access_policies)
+_69
+_70    def unlink_access_policy(self, access_policies):
+_71        self._delete_link('access_policy', access_policies)
+_72
+_73
+_74class ActivityLinker(BaseLinker):
+_75    """Subclass can link to Activities"""
+_76    _link_name = 'activity'
+_77
+_78    def link_activity(self, activity):
+_79        self._add_link('activity', activity)
+_80
+_81    def unlink_activity(self, activity):
+_82        self._delete_link('activity', activity)
+_83
+_84
+_85class BookingLinker(BaseLinker):
+_86    """Subclass can link to Bookings"""
+_87    _link_name = 'booking'
+_88
+_89    def link_booking(self, booking):
+_90        self._add_link('booking', booking)
+_91
+_92    def unlink_booking(self, booking):
+_93        self._delete_link('booking', booking)
+_94
+_95
+_96class CompanyLinker(BaseLinker):
+_97    """Subclass can link to Companies"""
+_98    _link_name = 'company'
+_99
+100    def link_company(self, companies):
+101        self._add_link('company', companies)
+102
+103    def unlink_company(self, companies):
+104        self._delete_link('company', companies)
+105
+106
+107class ContactLinker(BaseLinker):
+108    """Subclass can link to Contacts"""
+109    _link_name = 'contact'
+110
+111    def link_contact(self, contacts):
+112        self._add_link('contact', contacts)
+113
+114    def unlink_contact(self, contacts):
+115        self._delete_link('contact', contacts)
+116
+117
+118class CustomerLinker(BaseLinker):
+119    """Subclass can link to Customers"""
+120    _link_name = 'customer'
+121
+122    def link_customer(self, customers):
+123        self._add_link('customer', customers)
+124
+125    def unlink_customer(self, customers):
+126        self._delete_link('customer', customers)
 127
-128class FolderLinker(BaseLinker):
-129    """Subclass can link to Folders"""
-130    _link_name = 'folder'
-131    _link_key = 'folders'
+128
+129class DepartmentLinker(BaseLinker):
+130    """Subclass can link to Departments"""
+131    _link_name = 'department'
 132
-133    def link_folder(self, folders):
-134        self._add_link('folder', folders)
+133    def link_department(self, departments):
+134        self._add_link('department', departments)
 135
-136    def unlink_folder(self, folders):
-137        self._delete_link('folder', folders)
+136    def unlink_department(self, departments):
+137        self._delete_link('department', departments)
 138
 139
-140class LocationLinker(BaseLinker):
-141    """Subclass can link to Locations"""
-142    _link_name = 'location'
-143
-144    def link_location(self, locations):
-145        self._add_link('location', locations)
-146
-147    def unlink_location(self, locations):
-148        self._delete_link('location', locations)
-149
+140class FileLinker(BaseLinker):
+141    """Subclass can link to Files"""
+142    _link_name = 'file'
+143    _link_key = 'storageFileList'
+144
+145    def link_file(self, files):
+146        self._add_link('file', files)
+147
+148    def unlink_file(self, files):
+149        self._delete_link('file', files)
 150
-151class PermissionLinker(BaseLinker):
-152    """Subclass can link to Permissions"""
-153    _link_name = 'permission'
-154
-155    def link_permission(self, permissions):
-156        return self._add_link('permission', permissions)
-157
-158    def unlink_permission(self, permissions):
-159        return self._delete_link('permission', permissions)
-160
-161
-162class ProjectLinker(BaseLinker):
-163    """Subclass can link to Projects"""
-164    _link_name = 'project'
-165
-166    def link_project(self, projects):
-167        self._add_link('project', projects)
-168
-169    def unlink_project(self, projects):
-170        self._delete_link('project', projects)
-171
-172
-173class RebateLinker(BaseLinker):
-174    """Subclass can link to Rebates"""
-175    _link_name = 'rebate'
-176
-177    def link_rebate(self, rebates):
-178        self._add_link('rebate', rebates)
-179
-180    def unlink_rebate(self, rebates):
-181        self._delete_link('rebate', rebates)
-182
-183
-184class ResourceLinker(BaseLinker):
-185    """Subclass can link to Resources"""
-186    _link_name = 'resource'
-187    _link_data_name = 'resourceLink'
-188
-189    def link_resource(self, resources):
-190        self._add_link('resource', resources)
-191
-192    def relink_resource(self, resources):
-193        self._update_link('resource', resources)
-194
-195    def unlink_resource(self, resources):
-196        self._delete_link('resource', resources)
-197
-198
-199class SkillLinker(BaseLinker):
-200    """Subclass can link to Skills"""
-201    _link_name = 'skill'
-202    _link_data_name = 'skillLink'
+151
+152class FolderLinker(BaseLinker):
+153    """Subclass can link to Folders"""
+154    _link_name = 'folder'
+155    _link_key = 'folders'
+156
+157    def link_folder(self, folders):
+158        self._add_link('folder', folders)
+159
+160    def unlink_folder(self, folders):
+161        self._delete_link('folder', folders)
+162
+163
+164class LocationLinker(BaseLinker):
+165    """Subclass can link to Locations"""
+166    _link_name = 'location'
+167
+168    def link_location(self, locations):
+169        self._add_link('location', locations)
+170
+171    def unlink_location(self, locations):
+172        self._delete_link('location', locations)
+173
+174
+175class PermissionLinker(BaseLinker):
+176    """Subclass can link to Permissions"""
+177    _link_name = 'permission'
+178
+179    def link_permission(self, permissions):
+180        return self._add_link('permission', permissions)
+181
+182    def unlink_permission(self, permissions):
+183        return self._delete_link('permission', permissions)
+184
+185
+186class ProjectLinker(BaseLinker):
+187    """Subclass can link to Projects"""
+188    _link_name = 'project'
+189
+190    def link_project(self, projects):
+191        self._add_link('project', projects)
+192
+193    def unlink_project(self, projects):
+194        self._delete_link('project', projects)
+195
+196
+197class RebateLinker(BaseLinker):
+198    """Subclass can link to Rebates"""
+199    _link_name = 'rebate'
+200
+201    def link_rebate(self, rebates):
+202        self._add_link('rebate', rebates)
 203
-204    def link_skill(self, skills):
-205        self._add_link('skill', skills)
+204    def unlink_rebate(self, rebates):
+205        self._delete_link('rebate', rebates)
 206
-207    def relink_skill(self, skills):
-208        self._update_link('skill', skills)
-209
-210    def unlink_skill(self, skills):
-211        self._delete_link('skill', skills)
+207
+208class ResourceLinker(BaseLinker):
+209    """Subclass can link to Resources"""
+210    _link_name = 'resource'
+211    _link_data_name = 'resourceLink'
 212
-213
-214class StaffLinker(BaseLinker):
-215    """Subclass can link to Staff"""
-216    _link_name = 'staff'
-217    _link_data_name = 'resourceLink'
+213    def link_resource(self, resources):
+214        self._add_link('resource', resources)
+215
+216    def relink_resource(self, resources):
+217        self._update_link('resource', resources)
 218
-219    def link_staff(self, staffs):
-220        self._add_link('staff', staffs)
+219    def unlink_resource(self, resources):
+220        self._delete_link('resource', resources)
 221
-222    def relink_staff(self, staffs):
-223        self._update_link('staff', staffs)
-224
-225    def unlink_staff(self, staffs):
-226        self._delete_link('staff', staffs)
+222
+223class SkillLinker(BaseLinker):
+224    """Subclass can link to Skills"""
+225    _link_name = 'skill'
+226    _link_data_name = 'skillLink'
 227
-228
-229class StageLinker(BaseLinker):
-230    """Subclass can link to Stages"""
-231    _link_name = 'stage'
-232    _link_key = 'stage'
-233    _link_type = dict
-234
-235    def link_stage(self, stages):
-236        self._add_link('stage', stages)
+228    def link_skill(self, skills):
+229        self._add_link('skill', skills)
+230
+231    def relink_skill(self, skills):
+232        self._update_link('skill', skills)
+233
+234    def unlink_skill(self, skills):
+235        self._delete_link('skill', skills)
+236
 237
-238    def unlink_stage(self, stages):
-239        self._delete_link('stage', stages)
-240
-241
-242class StageListLinker(BaseLinker):
-243    """Subclass can link to Stage List"""
-244    _link_name = 'stage_list'
-245    _link_key = 'stageList'
-246    _link_entity = 'Stage'
-247
-248    def link_stage_list(self, stages):
-249        if not isinstance(stages, list):
-250            raise api.UsageException('Stage list link must be a list')
-251        self._add_link('stage_list', stages)
+238class StaffLinker(BaseLinker):
+239    """Subclass can link to Staff"""
+240    _link_name = 'staff'
+241    _link_data_name = 'resourceLink'
+242
+243    def link_staff(self, staffs):
+244        self._add_link('staff', staffs)
+245
+246    def relink_staff(self, staffs):
+247        self._update_link('staff', staffs)
+248
+249    def unlink_staff(self, staffs):
+250        self._delete_link('staff', staffs)
+251
 252
-253    def unlink_stage_list(self, stages):
-254        if not isinstance(stages, list):
-255            raise api.UsageException('Stage list unlink must be a list')
-256        stages = [{'uuId': s['uuId']} for s in stages]
-257        self._delete_link('stage_list', stages)
+253class StageLinker(BaseLinker):
+254    """Subclass can link to Stages"""
+255    _link_name = 'stage'
+256    _link_key = 'stage'
+257    _link_type = dict
 258
-259
-260class UserLinker(BaseLinker):
-261    _link_name = 'user'
-262
-263    def link_user(self, users):
-264        self._add_link('user', users)
+259    def link_stage(self, stages):
+260        self._add_link('stage', stages)
+261
+262    def unlink_stage(self, stages):
+263        self._delete_link('stage', stages)
+264
 265
-266    def unlink_user(self, users):
-267        self._delete_link('user', users)
-268
-269
-270class TaskLinker(BaseLinker):
-271    _link_name = 'task'
-272
-273    def link_task(self, tasks):
-274        self._add_link('task', tasks)
-275
-276    def unlink_task(self, tasks):
-277        self._delete_link('task', tasks)
-278
-279
-280class TaskTemplateLinker(BaseLinker):
-281    _link_name = 'task_template'
-282    _link_entity = 'TaskTemplate'
+266class StageListLinker(BaseLinker):
+267    """Subclass can link to Stage List"""
+268    _link_name = 'stage_list'
+269    _link_key = 'stageList'
+270    _link_entity = 'Stage'
+271
+272    def link_stage_list(self, stages):
+273        if not isinstance(stages, list):
+274            raise api.UsageException('Stage list link must be a list')
+275        self._add_link('stage_list', stages)
+276
+277    def unlink_stage_list(self, stages):
+278        if not isinstance(stages, list):
+279            raise api.UsageException('Stage list unlink must be a list')
+280        stages = [{'uuId': s['uuId']} for s in stages]
+281        self._delete_link('stage_list', stages)
+282
 283
-284    def link_task_template(self, task_templates):
-285        self._add_link('task_template', task_templates)
+284class UserLinker(BaseLinker):
+285    _link_name = 'user'
 286
-287    def unlink_task_template(self, task_templates):
-288        self._delete_link('task_template', task_templates)
+287    def link_user(self, users):
+288        self._add_link('user', users)
 289
-290class TagLinker(BaseLinker):
-291    _link_name = 'tag'
+290    def unlink_user(self, users):
+291        self._delete_link('user', users)
 292
-293    def link_tag(self, tags):
-294        self._add_link('tag', tags)
-295
-296    def unlink_tag(self, tags):
-297        self._delete_link('tag', tags)
-298
-299class NoteLinker(BaseLinker):
-300    _link_name = 'note'
-301
-302class CalendarLinker(BaseLinker):
-303    _link_name = 'calendar'
-304
-305# Projects have a list of tasks that we can fetch using the links=
-306# method, but they have no linker methods available.
-307class TaskInProjectLinker(BaseLinker):
-308    _link_name = "task"
+293
+294class TaskLinker(BaseLinker):
+295    _link_name = 'task'
+296
+297    def link_task(self, tasks):
+298        self._add_link('task', tasks)
+299
+300    def unlink_task(self, tasks):
+301        self._delete_link('task', tasks)
+302
+303
+304class TaskTemplateLinker(BaseLinker):
+305    _link_name = 'task_template'
+306    _link_entity = 'TaskTemplate'
+307
+308    def link_task_template(self, task_templates):
+309        self._add_link('task_template', task_templates)
+310
+311    def unlink_task_template(self, task_templates):
+312        self._delete_link('task_template', task_templates)
+313
+314class TagLinker(BaseLinker):
+315    _link_name = 'tag'
+316
+317    def link_tag(self, tags):
+318        self._add_link('tag', tags)
+319
+320    def unlink_tag(self, tags):
+321        self._delete_link('tag', tags)
+322
+323class NoteLinker(BaseLinker):
+324    _link_name = 'note'
+325
+326class CalendarLinker(BaseLinker):
+327    _link_name = 'calendar'
+328
+329# Projects have a list of tasks that we can fetch using the links=
+330# method, but they have no linker methods available.
+331class TaskInProjectLinker(BaseLinker):
+332    _link_name = "task"
   ⁰
 class BaseLinker: View Source
-34class BaseLinker:
-35    # _link_name is the link name (usually the entity name)
-36    _link_name = None
-37
-38    # _link_key is the key within the source object that points to the
-39    # links. E.g., 'skillList'
-40    _link_key = None
-41
-42    # _link_data_name is the key within the linked (target) object that
+35class BaseLinker:
+36    # _link_name is the link name (usually the entity name)
+37    _link_name = None
+38
+39    # _link_key is the key within the source object that points to the
+40    # links. E.g., 'skillList'
+41    _link_key = None
+42
+43    # _link_data_name is the key within the linked (target) object that
 points
-43    # to a store of custom values within that link. E.g, Skill objects,
-44    # when linked, have a 'skillLink' property that holds data about
-45    # the link.
-46    _link_data_name = None
-47
-48    # _link_type is the data type of the value in entity[link_key]. This is
-49    # usually a list since most links appear as 'skillList', 'staffList',
-50    # etc. But some links are single-entity only and appear as dicts like
-51    # project[stage] = Stage.
-52    _link_type = list
-53
-54    # _link_entity is the string name (capitalized, like Stage) of the Entity
-55    # class within this library that fetched links will be converted to.
-56    # This is useful when the name of the list differs from the entity
-57    # name. E.g: stage_list needs to be converted to Stage.
-58    _link_entity = None
+44    # to a store of custom values within that link. E.g, Skill objects,
+45    # when linked, have a 'skillLink' property that holds data about
+46    # the link.
+47    _link_data_name = None
+48
+49    # _link_type is the data type of the value in entity[link_key]. This is
+50    # usually a list since most links appear as 'skillList', 'staffList',
+51    # etc. But some links are single-entity only and appear as dicts like
+52    # project[stage] = Stage.
+53    _link_type = list
+54
+55    # _link_entity is the string name (capitalized, like Stage) of the Entity
+56    # class within this library that fetched links will be converted to.
+57    # This is useful when the name of the list differs from the entity
+58    # name. E.g: stage_list needs to be converted to Stage.
+59    _link_entity = None
 BaseLinker()
   ⁰
 class AccessPolicyLinker(BaseLinker): View Source
-60class AccessPolicyLinker(BaseLinker):
-61    """Subclass can link to Access Policies"""
-62    _link_name = 'access_policy'
-63    _link_key = 'accessPolicyList'
-64    _link_entity = 'AccessPolicy'
-65
-66    def link_access_policy(self, access_policies):
-67        self._add_link('access_policy', access_policies)
-68
-69    def unlink_access_policy(self, access_policies):
-70        self._delete_link('access_policy', access_policies)
+62class AccessPolicyLinker(BaseLinker):
+63    """Subclass can link to Access Policies"""
+64    _link_name = 'access_policy'
+65    _link_key = 'accessPolicyList'
+66    _link_entity = 'AccessPolicy'
+67
+68    def link_access_policy(self, access_policies):
+69        self._add_link('access_policy', access_policies)
+70
+71    def unlink_access_policy(self, access_policies):
+72        self._delete_link('access_policy', access_policies)
 Subclass can link to Access Policies
 AccessPolicyLinker()
 ⁰
 def link_access_policy(self, access_policies): View Source
-66    def link_access_policy(self, access_policies):
-67        self._add_link('access_policy', access_policies)
+68    def link_access_policy(self, access_policies):
+69        self._add_link('access_policy', access_policies)
 ⁰
 def unlink_access_policy(self, access_policies): View Source
-69    def unlink_access_policy(self, access_policies):
-70        self._delete_link('access_policy', access_policies)
+71    def unlink_access_policy(self, access_policies):
+72        self._delete_link('access_policy', access_policies)
+  ⁰
+class ActivityLinker(BaseLinker): View Source
+75class ActivityLinker(BaseLinker):
+76    """Subclass can link to Activities"""
+77    _link_name = 'activity'
+78
+79    def link_activity(self, activity):
+80        self._add_link('activity', activity)
+81
+82    def unlink_activity(self, activity):
+83        self._delete_link('activity', activity)
+Subclass can link to Activities
+ActivityLinker()
+⁰
+def link_activity(self, activity): View Source
+79    def link_activity(self, activity):
+80        self._add_link('activity', activity)
+⁰
+def unlink_activity(self, activity): View Source
+82    def unlink_activity(self, activity):
+83        self._delete_link('activity', activity)
+  ⁰
+class BookingLinker(BaseLinker): View Source
+86class BookingLinker(BaseLinker):
+87    """Subclass can link to Bookings"""
+88    _link_name = 'booking'
+89
+90    def link_booking(self, booking):
+91        self._add_link('booking', booking)
+92
+93    def unlink_booking(self, booking):
+94        self._delete_link('booking', booking)
+Subclass can link to Bookings
+BookingLinker()
+⁰
+def link_booking(self, booking): View Source
+90    def link_booking(self, booking):
+91        self._add_link('booking', booking)
+⁰
+def unlink_booking(self, booking): View Source
+93    def unlink_booking(self, booking):
+94        self._delete_link('booking', booking)
   ⁰
 class CompanyLinker(BaseLinker): View Source
-73class CompanyLinker(BaseLinker):
-74    """Subclass can link to Companies"""
-75    _link_name = 'company'
-76
-77    def link_company(self, companies):
-78        self._add_link('company', companies)
-79
-80    def unlink_company(self, companies):
-81        self._delete_link('company', companies)
+_97class CompanyLinker(BaseLinker):
+_98    """Subclass can link to Companies"""
+_99    _link_name = 'company'
+100
+101    def link_company(self, companies):
+102        self._add_link('company', companies)
+103
+104    def unlink_company(self, companies):
+105        self._delete_link('company', companies)
 Subclass can link to Companies
 CompanyLinker()
 ⁰
 def link_company(self, companies): View Source
-77    def link_company(self, companies):
-78        self._add_link('company', companies)
+101    def link_company(self, companies):
+102        self._add_link('company', companies)
 ⁰
 def unlink_company(self, companies): View Source
-80    def unlink_company(self, companies):
-81        self._delete_link('company', companies)
+104    def unlink_company(self, companies):
+105        self._delete_link('company', companies)
   ⁰
 class ContactLinker(BaseLinker): View Source
-84class ContactLinker(BaseLinker):
-85    """Subclass can link to Contacts"""
-86    _link_name = 'contact'
-87
-88    def link_contact(self, contacts):
-89        self._add_link('contact', contacts)
-90
-91    def unlink_contact(self, contacts):
-92        self._delete_link('contact', contacts)
+108class ContactLinker(BaseLinker):
+109    """Subclass can link to Contacts"""
+110    _link_name = 'contact'
+111
+112    def link_contact(self, contacts):
+113        self._add_link('contact', contacts)
+114
+115    def unlink_contact(self, contacts):
+116        self._delete_link('contact', contacts)
 Subclass can link to Contacts
 ContactLinker()
 ⁰
 def link_contact(self, contacts): View Source
-88    def link_contact(self, contacts):
-89        self._add_link('contact', contacts)
+112    def link_contact(self, contacts):
+113        self._add_link('contact', contacts)
 ⁰
 def unlink_contact(self, contacts): View Source
-91    def unlink_contact(self, contacts):
-92        self._delete_link('contact', contacts)
+115    def unlink_contact(self, contacts):
+116        self._delete_link('contact', contacts)
   ⁰
 class CustomerLinker(BaseLinker): View Source
-_95class CustomerLinker(BaseLinker):
-_96    """Subclass can link to Customers"""
-_97    _link_name = 'customer'
-_98
-_99    def link_customer(self, customers):
-100        self._add_link('customer', customers)
-101
-102    def unlink_customer(self, customers):
-103        self._delete_link('customer', customers)
+119class CustomerLinker(BaseLinker):
+120    """Subclass can link to Customers"""
+121    _link_name = 'customer'
+122
+123    def link_customer(self, customers):
+124        self._add_link('customer', customers)
+125
+126    def unlink_customer(self, customers):
+127        self._delete_link('customer', customers)
 Subclass can link to Customers
 CustomerLinker()
 ⁰
 def link_customer(self, customers): View Source
-_99    def link_customer(self, customers):
-100        self._add_link('customer', customers)
+123    def link_customer(self, customers):
+124        self._add_link('customer', customers)
 ⁰
 def unlink_customer(self, customers): View Source
-102    def unlink_customer(self, customers):
-103        self._delete_link('customer', customers)
+126    def unlink_customer(self, customers):
+127        self._delete_link('customer', customers)
   ⁰
 class DepartmentLinker(BaseLinker): View Source
-106class DepartmentLinker(BaseLinker):
-107    """Subclass can link to Departments"""
-108    _link_name = 'department'
-109
-110    def link_department(self, departments):
-111        self._add_link('department', departments)
-112
-113    def unlink_department(self, departments):
-114        self._delete_link('department', departments)
+130class DepartmentLinker(BaseLinker):
+131    """Subclass can link to Departments"""
+132    _link_name = 'department'
+133
+134    def link_department(self, departments):
+135        self._add_link('department', departments)
+136
+137    def unlink_department(self, departments):
+138        self._delete_link('department', departments)
 Subclass can link to Departments
 DepartmentLinker()
 ⁰
 def link_department(self, departments): View Source
-110    def link_department(self, departments):
-111        self._add_link('department', departments)
+134    def link_department(self, departments):
+135        self._add_link('department', departments)
 ⁰
 def unlink_department(self, departments): View Source
-113    def unlink_department(self, departments):
-114        self._delete_link('department', departments)
+137    def unlink_department(self, departments):
+138        self._delete_link('department', departments)
   ⁰
 class FileLinker(BaseLinker): View Source
-117class FileLinker(BaseLinker):
-118    """Subclass can link to Files"""
-119    _link_name = 'file'
-120    _link_key = 'storageFileList'
-121
-122    def link_file(self, files):
-123        self._add_link('file', files)
-124
-125    def unlink_file(self, files):
-126        self._delete_link('file', files)
+141class FileLinker(BaseLinker):
+142    """Subclass can link to Files"""
+143    _link_name = 'file'
+144    _link_key = 'storageFileList'
+145
+146    def link_file(self, files):
+147        self._add_link('file', files)
+148
+149    def unlink_file(self, files):
+150        self._delete_link('file', files)
 Subclass can link to Files
 FileLinker()
 ⁰
 def link_file(self, files): View Source
-122    def link_file(self, files):
-123        self._add_link('file', files)
+146    def link_file(self, files):
+147        self._add_link('file', files)
 ⁰
 def unlink_file(self, files): View Source
-125    def unlink_file(self, files):
-126        self._delete_link('file', files)
+149    def unlink_file(self, files):
+150        self._delete_link('file', files)
   ⁰
 class FolderLinker(BaseLinker): View Source
-129class FolderLinker(BaseLinker):
-130    """Subclass can link to Folders"""
-131    _link_name = 'folder'
-132    _link_key = 'folders'
-133
-134    def link_folder(self, folders):
-135        self._add_link('folder', folders)
-136
-137    def unlink_folder(self, folders):
-138        self._delete_link('folder', folders)
+153class FolderLinker(BaseLinker):
+154    """Subclass can link to Folders"""
+155    _link_name = 'folder'
+156    _link_key = 'folders'
+157
+158    def link_folder(self, folders):
+159        self._add_link('folder', folders)
+160
+161    def unlink_folder(self, folders):
+162        self._delete_link('folder', folders)
 Subclass can link to Folders
 FolderLinker()
 ⁰
 def link_folder(self, folders): View Source
-134    def link_folder(self, folders):
-135        self._add_link('folder', folders)
+158    def link_folder(self, folders):
+159        self._add_link('folder', folders)
 ⁰
 def unlink_folder(self, folders): View Source
-137    def unlink_folder(self, folders):
-138        self._delete_link('folder', folders)
+161    def unlink_folder(self, folders):
+162        self._delete_link('folder', folders)
   ⁰
 class LocationLinker(BaseLinker): View Source
-141class LocationLinker(BaseLinker):
-142    """Subclass can link to Locations"""
-143    _link_name = 'location'
-144
-145    def link_location(self, locations):
-146        self._add_link('location', locations)
-147
-148    def unlink_location(self, locations):
-149        self._delete_link('location', locations)
+165class LocationLinker(BaseLinker):
+166    """Subclass can link to Locations"""
+167    _link_name = 'location'
+168
+169    def link_location(self, locations):
+170        self._add_link('location', locations)
+171
+172    def unlink_location(self, locations):
+173        self._delete_link('location', locations)
 Subclass can link to Locations
 LocationLinker()
 ⁰
 def link_location(self, locations): View Source
-145    def link_location(self, locations):
-146        self._add_link('location', locations)
+169    def link_location(self, locations):
+170        self._add_link('location', locations)
 ⁰
 def unlink_location(self, locations): View Source
-148    def unlink_location(self, locations):
-149        self._delete_link('location', locations)
+172    def unlink_location(self, locations):
+173        self._delete_link('location', locations)
   ⁰
 class PermissionLinker(BaseLinker): View Source
-152class PermissionLinker(BaseLinker):
-153    """Subclass can link to Permissions"""
-154    _link_name = 'permission'
-155
-156    def link_permission(self, permissions):
-157        return self._add_link('permission', permissions)
-158
-159    def unlink_permission(self, permissions):
-160        return self._delete_link('permission', permissions)
+176class PermissionLinker(BaseLinker):
+177    """Subclass can link to Permissions"""
+178    _link_name = 'permission'
+179
+180    def link_permission(self, permissions):
+181        return self._add_link('permission', permissions)
+182
+183    def unlink_permission(self, permissions):
+184        return self._delete_link('permission', permissions)
 Subclass can link to Permissions
 PermissionLinker()
 ⁰
 def link_permission(self, permissions): View Source
-156    def link_permission(self, permissions):
-157        return self._add_link('permission', permissions)
+180    def link_permission(self, permissions):
+181        return self._add_link('permission', permissions)
 ⁰
 def unlink_permission(self, permissions): View Source
-159    def unlink_permission(self, permissions):
-160        return self._delete_link('permission', permissions)
+183    def unlink_permission(self, permissions):
+184        return self._delete_link('permission', permissions)
   ⁰
 class ProjectLinker(BaseLinker): View Source
-163class ProjectLinker(BaseLinker):
-164    """Subclass can link to Projects"""
-165    _link_name = 'project'
-166
-167    def link_project(self, projects):
-168        self._add_link('project', projects)
-169
-170    def unlink_project(self, projects):
-171        self._delete_link('project', projects)
+187class ProjectLinker(BaseLinker):
+188    """Subclass can link to Projects"""
+189    _link_name = 'project'
+190
+191    def link_project(self, projects):
+192        self._add_link('project', projects)
+193
+194    def unlink_project(self, projects):
+195        self._delete_link('project', projects)
 Subclass can link to Projects
 ProjectLinker()
 ⁰
 def link_project(self, projects): View Source
-167    def link_project(self, projects):
-168        self._add_link('project', projects)
+191    def link_project(self, projects):
+192        self._add_link('project', projects)
 ⁰
 def unlink_project(self, projects): View Source
-170    def unlink_project(self, projects):
-171        self._delete_link('project', projects)
+194    def unlink_project(self, projects):
+195        self._delete_link('project', projects)
   ⁰
 class RebateLinker(BaseLinker): View Source
-174class RebateLinker(BaseLinker):
-175    """Subclass can link to Rebates"""
-176    _link_name = 'rebate'
-177
-178    def link_rebate(self, rebates):
-179        self._add_link('rebate', rebates)
-180
-181    def unlink_rebate(self, rebates):
-182        self._delete_link('rebate', rebates)
+198class RebateLinker(BaseLinker):
+199    """Subclass can link to Rebates"""
+200    _link_name = 'rebate'
+201
+202    def link_rebate(self, rebates):
+203        self._add_link('rebate', rebates)
+204
+205    def unlink_rebate(self, rebates):
+206        self._delete_link('rebate', rebates)
 Subclass can link to Rebates
 RebateLinker()
 ⁰
 def link_rebate(self, rebates): View Source
-178    def link_rebate(self, rebates):
-179        self._add_link('rebate', rebates)
+202    def link_rebate(self, rebates):
+203        self._add_link('rebate', rebates)
 ⁰
 def unlink_rebate(self, rebates): View Source
-181    def unlink_rebate(self, rebates):
-182        self._delete_link('rebate', rebates)
+205    def unlink_rebate(self, rebates):
+206        self._delete_link('rebate', rebates)
   ⁰
 class ResourceLinker(BaseLinker): View Source
-185class ResourceLinker(BaseLinker):
-186    """Subclass can link to Resources"""
-187    _link_name = 'resource'
-188    _link_data_name = 'resourceLink'
-189
-190    def link_resource(self, resources):
-191        self._add_link('resource', resources)
-192
-193    def relink_resource(self, resources):
-194        self._update_link('resource', resources)
-195
-196    def unlink_resource(self, resources):
-197        self._delete_link('resource', resources)
+209class ResourceLinker(BaseLinker):
+210    """Subclass can link to Resources"""
+211    _link_name = 'resource'
+212    _link_data_name = 'resourceLink'
+213
+214    def link_resource(self, resources):
+215        self._add_link('resource', resources)
+216
+217    def relink_resource(self, resources):
+218        self._update_link('resource', resources)
+219
+220    def unlink_resource(self, resources):
+221        self._delete_link('resource', resources)
 Subclass can link to Resources
 ResourceLinker()
 ⁰
 def link_resource(self, resources): View Source
-190    def link_resource(self, resources):
-191        self._add_link('resource', resources)
+214    def link_resource(self, resources):
+215        self._add_link('resource', resources)
 ⁰
 def relink_resource(self, resources): View Source
-193    def relink_resource(self, resources):
-194        self._update_link('resource', resources)
+217    def relink_resource(self, resources):
+218        self._update_link('resource', resources)
 ⁰
 def unlink_resource(self, resources): View Source
-196    def unlink_resource(self, resources):
-197        self._delete_link('resource', resources)
+220    def unlink_resource(self, resources):
+221        self._delete_link('resource', resources)
   ⁰
 class SkillLinker(BaseLinker): View Source
-200class SkillLinker(BaseLinker):
-201    """Subclass can link to Skills"""
-202    _link_name = 'skill'
-203    _link_data_name = 'skillLink'
-204
-205    def link_skill(self, skills):
-206        self._add_link('skill', skills)
-207
-208    def relink_skill(self, skills):
-209        self._update_link('skill', skills)
-210
-211    def unlink_skill(self, skills):
-212        self._delete_link('skill', skills)
+224class SkillLinker(BaseLinker):
+225    """Subclass can link to Skills"""
+226    _link_name = 'skill'
+227    _link_data_name = 'skillLink'
+228
+229    def link_skill(self, skills):
+230        self._add_link('skill', skills)
+231
+232    def relink_skill(self, skills):
+233        self._update_link('skill', skills)
+234
+235    def unlink_skill(self, skills):
+236        self._delete_link('skill', skills)
 Subclass can link to Skills
 SkillLinker()
 ⁰
 def link_skill(self, skills): View Source
-205    def link_skill(self, skills):
-206        self._add_link('skill', skills)
+229    def link_skill(self, skills):
+230        self._add_link('skill', skills)
 ⁰
 def relink_skill(self, skills): View Source
-208    def relink_skill(self, skills):
-209        self._update_link('skill', skills)
+232    def relink_skill(self, skills):
+233        self._update_link('skill', skills)
 ⁰
 def unlink_skill(self, skills): View Source
-211    def unlink_skill(self, skills):
-212        self._delete_link('skill', skills)
+235    def unlink_skill(self, skills):
+236        self._delete_link('skill', skills)
   ⁰
 class StaffLinker(BaseLinker): View Source
-215class StaffLinker(BaseLinker):
-216    """Subclass can link to Staff"""
-217    _link_name = 'staff'
-218    _link_data_name = 'resourceLink'
-219
-220    def link_staff(self, staffs):
-221        self._add_link('staff', staffs)
-222
-223    def relink_staff(self, staffs):
-224        self._update_link('staff', staffs)
-225
-226    def unlink_staff(self, staffs):
-227        self._delete_link('staff', staffs)
+239class StaffLinker(BaseLinker):
+240    """Subclass can link to Staff"""
+241    _link_name = 'staff'
+242    _link_data_name = 'resourceLink'
+243
+244    def link_staff(self, staffs):
+245        self._add_link('staff', staffs)
+246
+247    def relink_staff(self, staffs):
+248        self._update_link('staff', staffs)
+249
+250    def unlink_staff(self, staffs):
+251        self._delete_link('staff', staffs)
 Subclass can link to Staff
 StaffLinker()
 ⁰
 def link_staff(self, staffs): View Source
-220    def link_staff(self, staffs):
-221        self._add_link('staff', staffs)
+244    def link_staff(self, staffs):
+245        self._add_link('staff', staffs)
 ⁰
 def relink_staff(self, staffs): View Source
-223    def relink_staff(self, staffs):
-224        self._update_link('staff', staffs)
+247    def relink_staff(self, staffs):
+248        self._update_link('staff', staffs)
 ⁰
 def unlink_staff(self, staffs): View Source
-226    def unlink_staff(self, staffs):
-227        self._delete_link('staff', staffs)
+250    def unlink_staff(self, staffs):
+251        self._delete_link('staff', staffs)
   ⁰
 class StageLinker(BaseLinker): View Source
-230class StageLinker(BaseLinker):
-231    """Subclass can link to Stages"""
-232    _link_name = 'stage'
-233    _link_key = 'stage'
-234    _link_type = dict
-235
-236    def link_stage(self, stages):
-237        self._add_link('stage', stages)
-238
-239    def unlink_stage(self, stages):
-240        self._delete_link('stage', stages)
+254class StageLinker(BaseLinker):
+255    """Subclass can link to Stages"""
+256    _link_name = 'stage'
+257    _link_key = 'stage'
+258    _link_type = dict
+259
+260    def link_stage(self, stages):
+261        self._add_link('stage', stages)
+262
+263    def unlink_stage(self, stages):
+264        self._delete_link('stage', stages)
 Subclass can link to Stages
 StageLinker()
 ⁰
 def link_stage(self, stages): View Source
-236    def link_stage(self, stages):
-237        self._add_link('stage', stages)
+260    def link_stage(self, stages):
+261        self._add_link('stage', stages)
 ⁰
 def unlink_stage(self, stages): View Source
-239    def unlink_stage(self, stages):
-240        self._delete_link('stage', stages)
+263    def unlink_stage(self, stages):
+264        self._delete_link('stage', stages)
   ⁰
 class StageListLinker(BaseLinker): View Source
-243class StageListLinker(BaseLinker):
-244    """Subclass can link to Stage List"""
-245    _link_name = 'stage_list'
-246    _link_key = 'stageList'
-247    _link_entity = 'Stage'
-248
-249    def link_stage_list(self, stages):
-250        if not isinstance(stages, list):
-251            raise api.UsageException('Stage list link must be a list')
-252        self._add_link('stage_list', stages)
-253
-254    def unlink_stage_list(self, stages):
-255        if not isinstance(stages, list):
-256            raise api.UsageException('Stage list unlink must be a list')
-257        stages = [{'uuId': s['uuId']} for s in stages]
-258        self._delete_link('stage_list', stages)
+267class StageListLinker(BaseLinker):
+268    """Subclass can link to Stage List"""
+269    _link_name = 'stage_list'
+270    _link_key = 'stageList'
+271    _link_entity = 'Stage'
+272
+273    def link_stage_list(self, stages):
+274        if not isinstance(stages, list):
+275            raise api.UsageException('Stage list link must be a list')
+276        self._add_link('stage_list', stages)
+277
+278    def unlink_stage_list(self, stages):
+279        if not isinstance(stages, list):
+280            raise api.UsageException('Stage list unlink must be a list')
+281        stages = [{'uuId': s['uuId']} for s in stages]
+282        self._delete_link('stage_list', stages)
 Subclass can link to Stage List
 StageListLinker()
 ⁰
 def link_stage_list(self, stages): View Source
-249    def link_stage_list(self, stages):
-250        if not isinstance(stages, list):
-251            raise api.UsageException('Stage list link must be a list')
-252        self._add_link('stage_list', stages)
+273    def link_stage_list(self, stages):
+274        if not isinstance(stages, list):
+275            raise api.UsageException('Stage list link must be a list')
+276        self._add_link('stage_list', stages)
 ⁰
 def unlink_stage_list(self, stages): View Source
-254    def unlink_stage_list(self, stages):
-255        if not isinstance(stages, list):
-256            raise api.UsageException('Stage list unlink must be a list')
-257        stages = [{'uuId': s['uuId']} for s in stages]
-258        self._delete_link('stage_list', stages)
+278    def unlink_stage_list(self, stages):
+279        if not isinstance(stages, list):
+280            raise api.UsageException('Stage list unlink must be a list')
+281        stages = [{'uuId': s['uuId']} for s in stages]
+282        self._delete_link('stage_list', stages)
   ⁰
 class UserLinker(BaseLinker): View Source
-261class UserLinker(BaseLinker):
-262    _link_name = 'user'
-263
-264    def link_user(self, users):
-265        self._add_link('user', users)
-266
-267    def unlink_user(self, users):
-268        self._delete_link('user', users)
+285class UserLinker(BaseLinker):
+286    _link_name = 'user'
+287
+288    def link_user(self, users):
+289        self._add_link('user', users)
+290
+291    def unlink_user(self, users):
+292        self._delete_link('user', users)
 UserLinker()
 ⁰
 def link_user(self, users): View Source
-264    def link_user(self, users):
-265        self._add_link('user', users)
+288    def link_user(self, users):
+289        self._add_link('user', users)
 ⁰
 def unlink_user(self, users): View Source
-267    def unlink_user(self, users):
-268        self._delete_link('user', users)
+291    def unlink_user(self, users):
+292        self._delete_link('user', users)
   ⁰
 class TaskLinker(BaseLinker): View Source
-271class TaskLinker(BaseLinker):
-272    _link_name = 'task'
-273
-274    def link_task(self, tasks):
-275        self._add_link('task', tasks)
-276
-277    def unlink_task(self, tasks):
-278        self._delete_link('task', tasks)
+295class TaskLinker(BaseLinker):
+296    _link_name = 'task'
+297
+298    def link_task(self, tasks):
+299        self._add_link('task', tasks)
+300
+301    def unlink_task(self, tasks):
+302        self._delete_link('task', tasks)
 TaskLinker()
 ⁰
 def link_task(self, tasks): View Source
-274    def link_task(self, tasks):
-275        self._add_link('task', tasks)
+298    def link_task(self, tasks):
+299        self._add_link('task', tasks)
 ⁰
 def unlink_task(self, tasks): View Source
-277    def unlink_task(self, tasks):
-278        self._delete_link('task', tasks)
+301    def unlink_task(self, tasks):
+302        self._delete_link('task', tasks)
   ⁰
 class TaskTemplateLinker(BaseLinker): View Source
-281class TaskTemplateLinker(BaseLinker):
-282    _link_name = 'task_template'
-283    _link_entity = 'TaskTemplate'
-284
-285    def link_task_template(self, task_templates):
-286        self._add_link('task_template', task_templates)
-287
-288    def unlink_task_template(self, task_templates):
-289        self._delete_link('task_template', task_templates)
+305class TaskTemplateLinker(BaseLinker):
+306    _link_name = 'task_template'
+307    _link_entity = 'TaskTemplate'
+308
+309    def link_task_template(self, task_templates):
+310        self._add_link('task_template', task_templates)
+311
+312    def unlink_task_template(self, task_templates):
+313        self._delete_link('task_template', task_templates)
 TaskTemplateLinker()
 ⁰
 def link_task_template(self, task_templates): View Source
-285    def link_task_template(self, task_templates):
-286        self._add_link('task_template', task_templates)
+309    def link_task_template(self, task_templates):
+310        self._add_link('task_template', task_templates)
 ⁰
 def unlink_task_template(self, task_templates): View Source
-288    def unlink_task_template(self, task_templates):
-289        self._delete_link('task_template', task_templates)
+312    def unlink_task_template(self, task_templates):
+313        self._delete_link('task_template', task_templates)
   ⁰
 class TagLinker(BaseLinker): View Source
-291class TagLinker(BaseLinker):
-292    _link_name = 'tag'
-293
-294    def link_tag(self, tags):
-295        self._add_link('tag', tags)
-296
-297    def unlink_tag(self, tags):
-298        self._delete_link('tag', tags)
+315class TagLinker(BaseLinker):
+316    _link_name = 'tag'
+317
+318    def link_tag(self, tags):
+319        self._add_link('tag', tags)
+320
+321    def unlink_tag(self, tags):
+322        self._delete_link('tag', tags)
 TagLinker()
 ⁰
 def link_tag(self, tags): View Source
-294    def link_tag(self, tags):
-295        self._add_link('tag', tags)
+318    def link_tag(self, tags):
+319        self._add_link('tag', tags)
 ⁰
 def unlink_tag(self, tags): View Source
-297    def unlink_tag(self, tags):
-298        self._delete_link('tag', tags)
+321    def unlink_tag(self, tags):
+322        self._delete_link('tag', tags)
   ⁰
 class NoteLinker(BaseLinker): View Source
-300class NoteLinker(BaseLinker):
-301    _link_name = 'note'
+324class NoteLinker(BaseLinker):
+325    _link_name = 'note'
 NoteLinker()
   ⁰
 class CalendarLinker(BaseLinker): View Source
-303class CalendarLinker(BaseLinker):
-304    _link_name = 'calendar'
+327class CalendarLinker(BaseLinker):
+328    _link_name = 'calendar'
 CalendarLinker()
   ⁰
 class TaskInProjectLinker(BaseLinker): View Source
-308class TaskInProjectLinker(BaseLinker):
-309    _link_name = "task"
+332class TaskInProjectLinker(BaseLinker):
+333    _link_name = "task"
 TaskInProjectLinker()
```

### Comparing `projectal-4.0.1/docs/projectal/profile.html` & `projectal-4.0.2/docs/projectal/profile.html`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/docs/projectal.html` & `projectal-4.0.2/docs/projectal.html`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,24 @@
 details = projectal.auth_details()
 </code></pre>
 
 <hr />
 
 <h2 id="changelog">Changelog</h2>
 
+<h3 id="402">4.0.2</h3>
+
+<ul>
+<li><p>Booking entity is now fetched with project field and either staff or resource field.</p></li>
+<li><p>Added missing link methods for 'Booking' entity (Note, File)</p></li>
+<li><p>Added missing link methods for 'Activity' entity (Booking, Note, File, Rebate)</p></li>
+<li><p>Reduced maximum number of link methods to 100 for a single batch request to prevent timeouts
+under heavy load.</p></li>
+</ul>
+
 <h3 id="401">4.0.1</h3>
 
 <ul>
 <li>Minimum Projectal version is now 4.0.0.</li>
 </ul>
 
 <h3 id="400">4.0.0</h3>
@@ -526,414 +536,424 @@
 </span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a><span class="sd">details = projectal.auth_details()</span>
 </span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a><span class="sd">```</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
 </span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="sd">----</span>
 </span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
 </span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a><span class="sd">## Changelog</span>
 </span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 4.0.1</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">- Minimum Projectal version is now 4.0.0.</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a><span class="sd">### 4.0.2</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="sd">- Booking entity is now fetched with project field and either staff or resource field.</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">### 4.0.0</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a><span class="sd">- Added missing link methods for &#39;Booking&#39; entity (Note, File)</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">Version 4.0.0 accompanies the release of Projectal 4.0.</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">- Added missing link methods for &#39;Activity&#39; entity (Booking, Note, File, Rebate)</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">- Added the `Activity` entity, new in Projectal 4.0.</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a><span class="sd">- Added the `Booking` entity, new in Projectal 4.0.</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">### 3.1.1</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="sd">- Reduced maximum number of link methods to 100 for a single batch request to prevent timeouts</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a><span class="sd">under heavy load.</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">### 4.0.1</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a><span class="sd">- Minimum Projectal version is now 4.0.0.</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="sd">### 4.0.0</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a><span class="sd">Version 4.0.0 accompanies the release of Projectal 4.0.</span>
 </span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">### 3.1.0</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">  from a webhook delete event.</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">  the Projectal server settings.</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    ```</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    resourceList: [</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">        &#39;added&#39;: [],</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">        &#39;updated&#39;: [</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">        ],</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">        &#39;removed&#39;: []</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">    ]</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">    ```</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">  clearly indicated.</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">### 3.0.2</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">### 3.0.1</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="sd">- Added the `Activity` entity, new in Projectal 4.0.</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a><span class="sd">- Added the `Booking` entity, new in Projectal 4.0.</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="sd">### 3.1.1</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a><span class="sd">- Link requests generated by &#39;projectal.Entity.create()&#39; and &#39;projectal.Entity.update()&#39; are now</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="sd">  executed in batches. This is enabled by default with the &#39;batch_linking=True&#39; parameter and can</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="sd">  be disabled to execute each link request individually. It is recommended to leave this parameter</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">  enabled as this can greatly reduce the number of network requests.</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a><span class="sd">### 3.1.0</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a><span class="sd">- Minimum Projectal version is now 3.1.5.</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a><span class="sd">- Added `projectal.Webhook.list_events()`. See API doc for details on how to use.</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="sd">- Added `deleted_at` parameter to `projectal.Entity.get()`. This value should be a UTC timestamp</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">  from a webhook delete event.</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a><span class="sd">- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD service configured in</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">  the Projectal server settings.</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">- Enhanced output of `projectal.Entity.changes()` function when reporting link changes.</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">  It no longer dumps the entire before-and-after list with the full content of each linked entity.</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a><span class="sd">  Now reports three lists: `added`, `updated`, `removed`. Entities within the `updated` list</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a><span class="sd">  follow the same `old` vs `new` dictionary model for the data attributes within them. E.g:</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a><span class="sd">    ```</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="sd">    resourceList: [</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a><span class="sd">        &#39;added&#39;: [],</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="sd">        &#39;updated&#39;: [</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">            {&#39;uuId&#39;: &#39;14eb4c31-0f92-49d1-8b4d-507ab939003e&#39;, &#39;resourceLink&#39;: {&#39;utilization&#39;: {&#39;old&#39;: 0.1, &#39;new&#39;: 0.9}}},</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a><span class="sd">        ],</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a><span class="sd">        &#39;removed&#39;: []</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a><span class="sd">    ]</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="sd">    ```</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="sd">  This should result in slimmer logs that are much easier to understand as the changes are</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a><span class="sd">  clearly indicated.</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a><span class="sd">### 3.0.2</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a><span class="sd">- Added `projectal.Entity.get_link_definitions()`. Exposes entity link definition dictionary.</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="sd">  Consumers can inspect which links an Entity knows about and their internal settings.</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a><span class="sd">  Link definitions that appear here are the links valid for `links=[]` parameters.</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a><span class="sd">### 3.0.1</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a><span class="sd">- Fixed fetching project with links=[&#39;task&#39;] not being available.</span>
 </span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">### 3.0</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a><span class="sd">    ```</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">    # Before:</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">    # Now:</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">    ```</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a><span class="sd">- Improved Permission.list(). Now returns a dict with the permission name as</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a><span class="sd">  key with Permission objects as the value (instead of list of uuIds).</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a><span class="sd">- Added a way to use the aliasing feature of the API (new in Projectal 3.0).</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="sd">Set `projectal.api_alias = &#39;uuid&#39;` to the UUID of a User object and all</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a><span class="sd">requests made will be done as that user. Restore this value to None to resume</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="sd">normal operation. (Some rules and limitations apply. See API for more details.)</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a><span class="sd">- Added complete support for the Tags entity (including linkers).</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a><span class="sd">### 3.0</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="sd">Version 3.0 accompanies the release of Projectal 3.0.</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="sd">**Breaking changes**:</span>
 </span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">  you can now do:</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="sd">    ```</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">    task.save()</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="sd">    ```</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">  capabilities and limitations.</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">    ```</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="sd">- The `links` parameter on `Entity` functions now consumes a list of entity</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="sd">  names instead of a comma-separated string. For example:</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a><span class="sd">    ```</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a><span class="sd">    # Before:</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=&#39;skill,location&#39;)  # No longer valid</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="sd">    # Now:</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a><span class="sd">    projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;, &#39;location&#39;])</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a><span class="sd">    ```</span>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a><span class="sd">- The `projectal.enums.SkillLevel` enum has had all values renamed to match the new values</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="sd">  used in Projectal (Junior, Mid, Senior). This includes the properties on</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a><span class="sd">  Skill entities indicating work time for auto-scheduling (now `juniorLevel`,</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a><span class="sd">  `midLevel`, `seniorLevel`).</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a><span class="sd">- Working with entity links has changed in this release. The previous methods</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="sd">  are still available and continue to work as before, but there is no need</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">  to interact with the `projectal.linkers` methods yourself anymore.</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">  You can now modify the list of links within an entity and save the entity</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a><span class="sd">  directly. The library will automatically determine how the links have been</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">  modified and issue the correct linker methods on your behalf. E.g.,</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">  you can now do:</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    ```</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a><span class="sd">    staff = projectal.Staff.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;skill&#39;])</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">    staff[&#39;firstName&#39;] = &quot;New name&quot;  # Field update</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a><span class="sd">    staff[&#39;skillList&#39;] = [skill1, skill2, skill3]  # Link update</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">    staff.save()  # Both changes are saved</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a><span class="sd">    task = projectal.Task.get(&#39;&lt;uuid&gt;&#39;, links=[&#39;stage&#39;])</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    task[&#39;stage&#39;] = stage1  # Uses a single object instead of list</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a><span class="sd">    task.save()</span>
 </span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    ```</span>
 </span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a><span class="sd">  See `examples/linking.py` for a more complete demonstration of linking</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a><span class="sd">  capabilities and limitations.</span>
 </span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">  writing something like:</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="sd">    ```</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a><span class="sd">    company.link_staff(staff)</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a><span class="sd">    ```</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a><span class="sd">- Linkers (`projectal.linkers`) can now be given a list of Entities (of one</span>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="sd"> type) to link/unlink/relink in bulk. E.g:</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a><span class="sd">    ```</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="sd">    staff.unlink_skill(skill1)  # Before</span>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    staff.unlink_skill([skill1, skill2, skill3])  # This works now too</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a><span class="sd">    ```</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a><span class="sd">- Linkers now strip the payload to only the required fields instead of passing</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="sd">  on the entire Entity object. This cuts down on network traffic significantly.</span>
 </span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">  strictly support it:</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a><span class="sd">- Linkers now also work in reverse. The Projectal server currently only supports</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="sd">  linking entities in one direction (e.g., Company to Staff), which often means</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a><span class="sd">  writing something like:</span>
 </span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">    ```</span>
 </span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">    staff.link_location(location)</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">    staff.link_company(company)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a><span class="sd">    company.link_staff(staff)</span>
 </span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">    ```</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a><span class="sd">  The change in direction is not very intuitive and would require you to constantly</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">  verify which direction is the one available to you in the documentation.</span>
 </span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">  lists, None for dicts).</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">  of a uuId.</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">  Projectal 3.0.</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a><span class="sd">  Reverse linkers hide this from you and figure out the direction of the relationship</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">  for you behind the scenes. So now this is possible, even though the API doesn&#39;t</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a><span class="sd">  strictly support it:</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">    ```</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a><span class="sd">    staff.link_location(location)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a><span class="sd">    staff.link_company(company)</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">    ```</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">    Caveat: the documentation for Staff will not list Company links. You will still</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">    have to look up the Company documentation for the link description.</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">- Requesting entity links with the `links=` parameter will now always ensure the</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">  link field (e.g., `taskList`) exists in the result, even if there are no links.</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">  The server may not always return a value, but we can use a default value ([] for</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">  lists, None for dicts).</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">- Added a `Permission` entity to correctly type Permissions in responses.</span>
 </span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">- Added a `Tag` entity, new in Projectal 3.0.</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a><span class="sd">  returned Task object.</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">  changes for a webhook timestamp.</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">- Added `links` parameter to `Company.get_primary_company()`</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">- `Department.tree()`: now consumes a `holder` Entity object instead</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">  of a uuId.</span>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">- `Department.tree()`: added `generic_staff` parameter, new in</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="sd">  Projectal 3.0.</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a><span class="sd">- Don&#39;t break on trailing slash in Projectal URL</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a><span class="sd">**Known issues**:</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">  ```</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a><span class="sd">  staff.save()</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">  # You must do this for now</span>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">  calendar.save()</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a><span class="sd">- When creating tasks, populate the `projectRef` and `parent` fields in the</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">  returned Task object.</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">- Added convenience functions for matching on fields where you only want</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">  one result (e.g match_one()) which return the first match found.</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">- Update the entity `history()` method for Projectal 3.0. Some new parameters</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a><span class="sd">  allow you to restrict the history to a particular range or to get only the</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">  changes for a webhook timestamp.</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a><span class="sd">- Entity objects can call `.history()` on themselves.</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="sd">- The library now keeps a reference to the User account that is currently logged</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a><span class="sd">  in and using the API: `projectal.api_auth_details`.</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">**Known issues**:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a><span class="sd">- You cannot save changes to Notes or Calendars via their holding entity. You</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">  must save the changes on the Note or Calendar directly. To illustrate:</span>
 </span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a><span class="sd">  ```</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">  This will be resolved in a future release.</span>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">  stored in the database.</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">### 2.1.0</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">  Projectal several versions ago.</span>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">  staff = projectal.Staff.get(&lt;uuid&gt;, links=[&#39;calendar&#39;])</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">  calendar = staff[&#39;calendarList&#39;][0]</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a><span class="sd">  calendar[&#39;name&#39;] = &#39;Calendar 2&#39;</span>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a><span class="sd">  # Cannot do this - will not pick up the changes</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a><span class="sd">  staff.save()</span>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">  # You must do this for now</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a><span class="sd">  calendar.save()</span>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a><span class="sd">  ```</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a><span class="sd">  This will be resolved in a future release.</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a><span class="sd">- When creating Notes, the `created` and `modified` values may differ by</span>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a><span class="sd">  1ms in the object you have a reference to compared to what is actually</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a><span class="sd">  stored in the database.</span>
 </span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">### 2.0.3</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">- Better support for calendars.</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">  the library.</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">  and the new values. E.g.</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">```</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">task.changes()</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">task.changes(old=True)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">```</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">### 2.0.2</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">- Fixed updating Webhook entities</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">### 2.0.1</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">### 2.0.0</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">  since the previous release.</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">  server when an update request is made.</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">### 1.2.0</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a><span class="sd">- Duration calculation is not precise yet (mentioned in 2.1.0)</span>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a><span class="sd">### 2.1.0</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a><span class="sd">- Getting location calendar is now done on an instance instead of class. So</span>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a><span class="sd">  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a><span class="sd">- The `CompanyType.Master` enum has been replaced with `CompanyType.Primary`.</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a><span class="sd">  This was a leftover reference to the Master Company which was renamed in</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a><span class="sd">  Projectal several versions ago.</span>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a><span class="sd">- Date conversion functions return None when given None or empty string</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a><span class="sd">- Added `Task.reset_duration()` as a basic duration calculator for tasks.</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a><span class="sd">  This is a work-in-progress and will be gradually improved. The duration</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a><span class="sd">  calculator takes into consideration the location to remove non-work</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a><span class="sd">  days from the estimate of working duration. It currently does not work</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a><span class="sd">  for the time component or `isWorking=True` exceptions.</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a><span class="sd">- Change detection in `Entity.changes()` now excludes cases where the</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a><span class="sd">  server has no value and the new value is None. Saving this change has</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a><span class="sd">  no effect and would always detect a change until a non-None value is</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a><span class="sd">  set, which is noisy and generates more network activity.</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a><span class="sd">### 2.0.3</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a><span class="sd">- Better support for calendars.</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a><span class="sd">  - Distinguish between calendar containers (&quot;Calendar&quot;) and the</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a><span class="sd">    calendar items within them (&quot;CalendarItem&quot;).</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a><span class="sd">  - Allow CalendarItems to be saved directly. E.G item.save()</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a><span class="sd">- Fix &#39;holder&#39; parameter in contact/staff/location/task_template not</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a><span class="sd">  permitting object type. Now consumes uuId or object to match rest of</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a><span class="sd">  the library.</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a><span class="sd">- `Entity.changes()` has been extended with an `old=True` flag. When</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a><span class="sd">  this flag is true, the set of changes will now return both the original</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a><span class="sd">  and the new values. E.g.</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a><span class="sd">```</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="sd">task.changes()</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd"># {&#39;name&#39;: &#39;current&#39;}</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">task.changes(old=True)</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd"># {&#39;name&#39;: {&#39;old&#39;: &#39;original&#39;, &#39;new&#39;: &#39;current&#39;}}</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">```</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">- Fixed entity link cache causing errors when deleting a link from an entity</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">  which has not been fetched with links (deleting from empty list).</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">### 2.0.2</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a><span class="sd">- Fixed updating Webhook entities</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">### 2.0.1</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">- Fixed application ID not being used correctly.</span>
 </span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">  the database.</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">### 2.0.0</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a><span class="sd">- Version 2.0 accompanies the release of Projectal 2.0. There are no major changes</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">  since the previous release.</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a><span class="sd">- Expose `Entity.changes()` function. It returns a list of fields on an entity that</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">  have changed since fetching it. These are the changes that will be sent over to the</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">  server when an update request is made.</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">- Added missing &#39;packaging&#39; dependency to requirements.</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">### 1.2.0</span>
 </span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">  large request. Values are configurable through</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">  the key and the data. E.g:</span>
-</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a>
-</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a><span class="sd">```</span>
-</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
-</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
-</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">task.profile_set(key, data)</span>
-</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">```</span>
-</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a>
-</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
-</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
-</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
-</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
-</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">  and delete.</span>
-</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a>
-</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
-</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
-</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a><span class="sd">  the object without requesting the link data as well</span>
-</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
-</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
-</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">  while the object is held.</span>
-</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a>
-</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
-</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
-</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
-</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
-</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
-</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a>
-</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
-</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
-</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
-</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
-</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a><span class="sd">  server after creation.</span>
-</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a>
-</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
-</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
-</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">  created objects without triggering this error.</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a><span class="sd">- Renamed `request_timestamp` to `response_timestamp` to better reflect its purpose.</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="sd">- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been reverted.</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="sd">  All date fields returned from the server remain as UTC timestamps.</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a><span class="sd">  The reason is that date fields on tasks contain a time component and converting them</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="sd">  into date strings was erasing the time, resulting in a value that does not match</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="sd">  the database.</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a><span class="sd">  Note: the server supports setting date fields using a date string like `2022-04-05`.</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a><span class="sd">  You may use this if you prefer but the server will always return a timestamp.</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a><span class="sd">  Note: we provide utility functions for easily converting dates from/to</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="sd">  timestamps expected by the Projectal server. See:</span>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a><span class="sd">  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and</span>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="sd">  `projectal.timestamp_from_datetime()`.</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>
+</span><span id="L-306"><a href="#L-306"><span class="linenos">306</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-307"><a href="#L-307"><span class="linenos">307</span></a><span class="sd">- Implement request chunking - for methods that consume a list of entities, we now</span>
+</span><span id="L-308"><a href="#L-308"><span class="linenos">308</span></a><span class="sd">  automatically batch them up into multiple requests to prevent timeouts on really</span>
+</span><span id="L-309"><a href="#L-309"><span class="linenos">309</span></a><span class="sd">  large request. Values are configurable through</span>
+</span><span id="L-310"><a href="#L-310"><span class="linenos">310</span></a><span class="sd">  `projectal.chunk_size_read` and `projectal.chunk_size_write`.</span>
+</span><span id="L-311"><a href="#L-311"><span class="linenos">311</span></a><span class="sd">  Default values: Read: 1000 items. Write: 200 items.</span>
+</span><span id="L-312"><a href="#L-312"><span class="linenos">312</span></a><span class="sd">- Added profile get/set functions on entities for easier use. Now you only need to supply</span>
+</span><span id="L-313"><a href="#L-313"><span class="linenos">313</span></a><span class="sd">  the key and the data. E.g:</span>
+</span><span id="L-314"><a href="#L-314"><span class="linenos">314</span></a>
+</span><span id="L-315"><a href="#L-315"><span class="linenos">315</span></a><span class="sd">```</span>
+</span><span id="L-316"><a href="#L-316"><span class="linenos">316</span></a><span class="sd">key = &#39;hr_connector&#39;</span>
+</span><span id="L-317"><a href="#L-317"><span class="linenos">317</span></a><span class="sd">data = {&#39;staff_source&#39;: &#39;company_z&#39;}</span>
+</span><span id="L-318"><a href="#L-318"><span class="linenos">318</span></a><span class="sd">task.profile_set(key, data)</span>
+</span><span id="L-319"><a href="#L-319"><span class="linenos">319</span></a><span class="sd">```</span>
+</span><span id="L-320"><a href="#L-320"><span class="linenos">320</span></a>
+</span><span id="L-321"><a href="#L-321"><span class="linenos">321</span></a><span class="sd">- Entity link methods now automatically update the entity&#39;s cached list of links. E.g:</span>
+</span><span id="L-322"><a href="#L-322"><span class="linenos">322</span></a><span class="sd">  a task fetched with staff links will have `task[&#39;staffList&#39;] = [Staff1,Staff2]`.</span>
+</span><span id="L-323"><a href="#L-323"><span class="linenos">323</span></a><span class="sd">  Before, doing a `task.link_staff(staff)` did not modify the list to reflect the</span>
+</span><span id="L-324"><a href="#L-324"><span class="linenos">324</span></a><span class="sd">  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same applies for update</span>
+</span><span id="L-325"><a href="#L-325"><span class="linenos">325</span></a><span class="sd">  and delete.</span>
+</span><span id="L-326"><a href="#L-326"><span class="linenos">326</span></a>
+</span><span id="L-327"><a href="#L-327"><span class="linenos">327</span></a><span class="sd">  This allows you to modify links and continue working with that object without having</span>
+</span><span id="L-328"><a href="#L-328"><span class="linenos">328</span></a><span class="sd">  to fetch it again to obtain the most recent link data. Be aware that if you acquire</span>
+</span><span id="L-329"><a href="#L-329"><span class="linenos">329</span></a><span class="sd">  the object without requesting the link data as well</span>
+</span><span id="L-330"><a href="#L-330"><span class="linenos">330</span></a><span class="sd">  (e.g: `projectal.Task.get(id, links=&#39;STAFF&#39;)`),</span>
+</span><span id="L-331"><a href="#L-331"><span class="linenos">331</span></a><span class="sd">  these lists will not accurately reflect what&#39;s in the database, only the changes made</span>
+</span><span id="L-332"><a href="#L-332"><span class="linenos">332</span></a><span class="sd">  while the object is held.</span>
+</span><span id="L-333"><a href="#L-333"><span class="linenos">333</span></a>
+</span><span id="L-334"><a href="#L-334"><span class="linenos">334</span></a><span class="sd">- Support new `applicationId` property on login. Set with: `projectal.api_application_id`.</span>
+</span><span id="L-335"><a href="#L-335"><span class="linenos">335</span></a><span class="sd">  The application ID is sent back to you in webhooks so you know which application was</span>
+</span><span id="L-336"><a href="#L-336"><span class="linenos">336</span></a><span class="sd">  the source of the event (and you can choose to filter them accordingly).</span>
+</span><span id="L-337"><a href="#L-337"><span class="linenos">337</span></a><span class="sd">- Added `Entity.set_readonly()` to allow setting values on entities that will not</span>
+</span><span id="L-338"><a href="#L-338"><span class="linenos">338</span></a><span class="sd">  be sent over to the server when updating/saving the entity.</span>
 </span><span id="L-339"><a href="#L-339"><span class="linenos">339</span></a>
-</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
-</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a>
-</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a>
-</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">### 1.1.1</span>
-</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
-</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a><span class="sd">  any entity. Not currently documented.</span>
-</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
-</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
-</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
-</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
-</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
-</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a><span class="sd">  if no timestamp in response)</span>
+</span><span id="L-340"><a href="#L-340"><span class="linenos">340</span></a><span class="sd">  The main use case for this is to populate cached entities which you have just created</span>
+</span><span id="L-341"><a href="#L-341"><span class="linenos">341</span></a><span class="sd">  with values you already know about. This is mainly a workaround for the limitation of</span>
+</span><span id="L-342"><a href="#L-342"><span class="linenos">342</span></a><span class="sd">  the server not sending the full object back after creating it, resulting in the client</span>
+</span><span id="L-343"><a href="#L-343"><span class="linenos">343</span></a><span class="sd">  needing to fetch the object in full again if it needs some of the fields set by the</span>
+</span><span id="L-344"><a href="#L-344"><span class="linenos">344</span></a><span class="sd">  server after creation.</span>
+</span><span id="L-345"><a href="#L-345"><span class="linenos">345</span></a>
+</span><span id="L-346"><a href="#L-346"><span class="linenos">346</span></a><span class="sd">  Additionally, some read-only fields will generate an error on the server if</span>
+</span><span id="L-347"><a href="#L-347"><span class="linenos">347</span></a><span class="sd">  included in the update request. This method lets you set these values on newly</span>
+</span><span id="L-348"><a href="#L-348"><span class="linenos">348</span></a><span class="sd">  created objects without triggering this error.</span>
+</span><span id="L-349"><a href="#L-349"><span class="linenos">349</span></a>
+</span><span id="L-350"><a href="#L-350"><span class="linenos">350</span></a><span class="sd">  A common example is setting the `projectRef` of a task you just created.</span>
+</span><span id="L-351"><a href="#L-351"><span class="linenos">351</span></a>
 </span><span id="L-352"><a href="#L-352"><span class="linenos">352</span></a>
-</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">### 1.1.0</span>
-</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
-</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a>
-</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">**Breaking changes**:</span>
-</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
-</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
-</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
-</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
-</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a><span class="sd">  down to only the tasks and fields you need.</span>
-</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
-</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">  to match the server.</span>
-</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
-</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
-</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
-</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
-</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
-</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a>
-</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">**Other changes**:</span>
-</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
-</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
-</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
-</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
-</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
-</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
-</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
-</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
-</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
-</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>
-</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">### 1.0.3</span>
-</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
-</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a>
-</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">### 1.0.2</span>
-</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
-</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
-</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>
-</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="sd">### 1.0.1</span>
-</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="sd">- Added `list()` function for all entities</span>
-</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
-</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="sd">- Added `Company.get_master_company()`</span>
-</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a><span class="sd">- Fixed adding template tasks</span>
-</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a>
-</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a><span class="sd">&quot;&quot;&quot;</span>
-</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="kn">import</span> <span class="nn">logging</span>
-</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-353"><a href="#L-353"><span class="linenos">353</span></a><span class="sd">### 1.1.1</span>
+</span><span id="L-354"><a href="#L-354"><span class="linenos">354</span></a><span class="sd">- Add support for &#39;profiles&#39; API. Profiles are a type of key-value storage that target</span>
+</span><span id="L-355"><a href="#L-355"><span class="linenos">355</span></a><span class="sd">  any entity. Not currently documented.</span>
+</span><span id="L-356"><a href="#L-356"><span class="linenos">356</span></a><span class="sd">- Fix handling error message parsing in ProjectalException for batch create operation</span>
+</span><span id="L-357"><a href="#L-357"><span class="linenos">357</span></a><span class="sd">- Add `Task.update_order()` to set task order</span>
+</span><span id="L-358"><a href="#L-358"><span class="linenos">358</span></a><span class="sd">- Return empty list when GETing empty list instead of failing (no request to server)</span>
+</span><span id="L-359"><a href="#L-359"><span class="linenos">359</span></a><span class="sd">- Expose the timestamp returned by requests that modify the database. Use</span>
+</span><span id="L-360"><a href="#L-360"><span class="linenos">360</span></a><span class="sd">  `projectal.request_timestamp` to get the value of the most recent request (None</span>
+</span><span id="L-361"><a href="#L-361"><span class="linenos">361</span></a><span class="sd">  if no timestamp in response)</span>
+</span><span id="L-362"><a href="#L-362"><span class="linenos">362</span></a>
+</span><span id="L-363"><a href="#L-363"><span class="linenos">363</span></a><span class="sd">### 1.1.0</span>
+</span><span id="L-364"><a href="#L-364"><span class="linenos">364</span></a><span class="sd">- Minimum Projectal version is now 1.9.4.</span>
+</span><span id="L-365"><a href="#L-365"><span class="linenos">365</span></a>
+</span><span id="L-366"><a href="#L-366"><span class="linenos">366</span></a><span class="sd">**Breaking changes**:</span>
+</span><span id="L-367"><a href="#L-367"><span class="linenos">367</span></a><span class="sd">- Entity `list()` now returns a list of UUIDs instead of full objects. You may provide</span>
+</span><span id="L-368"><a href="#L-368"><span class="linenos">368</span></a><span class="sd">  an `expand` parameter to restore the previous behavior: `Entity.list(expand=True)`.</span>
+</span><span id="L-369"><a href="#L-369"><span class="linenos">369</span></a><span class="sd">  This change is made for performance reasons where you may have thousands of tasks</span>
+</span><span id="L-370"><a href="#L-370"><span class="linenos">370</span></a><span class="sd">  and getting them all may time out. For those cases, we suggest writing a query to filter</span>
+</span><span id="L-371"><a href="#L-371"><span class="linenos">371</span></a><span class="sd">  down to only the tasks and fields you need.</span>
+</span><span id="L-372"><a href="#L-372"><span class="linenos">372</span></a><span class="sd">- `Company.get_master_company()` has been renamed to `Company.get_primary_company()`</span>
+</span><span id="L-373"><a href="#L-373"><span class="linenos">373</span></a><span class="sd">  to match the server.</span>
+</span><span id="L-374"><a href="#L-374"><span class="linenos">374</span></a><span class="sd">- The following date fields are converted into date strings upon fetch:</span>
+</span><span id="L-375"><a href="#L-375"><span class="linenos">375</span></a><span class="sd">  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.</span>
+</span><span id="L-376"><a href="#L-376"><span class="linenos">376</span></a><span class="sd">  These fields are added or updated using date strings (like `2022-03-02`), but the</span>
+</span><span id="L-377"><a href="#L-377"><span class="linenos">377</span></a><span class="sd">  server returns timestamps (e.g: 1646006400000) upon fetch, which is confusing. This</span>
+</span><span id="L-378"><a href="#L-378"><span class="linenos">378</span></a><span class="sd">  change ensures they are always date strings for consistency.</span>
+</span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a>
+</span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a><span class="sd">**Other changes**:</span>
+</span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">- When updating an entity, only the fields that have changed are sent to the server. When</span>
+</span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a><span class="sd">  updating a list of entities, unmodified entities are not sent to the server at all. This</span>
+</span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a><span class="sd">  dramatically reduces the payload size and should speed things up.</span>
+</span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">- When fetching entities, entity links are now typed as well. E.g. `project[&#39;rebateList&#39;]`</span>
+</span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">  contains a list of `Rebate` instead of `dict`.</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a><span class="sd">- Added `date_from_timestamp()` and `timestamp_from_date()` functions to help with</span>
+</span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a><span class="sd">  converting to/from dates and Projectal timestamps.</span>
+</span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a><span class="sd">- Entity history now uses `desc` by default (index 0 is newest)</span>
+</span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a><span class="sd">- Added `Project.tasks()` to list all task UUIDs within a project.</span>
+</span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a>
+</span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a><span class="sd">### 1.0.3</span>
+</span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a><span class="sd">- Fix another case of automatic JWT refresh not working</span>
+</span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>
+</span><span id="L-394"><a href="#L-394"><span class="linenos">394</span></a><span class="sd">### 1.0.2</span>
+</span><span id="L-395"><a href="#L-395"><span class="linenos">395</span></a><span class="sd">- Entity instances can `save()` or `delete()` on themselves</span>
+</span><span id="L-396"><a href="#L-396"><span class="linenos">396</span></a><span class="sd">- Fix broken `dict` methods (`get()` and `update()`) when called from Entity instances</span>
+</span><span id="L-397"><a href="#L-397"><span class="linenos">397</span></a><span class="sd">- Fix automatic JWT refresh only working in some cases</span>
 </span><span id="L-398"><a href="#L-398"><span class="linenos">398</span></a>
-</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
-</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
-</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a>
-</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_URL&#39;</span><span class="p">)</span>
-</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_USERNAME&#39;</span><span class="p">)</span>
-</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_PASSWORD&#39;</span><span class="p">)</span>
-</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
-</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
+</span><span id="L-399"><a href="#L-399"><span class="linenos">399</span></a><span class="sd">### 1.0.1</span>
+</span><span id="L-400"><a href="#L-400"><span class="linenos">400</span></a><span class="sd">- Added `list()` function for all entities</span>
+</span><span id="L-401"><a href="#L-401"><span class="linenos">401</span></a><span class="sd">- Added search functions for all entities (match-, search, query)</span>
+</span><span id="L-402"><a href="#L-402"><span class="linenos">402</span></a><span class="sd">- Added `Company.get_master_company()`</span>
+</span><span id="L-403"><a href="#L-403"><span class="linenos">403</span></a><span class="sd">- Fixed adding template tasks</span>
+</span><span id="L-404"><a href="#L-404"><span class="linenos">404</span></a>
+</span><span id="L-405"><a href="#L-405"><span class="linenos">405</span></a><span class="sd">&quot;&quot;&quot;</span>
+</span><span id="L-406"><a href="#L-406"><span class="linenos">406</span></a><span class="kn">import</span> <span class="nn">logging</span>
+</span><span id="L-407"><a href="#L-407"><span class="linenos">407</span></a><span class="kn">import</span> <span class="nn">os</span>
+</span><span id="L-408"><a href="#L-408"><span class="linenos">408</span></a>
+</span><span id="L-409"><a href="#L-409"><span class="linenos">409</span></a><span class="kn">from</span> <span class="nn">projectal.entities</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-410"><a href="#L-410"><span class="linenos">410</span></a><span class="kn">from</span> <span class="nn">.api</span> <span class="kn">import</span> <span class="o">*</span>
+</span><span id="L-411"><a href="#L-411"><span class="linenos">411</span></a><span class="kn">from</span> <span class="nn">.</span> <span class="kn">import</span> <span class="n">profile</span>
 </span><span id="L-412"><a href="#L-412"><span class="linenos">412</span></a>
-</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
-</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
-</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
-</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a>
-</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a>
-</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
-</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
-</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a><span class="c1"># raise an exception.</span>
-</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4.0.0&quot;</span>
-</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a>
-</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
-</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a>
-</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s1">&#39;projectal-api-client&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
+</span><span id="L-413"><a href="#L-413"><span class="linenos">413</span></a><span class="n">api_base</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_URL&#39;</span><span class="p">)</span>
+</span><span id="L-414"><a href="#L-414"><span class="linenos">414</span></a><span class="n">api_username</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_USERNAME&#39;</span><span class="p">)</span>
+</span><span id="L-415"><a href="#L-415"><span class="linenos">415</span></a><span class="n">api_password</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;PROJECTAL_PASSWORD&#39;</span><span class="p">)</span>
+</span><span id="L-416"><a href="#L-416"><span class="linenos">416</span></a><span class="n">api_application_id</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-417"><a href="#L-417"><span class="linenos">417</span></a><span class="n">api_auth_details</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-418"><a href="#L-418"><span class="linenos">418</span></a><span class="n">api_alias</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-419"><a href="#L-419"><span class="linenos">419</span></a><span class="n">cookies</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-420"><a href="#L-420"><span class="linenos">420</span></a><span class="n">chunk_size_read</span> <span class="o">=</span> <span class="mi">1000</span>
+</span><span id="L-421"><a href="#L-421"><span class="linenos">421</span></a><span class="n">chunk_size_write</span> <span class="o">=</span> <span class="mi">200</span>
+</span><span id="L-422"><a href="#L-422"><span class="linenos">422</span></a>
+</span><span id="L-423"><a href="#L-423"><span class="linenos">423</span></a><span class="c1"># Records the timestamp generated by the last request (database</span>
+</span><span id="L-424"><a href="#L-424"><span class="linenos">424</span></a><span class="c1"># event time). These are reported on add or updates; if there is</span>
+</span><span id="L-425"><a href="#L-425"><span class="linenos">425</span></a><span class="c1"># no timestamp in the response, this is set to None.</span>
+</span><span id="L-426"><a href="#L-426"><span class="linenos">426</span></a><span class="n">response_timestamp</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-427"><a href="#L-427"><span class="linenos">427</span></a>
+</span><span id="L-428"><a href="#L-428"><span class="linenos">428</span></a>
+</span><span id="L-429"><a href="#L-429"><span class="linenos">429</span></a><span class="c1"># The minimum version number of the Projectal instance that this</span>
+</span><span id="L-430"><a href="#L-430"><span class="linenos">430</span></a><span class="c1"># API client targets. Lower versions are not supported and will</span>
+</span><span id="L-431"><a href="#L-431"><span class="linenos">431</span></a><span class="c1"># raise an exception.</span>
+</span><span id="L-432"><a href="#L-432"><span class="linenos">432</span></a><span class="n">MIN_PROJECTAL_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4.0.0&quot;</span>
+</span><span id="L-433"><a href="#L-433"><span class="linenos">433</span></a>
+</span><span id="L-434"><a href="#L-434"><span class="linenos">434</span></a><span class="n">__verify</span> <span class="o">=</span> <span class="kc">True</span>
+</span><span id="L-435"><a href="#L-435"><span class="linenos">435</span></a>
+</span><span id="L-436"><a href="#L-436"><span class="linenos">436</span></a><span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s1">&#39;projectal-api-client&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">addHandler</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">NullHandler</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
     </main>
 <script>
     function escapeHTML(html) {
```

#### html2text {}

```diff
@@ -31,14 +31,22 @@
 status = projectal.status()
 
 # Test account credentials
 projectal.login()
 details = projectal.auth_details()
 ===============================================================================
 ***** Changelog *****
+**** 4.0.2 ****
+    * Booking entity is now fetched with project field and either staff or
+      resource field.
+    * Added missing link methods for 'Booking' entity (Note, File)
+    * Added missing link methods for 'Activity' entity (Booking, Note, File,
+      Rebate)
+    * Reduced maximum number of link methods to 100 for a single batch request
+      to prevent timeouts under heavy load.
 **** 4.0.1 ****
     * Minimum Projectal version is now 4.0.0.
 **** 4.0.0 ****
 Version 4.0.0 accompanies the release of Projectal 4.0.
     * Added the Activity entity, new in Projectal 4.0.
     * Added the Booking entity, new in Projectal 4.0.
 **** 3.1.1 ****
@@ -351,487 +359,500 @@
 _20details = projectal.auth_details()
 _21```
 _22
 _23----
 _24
 _25## Changelog
 _26
-_27### 4.0.1
-_28- Minimum Projectal version is now 4.0.0.
+_27### 4.0.2
+_28- Booking entity is now fetched with project field and either staff or
+resource field.
 _29
-_30### 4.0.0
+_30- Added missing link methods for 'Booking' entity (Note, File)
 _31
-_32Version 4.0.0 accompanies the release of Projectal 4.0.
+_32- Added missing link methods for 'Activity' entity (Booking, Note, File,
+Rebate)
 _33
-_34- Added the `Activity` entity, new in Projectal 4.0.
-_35
-_36- Added the `Booking` entity, new in Projectal 4.0.
-_37
-_38### 3.1.1
-_39- Link requests generated by 'projectal.Entity.create()' and
+_34- Reduced maximum number of link methods to 100 for a single batch request
+to prevent timeouts
+_35under heavy load.
+_36
+_37### 4.0.1
+_38- Minimum Projectal version is now 4.0.0.
+_39
+_40### 4.0.0
+_41
+_42Version 4.0.0 accompanies the release of Projectal 4.0.
+_43
+_44- Added the `Activity` entity, new in Projectal 4.0.
+_45
+_46- Added the `Booking` entity, new in Projectal 4.0.
+_47
+_48### 3.1.1
+_49- Link requests generated by 'projectal.Entity.create()' and
 'projectal.Entity.update()' are now
-_40  executed in batches. This is enabled by default with the
+_50  executed in batches. This is enabled by default with the
 'batch_linking=True' parameter and can
-_41  be disabled to execute each link request individually. It is recommended
+_51  be disabled to execute each link request individually. It is recommended
 to leave this parameter
-_42  enabled as this can greatly reduce the number of network requests.
-_43
-_44### 3.1.0
-_45- Minimum Projectal version is now 3.1.5.
-_46
-_47- Added `projectal.Webhook.list_events()`. See API doc for details on how to
+_52  enabled as this can greatly reduce the number of network requests.
+_53
+_54### 3.1.0
+_55- Minimum Projectal version is now 3.1.5.
+_56
+_57- Added `projectal.Webhook.list_events()`. See API doc for details on how to
 use.
-_48
-_49- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
+_58
+_59- Added `deleted_at` parameter to `projectal.Entity.get()`. This value
 should be a UTC timestamp
-_50  from a webhook delete event.
-_51
-_52- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
+_60  from a webhook delete event.
+_61
+_62- Added `projectal.ldap_sync()` to initiate a user sync with the LDAP/AD
 service configured in
-_53  the Projectal server settings.
-_54
-_55- Enhanced output of `projectal.Entity.changes()` function when reporting
+_63  the Projectal server settings.
+_64
+_65- Enhanced output of `projectal.Entity.changes()` function when reporting
 link changes.
-_56  It no longer dumps the entire before-and-after list with the full content
+_66  It no longer dumps the entire before-and-after list with the full content
 of each linked entity.
-_57  Now reports three lists: `added`, `updated`, `removed`. Entities within
+_67  Now reports three lists: `added`, `updated`, `removed`. Entities within
 the `updated` list
-_58  follow the same `old` vs `new` dictionary model for the data attributes
+_68  follow the same `old` vs `new` dictionary model for the data attributes
 within them. E.g:
-_59
-_60    ```
-_61    resourceList: [
-_62        'added': [],
-_63        'updated': [
-_64            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
+_69
+_70    ```
+_71    resourceList: [
+_72        'added': [],
+_73        'updated': [
+_74            {'uuId': '14eb4c31-0f92-49d1-8b4d-507ab939003e', 'resourceLink':
 {'utilization': {'old': 0.1, 'new': 0.9}}},
-_65        ],
-_66        'removed': []
-_67    ]
-_68    ```
-_69  This should result in slimmer logs that are much easier to understand as
+_75        ],
+_76        'removed': []
+_77    ]
+_78    ```
+_79  This should result in slimmer logs that are much easier to understand as
 the changes are
-_70  clearly indicated.
-_71
-_72### 3.0.2
-_73- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
+_80  clearly indicated.
+_81
+_82### 3.0.2
+_83- Added `projectal.Entity.get_link_definitions()`. Exposes entity link
 definition dictionary.
-_74  Consumers can inspect which links an Entity knows about and their internal
+_84  Consumers can inspect which links an Entity knows about and their internal
 settings.
-_75  Link definitions that appear here are the links valid for `links=[]`
+_85  Link definitions that appear here are the links valid for `links=[]`
 parameters.
-_76
-_77### 3.0.1
-_78- Fixed fetching project with links=['task'] not being available.
-_79
-_80- Improved Permission.list(). Now returns a dict with the permission name as
-_81  key with Permission objects as the value (instead of list of uuIds).
-_82
-_83- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
-_84Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
-_85requests made will be done as that user. Restore this value to None to
+_86
+_87### 3.0.1
+_88- Fixed fetching project with links=['task'] not being available.
+_89
+_90- Improved Permission.list(). Now returns a dict with the permission name as
+_91  key with Permission objects as the value (instead of list of uuIds).
+_92
+_93- Added a way to use the aliasing feature of the API (new in Projectal 3.0).
+_94Set `projectal.api_alias = 'uuid'` to the UUID of a User object and all
+_95requests made will be done as that user. Restore this value to None to
 resume
-_86normal operation. (Some rules and limitations apply. See API for more
+_96normal operation. (Some rules and limitations apply. See API for more
 details.)
-_87
-_88- Added complete support for the Tags entity (including linkers).
-_89
-_90### 3.0
-_91
-_92Version 3.0 accompanies the release of Projectal 3.0.
-_93
-_94**Breaking changes**:
-_95
-_96- The `links` parameter on `Entity` functions now consumes a list of entity
-_97  names instead of a comma-separated string. For example:
-_98
-_99    ```
-100    # Before:
-101    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
-102    # Now:
-103    projectal.Staff.get('<uuid>', links=['skill', 'location'])
-104    ```
+_97
+_98- Added complete support for the Tags entity (including linkers).
+_99
+100### 3.0
+101
+102Version 3.0 accompanies the release of Projectal 3.0.
+103
+104**Breaking changes**:
 105
-106- The `projectal.enums.SkillLevel` enum has had all values renamed to match
+106- The `links` parameter on `Entity` functions now consumes a list of entity
+107  names instead of a comma-separated string. For example:
+108
+109    ```
+110    # Before:
+111    projectal.Staff.get('<uuid>', links='skill,location')  # No longer valid
+112    # Now:
+113    projectal.Staff.get('<uuid>', links=['skill', 'location'])
+114    ```
+115
+116- The `projectal.enums.SkillLevel` enum has had all values renamed to match
 the new values
-107  used in Projectal (Junior, Mid, Senior). This includes the properties on
-108  Skill entities indicating work time for auto-scheduling (now
+117  used in Projectal (Junior, Mid, Senior). This includes the properties on
+118  Skill entities indicating work time for auto-scheduling (now
 `juniorLevel`,
-109  `midLevel`, `seniorLevel`).
-110
-111**Other changes**:
-112
-113- Working with entity links has changed in this release. The previous
+119  `midLevel`, `seniorLevel`).
+120
+121**Other changes**:
+122
+123- Working with entity links has changed in this release. The previous
 methods
-114  are still available and continue to work as before, but there is no need
-115  to interact with the `projectal.linkers` methods yourself anymore.
-116
-117  You can now modify the list of links within an entity and save the entity
-118  directly. The library will automatically determine how the links have been
-119  modified and issue the correct linker methods on your behalf. E.g.,
-120  you can now do:
-121
-122    ```
-123    staff = projectal.Staff.get('<uuid>', links=['skill'])
-124    staff['firstName'] = "New name"  # Field update
-125    staff['skillList'] = [skill1, skill2, skill3]  # Link update
-126    staff.save()  # Both changes are saved
-127
-128    task = projectal.Task.get('<uuid>', links=['stage'])
-129    task['stage'] = stage1  # Uses a single object instead of list
-130    task.save()
-131    ```
-132
-133  See `examples/linking.py` for a more complete demonstration of linking
-134  capabilities and limitations.
-135
-136- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
-137 type) to link/unlink/relink in bulk. E.g:
-138    ```
-139    staff.unlink_skill(skill1)  # Before
-140    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
+124  are still available and continue to work as before, but there is no need
+125  to interact with the `projectal.linkers` methods yourself anymore.
+126
+127  You can now modify the list of links within an entity and save the entity
+128  directly. The library will automatically determine how the links have been
+129  modified and issue the correct linker methods on your behalf. E.g.,
+130  you can now do:
+131
+132    ```
+133    staff = projectal.Staff.get('<uuid>', links=['skill'])
+134    staff['firstName'] = "New name"  # Field update
+135    staff['skillList'] = [skill1, skill2, skill3]  # Link update
+136    staff.save()  # Both changes are saved
+137
+138    task = projectal.Task.get('<uuid>', links=['stage'])
+139    task['stage'] = stage1  # Uses a single object instead of list
+140    task.save()
 141    ```
 142
-143- Linkers now strip the payload to only the required fields instead of
+143  See `examples/linking.py` for a more complete demonstration of linking
+144  capabilities and limitations.
+145
+146- Linkers (`projectal.linkers`) can now be given a list of Entities (of one
+147 type) to link/unlink/relink in bulk. E.g:
+148    ```
+149    staff.unlink_skill(skill1)  # Before
+150    staff.unlink_skill([skill1, skill2, skill3])  # This works now too
+151    ```
+152
+153- Linkers now strip the payload to only the required fields instead of
 passing
-144  on the entire Entity object. This cuts down on network traffic
+154  on the entire Entity object. This cuts down on network traffic
 significantly.
-145
-146- Linkers now also work in reverse. The Projectal server currently only
+155
+156- Linkers now also work in reverse. The Projectal server currently only
 supports
-147  linking entities in one direction (e.g., Company to Staff), which often
+157  linking entities in one direction (e.g., Company to Staff), which often
 means
-148  writing something like:
-149    ```
-150    staff.link_location(location)
-151    company.link_staff(staff)
-152    ```
-153  The change in direction is not very intuitive and would require you to
-constantly
-154  verify which direction is the one available to you in the documentation.
-155
-156  Reverse linkers hide this from you and figure out the direction of the
-relationship
-157  for you behind the scenes. So now this is possible, even though the API
-doesn't
-158  strictly support it:
+158  writing something like:
 159    ```
 160    staff.link_location(location)
-161    staff.link_company(company)
+161    company.link_staff(staff)
 162    ```
-163    Caveat: the documentation for Staff will not list Company links. You
-will still
-164    have to look up the Company documentation for the link description.
+163  The change in direction is not very intuitive and would require you to
+constantly
+164  verify which direction is the one available to you in the documentation.
 165
-166- Requesting entity links with the `links=` parameter will now always ensure
+166  Reverse linkers hide this from you and figure out the direction of the
+relationship
+167  for you behind the scenes. So now this is possible, even though the API
+doesn't
+168  strictly support it:
+169    ```
+170    staff.link_location(location)
+171    staff.link_company(company)
+172    ```
+173    Caveat: the documentation for Staff will not list Company links. You
+will still
+174    have to look up the Company documentation for the link description.
+175
+176- Requesting entity links with the `links=` parameter will now always ensure
 the
-167  link field (e.g., `taskList`) exists in the result, even if there are no
+177  link field (e.g., `taskList`) exists in the result, even if there are no
 links.
-168  The server may not always return a value, but we can use a default value (
+178  The server may not always return a value, but we can use a default value (
 [] for
-169  lists, None for dicts).
-170
-171- Added a `Permission` entity to correctly type Permissions in responses.
-172
-173- Added a `Tag` entity, new in Projectal 3.0.
-174
-175- Added `links` parameter to `Company.get_primary_company()`
-176
-177- `Department.tree()`: now consumes a `holder` Entity object instead
-178  of a uuId.
-179
-180- `Department.tree()`: added `generic_staff` parameter, new in
-181  Projectal 3.0.
+179  lists, None for dicts).
+180
+181- Added a `Permission` entity to correctly type Permissions in responses.
 182
-183- Don't break on trailing slash in Projectal URL
+183- Added a `Tag` entity, new in Projectal 3.0.
 184
-185- When creating tasks, populate the `projectRef` and `parent` fields in the
-186  returned Task object.
-187
-188- Added convenience functions for matching on fields where you only want
-189  one result (e.g match_one()) which return the first match found.
-190
-191- Update the entity `history()` method for Projectal 3.0. Some new
-parameters
-192  allow you to restrict the history to a particular range or to get only the
-193  changes for a webhook timestamp.
+185- Added `links` parameter to `Company.get_primary_company()`
+186
+187- `Department.tree()`: now consumes a `holder` Entity object instead
+188  of a uuId.
+189
+190- `Department.tree()`: added `generic_staff` parameter, new in
+191  Projectal 3.0.
+192
+193- Don't break on trailing slash in Projectal URL
 194
-195- Entity objects can call `.history()` on themselves.
-196
-197- The library now keeps a reference to the User account that is currently
+195- When creating tasks, populate the `projectRef` and `parent` fields in the
+196  returned Task object.
+197
+198- Added convenience functions for matching on fields where you only want
+199  one result (e.g match_one()) which return the first match found.
+200
+201- Update the entity `history()` method for Projectal 3.0. Some new
+parameters
+202  allow you to restrict the history to a particular range or to get only the
+203  changes for a webhook timestamp.
+204
+205- Entity objects can call `.history()` on themselves.
+206
+207- The library now keeps a reference to the User account that is currently
 logged
-198  in and using the API: `projectal.api_auth_details`.
-199
-200**Known issues**:
-201- You cannot save changes to Notes or Calendars via their holding entity.
+208  in and using the API: `projectal.api_auth_details`.
+209
+210**Known issues**:
+211- You cannot save changes to Notes or Calendars via their holding entity.
 You
-202  must save the changes on the Note or Calendar directly. To illustrate:
-203  ```
-204  staff = projectal.Staff.get(<uuid>, links=['calendar'])
-205  calendar = staff['calendarList'][0]
-206  calendar['name'] = 'Calendar 2'
-207
-208  # Cannot do this - will not pick up the changes
-209  staff.save()
-210
-211  # You must do this for now
-212  calendar.save()
+212  must save the changes on the Note or Calendar directly. To illustrate:
 213  ```
-214  This will be resolved in a future release.
-215
-216- When creating Notes, the `created` and `modified` values may differ by
-217  1ms in the object you have a reference to compared to what is actually
-218  stored in the database.
-219
-220- Duration calculation is not precise yet (mentioned in 2.1.0)
-221
-222### 2.1.0
-223**Breaking changes**:
-224- Getting location calendar is now done on an instance instead of class. So
-225  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
-226- The `CompanyType.Master` enum has been replaced with
-`CompanyType.Primary`.
-227  This was a leftover reference to the Master Company which was renamed in
-228  Projectal several versions ago.
+214  staff = projectal.Staff.get(<uuid>, links=['calendar'])
+215  calendar = staff['calendarList'][0]
+216  calendar['name'] = 'Calendar 2'
+217
+218  # Cannot do this - will not pick up the changes
+219  staff.save()
+220
+221  # You must do this for now
+222  calendar.save()
+223  ```
+224  This will be resolved in a future release.
+225
+226- When creating Notes, the `created` and `modified` values may differ by
+227  1ms in the object you have a reference to compared to what is actually
+228  stored in the database.
 229
-230**Other changes**:
-231- Date conversion functions return None when given None or empty string
-232- Added `Task.reset_duration()` as a basic duration calculator for tasks.
-233  This is a work-in-progress and will be gradually improved. The duration
-234  calculator takes into consideration the location to remove non-work
-235  days from the estimate of working duration. It currently does not work
-236  for the time component or `isWorking=True` exceptions.
-237- Change detection in `Entity.changes()` now excludes cases where the
-238  server has no value and the new value is None. Saving this change has
-239  no effect and would always detect a change until a non-None value is
-240  set, which is noisy and generates more network activity.
-241
-242### 2.0.3
-243- Better support for calendars.
-244  - Distinguish between calendar containers ("Calendar") and the
-245    calendar items within them ("CalendarItem").
-246  - Allow CalendarItems to be saved directly. E.G item.save()
-247- Fix 'holder' parameter in contact/staff/location/task_template not
-248  permitting object type. Now consumes uuId or object to match rest of
-249  the library.
-250- `Entity.changes()` has been extended with an `old=True` flag. When
-251  this flag is true, the set of changes will now return both the original
-252  and the new values. E.g.
-253```
-254task.changes()
-255# {'name': 'current'}
-256task.changes(old=True)
-257# {'name': {'old': 'original', 'new': 'current'}}
-258```
-259- Fixed entity link cache causing errors when deleting a link from an entity
-260  which has not been fetched with links (deleting from empty list).
-261
-262### 2.0.2
-263- Fixed updating Webhook entities
-264
-265### 2.0.1
-266- Fixed application ID not being used correctly.
-267
-268### 2.0.0
-269- Version 2.0 accompanies the release of Projectal 2.0. There are no major
+230- Duration calculation is not precise yet (mentioned in 2.1.0)
+231
+232### 2.1.0
+233**Breaking changes**:
+234- Getting location calendar is now done on an instance instead of class. So
+235  `projectal.Location.calendar(uuid)` is now simply `location.calendar()`
+236- The `CompanyType.Master` enum has been replaced with
+`CompanyType.Primary`.
+237  This was a leftover reference to the Master Company which was renamed in
+238  Projectal several versions ago.
+239
+240**Other changes**:
+241- Date conversion functions return None when given None or empty string
+242- Added `Task.reset_duration()` as a basic duration calculator for tasks.
+243  This is a work-in-progress and will be gradually improved. The duration
+244  calculator takes into consideration the location to remove non-work
+245  days from the estimate of working duration. It currently does not work
+246  for the time component or `isWorking=True` exceptions.
+247- Change detection in `Entity.changes()` now excludes cases where the
+248  server has no value and the new value is None. Saving this change has
+249  no effect and would always detect a change until a non-None value is
+250  set, which is noisy and generates more network activity.
+251
+252### 2.0.3
+253- Better support for calendars.
+254  - Distinguish between calendar containers ("Calendar") and the
+255    calendar items within them ("CalendarItem").
+256  - Allow CalendarItems to be saved directly. E.G item.save()
+257- Fix 'holder' parameter in contact/staff/location/task_template not
+258  permitting object type. Now consumes uuId or object to match rest of
+259  the library.
+260- `Entity.changes()` has been extended with an `old=True` flag. When
+261  this flag is true, the set of changes will now return both the original
+262  and the new values. E.g.
+263```
+264task.changes()
+265# {'name': 'current'}
+266task.changes(old=True)
+267# {'name': {'old': 'original', 'new': 'current'}}
+268```
+269- Fixed entity link cache causing errors when deleting a link from an entity
+270  which has not been fetched with links (deleting from empty list).
+271
+272### 2.0.2
+273- Fixed updating Webhook entities
+274
+275### 2.0.1
+276- Fixed application ID not being used correctly.
+277
+278### 2.0.0
+279- Version 2.0 accompanies the release of Projectal 2.0. There are no major
 changes
-270  since the previous release.
-271- Expose `Entity.changes()` function. It returns a list of fields on an
+280  since the previous release.
+281- Expose `Entity.changes()` function. It returns a list of fields on an
 entity that
-272  have changed since fetching it. These are the changes that will be sent
+282  have changed since fetching it. These are the changes that will be sent
 over to the
-273  server when an update request is made.
-274- Added missing 'packaging' dependency to requirements.
-275
-276### 1.2.0
-277
-278**Breaking changes**:
-279
-280- Renamed `request_timestamp` to `response_timestamp` to better reflect its
+283  server when an update request is made.
+284- Added missing 'packaging' dependency to requirements.
+285
+286### 1.2.0
+287
+288**Breaking changes**:
+289
+290- Renamed `request_timestamp` to `response_timestamp` to better reflect its
 purpose.
-281- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
+291- Automatic timestamp conversion into dates (introduced in `1.1.0`) has been
 reverted.
-282  All date fields returned from the server remain as UTC timestamps.
-283
-284  The reason is that date fields on tasks contain a time component and
+292  All date fields returned from the server remain as UTC timestamps.
+293
+294  The reason is that date fields on tasks contain a time component and
 converting them
-285  into date strings was erasing the time, resulting in a value that does not
+295  into date strings was erasing the time, resulting in a value that does not
 match
-286  the database.
-287
-288  Note: the server supports setting date fields using a date string like
+296  the database.
+297
+298  Note: the server supports setting date fields using a date string like
 `2022-04-05`.
-289  You may use this if you prefer but the server will always return a
+299  You may use this if you prefer but the server will always return a
 timestamp.
-290
-291  Note: we provide utility functions for easily converting dates from/to
-292  timestamps expected by the Projectal server. See:
-293  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
-294  `projectal.timestamp_from_datetime()`.
-295
-296**Other changes**:
-297- Implement request chunking - for methods that consume a list of entities,
+300
+301  Note: we provide utility functions for easily converting dates from/to
+302  timestamps expected by the Projectal server. See:
+303  `projectal.date_from_timestamp()`,`projectal.timestamp_from_date()`, and
+304  `projectal.timestamp_from_datetime()`.
+305
+306**Other changes**:
+307- Implement request chunking - for methods that consume a list of entities,
 we now
-298  automatically batch them up into multiple requests to prevent timeouts on
+308  automatically batch them up into multiple requests to prevent timeouts on
 really
-299  large request. Values are configurable through
-300  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
-301  Default values: Read: 1000 items. Write: 200 items.
-302- Added profile get/set functions on entities for easier use. Now you only
+309  large request. Values are configurable through
+310  `projectal.chunk_size_read` and `projectal.chunk_size_write`.
+311  Default values: Read: 1000 items. Write: 200 items.
+312- Added profile get/set functions on entities for easier use. Now you only
 need to supply
-303  the key and the data. E.g:
-304
-305```
-306key = 'hr_connector'
-307data = {'staff_source': 'company_z'}
-308task.profile_set(key, data)
-309```
-310
-311- Entity link methods now automatically update the entity's cached list of
+313  the key and the data. E.g:
+314
+315```
+316key = 'hr_connector'
+317data = {'staff_source': 'company_z'}
+318task.profile_set(key, data)
+319```
+320
+321- Entity link methods now automatically update the entity's cached list of
 links. E.g:
-312  a task fetched with staff links will have `task['staffList'] =
+322  a task fetched with staff links will have `task['staffList'] =
 [Staff1,Staff2]`.
-313  Before, doing a `task.link_staff(staff)` did not modify the list to
+323  Before, doing a `task.link_staff(staff)` did not modify the list to
 reflect the
-314  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
+324  addition. Now, it will turn into `[Staff1,Staff2,Staff3]`. The same
 applies for update
-315  and delete.
-316
-317  This allows you to modify links and continue working with that object
+325  and delete.
+326
+327  This allows you to modify links and continue working with that object
 without having
-318  to fetch it again to obtain the most recent link data. Be aware that if
+328  to fetch it again to obtain the most recent link data. Be aware that if
 you acquire
-319  the object without requesting the link data as well
-320  (e.g: `projectal.Task.get(id, links='STAFF')`),
-321  these lists will not accurately reflect what's in the database, only the
+329  the object without requesting the link data as well
+330  (e.g: `projectal.Task.get(id, links='STAFF')`),
+331  these lists will not accurately reflect what's in the database, only the
 changes made
-322  while the object is held.
-323
-324- Support new `applicationId` property on login. Set with:
+332  while the object is held.
+333
+334- Support new `applicationId` property on login. Set with:
 `projectal.api_application_id`.
-325  The application ID is sent back to you in webhooks so you know which
+335  The application ID is sent back to you in webhooks so you know which
 application was
-326  the source of the event (and you can choose to filter them accordingly).
-327- Added `Entity.set_readonly()` to allow setting values on entities that
+336  the source of the event (and you can choose to filter them accordingly).
+337- Added `Entity.set_readonly()` to allow setting values on entities that
 will not
-328  be sent over to the server when updating/saving the entity.
-329
-330  The main use case for this is to populate cached entities which you have
+338  be sent over to the server when updating/saving the entity.
+339
+340  The main use case for this is to populate cached entities which you have
 just created
-331  with values you already know about. This is mainly a workaround for the
+341  with values you already know about. This is mainly a workaround for the
 limitation of
-332  the server not sending the full object back after creating it, resulting
+342  the server not sending the full object back after creating it, resulting
 in the client
-333  needing to fetch the object in full again if it needs some of the fields
+343  needing to fetch the object in full again if it needs some of the fields
 set by the
-334  server after creation.
-335
-336  Additionally, some read-only fields will generate an error on the server
+344  server after creation.
+345
+346  Additionally, some read-only fields will generate an error on the server
 if
-337  included in the update request. This method lets you set these values on
+347  included in the update request. This method lets you set these values on
 newly
-338  created objects without triggering this error.
-339
-340  A common example is setting the `projectRef` of a task you just created.
-341
-342
-343### 1.1.1
-344- Add support for 'profiles' API. Profiles are a type of key-value storage
+348  created objects without triggering this error.
+349
+350  A common example is setting the `projectRef` of a task you just created.
+351
+352
+353### 1.1.1
+354- Add support for 'profiles' API. Profiles are a type of key-value storage
 that target
-345  any entity. Not currently documented.
-346- Fix handling error message parsing in ProjectalException for batch create
+355  any entity. Not currently documented.
+356- Fix handling error message parsing in ProjectalException for batch create
 operation
-347- Add `Task.update_order()` to set task order
-348- Return empty list when GETing empty list instead of failing (no request to
+357- Add `Task.update_order()` to set task order
+358- Return empty list when GETing empty list instead of failing (no request to
 server)
-349- Expose the timestamp returned by requests that modify the database. Use
-350  `projectal.request_timestamp` to get the value of the most recent request
+359- Expose the timestamp returned by requests that modify the database. Use
+360  `projectal.request_timestamp` to get the value of the most recent request
 (None
-351  if no timestamp in response)
-352
-353### 1.1.0
-354- Minimum Projectal version is now 1.9.4.
-355
-356**Breaking changes**:
-357- Entity `list()` now returns a list of UUIDs instead of full objects. You
+361  if no timestamp in response)
+362
+363### 1.1.0
+364- Minimum Projectal version is now 1.9.4.
+365
+366**Breaking changes**:
+367- Entity `list()` now returns a list of UUIDs instead of full objects. You
 may provide
-358  an `expand` parameter to restore the previous behavior: `Entity.list
+368  an `expand` parameter to restore the previous behavior: `Entity.list
 (expand=True)`.
-359  This change is made for performance reasons where you may have thousands
+369  This change is made for performance reasons where you may have thousands
 of tasks
-360  and getting them all may time out. For those cases, we suggest writing a
+370  and getting them all may time out. For those cases, we suggest writing a
 query to filter
-361  down to only the tasks and fields you need.
-362- `Company.get_master_company()` has been renamed to
+371  down to only the tasks and fields you need.
+372- `Company.get_master_company()` has been renamed to
 `Company.get_primary_company()`
-363  to match the server.
-364- The following date fields are converted into date strings upon fetch:
-365  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
-366  These fields are added or updated using date strings (like `2022-03-02`),
+373  to match the server.
+374- The following date fields are converted into date strings upon fetch:
+375  `startTime`, `closeTime`, `scheduleStart`, `scheduleFinish`.
+376  These fields are added or updated using date strings (like `2022-03-02`),
 but the
-367  server returns timestamps (e.g: 1646006400000) upon fetch, which is
+377  server returns timestamps (e.g: 1646006400000) upon fetch, which is
 confusing. This
-368  change ensures they are always date strings for consistency.
-369
-370**Other changes**:
-371- When updating an entity, only the fields that have changed are sent to the
+378  change ensures they are always date strings for consistency.
+379
+380**Other changes**:
+381- When updating an entity, only the fields that have changed are sent to the
 server. When
-372  updating a list of entities, unmodified entities are not sent to the
+382  updating a list of entities, unmodified entities are not sent to the
 server at all. This
-373  dramatically reduces the payload size and should speed things up.
-374- When fetching entities, entity links are now typed as well. E.g. `project
+383  dramatically reduces the payload size and should speed things up.
+384- When fetching entities, entity links are now typed as well. E.g. `project
 ['rebateList']`
-375  contains a list of `Rebate` instead of `dict`.
-376- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
+385  contains a list of `Rebate` instead of `dict`.
+386- Added `date_from_timestamp()` and `timestamp_from_date()` functions to
 help with
-377  converting to/from dates and Projectal timestamps.
-378- Entity history now uses `desc` by default (index 0 is newest)
-379- Added `Project.tasks()` to list all task UUIDs within a project.
-380
-381### 1.0.3
-382- Fix another case of automatic JWT refresh not working
-383
-384### 1.0.2
-385- Entity instances can `save()` or `delete()` on themselves
-386- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
+387  converting to/from dates and Projectal timestamps.
+388- Entity history now uses `desc` by default (index 0 is newest)
+389- Added `Project.tasks()` to list all task UUIDs within a project.
+390
+391### 1.0.3
+392- Fix another case of automatic JWT refresh not working
+393
+394### 1.0.2
+395- Entity instances can `save()` or `delete()` on themselves
+396- Fix broken `dict` methods (`get()` and `update()`) when called from Entity
 instances
-387- Fix automatic JWT refresh only working in some cases
-388
-389### 1.0.1
-390- Added `list()` function for all entities
-391- Added search functions for all entities (match-, search, query)
-392- Added `Company.get_master_company()`
-393- Fixed adding template tasks
-394
-395"""
-396import logging
-397import os
+397- Fix automatic JWT refresh only working in some cases
 398
-399from projectal.entities import *
-400from .api import *
-401from . import profile
-402
-403api_base = os.getenv('PROJECTAL_URL')
-404api_username = os.getenv('PROJECTAL_USERNAME')
-405api_password = os.getenv('PROJECTAL_PASSWORD')
-406api_application_id = None
-407api_auth_details = None
-408api_alias = None
-409cookies = None
-410chunk_size_read = 1000
-411chunk_size_write = 200
+399### 1.0.1
+400- Added `list()` function for all entities
+401- Added search functions for all entities (match-, search, query)
+402- Added `Company.get_master_company()`
+403- Fixed adding template tasks
+404
+405"""
+406import logging
+407import os
+408
+409from projectal.entities import *
+410from .api import *
+411from . import profile
 412
-413# Records the timestamp generated by the last request (database
-414# event time). These are reported on add or updates; if there is
-415# no timestamp in the response, this is set to None.
-416response_timestamp = None
-417
-418
-419# The minimum version number of the Projectal instance that this
-420# API client targets. Lower versions are not supported and will
-421# raise an exception.
-422MIN_PROJECTAL_VERSION = "4.0.0"
-423
-424__verify = True
-425
-426logging.getLogger('projectal-api-client').addHandler(logging.NullHandler())
+413api_base = os.getenv('PROJECTAL_URL')
+414api_username = os.getenv('PROJECTAL_USERNAME')
+415api_password = os.getenv('PROJECTAL_PASSWORD')
+416api_application_id = None
+417api_auth_details = None
+418api_alias = None
+419cookies = None
+420chunk_size_read = 1000
+421chunk_size_write = 200
+422
+423# Records the timestamp generated by the last request (database
+424# event time). These are reported on add or updates; if there is
+425# no timestamp in the response, this is set to None.
+426response_timestamp = None
+427
+428
+429# The minimum version number of the Projectal instance that this
+430# API client targets. Lower versions are not supported and will
+431# raise an exception.
+432MIN_PROJECTAL_VERSION = "4.0.0"
+433
+434__verify = True
+435
+436logging.getLogger('projectal-api-client').addHandler(logging.NullHandler())
```

### Comparing `projectal-4.0.1/examples/linking.py` & `projectal-4.0.2/examples/linking.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/examples/task.py` & `projectal-4.0.2/examples/task.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/examples/webhook.py` & `projectal-4.0.2/examples/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/__init__.py` & `projectal-4.0.2/projectal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,24 @@
 details = projectal.auth_details()
 ```
 
 ----
 
 ## Changelog
 
+### 4.0.2
+- Booking entity is now fetched with project field and either staff or resource field.
+
+- Added missing link methods for 'Booking' entity (Note, File)
+
+- Added missing link methods for 'Activity' entity (Booking, Note, File, Rebate)
+
+- Reduced maximum number of link methods to 100 for a single batch request to prevent timeouts
+under heavy load.
+
 ### 4.0.1
 - Minimum Projectal version is now 4.0.0.
 
 ### 4.0.0
 
 Version 4.0.0 accompanies the release of Projectal 4.0.
```

### Comparing `projectal-4.0.1/projectal/api.py` & `projectal-4.0.2/projectal/api.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/__init__.py` & `projectal-4.0.2/projectal/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/calendar.py` & `projectal-4.0.2/projectal/entities/calendar.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/company.py` & `projectal-4.0.2/projectal/entities/company.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/contact.py` & `projectal-4.0.2/projectal/entities/contact.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/department.py` & `projectal-4.0.2/projectal/entities/department.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/file.py` & `projectal-4.0.2/projectal/entities/file.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/folder.py` & `projectal-4.0.2/projectal/entities/folder.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/location.py` & `projectal-4.0.2/projectal/entities/location.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/note.py` & `projectal-4.0.2/projectal/entities/note.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/permission.py` & `projectal-4.0.2/projectal/entities/permission.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/project.py` & `projectal-4.0.2/projectal/entities/project.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/project_template.py` & `projectal-4.0.2/projectal/entities/project_template.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/staff.py` & `projectal-4.0.2/projectal/entities/staff.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/task.py` & `projectal-4.0.2/projectal/entities/task.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/task_template.py` & `projectal-4.0.2/projectal/entities/task_template.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/user.py` & `projectal-4.0.2/projectal/entities/user.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entities/webhook.py` & `projectal-4.0.2/projectal/entities/webhook.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/entity.py` & `projectal-4.0.2/projectal/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         }
         self._link_def_by_key[d['link_key']] = d
         self._link_def_by_name[d['name']] = d
 
     def _add_link(self, to_entity_name, to_link):
         self._link(to_entity_name, to_link, 'add', batch_linking=False)
 
-    def _update_link(self,to_entity_name, to_link):
+    def _update_link(self, to_entity_name, to_link):
         self._link(to_entity_name, to_link, 'update', batch_linking=False)
 
     def _delete_link(self, to_entity_name, to_link):
         self._link(to_entity_name, to_link, 'delete', batch_linking=False)
 
     def _link(self, to_entity_name, to_link, operation, update_cache=True, batch_linking=True):
         """
@@ -318,16 +318,16 @@
         # API requests
         link_request_batch = []
         for e in e_list:
             requests = e.__apply_link_changes(batch_linking=batch_linking)
             link_request_batch.extend(requests)
 
         if len(link_request_batch) > 0 and batch_linking:
-            for i in range(0, len(link_request_batch), 1000):
-                chunk = link_request_batch[i:i + 1000]
+            for i in range(0, len(link_request_batch), 100):
+                chunk = link_request_batch[i:i + 100]
                 api.post('/api/composite', chunk)
 
         if not isinstance(entities, list):
             return objects[0]
         return objects
 
     @classmethod
@@ -511,16 +511,16 @@
         link_request_batch = []
         for e in e_list:
             if isinstance(e, Entity):
                 requests = e.__apply_link_changes(batch_linking=batch_linking)
                 link_request_batch.extend(requests)
 
         if len(link_request_batch) > 0 and batch_linking:
-            for i in range(0, len(link_request_batch), 1000):
-                chunk = link_request_batch[i:i + 1000]
+            for i in range(0, len(link_request_batch), 100):
+                chunk = link_request_batch[i:i + 100]
                 api.post('/api/composite', chunk)
 
         return True
 
     def __update(self, *args, **kwargs):
         """Use the dict update for instances."""
         return super(Entity, self).update(*args, **kwargs)
```

### Comparing `projectal-4.0.1/projectal/enums.py` & `projectal-4.0.2/projectal/enums.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/errors.py` & `projectal-4.0.2/projectal/errors.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal/linkers.py` & `projectal-4.0.2/projectal/linkers.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 task.link_staff(staff)
 ```
 
 """
 
 from projectal import api
 
+
 class BaseLinker:
     # _link_name is the link name (usually the entity name)
     _link_name = None
 
     # _link_key is the key within the source object that points to the
     # links. E.g., 'skillList'
     _link_key = None
@@ -52,27 +53,50 @@
 
     # _link_entity is the string name (capitalized, like Stage) of the Entity
     # class within this library that fetched links will be converted to.
     # This is useful when the name of the list differs from the entity
     # name. E.g: stage_list needs to be converted to Stage.
     _link_entity = None
 
+
 class AccessPolicyLinker(BaseLinker):
     """Subclass can link to Access Policies"""
     _link_name = 'access_policy'
     _link_key = 'accessPolicyList'
     _link_entity = 'AccessPolicy'
 
     def link_access_policy(self, access_policies):
         self._add_link('access_policy', access_policies)
 
     def unlink_access_policy(self, access_policies):
         self._delete_link('access_policy', access_policies)
 
 
+class ActivityLinker(BaseLinker):
+    """Subclass can link to Activities"""
+    _link_name = 'activity'
+
+    def link_activity(self, activity):
+        self._add_link('activity', activity)
+
+    def unlink_activity(self, activity):
+        self._delete_link('activity', activity)
+
+
+class BookingLinker(BaseLinker):
+    """Subclass can link to Bookings"""
+    _link_name = 'booking'
+
+    def link_booking(self, booking):
+        self._add_link('booking', booking)
+
+    def unlink_booking(self, booking):
+        self._delete_link('booking', booking)
+
+
 class CompanyLinker(BaseLinker):
     """Subclass can link to Companies"""
     _link_name = 'company'
 
     def link_company(self, companies):
         self._add_link('company', companies)
```

### Comparing `projectal-4.0.1/projectal/profile.py` & `projectal-4.0.2/projectal/profile.py`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/projectal.egg-info/PKG-INFO` & `projectal-4.0.2/projectal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: projectal
-Version: 4.0.1
+Version: 4.0.2
 Summary: Python bindings for the Projectal API
 Home-page: https://projectal.com/resources/developer
 Author: Projectal
 Author-email: support@projectal.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `projectal-4.0.1/projectal.egg-info/SOURCES.txt` & `projectal-4.0.2/projectal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `projectal-4.0.1/setup.py` & `projectal-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='projectal',
-    version='4.0.1',
+    version='4.0.2',
     description='Python bindings for the Projectal API',
     long_description="The Python library allows developers to write Python-based apps that talk directly with Projectal. This gives developers immense freedom to access all data points in Projectal and to integrate Projectal with their workflow.",
     long_description_content_type="text/plain",
     url='https://projectal.com/resources/developer',
     author='Projectal',
     author_email='support@projectal.com',
     license='MIT',
```

