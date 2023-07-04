# Comparing `tmp/versionoverlord-0.5.8.tar.gz` & `tmp/versionoverlord-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versionoverlord-0.5.8.tar", last modified: Thu Apr 13 18:22:41 2023, max compression
+gzip compressed data, was "versionoverlord-0.6.0.tar", last modified: Tue Jul  4 23:18:05 2023, max compression
```

## Comparing `versionoverlord-0.5.8.tar` & `versionoverlord-0.6.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248697 versionoverlord-0.5.8/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 versionoverlord-0.5.8/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45827 2023-04-13 18:22:41.248554 versionoverlord-0.5.8/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5648 2023-04-07 13:27:31.000000 versionoverlord-0.5.8/README.md
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-04-13 18:22:41.248734 versionoverlord-0.5.8/setup.cfg
--rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1524 2023-04-13 18:09:11.000000 versionoverlord-0.5.8/setup.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.244903 versionoverlord-0.5.8/versionoverlord/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2402 2023-03-05 20:39:51.000000 versionoverlord-0.5.8/versionoverlord/BaseHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2188 2023-03-29 19:49:28.000000 versionoverlord-0.5.8/versionoverlord/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2032 2023-02-23 17:30:59.000000 versionoverlord-0.5.8/versionoverlord/DisplayVersions.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-03-05 20:25:19.000000 versionoverlord-0.5.8/versionoverlord/EnvironmentBase.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      629 2023-03-29 21:30:54.000000 versionoverlord-0.5.8/versionoverlord/FileNameToSlugs.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2245 2023-03-29 21:38:10.000000 versionoverlord-0.5.8/versionoverlord/GitHubAdapter.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1642 2023-03-27 15:42:18.000000 versionoverlord-0.5.8/versionoverlord/SlugHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2745 2023-03-27 15:41:21.000000 versionoverlord-0.5.8/versionoverlord/TemplateHandler.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:09:59.000000 versionoverlord-0.5.8/versionoverlord/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.245880 versionoverlord-0.5.8/versionoverlord/circleci/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3292 2023-03-03 01:44:06.000000 versionoverlord-0.5.8/versionoverlord/circleci/HandleCircleCI.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-01 21:02:11.000000 versionoverlord-0.5.8/versionoverlord/circleci/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.246333 versionoverlord-0.5.8/versionoverlord/commands/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1351 2023-04-08 17:49:26.000000 versionoverlord-0.5.8/versionoverlord/commands/CreateSpecification.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1990 2023-04-08 17:50:44.000000 versionoverlord-0.5.8/versionoverlord/commands/QuerySlugs.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3673 2023-04-08 17:51:18.000000 versionoverlord-0.5.8/versionoverlord/commands/UpdateDependencies.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-15 02:24:41.000000 versionoverlord-0.5.8/versionoverlord/commands/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.247492 versionoverlord-0.5.8/versionoverlord/exceptions/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      164 2023-02-27 00:53:40.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoFileException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-02-24 16:20:38.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoGitHubAccessTokenException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      342 2023-02-27 00:59:06.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoRequirementsTxtsException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-02-27 00:58:06.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NoSetupPyFileException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-03-01 21:16:59.000000 versionoverlord-0.5.8/versionoverlord/exceptions/NotACircleCIProjectException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 versionoverlord-0.5.8/versionoverlord/exceptions/ProjectNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 versionoverlord-0.5.8/versionoverlord/exceptions/ProjectsBaseNotSetException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-02-24 16:20:52.000000 versionoverlord-0.5.8/versionoverlord/exceptions/UnknownGitHubRepositoryException.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:25:38.000000 versionoverlord-0.5.8/versionoverlord/exceptions/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.247713 versionoverlord-0.5.8/versionoverlord/requirements/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3045 2023-03-02 22:02:08.000000 versionoverlord-0.5.8/versionoverlord/requirements/HandleRequirementsTxt.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-26 22:29:17.000000 versionoverlord-0.5.8/versionoverlord/requirements/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248017 versionoverlord-0.5.8/versionoverlord/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:25:28.000000 versionoverlord-0.5.8/versionoverlord/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-03-12 20:23:35.000000 versionoverlord-0.5.8/versionoverlord/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.248326 versionoverlord-0.5.8/versionoverlord/setup/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2648 2023-03-01 21:08:09.000000 versionoverlord-0.5.8/versionoverlord/setup/HandleSetupPy.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:21:11.000000 versionoverlord-0.5.8/versionoverlord/setup/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-04-13 18:22:41.245650 versionoverlord-0.5.8/versionoverlord.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45827 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1548 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      227 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       16 2023-04-13 18:22:41.000000 versionoverlord-0.5.8/versionoverlord.egg-info/top_level.txt
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.337626 versionoverlord-0.6.0/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2022-07-23 19:00:15.000000 versionoverlord-0.6.0/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45869 2023-07-04 23:18:05.337467 versionoverlord-0.6.0/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     5690 2023-05-08 18:49:54.000000 versionoverlord-0.6.0/README.md
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-07-04 23:18:05.337663 versionoverlord-0.6.0/setup.cfg
+-rw-------   0 humberto.a.sanchez.ii   (501) staff       (20)     1634 2023-07-04 23:13:48.000000 versionoverlord-0.6.0/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.333896 versionoverlord-0.6.0/versionoverlord/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2402 2023-03-05 20:39:51.000000 versionoverlord-0.6.0/versionoverlord/BaseHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2188 2023-03-29 19:49:28.000000 versionoverlord-0.6.0/versionoverlord/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2032 2023-02-23 17:30:59.000000 versionoverlord-0.6.0/versionoverlord/DisplayVersions.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1080 2023-03-05 20:25:19.000000 versionoverlord-0.6.0/versionoverlord/EnvironmentBase.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      629 2023-03-29 21:30:54.000000 versionoverlord-0.6.0/versionoverlord/FileNameToSlugs.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2245 2023-07-03 18:37:32.000000 versionoverlord-0.6.0/versionoverlord/GitHubAdapter.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1839 2023-07-03 18:52:33.000000 versionoverlord-0.6.0/versionoverlord/SlugHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3404 2023-07-03 20:28:43.000000 versionoverlord-0.6.0/versionoverlord/TemplateHandler.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:09:59.000000 versionoverlord-0.6.0/versionoverlord/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.334903 versionoverlord-0.6.0/versionoverlord/circleci/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3292 2023-03-03 01:44:06.000000 versionoverlord-0.6.0/versionoverlord/circleci/HandleCircleCI.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-01 21:02:11.000000 versionoverlord-0.6.0/versionoverlord/circleci/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.335497 versionoverlord-0.6.0/versionoverlord/commands/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2174 2023-07-03 20:47:56.000000 versionoverlord-0.6.0/versionoverlord/commands/CreateSpecification.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1992 2023-07-03 20:46:59.000000 versionoverlord-0.6.0/versionoverlord/commands/QuerySlugs.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3681 2023-07-03 20:48:21.000000 versionoverlord-0.6.0/versionoverlord/commands/UpdateDependencies.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      433 2023-07-04 17:41:42.000000 versionoverlord-0.6.0/versionoverlord/commands/VersionOverlord.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-03-15 02:24:41.000000 versionoverlord-0.6.0/versionoverlord/commands/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.336573 versionoverlord-0.6.0/versionoverlord/exceptions/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      164 2023-02-27 00:53:40.000000 versionoverlord-0.6.0/versionoverlord/exceptions/NoFileException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-02-24 16:20:38.000000 versionoverlord-0.6.0/versionoverlord/exceptions/NoGitHubAccessTokenException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      342 2023-02-27 00:59:06.000000 versionoverlord-0.6.0/versionoverlord/exceptions/NoRequirementsTxtsException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      330 2023-02-27 00:58:06.000000 versionoverlord-0.6.0/versionoverlord/exceptions/NoSetupPyFileException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       57 2023-03-01 21:16:59.000000 versionoverlord-0.6.0/versionoverlord/exceptions/NotACircleCIProjectException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       51 2023-02-25 02:47:03.000000 versionoverlord-0.6.0/versionoverlord/exceptions/ProjectNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       56 2023-02-25 02:28:42.000000 versionoverlord-0.6.0/versionoverlord/exceptions/ProjectsBaseNotSetException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      237 2023-02-24 16:20:52.000000 versionoverlord-0.6.0/versionoverlord/exceptions/UnknownGitHubRepositoryException.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:25:38.000000 versionoverlord-0.6.0/versionoverlord/exceptions/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.336795 versionoverlord-0.6.0/versionoverlord/requirements/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     3045 2023-03-02 22:02:08.000000 versionoverlord-0.6.0/versionoverlord/requirements/HandleRequirementsTxt.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-26 22:29:17.000000 versionoverlord-0.6.0/versionoverlord/requirements/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.336982 versionoverlord-0.6.0/versionoverlord/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-23 02:25:28.000000 versionoverlord-0.6.0/versionoverlord/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      857 2023-03-12 20:23:35.000000 versionoverlord-0.6.0/versionoverlord/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.337226 versionoverlord-0.6.0/versionoverlord/setup/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2648 2023-03-01 21:08:09.000000 versionoverlord-0.6.0/versionoverlord/setup/HandleSetupPy.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-02-25 02:21:11.000000 versionoverlord-0.6.0/versionoverlord/setup/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-07-04 23:18:05.334655 versionoverlord-0.6.0/versionoverlord.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    45869 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1592 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      324 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       49 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       16 2023-07-04 23:18:05.000000 versionoverlord-0.6.0/versionoverlord.egg-info/top_level.txt
```

### Comparing `versionoverlord-0.5.8/LICENSE` & `versionoverlord-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/PKG-INFO` & `versionoverlord-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versionoverlord
-Version: 0.5.8
+Version: 0.6.0
 Summary: Dependency Manager
 Home-page: https://github.com/versionoverlord
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -723,15 +723,15 @@
 
 
 
 ## Python Console Scripts
 
 VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
