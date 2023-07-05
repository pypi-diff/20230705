# Comparing `tmp/aiorun-2022.4.1.tar.gz` & `tmp/aiorun-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorun-2022.4.1.tar", last modified: Wed Apr 20 12:12:17 2022, max compression
+gzip compressed data, was "aiorun-2023.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiorun-2022.4.1.tar` & `aiorun-2023.7.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0      176 2020-08-23 12:13:16.000000 aiorun-2022.4.1/.coveragerc
--rw-r--r--   0        0        0      214 2020-08-23 12:13:16.000000 aiorun-2022.4.1/.dockerignore
--rw-r--r--   0        0        0       32 2020-08-23 12:13:16.000000 aiorun-2022.4.1/.flake8
--rw-r--r--   0        0        0       62 2020-08-23 12:13:16.000000 aiorun-2022.4.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      143 2021-08-20 12:27:36.345356 aiorun-2022.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2010 2022-04-20 12:02:01.870032 aiorun-2022.4.1/.github/workflows/pythonapp.yml
--rw-r--r--   0        0        0     1157 2020-08-23 12:13:16.000000 aiorun-2022.4.1/.gitignore
--rw-r--r--   0        0        0      751 2022-04-20 12:10:42.297949 aiorun-2022.4.1/CHANGES
--rw-r--r--   0        0        0      149 2022-04-20 11:50:37.599783 aiorun-2022.4.1/CONTRIBUTORS
--rw-r--r--   0        0        0    11357 2020-08-23 12:13:16.000000 aiorun-2022.4.1/LICENSE
--rw-r--r--   0        0        0    17615 2020-08-23 12:13:16.000000 aiorun-2022.4.1/README.rst
--rw-r--r--   0        0        0      193 2020-08-23 12:13:16.000000 aiorun-2022.4.1/TODO
--rw-r--r--   0        0        0    15634 2022-04-20 12:08:58.709102 aiorun-2022.4.1/aiorun.py
--rw-r--r--   0        0        0      171 2020-08-23 12:13:16.000000 aiorun-2022.4.1/docker-compose.yml
--rw-r--r--   0        0        0      442 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/echo_client.py
--rw-r--r--   0        0        0      705 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/echo_server.py
--rw-r--r--   0        0        0      147 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/stop_unhandled.py
--rw-r--r--   0        0        0      683 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/stop_unhandled_custom.py
--rw-r--r--   0        0        0      324 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/stop_unhandled_illegal.py
--rw-r--r--   0        0        0      262 2020-08-23 12:13:16.000000 aiorun-2022.4.1/examples/stop_unhandled_task.py
--rw-r--r--   0        0        0      884 2021-10-23 07:24:12.247204 aiorun-2022.4.1/pyproject.toml
--rw-r--r--   0        0        0      311 2020-08-23 12:13:16.000000 aiorun-2022.4.1/pytest.ini
--rw-r--r--   0        0        0       96 2021-10-23 07:24:12.247204 aiorun-2022.4.1/requirements-test.txt
--rw-r--r--   0        0        0      331 2020-08-23 12:13:16.000000 aiorun-2022.4.1/test.dockerfile
--rw-r--r--   0        0        0      330 2020-08-23 12:13:16.000000 aiorun-2022.4.1/test38.dockerfile
--rw-r--r--   0        0        0      359 2020-08-23 12:13:16.000000 aiorun-2022.4.1/tests/conftest.py
--rw-r--r--   0        0        0      290 2020-08-23 12:13:16.000000 aiorun-2022.4.1/tests/fake_main.py
--rw-r--r--   0        0        0    12135 2020-12-30 03:06:44.000000 aiorun-2022.4.1/tests/test_posix.py
--rw-r--r--   0        0        0     1732 2020-08-23 12:13:16.000000 aiorun-2022.4.1/tests/test_stop_on_errors.py
--rw-r--r--   0        0        0      947 2020-08-23 12:13:16.000000 aiorun-2022.4.1/tests/test_win.py
--rw-r--r--   0        0        0       84 2020-08-23 12:13:16.000000 aiorun-2022.4.1/watchtest.sh
--rw-r--r--   0        0        0    18522 1970-01-01 00:00:00.000000 aiorun-2022.4.1/PKG-INFO
+-rw-r--r--   0        0        0      176 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.coveragerc
+-rw-r--r--   0        0        0      214 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.dockerignore
+-rw-r--r--   0        0        0       32 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.flake8
+-rw-r--r--   0        0        0       62 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      143 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2045 2023-07-05 11:37:00.734767 aiorun-2023.7.1/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0     1157 2022-10-24 05:13:26.729633 aiorun-2023.7.1/.gitignore
+-rw-r--r--   0        0        0      751 2022-10-24 05:13:26.729633 aiorun-2023.7.1/CHANGES
+-rw-r--r--   0        0        0      213 2023-07-05 11:37:29.070554 aiorun-2023.7.1/CONTRIBUTORS
+-rw-r--r--   0        0        0    11357 2022-10-24 05:13:26.729633 aiorun-2023.7.1/LICENSE
+-rw-r--r--   0        0        0    18697 2022-10-24 05:13:26.729633 aiorun-2023.7.1/README.rst
+-rw-r--r--   0        0        0      193 2022-10-24 05:13:26.729633 aiorun-2023.7.1/TODO
+-rw-r--r--   0        0        0    17429 2023-07-05 11:52:31.187930 aiorun-2023.7.1/aiorun.py
+-rw-r--r--   0        0        0      171 2022-10-24 05:13:26.729633 aiorun-2023.7.1/docker-compose.yml
+-rw-r--r--   0        0        0      442 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/echo_client.py
+-rw-r--r--   0        0        0      705 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/echo_server.py
+-rw-r--r--   0        0        0      147 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/stop_unhandled.py
+-rw-r--r--   0        0        0      683 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/stop_unhandled_custom.py
+-rw-r--r--   0        0        0      324 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/stop_unhandled_illegal.py
+-rw-r--r--   0        0        0      262 2022-10-24 05:13:26.729633 aiorun-2023.7.1/examples/stop_unhandled_task.py
+-rw-r--r--   0        0        0      794 2023-03-18 17:49:30.751617 aiorun-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0      311 2022-10-24 05:13:26.729633 aiorun-2023.7.1/pytest.ini
+-rw-r--r--   0        0        0       96 2022-10-24 05:13:26.729633 aiorun-2023.7.1/requirements-test.txt
+-rw-r--r--   0        0        0      331 2022-10-24 05:13:26.729633 aiorun-2023.7.1/test.dockerfile
+-rw-r--r--   0        0        0      330 2022-10-24 05:13:26.729633 aiorun-2023.7.1/test38.dockerfile
+-rw-r--r--   0        0        0      359 2022-10-24 05:13:26.729633 aiorun-2023.7.1/tests/conftest.py
+-rw-r--r--   0        0        0      290 2022-10-24 05:13:26.729633 aiorun-2023.7.1/tests/fake_main.py
+-rw-r--r--   0        0        0    12135 2022-10-24 05:13:26.729633 aiorun-2023.7.1/tests/test_posix.py
+-rw-r--r--   0        0        0     2625 2023-03-18 17:43:59.033791 aiorun-2023.7.1/tests/test_stop_on_errors.py
+-rw-r--r--   0        0        0      947 2022-10-24 05:13:26.729633 aiorun-2023.7.1/tests/test_win.py
+-rw-r--r--   0        0        0      315 2022-10-24 05:13:26.729633 aiorun-2023.7.1/testshield.py
+-rw-r--r--   0        0        0       84 2022-10-24 05:13:26.729633 aiorun-2023.7.1/watchtest.sh
+-rw-r--r--   0        0        0    19509 1970-01-01 00:00:00.000000 aiorun-2023.7.1/PKG-INFO
```

### Comparing `aiorun-2022.4.1/.github/workflows/pythonapp.yml` & `aiorun-2023.7.1/.github/workflows/pythonapp.yml`

 * *Files 21% similar despite different names*

```diff
@@ -10,21 +10,16 @@
 
 jobs:
   build:
     name: Test on Python ${{ matrix.python-version }} and ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ['3.5', '3.6', '3.7', '3.8', '3.9', '3.10']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         os: [ubuntu-latest, windows-latest, macOS-latest]
