# Comparing `tmp/bittensor-wallet-0.0.1.tar.gz` & `tmp/bittensor-wallet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-wallet-0.0.1.tar", last modified: Tue Jun 27 21:47:10 2023, max compression
+gzip compressed data, was "bittensor-wallet-0.0.2.tar", last modified: Wed Jul  5 20:29:07 2023, max compression
```

## Comparing `bittensor-wallet-0.0.1.tar` & `bittensor-wallet-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-27 21:47:10.165287 bittensor-wallet-0.0.1/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.1/LICENSE
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-06-27 21:47:10.165137 bittensor-wallet-0.0.1/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-06-27 20:58:47.000000 bittensor-wallet-0.0.1/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-27 21:47:10.163504 bittensor-wallet-0.0.1/bittensor_wallet/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-06-27 17:53:12.000000 bittensor-wallet-0.0.1/bittensor_wallet/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-27 21:47:10.164603 bittensor-wallet-0.0.1/bittensor_wallet/_keyfile/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-06-27 17:53:12.000000 bittensor-wallet-0.0.1/bittensor_wallet/_keyfile/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.1/bittensor_wallet/_keyfile/keyfile_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.1/bittensor_wallet/keypair_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.1/bittensor_wallet/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.1/bittensor_wallet/wallet_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-27 21:47:10.164318 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-06-27 21:47:10.000000 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      461 2023-06-27 21:47:10.000000 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-06-27 21:47:10.000000 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      165 2023-06-27 21:47:10.000000 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-06-27 21:47:10.000000 bittensor-wallet-0.0.1/bittensor_wallet.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-06-27 21:47:10.165331 bittensor-wallet-0.0.1/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-06-27 17:53:12.000000 bittensor-wallet-0.0.1/setup.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-06-27 21:47:10.164920 bittensor-wallet-0.0.1/tests/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11791 2023-06-26 22:03:52.000000 bittensor-wallet-0.0.1/tests/test.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9441 2023-06-26 22:03:51.000000 bittensor-wallet-0.0.1/tests/test_keypair.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.687801 bittensor-wallet-0.0.2/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1085 2023-06-27 17:13:40.000000 bittensor-wallet-0.0.2/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-05 20:29:07.687634 bittensor-wallet-0.0.2/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      711 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.684526 bittensor-wallet-0.0.2/bittensor_wallet/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5677 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.686058 bittensor-wallet-0.0.2/bittensor_wallet/_keyfile/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1796 2023-07-05 19:20:29.000000 bittensor-wallet-0.0.2/bittensor_wallet/_keyfile/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    20057 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.2/bittensor_wallet/_keyfile/keyfile_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1204 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.2/bittensor_wallet/keypair_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.686774 bittensor-wallet-0.0.2/bittensor_wallet/mock/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1226 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/mock/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3235 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/mock/keyfile_mock.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.687290 bittensor-wallet-0.0.2/bittensor_wallet/mock/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1122 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/mock/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1669 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/mock/utils/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3468 2023-07-05 20:25:59.000000 bittensor-wallet-0.0.2/bittensor_wallet/mock/wallet_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3781 2023-06-26 22:00:48.000000 bittensor-wallet-0.0.2/bittensor_wallet/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    24066 2023-06-26 22:09:07.000000 bittensor-wallet-0.0.2/bittensor_wallet/wallet_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-05 20:29:07.685531 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1944 2023-07-05 20:29:07.000000 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      611 2023-07-05 20:29:07.000000 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-05 20:29:07.000000 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      165 2023-07-05 20:29:07.000000 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       17 2023-07-05 20:29:07.000000 bittensor-wallet-0.0.2/bittensor_wallet.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-05 20:29:07.687880 bittensor-wallet-0.0.2/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3635 2023-07-05 19:20:29.000000 bittensor-wallet-0.0.2/setup.py
```

### Comparing `bittensor-wallet-0.0.1/LICENSE` & `bittensor-wallet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/PKG-INFO` & `bittensor-wallet-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.1
+Version: 0.0.2
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.0
+# BittensorWallet - v0.0.2
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.0
+pip install bittensor-wallet==0.0.2
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.1/README.md` & `bittensor-wallet-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# BittensorWallet - v0.0.0
+# BittensorWallet - v0.0.2
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.0
+pip install bittensor-wallet==0.0.2
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/__init__.py` & `bittensor-wallet-0.0.2/bittensor_wallet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO
 # THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 # OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __ss58_format__ = 42 # Bittensor ss58 format
 
 import argparse
 import copy
 import os
 from typing import Optional
```

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/_keyfile/__init__.py` & `bittensor-wallet-0.0.2/bittensor_wallet/_keyfile/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/_keyfile/keyfile_impl.py` & `bittensor-wallet-0.0.2/bittensor_wallet/_keyfile/keyfile_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/keypair_impl.py` & `bittensor-wallet-0.0.2/bittensor_wallet/keypair_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/utils.py` & `bittensor-wallet-0.0.2/bittensor_wallet/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet/wallet_impl.py` & `bittensor-wallet-0.0.2/bittensor_wallet/wallet_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-wallet-0.0.1/bittensor_wallet.egg-info/PKG-INFO` & `bittensor-wallet-0.0.2/bittensor_wallet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor-wallet
-Version: 0.0.1
+Version: 0.0.2
 Summary: BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the Bittensor API.
 Home-page: https://github.com/opentensor/bittensor-wallet
 Author: opentensor.ai
 Author-email: hello@opentensor.dev
 Maintainer: 
 Maintainer-email: 
 License: MIT
@@ -22,24 +22,24 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# BittensorWallet - v0.0.0
+# BittensorWallet - v0.0.2
 
 BittensorWallet is a library for managing wallet keypairs, keyfiles, etc. for the [Bittensor Python API](https://github.com/opentensor/bittensor).  
 
 The purpose of this repo is to separate the concern of keyfile management from the https://github.com/opentensor/bittensor repo, to decrease the attack surface of Bittensor related to local keys and wallet functionality.  
 
 # Installation
 This package can be installed from [PyPi.org](https://pypi.org/project/bittensor-wallet/):
 ```bash
-pip install bittensor-wallet==0.0.0
+pip install bittensor-wallet==0.0.2
 ```
 or via this repo (using [gh-cli](https://cli.github.com/)):  
 ```bash
 gh repo clone opentensor/bittensor-wallet
 cd bittensor-wallet
 pip install -e .
 ```
```

### Comparing `bittensor-wallet-0.0.1/setup.py` & `bittensor-wallet-0.0.2/setup.py`

 * *Files identical despite different names*

