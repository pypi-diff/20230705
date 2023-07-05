# Comparing `tmp/qiskit_debugger-0.1.0.tar.gz` & `tmp/qiskit_debugger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_debugger-0.1.0.tar", last modified: Mon Jul  3 21:38:52 2023, max compression
+gzip compressed data, was "qiskit_debugger-0.1.1.tar", last modified: Wed Jul  5 14:11:32 2023, max compression
```

## Comparing `qiskit_debugger-0.1.0.tar` & `qiskit_debugger-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:38:52.938912 qiskit_debugger-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1104 2023-05-05 22:01:01.000000 qiskit_debugger-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      338 2023-07-03 21:38:52.938912 qiskit_debugger-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6651 2023-05-05 21:46:02.000000 qiskit_debugger-0.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       87 2023-05-05 22:01:58.000000 qiskit_debugger-0.1.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:38:52.938912 qiskit_debugger-0.1.0/qiskit_debugger/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 21:38:52.938912 qiskit_debugger-0.1.0/qiskit_debugger/qiskit_debugger.egg-info/
--rw-r--r--   0 root         (0) root         (0)      338 2023-07-03 21:38:52.000000 qiskit_debugger-0.1.0/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      261 2023-07-03 21:38:52.000000 qiskit_debugger-0.1.0/qiskit_debugger/qiskit_debugger.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 21:38:52.000000 qiskit_debugger-0.1.0/qiskit_debugger/qiskit_debugger.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-03 21:38:52.000000 qiskit_debugger-0.1.0/qiskit_debugger/qiskit_debugger.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 21:38:52.938912 qiskit_debugger-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-03 21:00:56.000000 qiskit_debugger-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-05-05 22:01:01.000000 qiskit_debugger-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7050 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-07-05 14:10:54.000000 qiskit_debugger-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-05 22:01:58.000000 qiskit_debugger-0.1.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/qiskit_debugger/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7050 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-05 14:11:32.000000 qiskit_debugger-0.1.1/qiskit_debugger/qiskit_debugger.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 14:11:32.524083 qiskit_debugger-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-04 21:50:24.000000 qiskit_debugger-0.1.1/setup.py
```

### Comparing `qiskit_debugger-0.1.0/LICENSE` & `qiskit_debugger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_debugger-0.1.0/README.md` & `qiskit_debugger-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 # Breakpoint Debugging on a Physical Qunatum Circuit
 
-## Group Members
-- Palvit Garg (pgarg5)
-- Harshwardhan Joshi (hjoshi2)
-- Shawn Salekin (ssaleki)
-
-#### Presentation
-[URL](https://docs.google.com/presentation/d/1SCwHKmPCc7U0Hl_CVZLNMto9HAEyD_zuz_fqGwnIzuc/edit?usp=sharing)
-
 ## Problem Description
 In classical computing, debugging with breakpoint means halting the program
 execution at any given point and freezing the program state. This allows
 programmers to examine the program internals mid-execution (as in, what
 variables contain which values, analyze control flow etc.) Unfortunately, in
 quantum computing, doing this is not possible. Qubits in a quantum circuit have
 probabilistic values (in superposition), and the act of measuring collapses the
 qubits to a deterministic state.
 
 Breakpoint debugging is still needed for quantum computing, so our problem boils
 down to measuring at the breakpoint and preserving enough information to
 “recreate” that state and continue execution from that point.
 
+## Group Members
+- Palvit Garg (pgarg5)
+- Harshwardhan Joshi (hjoshi2)
+- Shawn Salekin (ssaleki)
+
+#### Presentation
+[URL](https://docs.google.com/presentation/d/1SCwHKmPCc7U0Hl_CVZLNMto9HAEyD_zuz_fqGwnIzuc/edit?usp=sharing)
+
 ## How To Test
 We are assuming you are faimilar with Qiskit and git. We'd also assume you have
 jupyter notebook installed on your system. 
 
-1. clone this repo: `git clone https://github.ncsu.edu/ssaleki/qc_besteffort_breakpoint_debugging.git`
+1. Install this library via pip
+```
+pip install qiskit_debugger
+``` 
 
 2. Ensure the following python libraries are installed in either a) python virtual environment, or b) jupyter notebook kernel.
 ```
 qiskit-ibm-runtime==0.6.2
 qiskit-aer==0.11.0
 matplotlib==3.6.0
 ```
```

### Comparing `qiskit_debugger-0.1.0/setup.py` & `qiskit_debugger-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from setuptools import setup
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE/"README.md").read_text()
 
 setup(
    name="qiskit_debugger", 
-   version="0.1.0", 
-   descp="Quantum Circuit debugger for the Qiskit SDK.", 
-   long_descp=README,
-   long_descp_content="text/markdown", 
+   version="0.1.1", 
+   description="Quantum Circuit debugger for the Qiskit SDK.", 
+   long_description=README,
+   long_description_content_type="text/markdown",
    URL="https://github.com/salekinsirajus/qiskit_quantum_circuit_debugger", 
    author="Sirajus Salekin", 
    authoremail="ssalekin14@gmail.com", 
    license="MIT", 
    classifiers=[ 
         "License :: OSI Approved :: MIT License", 
         "Programming Language :: Python :: 3",
```

