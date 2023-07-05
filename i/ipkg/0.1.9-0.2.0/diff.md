# Comparing `tmp/ipkg-0.1.9.tar.gz` & `tmp/ipkg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipkg-0.1.9.tar", max compression
+gzip compressed data, was "ipkg-0.2.0.tar", max compression
```

## Comparing `ipkg-0.1.9.tar` & `ipkg-0.2.0.tar`

### file list

```diff
@@ -1,64 +1,26 @@
--rw-r--r--   0        0        0     1068 2023-01-25 19:49:33.644008 ipkg-0.1.9/LICENSE
--rw-r--r--   0        0        0       27 2023-01-25 19:49:33.644008 ipkg-0.1.9/README.md
--rw-r--r--   0        0        0       22 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/__init__.py
--rw-r--r--   0        0        0     1627 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/__main__.py
--rw-r--r--   0        0        0        0 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/__init__.py
--rw-r--r--   0        0        0      501 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/cache.py
--rw-r--r--   0        0        0     1235 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/install.py
--rw-r--r--   0        0        0     1767 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/list.py
--rw-r--r--   0        0        0      385 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/load.py
--rw-r--r--   0        0        0      257 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/post_install.py
--rw-r--r--   0        0        0      540 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/remove.py
--rw-r--r--   0        0        0      625 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/shell_env.py
--rw-r--r--   0        0        0      253 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/cmd/unload.py
--rw-r--r--   0        0        0      191 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/__init__.py
--rw-r--r--   0        0        0      246 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/android_studio/__init__.py
--rw-r--r--   0        0        0     1208 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/android_studio/install.py
--rw-r--r--   0        0        0      268 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/android_studio/post_install.py
--rw-r--r--   0        0        0      442 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/android_studio/remove.py
--rw-r--r--   0        0        0      428 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/brew/__init__.py
--rw-r--r--   0        0        0      859 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/brew/install.py
--rw-r--r--   0        0        0      289 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/cfw/__init__.py
--rw-r--r--   0        0        0     1278 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/cfw/install.py
--rw-r--r--   0        0        0      272 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/cfw/remove.py
--rw-r--r--   0        0        0      941 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/code/__init__.py
--rw-r--r--   0        0        0      920 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/code/install.py
--rw-r--r--   0        0        0      137 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/conda/__init__.py
--rw-r--r--   0        0        0     1368 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/conda/install.py
--rw-r--r--   0        0        0      634 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/conda/load.py
--rw-r--r--   0        0        0      625 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/conda/remove.py
--rw-r--r--   0        0        0       68 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/docker/__init__.py
--rw-r--r--   0        0        0      631 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/docker/install.py
--rw-r--r--   0        0        0      245 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/docker/load.py
--rw-r--r--   0        0        0      385 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/edge/__init__.py
--rw-r--r--   0        0        0      789 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/edge/install.py
--rw-r--r--   0        0        0      100 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/fonts/__init__.py
--rw-r--r--   0        0        0     1970 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/fonts/install.py
--rw-r--r--   0        0        0      344 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/fonts/remove.py
--rw-r--r--   0        0        0       17 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/gh/__init__.py
--rw-r--r--   0        0        0      197 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/gh/post_install.py
--rw-r--r--   0        0        0       19 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/llvm/__init__.py
--rw-r--r--   0        0        0      824 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/llvm/load.py
--rw-r--r--   0        0        0      212 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/llvm/unload.py
--rw-r--r--   0        0        0      179 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/motrix/__init__.py
--rw-r--r--   0        0        0      624 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/motrix/install.py
--rw-r--r--   0        0        0      295 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/motrix/remove.py
--rw-r--r--   0        0        0       18 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/obs/__init__.py
--rw-r--r--   0        0        0      296 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/obs/install.py
--rw-r--r--   0        0        0       42 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/reserves_lib_tsinghua_downloader/__init__.py
--rw-r--r--   0        0        0      961 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/reserves_lib_tsinghua_downloader/install.py
--rw-r--r--   0        0        0      322 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/typora/__init__.py
--rw-r--r--   0        0        0      685 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/typora/install.py
--rw-r--r--   0        0        0      129 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/virtualbox/__init__.py
--rw-r--r--   0        0        0     1135 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/virtualbox/install.py
--rw-r--r--   0        0        0      160 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/zotero/__init__.py
--rw-r--r--   0        0        0     1425 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/zotero/install.py
--rw-r--r--   0        0        0      275 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/pkg/zotero/remove.py
--rw-r--r--   0        0        0        0 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/utils/__init__.py
--rw-r--r--   0        0        0     1629 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/utils/cache.py
--rw-r--r--   0        0        0      157 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/utils/text.py
--rw-r--r--   0        0        0      103 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/utils/ubuntu/__init__.py
--rw-r--r--   0        0        0     1200 2023-01-25 19:49:33.644008 ipkg-0.1.9/ipkg/utils/ubuntu/desktop.py
--rw-r--r--   0        0        0      613 2023-01-25 19:49:33.644008 ipkg-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1161 1970-01-01 00:00:00.000000 ipkg-0.1.9/setup.py
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 ipkg-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-05 08:15:24.948840 ipkg-0.2.0/LICENSE
+-rw-r--r--   0        0        0      354 2023-07-05 08:15:24.948840 ipkg-0.2.0/README.md
+-rw-r--r--   0        0        0       19 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/__init__.py
+-rw-r--r--   0        0        0      820 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/cmd/main.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/config/__init__.py
+-rw-r--r--   0        0        0      301 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/config/path.py
+-rw-r--r--   0        0        0     1550 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/logging.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/btop/__init__.py
+-rw-r--r--   0        0        0      584 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/btop/install.py
+-rw-r--r--   0        0        0      419 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/btop/remove.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/conda/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/conda/install.py
+-rw-r--r--   0        0        0      188 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/pkg/conda/remove.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/__init__.py
+-rw-r--r--   0        0        0     1891 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/download.py
+-rw-r--r--   0        0        0      926 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/extract.py
+-rw-r--r--   0        0        0      212 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/mkdir.py
+-rw-r--r--   0        0        0      508 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/remove.py
+-rw-r--r--   0        0        0      240 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/shutils/run.py
+-rw-r--r--   0        0        0        0 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/utils/__init__.py
+-rw-r--r--   0        0        0      784 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/utils/github.py
+-rw-r--r--   0        0        0       62 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/utils/pkg.py
+-rw-r--r--   0        0        0      283 2023-07-05 08:15:24.948840 ipkg-0.2.0/ipkg/utils/typer.py
+-rw-r--r--   0        0        0      635 2023-07-05 08:15:24.952840 ipkg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 ipkg-0.2.0/PKG-INFO
```

### Comparing `ipkg-0.1.9/LICENSE` & `ipkg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipkg-0.1.9/pyproject.toml` & `ipkg-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
-[tool.isort]
-profile = "black"
-
 [tool.poetry]
-authors = ["Qin Li <liblaf@outlook.com>"]
+authors = ["liblaf <i@liblaf.me>"]
 description = "My Package Manager"
+documentation = "https://liblaf.github.io/ipkg/"
 license = "MIT"
 name = "ipkg"
 readme = "README.md"
 repository = "https://github.com/liblaf/ipkg"
-version = "0.1.9"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
-click = "^8.1.3"
-httpie = "^3.2.1"
-ishutils = "^0.2.0"
+httpie = "^3.2.2"
+pygithub = "^1.59.0"
 python = ">=3.11,<3.12"
-questionary = "^1.10.0"
-requests = "^2.28.1"
-
-[tool.poetry.group.build.dependencies]
-pyinstaller = "^5.7.0"
+requests = "^2.31.0"
+rich = "^13.4.2"
+tenacity = "^8.2.2"
+typer = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-isort = "^5.11.2"
+black = "^23.3.0"
+isort = "^5.12.0"
+nuitka = "^1.7"
+pyinstaller = "^5.13.0"
+typer-cli = "^0.0.13"
```