-        exclude:
-          - os: macOS-latest
-            python-version: '3.5'
-          - os: macOS-latest
-            python-version: '3.6'
       fail-fast: false
     timeout-minutes: 15
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
@@ -49,19 +44,25 @@
 
     - name: Extract branch name
       shell: bash
       run: echo "##[set-output name=branch;]$(echo ${GITHUB_REF#refs/heads/})"
       id: extract_branch
     - name: Upload coverage
       env:
+          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
           COVERALLS_REPO_TOKEN: ${{ secrets.COVERALLS_REPO_TOKEN }}
           COVERALLS_PARALLEL: "true"
       if: matrix.os == 'ubuntu-latest'
       run: |
-        coveralls
-    - name: Finish parallel coverage
+        coveralls --service=github
+
+  coveralls:
+    name: Indicate completion to coveralls.io
+    needs: build
+    runs-on: ubuntu-latest
+    steps:
+    - name: Finished
       env:
-          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
-      if: matrix.os == 'ubuntu-latest'
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       run: |
-        coveralls --finish
-
+        pip3 install --upgrade coveralls
+        coveralls --service=github --finish
```

### Comparing `aiorun-2022.4.1/.gitignore` & `aiorun-2023.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/CHANGES` & `aiorun-2023.7.1/CHANGES`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/LICENSE` & `aiorun-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/README.rst` & `aiorun-2023.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,30 @@
     without a coroutine parameter, and it will still run forever.
 
     This is surprising to many people, because they sometimes expect that
     unhandled exceptions should abort the program, with an exception and
     a traceback. If you want this behaviour, please see the section on
     *error handling* further down.
 
+.. warning::
+
+    Note that `aiorun.run(coro)` will create a **new event loop instance**
+    every time it is invoked (same as `asyncio.run`). This might cause
+    confusing errors if your code interacts with the default event loop
+    instance provided by the stdlib `asyncio` library. For such situations
+    you can provide the actual loop you're using with
+    `aiorun.run(coro, loop=loop)`. There is more info about this further down.
+
+    However, generally speaking, configuring your own loop and providing
+    it in this way is a code smell. You will find it much easier to
+    reason about your code if you do all your task creation *inside*
+    an async context, such as within an `async def` function, because then
+    there will no ambiguity about which event loop is in play: it will
+    always be the one returned by `asyncio.get_running_loop()`.
+
 
 🤔 Why?
 ----------------
 
 The ``run()`` function will handle **everything** that normally needs
 to be done during the shutdown sequence of the application.  All you
 need to do is write your coroutines and run them.
@@ -400,29 +416,50 @@
 
 .. code-block:: python
 
     import asyncio
     from aiorun import run, shutdown_waits_for
 
     async def corofn():
-        await asyncio.sleep(60)
+        for i in range(10):
+            print(i)
+            await asyncio.sleep(1)
         print('done!')
 
     async def main():
         try:
             await shutdown_waits_for(corofn())
-        except asyncio.CancelledError
+        except asyncio.CancelledError:
             print('oh noes!')
 
     run(main())
 
-If you hit ``CTRL-C`` *before* 60 seconds has passed, you will see
-``oh noes!`` printed immediately, and then after 60 seconds (since start),
+If you hit ``CTRL-C`` *before* 10 seconds has passed, you will see
+``oh noes!`` printed immediately, and then after 10 seconds (since start),
 ``done!`` is printed, and thereafter the program exits.
 
+Output:
+
+.. code-block:: shell
+
+    $ python testshield.py
+    0
+    1
+    2
+    3
+    4
+    ^CStopping the loop
+    oh noes!
+    5
+    6
+    7
+    8
+    9
+    done!
+
 Behind the scenes, ``all_tasks()`` would have been cancelled by ``CTRL-C``,
 *except* ones wrapped in ``shutdown_waits_for()`` calls.  In this respect, it
 is loosely similar to ``asyncio.shield()``, but with special applicability
 to our shutdown scenario in ``aiorun()``.
 
 Be careful with this: the coroutine should still finish up at some point.
 The main use case for this is short-lived tasks that you don't want to
```

