# Comparing `tmp/lazylinks-0.1.0.tar.gz` & `tmp/lazylinks-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazylinks-0.1.0.tar", last modified: Sun Jul  2 02:26:52 2023, max compression
+gzip compressed data, was "lazylinks-0.1.1.tar", last modified: Wed Jul  5 01:57:29 2023, max compression
```

## Comparing `lazylinks-0.1.0.tar` & `lazylinks-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:52.468925 lazylinks-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:52.468925 lazylinks-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:52.468925 lazylinks-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-02 02:26:42.000000 lazylinks-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-02 02:26:42.000000 lazylinks-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-02 02:26:42.000000 lazylinks-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-02 02:26:52.468925 lazylinks-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-02 02:26:42.000000 lazylinks-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:52.468925 lazylinks-0.1.0/lazylinks/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-02 02:26:42.000000 lazylinks-0.1.0/lazylinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-02 02:26:42.000000 lazylinks-0.1.0/lazylinks/dotdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-07-02 02:26:42.000000 lazylinks-0.1.0/lazylinks/lazylinks.mako
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-02 02:26:42.000000 lazylinks-0.1.0/lazylinks/lazylinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 02:26:52.468925 lazylinks-0.1.0/lazylinks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-02 02:26:52.000000 lazylinks-0.1.0/lazylinks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-02 02:26:42.000000 lazylinks-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 02:26:52.468925 lazylinks-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-05 01:57:18.000000 lazylinks-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-05 01:57:18.000000 lazylinks-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 01:57:18.000000 lazylinks-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 01:57:29.340338 lazylinks-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-05 01:57:18.000000 lazylinks-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/lazylinks/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/dotdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/lazylinks.mako
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-05 01:57:18.000000 lazylinks-0.1.1/lazylinks/lazylinks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 01:57:29.340338 lazylinks-0.1.1/lazylinks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 01:57:29.000000 lazylinks-0.1.1/lazylinks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-05 01:57:18.000000 lazylinks-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 01:57:29.340338 lazylinks-0.1.1/setup.cfg
```

### Comparing `lazylinks-0.1.0/.github/workflows/python-publish.yml` & `lazylinks-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/.gitignore` & `lazylinks-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/LICENSE` & `lazylinks-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/PKG-INFO` & `lazylinks-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinks
-Version: 0.1.0
+Version: 0.1.1
 Summary: Linktree-style links for lazy people
 Author-email: Samuel Colburn <samuel.colburn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Samuel Colburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lazylinks-0.1.0/README.md` & `lazylinks-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/lazylinks/dotdict.py` & `lazylinks-0.1.1/lazylinks/dotdict.py`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/lazylinks/lazylinks.mako` & `lazylinks-0.1.1/lazylinks/lazylinks.mako`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,19 @@
   % for section in links:
     <div id="${section.title}" class="sectionTitle">
       ${section.title}
     </div>
     <div class="links">
       % for link in section.links:
         % if 'href' in link and 'copy' in link:
-          <a class="link" href="${link.href}" target="_blank">
+          <a class="link"
+          % if 'more' in link:
+          ${link.more}
+          % endif
+          href="${link.href}" target="_blank">
             <div class="tooltip hidden min">
               <i class="fa-solid fa-copy"></i>
             </div>
             <div class="inline-block">
               <i class="${link.icon}"></i> ${link.text}
               % if 'info' in link:
               <div class="info">${link.info}</div>
@@ -76,15 +80,19 @@
               <span class="" href="#" onclick="copytext('${link.copy}','${link._id}')" onmouseout="outFunc('${link._id}')">
                 <span class="tooltiptext-left" id="${link._id}">Copy to clipboard</span>
                 <i class="fa-solid fa-copy"></i>
               </span>
             </div>
           </a>
         % elif 'href' in link:
-        <a class="link" href="${link.href}" target="_blank">
+        <a class="link"
+        % if 'more' in link:
+        ${link.more}
+        % endif
+        href="${link.href}" target="_blank">
           <i class="${link.icon}"></i> ${link.text}
           % if 'info' in link:
           <div class="info">${link.info}</div>
           % endif
         </a>
         % elif 'copy' in link:
         <div class="tooltip block">
```

#### html2text {}

```diff
@@ -9,22 +9,24 @@
 % if 'pronouns' in config:
 ${config.pronouns}
 % endif
 ${config.description}
 % for section in links:
 ${section.title}
 % for link in section.links: % if 'href' in link and 'copy' in link:
- ${link.text}_%_if_'info'_in_link:
+ if 'more' in link: ${link.more} % endif href="${link.href}" target="_blank">
+ ${link.text} % if 'info' in link:
 ${link.info}
-%_endif
- Copy_to_clipboard
+% endif
+ Copy to clipboard
  % elif 'href' in link:
- ${link.text}_%_if_'info'_in_link:
+ if 'more' in link: ${link.more} % endif href="${link.href}" target="_blank">
+${link.text} % if 'info' in link:
 ${link.info}
-%_endif
+% endif
  % elif 'copy' in link:
 Copy_to_clipboard__${link.text}
 % endif % endfor
 % endfor  % if 'qrcode' in config:
 [${config.qrcode}]
 % endif
 Last updated: ${metadata.last_updated}
```

### Comparing `lazylinks-0.1.0/lazylinks/lazylinks.py` & `lazylinks-0.1.1/lazylinks/lazylinks.py`

 * *Files identical despite different names*

### Comparing `lazylinks-0.1.0/lazylinks.egg-info/PKG-INFO` & `lazylinks-0.1.1/lazylinks.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylinks
-Version: 0.1.0
+Version: 0.1.1
 Summary: Linktree-style links for lazy people
 Author-email: Samuel Colburn <samuel.colburn@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Samuel Colburn
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `lazylinks-0.1.0/pyproject.toml` & `lazylinks-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lazylinks"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Samuel Colburn", email = "samuel.colburn@gmail.com"},
 ]
 description = "Linktree-style links for lazy people"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