-* querySlug -- queries repositories for their latest release version
+* querySlugs -- queries repositories for their latest release version
 * createSpec -- creates a dependency specification for a project 
 * updateDeps -- updates the supported dependency locations using the generated specification
 
 
 
 ## Required Environment Variables
 
@@ -809,15 +809,15 @@
 
 
 ## 
 
 
 ___
 
-Written by [Humberto A. Sanchez II](mailto@humberto.a.sanchez.ii@gmail.com) (C) 2023
+Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 
 ## Note
 For all kind of problems, requests, enhancements, bug reports, etc.,
 please drop me an e-mail.
```

### Comparing `versionoverlord-0.5.8/README.md` & `versionoverlord-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 
 ## Python Console Scripts
 
 VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
-* querySlug -- queries repositories for their latest release version
+* querySlugs -- queries repositories for their latest release version
 * createSpec -- creates a dependency specification for a project 
 * updateDeps -- updates the supported dependency locations using the generated specification
 
 
 
 ## Required Environment Variables
 
@@ -135,15 +135,15 @@
 
 
 ## 
 
 
 ___
 
-Written by [Humberto A. Sanchez II](mailto@humberto.a.sanchez.ii@gmail.com) (C) 2023
+Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 
 ## Note
 For all kind of problems, requests, enhancements, bug reports, etc.,
 please drop me an e-mail.