### Comparing `aiorun-2022.4.1/aiorun.py` & `aiorun-2023.7.1/aiorun.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,34 @@
 """Boilerplate for asyncio applications"""
+import asyncio
+import contextlib
+import inspect
+import logging
 import signal
 import sys
-import logging
-import inspect
-import asyncio
-from asyncio import get_event_loop, AbstractEventLoop, Task, gather, CancelledError
+from asyncio import AbstractEventLoop, CancelledError, all_tasks, get_event_loop
 from concurrent.futures import Executor, ThreadPoolExecutor
-from typing import Optional, Callable, Union, Any
+from functools import partial
+from typing import Awaitable, Callable, Coroutine, Optional, Union
+from weakref import WeakSet
 
-try:  # pragma: no cover
-    # Coroutine only arrived in Python 3.5.3, and Ubuntu 16.04 is unfortunately
-    # stuck on 3.5.2 for the time being. Revisit this in a year.
-    from typing import Coroutine, Awaitable
-
-    ShutdownCallback = Optional[
-        Union[
-            Awaitable,
-            Callable[[AbstractEventLoop], Awaitable],
-            Callable[[AbstractEventLoop], None],
-        ]
+ShutdownCallback = Optional[
+    Union[
+        Awaitable,
+        Callable[[AbstractEventLoop], Awaitable],
+        Callable[[AbstractEventLoop], None],
     ]
-
-except ImportError:  # pragma: no cover
-    Coroutine = Any
-    Awaitable = Any
-    ShutdownCallback = Any
-
-from weakref import WeakSet
-from functools import partial
+]
 
 
 __all__ = ["run", "shutdown_waits_for"]
-__version__ = "2022.04.1"
+__version__ = "2023.7.1"
 logger = logging.getLogger("aiorun")
 WINDOWS = sys.platform == "win32"
 
-try:
-    # asyncio.Task.all_tasks is deprecated in favour of asyncio.all_tasks
-    # in Python 3.7; remove ImportError handling when we drop support for
-    # 3.6.
-    from asyncio import all_tasks
-except ImportError:  # pragma: no cover
-    all_tasks = Task.all_tasks
-
 
 _DO_NOT_CANCEL_COROS = WeakSet()
 
 
 def shutdown_waits_for(coro, loop=None):
     """Prevent coro from being cancelled during the shutdown sequence.
 
@@ -129,26 +111,26 @@
     *,
     loop: Optional[AbstractEventLoop] = None,
     shutdown_handler: Optional[Callable[[AbstractEventLoop], None]] = None,
     shutdown_callback: "ShutdownCallback" = None,
     executor_workers: Optional[int] = None,
     executor: Optional[Executor] = None,
     use_uvloop: bool = False,
-    stop_on_unhandled_errors: bool = False
+    stop_on_unhandled_errors: bool = False,
+    timeout_task_shutdown: float = 60
 ) -> None:
     """
     Start up the event loop, and wait for a signal to shut down.
 
     :param coro: Optionally supply a coroutine. The loop will still
         run if missing. The loop will continue to run after the supplied
         coroutine finishes. The supplied coroutine is typically
         a "main" coroutine from which all other work is spawned.
-    :param loop: Optionally supply your own loop. If missing, the
-        default loop attached to the current thread context will
-        be used, i.e., whatever ``asyncio.get_event_loop()`` returns.
+    :param loop: Optionally supply your own loop. If missing, a new
+        event loop instance will be created.
     :param shutdown_handler: By default, SIGINT and SIGTERM will be
         handled and will stop the loop, thereby invoking the shutdown
         sequence. Alternatively you can supply your own shutdown
         handler function. It should conform to the type spec as shown
         in the function signature.
     :param shutdown_callback: Callable, executed after loop is stopped, before
         cancelling any tasks.
@@ -165,14 +147,20 @@
         ``ImportError`` will be raised.
     :param stop_on_unhandled_errors: By default, the event loop will
         handle any exceptions that get raised and are not handled. This
         means that the event loop will continue running regardless of errors,
         and the only way to stop it is to call `loop.stop()`. However, if
         this flag is set, any unhandled exceptions will stop the loop, and
         be re-raised after the normal shutdown sequence is completed.
+    :param timeout_task_shutdown: When shutdown is initiated, for example
+        by a signal like SIGTERM, or even by an unhandled exception if
+        ``stop_on_unhandled_errors`` is True, then the first action taken
+        during shutdown is to cancel all currently pending or running tasks
+        and then wait for them all to complete. This timeout sets an upper
+        limit on how long to wait.
     """
     _clear_signal_handlers()
     logger.debug("Entering run()")
     # Disable default signal handling ASAP
 
     if loop and use_uvloop:
         raise Exception(
@@ -223,18 +211,16 @@
             if a CancelledError bubbles up from anything in the
             group. To counteract that, we'll try to handle
             any CancelledErrors that bubble up from the given
             coro. This isn't fool-proof: if the user doesn't
             provide a coro, and instead creates their own with
             loop.create_task, that task might bubble
             a CancelledError into the run_until_complete()."""
-            try:
+            with contextlib.suppress(asyncio.CancelledError):
                 await coro
-            except asyncio.CancelledError:
-                pass
 
         loop.create_task(new_coro())
 
     shutdown_handler = shutdown_handler or _shutdown_handler
     # Setting up signal handlers. The callback configured by the
     # underlying system (non-asyncio) API ``signal.signal`` is
     # pre-emptive, which means you can't safely do loop manipulation
@@ -269,26 +255,26 @@
         logger.info("Got KeyboardInterrupt")
         if WINDOWS:
             # Windows doesn't do any POSIX signal handling, and no
             # abstraction layer for signals is currently implemented in
             # asyncio. So we fall back to KeyboardInterrupt (triggered
             # by the user/environment sending CTRL-C, or signal.CTRL_C_EVENT
             shutdown_handler(loop)
-    logger.info("Entering shutdown phase.")
 
+    logger.info("Entering shutdown phase.")
     if shutdown_callback is not None:
         logger.info("Executing provided shutdown_callback.")
         try:
             if inspect.iscoroutine(shutdown_callback):
                 loop.run_until_complete(shutdown_callback)
             elif inspect.iscoroutinefunction(shutdown_callback):
                 loop.run_until_complete(shutdown_callback(loop))
             elif callable(shutdown_callback):
                 shutdown_callback(loop)
-            else:
+            else:  # pragma: no cover
                 raise TypeError(
                     "The provided shutdown_callback must be either a function,"
                     "an awaitable, or a coroutine object, but it was "
                     + str(type(shutdown_callback))
                 )
         except BaseException as exc:
             if pending_exception_to_raise:
@@ -296,49 +282,90 @@
                     "The shutdown_callback() raised an error, but there is "
                     "already a different exception raised from the loop, so "
                     "this log message is all you're going to see about it."
                 )
             else:
                 pending_exception_to_raise = exc
 
