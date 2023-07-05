# Comparing `tmp/sinol-make-1.1.2.tar.gz` & `tmp/sinol-make-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinol-make-1.1.2.tar", last modified: Mon Jul  3 17:26:47 2023, max compression
+gzip compressed data, was "sinol-make-1.2.0.tar", last modified: Wed Jul  5 08:33:47 2023, max compression
```

## Comparing `sinol-make-1.1.2.tar` & `sinol-make-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.400143 sinol-make-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-03 17:26:33.000000 sinol-make-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 17:26:47.400143 sinol-make-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-03 17:26:33.000000 sinol-make-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 17:26:33.000000 sinol-make-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:26:47.400143 sinol-make-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.392143 sinol-make-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.392143 sinol-make-1.1.2/src/sinol_make/commands/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/commands/run/
--rw-r--r--   0 runner    (1001) docker     (123)    36291 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/commands/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/commands/run/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/helpers/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/BaseCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-03 17:26:33.000000 sinol-make-1.1.2/src/sinol_make/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/src/sinol_make.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 17:26:47.000000 sinol-make-1.1.2/src/sinol_make.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:26:47.396143 sinol-make-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 17:26:33.000000 sinol-make-1.1.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.896764 sinol-make-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-05 08:33:37.000000 sinol-make-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 08:33:47.896764 sinol-make-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-05 08:33:37.000000 sinol-make-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-05 08:33:37.000000 sinol-make-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 08:33:47.896764 sinol-make-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/commands/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/commands/inwer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/commands/inwer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/commands/inwer/inwer_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/commands/inwer/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/commands/run/
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/commands/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/commands/run/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/helpers/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/helpers/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/helpers/package_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/helpers/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/interfaces/BaseCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/interfaces/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/structs/compiler_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-07-05 08:33:37.000000 sinol-make-1.2.0/src/sinol_make/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.892764 sinol-make-1.2.0/src/sinol_make.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 08:33:47.000000 sinol-make-1.2.0/src/sinol_make.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:33:47.896764 sinol-make-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-05 08:33:37.000000 sinol-make-1.2.0/tests/test_util.py
```

### Comparing `sinol-make-1.1.2/LICENSE` & `sinol-make-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.2/PKG-INFO` & `sinol-make-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.2
+Version: 1.2.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,13 +66,14 @@
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
 Run `sinol-make run --help` to see available flags.