```

### Comparing `versionoverlord-0.5.8/setup.py` & `versionoverlord-0.6.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 DATA_FILES = [
     ('versionoverlord/resources', ['versionoverlord/resources/loggingConfiguration.json']),
 ]
 
 setup(
     name="versionoverlord",
-    version="0.5.8",
+    version="0.6.0",
     author='Humberto A. Sanchez II',
     author_email='humberto.a.sanchez.ii@gmail.com',
     maintainer='Humberto A. Sanchez II',
     maintainer_email='humberto.a.sanchez.ii@gmail.com',
     description='Dependency Manager',
     long_description=README,
     long_description_content_type="text/markdown",
@@ -38,13 +38,14 @@
     install_requires=[
         'PyGithub==1.58.1',
         'click~=8.1.3',
         'hasiihelper~=0.2.0',
     ],
     entry_points={
         "console_scripts": [
-            "querySlugs=versionoverlord.commands.QuerySlugs:commandHandler",
-            "createSpec=versionoverlord.commands.CreateSpecification:commandHandler",
-            "updateDeps=versionoverlord.commands.UpdateDependencies:commandHandler",
+            "querySlugs=versionoverlord.commands.QuerySlugs:querySlugs",
+            "createSpecification=versionoverlord.commands.CreateSpecification:createSpecification",
+            "updateDependencies=versionoverlord.commands.UpdateDependencies:updateDependencies",
+            "versionOverlord=versionoverlord.commands.VersionOverlord:versionOverlord",
         ]
     },
 )