-    def sep():
-        tasks = all_tasks(loop=loop)
-        do_not_cancel = set()
+    tasks = all_tasks(loop=loop)
+
+    if tasks:
+        logger.info("Cancelling pending tasks.")
         for t in tasks:
             # TODO: we don't need access to the coro. We could simply
             # TODO: store the task itself in the weakset.
-            if t._coro in _DO_NOT_CANCEL_COROS:
-                do_not_cancel.add(t)
+            if t._coro not in _DO_NOT_CANCEL_COROS:
+                logger.debug("Cancelling task: %s", t)
+                t.cancel()
+
+    async def wait_for_cancelled_tasks(timeout):
+        """ Wait for the cancelled tasks to finish up. They have received
+        CancelledError and must exit. However, it is possible that some
+        badly-behaved tasks catch CancelledError (or BaseException) and
+        then do not exit as they're supposed to. Thus, we only wait for
+        ``timeout`` and then return anyway.
+
+        To make it a bit easier to figure out when this is happening and
+        why, there is is a log message (WARNING level) that will show
+        the stack frames of all tasks that are still alive at the timeout.
+        This can be used to troubleshoot why those tasks did not exit.
+
+        Here is a sample of what the logs might look like (taken from one
+        of the tests.)
+
+        .. code-block::
+
+            <snip>
+            INFO:aiorun:Entering shutdown phase.
+            INFO:aiorun:Cancelling pending tasks.
+            DEBUG:aiorun:Cancelling task: \
+                <Task pending name='Task-2' coro=<test_stop_must_be_obeyed.<locals>.naughty_task() \
+                running at /home/caleb/Documents/repos/aiorun/tests/test_stop_on_errors.py:75> \
+                wait_for=<Future pending cb=[Task.task_wakeup()]>>
+            INFO:aiorun:Running pending tasks till complete
+            WARNING:aiorun:During shutdown, the following tasks were cancelled but refused to \
+                exit after 2.0 seconds: [<frame at 0x7f94484a3bc0, file \
+                '/home/caleb/Documents/repos/aiorun/tests/test_stop_on_errors.py', line 77, \
+                code naughty_task>]
+            INFO:aiorun:Waiting for executor shutdown.
+            INFO:aiorun:Shutting down async generators
+            INFO:aiorun:Closing the loop.
+            INFO:aiorun:Leaving. Bye!
+            INFO:aiorun:Reraising unhandled exception
+            <snip>
 
-        tasks -= do_not_cancel
-
-        logger.info("Cancelling pending tasks.")
-        for t in tasks:
-            logger.debug("Cancelling task: %s", t)
-            t.cancel()
-        return tasks, do_not_cancel
-
-    tasks, do_not_cancel = sep()
-     
-    async def wait_for_cancelled_tasks():
-        return await gather(*tasks, *do_not_cancel, return_exceptions=True)
+        """
+        _, pending = await asyncio.wait([*tasks], timeout=timeout)
+        if pending:
+            tasks_info = '\n\n'.join(str(t.get_stack()) for t in pending)
+            msg = (
+                "During shutdown, the following tasks refused "
+                "to exit after {timeout} seconds: {tasks_info}".format(
+                    timeout=timeout,
+                    tasks_info=tasks_info
+                )
+            )
+            logger.warning(msg)
 