+- `sinol-make inwer` -- Verifies whether input files are correct using your "inwer.cpp" program. You can specify what inwer
+program to use, what tests to check and how many CPUs to use. Run `sinol-make inwer --help` to see available flags.
 
 ### Reporting bugs and contributing code
 
 - Want to report a bug or request a feature? [Open an issue](https://github.com/sio2project/sinol-make/issues).
 - Want to help us build `sinol-make`? Create a Pull Request and we will gladly review it.
-
```

### Comparing `sinol-make-1.1.2/README.md` & `sinol-make-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -50,13 +50,14 @@
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
 Run `sinol-make run --help` to see available flags.
+- `sinol-make inwer` -- Verifies whether input files are correct using your "inwer.cpp" program. You can specify what inwer
+program to use, what tests to check and how many CPUs to use. Run `sinol-make inwer --help` to see available flags.
 
 ### Reporting bugs and contributing code
 
 - Want to report a bug or request a feature? [Open an issue](https://github.com/sio2project/sinol-make/issues).
 - Want to help us build `sinol-make`? Create a Pull Request and we will gladly review it.
-
```

### Comparing `sinol-make-1.1.2/pyproject.toml` & `sinol-make-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.2/src/sinol_make/__init__.py` & `sinol-make-1.2.0/src/sinol_make/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 import sys
 
 from sinol_make import util
 
-__version__ = "1.1.2"
+__version__ = "1.2.0"
 
 def configure_parsers():
     parser = argparse.ArgumentParser(
         prog='sinol-make',
         description='Tool for creating and testing sio2 tasks',
     )
     parser.add_argument("-v", "--version", action="version", version="%(prog)s " + __version__)
```

### Comparing `sinol-make-1.1.2/src/sinol_make/commands/run/__init__.py` & `sinol-make-1.2.0/src/sinol_make/commands/run/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Modified version of https://sinol3.dasie.mimuw.edu.pl/oij/jury/package/-/blob/master/runner.py
 # Author of the original code: Bartosz Kostka <kostka@oij.edu.pl>
 # Version 0.6 (2021-08-29)
 
 from sinol_make.commands.run.structs import ExecutionResult, ResultChange, ValidationResult, ExecutionData
+from sinol_make.helpers.parsers import add_compilation_arguments
 from sinol_make.interfaces.BaseCommand import BaseCommand
 from sinol_make.interfaces.Errors import CompilationError
-from sinol_make.helpers import compile, compiler
+from sinol_make.helpers import compile, compiler, package_util
 import sinol_make.util as util
 import yaml, os, collections, sys, re, math, dictdiffer
 import multiprocessing as mp
 
 class Command(BaseCommand):
     """
     Class for running current task
@@ -45,22 +46,15 @@
                             help='hide memory usage in report')
         parser.add_argument('--solutions_report', type=str,
                             help='file to store report from solution executions (in markdown)')
         parser.add_argument('--time_tool', choices=['oiejq', 'time'], default=default_timetool,
                             help='tool to measure time and memory usage (default when possible: oiejq)')
         parser.add_argument('--oiejq_path', type=str,
                             help='path to oiejq executable (default: `~/.local/bin/oiejq`)')
-        parser.add_argument('--c_compiler_path', type=str, default=compiler.get_c_compiler_path(),
-                            help='C compiler to use (default for Linux and Windows: gcc, default for Mac: gcc-9 or gcc-10)')
-        parser.add_argument('--cpp_compiler_path', type=str, default=compiler.get_cpp_compiler_path(),
-                            help='C++ compiler to use (default for Linux and Windows: g++, default for Mac: g++-9 or g++-10)')
-        parser.add_argument('--python_interpreter_path', type=str, default=compiler.get_python_interpreter_path(),
-                            help='Python interpreter to use (default: python3)')
-        parser.add_argument('--java_compiler_path', type=str, default=compiler.get_java_compiler_path(),
-                            help='Java compiler to use (default: javac)')
+        add_compilation_arguments(parser)
         parser.add_argument('--weak_compilation_flags', dest='weak_compilation_flags', action='store_true',
                             help='use weaker compilation flags')
         parser.add_argument('--apply_suggestions', dest='apply_suggestions', action='store_true',
                             help='apply suggestions from expected scores report')
 
 
     def color_memory(self, memory, limit):
@@ -91,41 +85,28 @@
 
 
     def parse_memory(self, memory_str):
         if len(memory_str) < 3: return -1
         return int(memory_str[:-2])
 
 
-    def extract_test_no(self, test_path):
-        return os.path.split(os.path.splitext(test_path)[0])[1][3:]
+    def extract_test_id(self, test_path):
+        return os.path.split(os.path.splitext(test_path)[0])[1][len(self.ID):]
 
 
     def extract_file_name(self, file_path):
         return os.path.split(file_path)[1]
 
 
     def get_group(self, test_path):
-        return int("".join(filter(str.isdigit, self.extract_test_no(test_path))))
-
-
-    def get_test_key(self, test):
-        return (self.get_group(test), test)
-
-
-    def get_tests(self, arg_tests):
-        if arg_tests is None:
-            all_tests = ["in/%s" % test for test in os.listdir("in/")
-                         if test[-3:] == ".in"]
-            return sorted(all_tests, key=self.get_test_key)
-        else:
-            return sorted(list(set(arg_tests)), key=self.get_test_key)
+        return int("".join(filter(str.isdigit, self.extract_test_id(test_path))))
 
 
     def get_executable_key(self, executable):
-        name = self.extract_file_name(executable)
+        name = package_util.get_file_name(executable)
         value = [0, 0]
         if name[3] == 's':
             value[0] = 1
             suffix = name.split(".")[0][4:]
         elif name[3] == 'b':
             value[0] = 2
             suffix = name.split(".")[0][4:]
@@ -154,20 +135,16 @@
             for solution in args_solutions:
                 if not os.path.isfile(solution):
                     util.exit_with_error("Solution %s does not exist" % solution)
                 solutions.append(os.path.basename(solution))
             return sorted(solutions, key=self.get_executable_key)
 
 
-    def get_executable(self, file):
-        return os.path.splitext(self.extract_file_name(file))[0] + ".e"
-
-
     def get_executables(self, args_solutions):
-        return [os.get_executable(solution) for solution in self.get_solutions(args_solutions)]
+        return [package_util.get_executable(solution) for solution in self.get_solutions(args_solutions)]
 
 
     def get_possible_score(self, groups):
         possible_score = 0
         for group in groups:
             possible_score += self.scores[group]
         return possible_score
@@ -186,28 +163,28 @@
         if not all(compilation_results):
             util.exit_with_error("\nCompilation failed.")
         return compilation_results
 
 
     def compile(self, solution):
         compile_log_file = os.path.join(
-            self.COMPILATION_DIR, "%s.compile_log" % self.extract_file_name(solution))
+            self.COMPILATION_DIR, "%s.compile_log" % package_util.get_file_name(solution))
         source_file = os.path.join(os.getcwd(), "prog", self.get_solution_from_exe(solution))
-        output = os.path.join(self.EXECUTABLES_DIR, self.get_executable(solution))
+        output = os.path.join(self.EXECUTABLES_DIR, package_util.get_executable(solution))
 
         try:
             compile.compile(source_file, output, self.compilers,
                             open(compile_log_file, "w"), self.args.weak_compilation_flags)
             print(util.info("Compilation of file %s was successful."
-                            % self.extract_file_name(solution)))
+                            % package_util.get_file_name(solution)))
             return True
         except CompilationError as e:
             print(util.error("Compilation of file %s was unsuccessful."
-                             % self.extract_file_name(solution)))
-            os.system("head -c 500 %s" % compile_log_file) # TODO: make this work on Windows
+                             % package_util.get_file_name(solution)))
+            compile.print_compile_log(compile_log_file)
             return False
 
 
     def execute_oiejq(self, command, result_file, output_file, answer_file, time_limit, memory_limit):
         timeout_exit_code = os.system(command)
         result = ExecutionResult(None, None, None)
         with open(result_file) as r:
@@ -287,15 +264,15 @@
 
     def run_solution(self, data_for_execution: ExecutionData):
         """
         Run an execution and return the result as ExecutionResult object.
         """
 
         (name, executable, test, time_limit, memory_limit, timetool_path) = data_for_execution
-        file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, self.extract_test_no(test))
+        file_no_ext = os.path.join(self.EXECUTIONS_DIR, name, self.extract_test_id(test))
         output_file = file_no_ext + ".out"
         result_file = file_no_ext + ".res"
         hard_time_limit_in_s = math.ceil(2 * time_limit / 1000.0)
 
         if self.args.time_tool == 'oiejq':
             command = "MEM_LIMIT=%sK MEASURE_MEM=true timeout -k %ds -s SIGKILL %ds %s %s <%s >%s 2>%s" \
                       % (memory_limit, hard_time_limit_in_s,
@@ -433,15 +410,15 @@
                 # TODO: always display both tables
                 # if self.args.verbose:
                 #   print_stream(6*" ", end=" | ")
                 #   for program in program_group:
                 #       print_stream(10*" ", end=" | ")
                 #   print_stream()
                 #   for test in self.tests:
-                #       print_stream("%6s" % self.extract_test_no(test), end=" | ")
+                #       print_stream("%6s" % self.extract_test_id(test), end=" | ")
                 #       for program in program_group:
                 #           result = all_results[program][self.get_group(test)][test]
                 #           status = result.Status
                 #           if status == "  ": print_stream(10*' ', end=" | ")
                 #           else:
                 #               print_stream("%3s" % self.colorize_status(status),
                 #                   ("%17s" % self.color_time(result.Time, self.time_limit)) if getattr(result, "Time") is not None else 7*" ", end=" | ")
@@ -480,15 +457,15 @@
                 points += self.config["scores"][group]
         return points
 
 
     def compile_and_run(self, solutions):
         compilation_results = self.compile_solutions(solutions)
         os.makedirs(self.EXECUTIONS_DIR, exist_ok=True)
-        executables = [os.path.join(self.EXECUTABLES_DIR, self.get_executable(solution))
+        executables = [os.path.join(self.EXECUTABLES_DIR, package_util.get_executable(solution))
                        for solution in solutions]
         compiled_commands = zip(solutions, executables, compilation_results)
         names = solutions
         return self.run_solutions(compiled_commands, names, solutions, self.args.solutions_report)
 
 
     def print_expected_scores(self, expected_scores):
@@ -634,62 +611,26 @@
                 util.save_config(self.config)
                 print(util.info("Saved suggested expected scores description."))
             else:
                 util.exit_with_error("Use flag --apply_suggestions to apply suggestions.")
 
 
     def set_constants(self):
-        self.ID = os.path.split(os.getcwd())[-1]
+        self.ID = package_util.get_task_id()
         self.TMP_DIR = os.path.join(os.getcwd(), "cache")
         self.COMPILATION_DIR = os.path.join(self.TMP_DIR, "compilation")
         self.EXECUTIONS_DIR = os.path.join(self.TMP_DIR, "executions")
         self.EXECUTABLES_DIR = os.path.join(self.TMP_DIR, "executables")
         self.SOURCE_EXTENSIONS = ['.c', '.cpp', '.py', '.java']
         self.PROGRAMS_IN_ROW = 8
         self.SOLUTIONS_RE = re.compile(r"^%s[bs]?[0-9]*\.(cpp|cc|java|py|pas)$" % self.ID)
 
 
     def validate_arguments(self, args):
-        for solution in self.get_solutions(None):
-            ext = os.path.splitext(solution)[1]
-            compiler = ""
-            tried = ""
-            flag = ""
-            if ext == '.c' and args.c_compiler_path is None:
-                compiler = 'C compiler'
-                flag = '--c_compiler_path'
-                if sys.platform == 'darwin':
-                    tried = 'gcc-{9,10}'
-                else:
-                    tried = 'gcc'
-            elif ext == '.cpp' and args.cpp_compiler_path is None:
-                compiler = 'C++ compiler'
-                flag = '--cpp_compiler_path'
-                if sys.platform == 'darwin':
-                    tried = 'g++-{9,10}'
-                else:
-                    tried = 'g++'
-            elif ext == '.py' and args.python_interpreter_path is None:
-                compiler = 'Python interpreter'
-                flag = '--python_interpreter_path'
-                tried = 'python3'
-            elif ext == '.java' and args.java_compiler_path is None:
-                compiler = 'Java compiler'
-                flag = '--java_compiler_path'
-                tried = 'javac'
-
-            if compiler != "":
-                util.exit_with_error('Couldn\'t find a %s. Tried %s. Try specifying a compiler with %s.' % (compiler, tried, flag))
-
-        compilers = {
-            'c_compiler_path': args.c_compiler_path,
-            'cpp_compiler_path': args.cpp_compiler_path,
-            'python_interpreter_path': args.python_interpreter_path,
-            'java_compiler_path': args.java_compiler_path
-        }
+        compilers = compiler.verify_compilers(args, self.get_solutions(None))
 
         timetool_path = None
         if args.time_tool == 'oiejq':
             if sys.platform != 'linux':
                 util.exit_with_error('oiejq is only available on Linux.')
             if 'oiejq_path' in args and args.oiejq_path is not None:
                 if not util.check_oiejq(args.oiejq_path):
@@ -726,42 +667,52 @@
             util.exit_with_error('Memory limit was not defined in config.yml.')
         if not 'scores' in self.config.keys():
             util.exit_with_error('Scores were not defined in config.yml.')
 
         self.compilers, self.timetool_path = self.validate_arguments(args)
 
         title = self.config["title"]
-        print("Task %s (%s)" % (title, self.ID))
+        print("Task: %s (tag: %s)" % (title, self.ID))
         config_time_limit = self.config["time_limit"]
         config_memory_limit = self.config["memory_limit"]
         self.time_limit = args.tl * 1000.0 if args.tl is not None else config_time_limit
         self.memory_limit = args.ml * 1024 if args.ml is not None else config_memory_limit
         self.cpus = args.cpus or mp.cpu_count()
         if self.time_limit == config_time_limit:
-            print("Time limit (in ms):", self.time_limit)
+            print(f'Time limit: {self.time_limit} ms')
         else:
-            print("Time limit (in ms):", self.time_limit,
+            print(f'Time limit: {self.time_limit} ms',
                   util.warning(("[originally was %.1f ms]" % config_time_limit)))
         if self.memory_limit == config_memory_limit:
-            print("Memory limit (in kb):", self.memory_limit)
+            print(f'Memory limit: {self.memory_limit} kB')
         else:
-            print("Memory limit (in kb):", self.memory_limit,
+            print(f'Memory limit: {self.memory_limit} kB',
                   util.warning(("[originally was %.1f kb]" % config_memory_limit)))
         self.scores = collections.defaultdict(int)
         print("Scores:")
         total_score = 0
         for group in self.config["scores"]:
             self.scores[group] = self.config["scores"][group]
             print("%2d: %3d" % (group, self.scores[group]))
             total_score += self.scores[group]
         if total_score != 100:
             print(util.warning("WARN: Scores sum up to %d (instead of 100)." % total_score))
         print()
 
-        self.tests = self.get_tests(args.tests)
+        self.tests = package_util.get_tests(args.tests)
+
+        if len(self.tests) > 0:
+            print(util.bold('Tests that will be run:'), ' '.join([self.extract_file_name(test) for test in self.tests]))
+
+            example_tests = [test for test in self.tests if self.get_group(test) == 0]
+            if len(example_tests) == len(self.tests):
+                print(util.warning('Running only on example tests.'))
+        else:
+            print(util.warning('There are no tests to run.'))
+
         self.groups = list(sorted(set([self.get_group(test) for test in self.tests])))
         self.possible_score = self.get_possible_score(self.groups)
 
         solutions = self.get_solutions(self.args.solutions)
         results = self.compile_and_run(solutions)
         validation_results = self.validate_expected_scores(results)
         self.print_expected_scores_diff(validation_results)
```

### Comparing `sinol-make-1.1.2/src/sinol_make/commands/run/structs.py` & `sinol-make-1.2.0/src/sinol_make/commands/run/structs.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.2/src/sinol_make/helpers/compile.py` & `sinol-make-1.2.0/src/sinol_make/helpers/compile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,43 @@
+from typing import Tuple
+
 import sinol_make.helpers.compiler as compiler
 from sinol_make.interfaces.Errors import CompilationError
+from sinol_make.structs.compiler_structs import Compilers
 import os, subprocess, sys
 
-def compile(program, output, compilers = None, compile_log = None, weak_compilation_flags = False):
+def compile(program, output, compilers: Compilers = None, compile_log = None, weak_compilation_flags = False):
     """
     Compile a program
-    compilers - A dictionary of compilers to use. If not set, the default compilers will be used
+    compilers - A Compilers object with compilers to use. If None, default compilers will be used.
     """
     gcc_compilation_flags = '-Werror -Wall -Wextra -Wshadow -Wconversion -Wno-unused-result -Wfloat-equal'
     if weak_compilation_flags:
         gcc_compilation_flags = '-w' # Disable all warnings
 
+    if compilers is None:
+        compilers = Compilers()
+
     ext = os.path.splitext(program)[1]
     arguments = []
     if ext == '.cpp':
-        arguments = [compilers['cpp_compiler_path'] or compiler.get_cpp_compiler_path(), program, '-o', output] + \
+        arguments = [compilers.cpp_compiler_path or compiler.get_cpp_compiler_path(), program, '-o', output] + \
                     f'--std=c++17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.c':
-        arguments = [compilers['c_compiler_path'] or compiler.get_c_compiler_path(), program, '-o', output] + \
+        arguments = [compilers.c_compiler_path, program, '-o', output] + \
                     f'--std=c17 -O3 -lm {gcc_compilation_flags} -fdiagnostics-color'.split(' ')
     elif ext == '.py':
         if sys.platform == 'win32' or sys.platform == 'cygwin':
             # TODO: Make this work on Windows
             pass
         else:
             open(output, 'w').write('#!/usr/bin/python3\n')
             open(output, 'a').write(open(program, 'r').read())
             subprocess.call(['chmod', '+x', output])
-        arguments = [compilers['python_interpreter_path'] or compiler.get_python_interpreter_path(), '-m', 'py_compile', program]
+        arguments = [compilers.python_interpreter_path, '-m', 'py_compile', program]
     elif ext == '.java':
         raise NotImplementedError('Java compilation is not implemented')
     else:
         raise CompilationError('Unknown file extension: ' + ext)
 
     process = subprocess.Popen(arguments, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     process.wait()
@@ -42,7 +48,47 @@
     else:
         print(out.decode('utf-8'))
 
     if process.returncode != 0:
         raise CompilationError('Compilation failed')
     else:
         return True
+
+
+def compile_file(file_path: str, name: str, compilers: Compilers) -> Tuple[str or None, str]:
+    """
+    Compile a file
+    :param file_path: Path to the file to compile
+    :param name: Name of the executable
+    :param compilers: Compilers object
+    :return: Tuple of (executable path or None if compilation failed, log path)
+    """
+
+    executable_dir = os.path.join(os.getcwd(), 'cache', 'executables')
+    compile_log_dir = os.path.join(os.getcwd(), 'cache', 'compilation')
+    os.makedirs(executable_dir, exist_ok=True)
+    os.makedirs(compile_log_dir, exist_ok=True)
+
+    output = os.path.join(executable_dir, name)
+    compile_log_path = os.path.join(compile_log_dir, os.path.splitext(name)[0] + '.compile_log')
+    compile_log = open(compile_log_path, 'w')
+
+    try:
+        if compile(file_path, output, compilers, compile_log):
+            return output, compile_log_path
+        else:
+            return None, compile_log_path
+    except CompilationError:
+        return None, compile_log_path
+
+
+def print_compile_log(compile_log_path: str):
+    """
+    Print the first 500 lines of compilation log
+    :param compile_log_path: path to the compilation log
+    """
+
+    compile_log = open(compile_log_path, 'r')
+    lines = compile_log.readlines()
+    compile_log.close()
+    for line in lines[:500]:
+        print(line, end='')
```

### Comparing `sinol-make-1.1.2/src/sinol_make/util.py` & `sinol-make-1.2.0/src/sinol_make/util.py`

 * *Files identical despite different names*

### Comparing `sinol-make-1.1.2/src/sinol_make.egg-info/PKG-INFO` & `sinol-make-1.2.0/src/sinol_make.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinol-make
-Version: 1.1.2
+Version: 1.2.0
 Summary: CLI tool for creating sio2 task packages
 Author-email: Mateusz Masiarz <m.masiarz@fri.edu.pl>
 Maintainer-email: Tomasz Nowak <tomasz.nowak@tonowak.com>
 Project-URL: Homepage, https://github.com/sio2project/sinol-make
 Project-URL: Bug Tracker, https://github.com/sio2project/sinol-make/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -66,13 +66,14 @@
 
 The availabe commands (see `sinol-make --help`) are:
 
 - `sinol-make run` -- Runs selected solutions (by default all solutions) on selected tests (by default all tests) with a given number
 of CPUs. Measures the solutions' time with oiejq, unless specified otherwise. After running the solutions, it
 compares the solutions' scores with the ones saved in config.yml.
 Run `sinol-make run --help` to see available flags.
+- `sinol-make inwer` -- Verifies whether input files are correct using your "inwer.cpp" program. You can specify what inwer
+program to use, what tests to check and how many CPUs to use. Run `sinol-make inwer --help` to see available flags.
 
 ### Reporting bugs and contributing code
 
 - Want to report a bug or request a feature? [Open an issue](https://github.com/sio2project/sinol-make/issues).
 - Want to help us build `sinol-make`? Create a Pull Request and we will gladly review it.
-
```

### Comparing `sinol-make-1.1.2/src/sinol_make.egg-info/SOURCES.txt` & `sinol-make-1.2.0/src/sinol_make.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 src/sinol_make/util.py
 src/sinol_make.egg-info/PKG-INFO
 src/sinol_make.egg-info/SOURCES.txt
 src/sinol_make.egg-info/dependency_links.txt
 src/sinol_make.egg-info/entry_points.txt
 src/sinol_make.egg-info/requires.txt
 src/sinol_make.egg-info/top_level.txt
+src/sinol_make/commands/inwer/__init__.py
+src/sinol_make/commands/inwer/inwer_util.py
+src/sinol_make/commands/inwer/structs.py
 src/sinol_make/commands/run/__init__.py
 src/sinol_make/commands/run/structs.py
 src/sinol_make/helpers/__init__.py
 src/sinol_make/helpers/compile.py
 src/sinol_make/helpers/compiler.py
+src/sinol_make/helpers/package_util.py
+src/sinol_make/helpers/parsers.py
 src/sinol_make/interfaces/BaseCommand.py
 src/sinol_make/interfaces/Errors.py
 src/sinol_make/interfaces/__init__.py
+src/sinol_make/structs/compiler_structs.py
 tests/test_util.py
```