```

### Comparing `versionoverlord-0.5.8/versionoverlord/BaseHandler.py` & `versionoverlord-0.6.0/versionoverlord/BaseHandler.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/Common.py` & `versionoverlord-0.6.0/versionoverlord/Common.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/DisplayVersions.py` & `versionoverlord-0.6.0/versionoverlord/DisplayVersions.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/EnvironmentBase.py` & `versionoverlord-0.6.0/versionoverlord/EnvironmentBase.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/FileNameToSlugs.py` & `versionoverlord-0.6.0/versionoverlord/FileNameToSlugs.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/GitHubAdapter.py` & `versionoverlord-0.6.0/versionoverlord/GitHubAdapter.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/SlugHandler.py` & `versionoverlord-0.6.0/versionoverlord/SlugHandler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 from logging import Logger
 from logging import getLogger
 
+from click import ClickException
+from click import secho
 from hasiihelper.SemanticVersion import SemanticVersion
 
 from versionoverlord.Common import Slugs
 
 from versionoverlord.DisplayVersions import DisplayVersions
 from versionoverlord.DisplayVersions import SlugVersion
 from versionoverlord.DisplayVersions import SlugVersions
@@ -27,15 +29,18 @@
 
             slugVersions: SlugVersions = SlugVersions([])
             for slug in self._slugs:
                 version: SemanticVersion = gitHubAdapter.getLatestVersionNumber(slug)
                 slugVersion: SlugVersion = SlugVersion(slug=slug, version=str(version))
                 slugVersions.append(slugVersion)
 
-            displayVersions: DisplayVersions = DisplayVersions()
-            displayVersions.displaySlugs(slugVersions=slugVersions)
+            if len(slugVersions) == 0:
+                secho('Nothing to see here')
+            else:
+                displayVersions: DisplayVersions = DisplayVersions()
+                displayVersions.displaySlugs(slugVersions=slugVersions)
         except NoGitHubAccessTokenException:
-            print(f'Your must provide a GitHub access token via the environment variable `GITHUB_ACCESS_TOKEN`')
+            raise ClickException(f'Your must provide a GitHub access token via the environment variable `GITHUB_ACCESS_TOKEN`')
         except UnknownGitHubRepositoryException as e:
-            print(f'Unknown GitHub Repository: `{e.repositorySlug}`')
+            raise ClickException(f'Unknown GitHub Repository: `{e.repositorySlug}`')
         except (ValueError, Exception) as e:
             print(f'{e}')
```

### Comparing `versionoverlord-0.5.8/versionoverlord/TemplateHandler.py` & `versionoverlord-0.6.0/versionoverlord/TemplateHandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,32 +43,48 @@
             slugVersions.append(slugVersion)
 
         versionUpdateSpecification: Path = Path(SPECIFICATION_FILE)
         with versionUpdateSpecification.open(mode='w') as fd:
             fd.write(f'PackageName,OldVersion,NewVersion{osLineSep}')
             for slugVersion in slugVersions:
                 oldVersion: str = self._findRequirementVersion(self._extractPackageName(slugVersion.slug))
-                pkgName: str = self._extractPackageName(slug=slugVersion.slug)
-                fd.write(f'{pkgName},{oldVersion},{slugVersion.version}{osLineSep}')
+                if oldVersion == '':
+                    print(f'{slugVersion.slug} Did not find requirement')
+                else:
+                    pkgName:    str = self._extractPackageName(slug=slugVersion.slug)
+                    fd.write(f'{pkgName},{oldVersion},{slugVersion.version}{osLineSep}')
 
     def _extractPackageName(self, slug: str) -> str:
         splitSlug: List[str] = slug.split(sep='/')
 
         pkgName: str = splitSlug[1]
         return pkgName
 
     def _findRequirementVersion(self, packageName: str) -> str:
-
+        """
+        Can handle requirements specifications like:
+        pkgName==versionNumber
+        pkgName~=versionNumber
+
+        Args:
+            packageName:   The package name to search for
+
+        Returns:  A version number from the requirement file that matches the package name
+                 If the requirement is not listed returns an empty string
+        """
         lookupRequirement: str = f'{packageName}=='
 
         req: List[str] = self._searchRequirements(lookupRequirement)
         if len(req) == 0:
-            lookupRequirement = f'{packageName}~='
+            lookupRequirement = f'{packageName}~='      # did not find '=='  how about '~='
             req = self._searchRequirements(lookupRequirement)
-            splitRequirement: List[str] = req[0].split('~=')
+            if len(req) == 0:
+                splitRequirement: List[str]  = ['', '']
+            else:
+                splitRequirement = req[0].split('~=')
         else:
             splitRequirement = req[0].split('==')
 
         return splitRequirement[1]
 
     def _searchRequirements(self, reqLine: str) -> List[str]:
         req = [match for match in self._requirementsTxt if reqLine in match]
```

### Comparing `versionoverlord-0.5.8/versionoverlord/circleci/HandleCircleCI.py` & `versionoverlord-0.6.0/versionoverlord/circleci/HandleCircleCI.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/commands/CreateSpecification.py` & `versionoverlord-0.6.0/versionoverlord/commands/CreateSpecification.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,53 @@
 from logging import Logger
 from logging import getLogger
+from pathlib import Path
 from typing import Tuple
 from typing import cast
 
 from click import command
 from click import option
+from click import secho
 from click import version_option
 
 from versionoverlord.Common import __version__
 from versionoverlord.Common import Slugs
 from versionoverlord.Common import setUpLogging
+from versionoverlord.FileNameToSlugs import FileNameToSlugs
 from versionoverlord.TemplateHandler import TemplateHandler
 
 
-class CreateSpecification:
-    def __init__(self):
-        self.logger: Logger = getLogger(__name__)
-
-
 @command()
 @version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
-@option('--slugs', '-s',  multiple=True, required=False, help='Create package update specification')
-def commandHandler(slugs: Tuple[str]):
+@option('--slugs',     '-s',  multiple=True, required=False, help='Create package update specification')
+@option('--input-file', '-i', required=False,                help='Use input file for slug list')
+def createSpecification(slugs: Tuple[str], input_file: str):
     """
     \b
     This command creates .csv specification file
     It uses the following environment variables:
     \b
         GITHUB_ACCESS_TOKEN - A personal GitHub access token necessary to read repository release information
         PROJECTS_BASE -  The local directory where the python projects are based
         PROJECT       -  The name of the project;  It should be a directory name
     """
 
     if len(slugs) != 0:
         templateHandler: TemplateHandler = TemplateHandler(slugs=cast(Slugs, slugs))
         templateHandler.createSpecification()
+    elif input_file is not None:
+        fqFileName: Path = Path(input_file)
+        if fqFileName.exists() is False:
+            secho('                          ', fg='red', bg='black', bold=True)
+            secho('Input file does not exist ', fg='red', bg='black', bold=True)
+            secho('                          ', fg='red', bg='black', bold=True)
+        else:
+            fileNameToSlugs: FileNameToSlugs = FileNameToSlugs(path=fqFileName)
+            inputSlugs:      Slugs           = fileNameToSlugs.getSlugs()
+
+            templateHandler = TemplateHandler(slugs=inputSlugs)
+            templateHandler.createSpecification()
 
 
 if __name__ == "__main__":
     setUpLogging()
-    commandHandler()
+    createSpecification(['-i', 'tests/resources/testdata/query.slg'])
```

### Comparing `versionoverlord-0.5.8/versionoverlord/commands/QuerySlugs.py` & `versionoverlord-0.6.0/versionoverlord/commands/QuerySlugs.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 from versionoverlord.SlugHandler import SlugHandler
 from versionoverlord.SlugHandler import Slugs
 
 
 @command()
 @version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