-    if tasks or do_not_cancel:
+    if tasks:
         logger.info("Running pending tasks till complete")
         # TODO: obtain all the results, and log any results that are exceptions
         # other than CancelledError. Will be useful for troubleshooting.
-        loop.run_until_complete(wait_for_cancelled_tasks())
+        loop.run_until_complete(
+            wait_for_cancelled_tasks(
+                timeout=timeout_task_shutdown,
+            ),
+        )
 
     logger.info("Waiting for executor shutdown.")
     executor.shutdown(wait=True)
     # If loop was supplied, it's up to the caller to close!
     if not loop_was_supplied:
-        if sys.version_info >= (3, 6):
-            logger.info("Shutting down async generators")
-            loop.run_until_complete(loop.shutdown_asyncgens())
+        logger.info("Shutting down async generators")
+        loop.run_until_complete(loop.shutdown_asyncgens())
         logger.info("Closing the loop.")
         loop.close()
     logger.info("Leaving. Bye!")
 
     if pending_exception_to_raise:
         logger.info("Reraising unhandled exception")
         raise pending_exception_to_raise
@@ -361,15 +388,15 @@
     loop.call_soon_threadsafe(actual_handler, loop)
 
 
 def _shutdown_handler(loop):
     logger.debug("Entering shutdown handler")
     loop = loop or get_event_loop()
 
-    logger.critical("Stopping the loop")
+    logger.warning("Stopping the loop")
     loop.stop()
 
 
 def _set_signal_handlers(threadsafe_func):
     if WINDOWS:  # pragma: no cover
         signal.signal(signal.SIGBREAK, threadsafe_func)
         signal.signal(signal.SIGINT, threadsafe_func)
```

### Comparing `aiorun-2022.4.1/examples/echo_server.py` & `aiorun-2023.7.1/examples/echo_server.py`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/examples/stop_unhandled_custom.py` & `aiorun-2023.7.1/examples/stop_unhandled_custom.py`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/pyproject.toml` & `aiorun-2023.7.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 author = "Caleb Hattingh"
 author-email = "caleb.hattingh@gmail.com"
 home-page = "https://github.com/cjrh/aiorun"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent"
     ]
 description-file = "README.rst"
-requires = ["typing; python_version < '3.5'"]
-requires-python = ">=3.5"
+requires-python = ">=3.7"
 
 [tool.flit.metadata.requires-extra]
 dev = [
     "pytest",
     "pytest-cov"
 ]
```

### Comparing `aiorun-2022.4.1/tests/test_posix.py` & `aiorun-2023.7.1/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/tests/test_stop_on_errors.py` & `aiorun-2023.7.1/tests/test_stop_on_errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,7 +59,41 @@
         with pytest.raises(raised_exc) as excinfo:
             run(main(), stop_on_unhandled_errors=True)
             assert "test error" in str(excinfo.value)
     else:
         run(main(), stop_on_unhandled_errors=True)
 
     assert all(t.cancelled for t in created_tasks)