-@option('--slugs', '-s', required=False, multiple=True, help='GitHub slugs to query')
-@option('--input-file', '-i', required=False,           help='Use input file for slug list')
-def commandHandler(slugs: Tuple[str], input_file):
+@option('--slugs',      '-s', required=False, multiple=True, help='GitHub slugs to query')
+@option('--input-file', '-i', required=False,                help='Use input file for slug list')
+def querySlugs(slugs: Tuple[str], input_file):
     """
         \b
         This command reads the repository for each input slug and displays
         their latest release version
 
         Input slugs can be on the command line or via file input
         \b
@@ -50,8 +50,8 @@
             inputSlugs:      Slugs           = fileNameToSlugs.getSlugs()
             slugHandler = SlugHandler(slugs=inputSlugs)
             slugHandler.handleSlugs()
 
 
 if __name__ == "__main__":
     setUpLogging()
-    commandHandler()
+    querySlugs()
```

### Comparing `versionoverlord-0.5.8/versionoverlord/commands/UpdateDependencies.py` & `versionoverlord-0.6.0/versionoverlord/commands/UpdateDependencies.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 @version_option(version=f'{__version__}', message='%(prog)s version %(version)s')
 @option('--specification', '-s', is_flag=False, flag_value='versionSpecification.csv', default='versionSpecification.csv',
         type=Path(exists=True, path_type=PyPath),
         required=False,
         help='Update the project using a specification file')
 @argument('projectsBase', envvar='PROJECTS_BASE')
 @argument('project', envvar='PROJECT')
-def commandHandler(projectsbase: str, project: str, specification: PyPath):
+def updateDependencies(projectsbase: str, project: str, specification: PyPath):
     """
     \b
     This command uses the .csv file created by createSpec
 
     It uses the following environment variables:
 
     \b
@@ -89,8 +89,8 @@
     secho('')
     setUpLogging()
     vUpdate: UpdateDependencies = UpdateDependencies(specification=specification)
     vUpdate.update()
 
 
 if __name__ == "__main__":
-    commandHandler()
+    updateDependencies()
```

### Comparing `versionoverlord-0.5.8/versionoverlord/requirements/HandleRequirementsTxt.py` & `versionoverlord-0.6.0/versionoverlord/requirements/HandleRequirementsTxt.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/resources/loggingConfiguration.json` & `versionoverlord-0.6.0/versionoverlord/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord/setup/HandleSetupPy.py` & `versionoverlord-0.6.0/versionoverlord/setup/HandleSetupPy.py`

 * *Files identical despite different names*

### Comparing `versionoverlord-0.5.8/versionoverlord.egg-info/PKG-INFO` & `versionoverlord-0.6.0/versionoverlord.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: versionoverlord
-Version: 0.5.8
+Version: 0.6.0
 Summary: Dependency Manager
 Home-page: https://github.com/versionoverlord
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
@@ -723,15 +723,15 @@
 
 
 
 ## Python Console Scripts
 
 VersionOverlord means to handle this problem by providing a set of Python command line scripts to automate updating the first three of the above dependency specification locations
 
-* querySlug -- queries repositories for their latest release version
+* querySlugs -- queries repositories for their latest release version
 * createSpec -- creates a dependency specification for a project 
 * updateDeps -- updates the supported dependency locations using the generated specification
 
 
 
 ## Required Environment Variables
 
@@ -809,15 +809,15 @@
 
 
 ## 
 
 
 ___
 
-Written by [Humberto A. Sanchez II](mailto@humberto.a.sanchez.ii@gmail.com) (C) 2023
+Written by <a href="mailto:email@humberto.a.sanchez.ii@gmail.com?subject=Hello Humberto">Humberto A. Sanchez II</a>  (C) 2023
 
 
 ## Note
 For all kind of problems, requests, enhancements, bug reports, etc.,
 please drop me an e-mail.
```

### Comparing `versionoverlord-0.5.8/versionoverlord.egg-info/SOURCES.txt` & `versionoverlord-0.6.0/versionoverlord.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 versionoverlord.egg-info/requires.txt
 versionoverlord.egg-info/top_level.txt
 versionoverlord/circleci/HandleCircleCI.py
 versionoverlord/circleci/__init__.py
 versionoverlord/commands/CreateSpecification.py
 versionoverlord/commands/QuerySlugs.py
 versionoverlord/commands/UpdateDependencies.py
+versionoverlord/commands/VersionOverlord.py
 versionoverlord/commands/__init__.py
 versionoverlord/exceptions/NoFileException.py
 versionoverlord/exceptions/NoGitHubAccessTokenException.py
 versionoverlord/exceptions/NoRequirementsTxtsException.py
 versionoverlord/exceptions/NoSetupPyFileException.py
 versionoverlord/exceptions/NotACircleCIProjectException.py
 versionoverlord/exceptions/ProjectNotSetException.py
```