+
+
+def test_stop_must_be_obeyed(caplog):
+    """Basic SIGTERM"""
+
+    created_tasks = []
+
+    async def naughty_task():
+        try:
+            await asyncio.sleep(10)
+        except asyncio.CancelledError:
+            await asyncio.sleep(10)
+
+    async def main():
+        # loop = asyncio.get_running_loop()
+        loop = asyncio.get_event_loop()
+        created_tasks.append(
+            loop.create_task(
+                naughty_task(),
+            )
+        )
+        await asyncio.sleep(0.01)
+        raise Exception("Stops the loop")
+
+    with pytest.raises(Exception) as excinfo:
+        run(main(), stop_on_unhandled_errors=True, timeout_task_shutdown=2.0)
+
+    print(excinfo.value)
+    print(excinfo.traceback)
+    assert "tasks refused to exit after 2.0 seconds" in caplog.text
+    assert "Stops the loop" in str(excinfo.value)
+    assert all(t.cancelled for t in created_tasks)
+
+
```

### Comparing `aiorun-2022.4.1/tests/test_win.py` & `aiorun-2023.7.1/tests/test_win.py`

 * *Files identical despite different names*

### Comparing `aiorun-2022.4.1/PKG-INFO` & `aiorun-2023.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: aiorun
-Version: 2022.4.1
+Version: 2023.7.1
 Summary: Boilerplate for asyncio applications
 Home-page: https://github.com/cjrh/aiorun
 Author: Caleb Hattingh
 Author-email: caleb.hattingh@gmail.com
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Dist: typing; python_version < '3.5'
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
 Provides-Extra: dev
 
 .. image:: https://github.com/cjrh/aiorun/workflows/Python%20application/badge.svg
     :target: https://github.com/cjrh/aiorun/actions
 
@@ -84,14 +82,30 @@
     without a coroutine parameter, and it will still run forever.
 
     This is surprising to many people, because they sometimes expect that
     unhandled exceptions should abort the program, with an exception and
     a traceback. If you want this behaviour, please see the section on
     *error handling* further down.
 
+.. warning::
+
+    Note that `aiorun.run(coro)` will create a **new event loop instance**
+    every time it is invoked (same as `asyncio.run`). This might cause
+    confusing errors if your code interacts with the default event loop
+    instance provided by the stdlib `asyncio` library. For such situations
+    you can provide the actual loop you're using with
+    `aiorun.run(coro, loop=loop)`. There is more info about this further down.
+
+    However, generally speaking, configuring your own loop and providing
+    it in this way is a code smell. You will find it much easier to
+    reason about your code if you do all your task creation *inside*
+    an async context, such as within an `async def` function, because then
+    there will no ambiguity about which event loop is in play: it will
+    always be the one returned by `asyncio.get_running_loop()`.
+
 
 🤔 Why?
 ----------------
 
 The ``run()`` function will handle **everything** that normally needs
 to be done during the shutdown sequence of the application.  All you
 need to do is write your coroutines and run them.
@@ -424,29 +438,50 @@
 
 .. code-block:: python
 
     import asyncio
     from aiorun import run, shutdown_waits_for
 
     async def corofn():
-        await asyncio.sleep(60)
+        for i in range(10):
+            print(i)
+            await asyncio.sleep(1)
         print('done!')
 
     async def main():
         try:
             await shutdown_waits_for(corofn())
-        except asyncio.CancelledError
+        except asyncio.CancelledError:
             print('oh noes!')
 
     run(main())
 
-If you hit ``CTRL-C`` *before* 60 seconds has passed, you will see
-``oh noes!`` printed immediately, and then after 60 seconds (since start),
+If you hit ``CTRL-C`` *before* 10 seconds has passed, you will see
+``oh noes!`` printed immediately, and then after 10 seconds (since start),
 ``done!`` is printed, and thereafter the program exits.
 
+Output:
+
+.. code-block:: shell
+
+    $ python testshield.py
+    0
+    1
+    2
+    3
+    4
+    ^CStopping the loop
+    oh noes!
+    5
+    6
+    7
+    8
+    9
+    done!
+
 Behind the scenes, ``all_tasks()`` would have been cancelled by ``CTRL-C``,
 *except* ones wrapped in ``shutdown_waits_for()`` calls.  In this respect, it
 is loosely similar to ``asyncio.shield()``, but with special applicability
 to our shutdown scenario in ``aiorun()``.
 
 Be careful with this: the coroutine should still finish up at some point.
 The main use case for this is short-lived tasks that you don't want to
```

