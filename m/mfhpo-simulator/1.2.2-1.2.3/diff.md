# Comparing `tmp/mfhpo_simulator-1.2.2-py3-none-any.whl.zip` & `tmp/mfhpo_simulator-1.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 26041 bytes, number of entries: 15
--rw-rw-r--  2.0 unx      560 b- defN 23-Jul-01 06:46 benchmark_simulator/__init__.py
--rw-rw-r--  2.0 unx     6127 b- defN 23-Jul-01 05:59 benchmark_simulator/_constants.py
--rw-rw-r--  2.0 unx    11227 b- defN 23-Jul-01 05:59 benchmark_simulator/_secure_proc.py
+Zip file size: 27265 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx      560 b- defN 23-Jul-05 11:48 benchmark_simulator/__init__.py
+-rw-rw-r--  2.0 unx     7646 b- defN 23-Jul-04 15:16 benchmark_simulator/_constants.py
+-rw-rw-r--  2.0 unx    11741 b- defN 23-Jul-04 14:42 benchmark_simulator/_secure_proc.py
 -rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-14 22:34 benchmark_simulator/_utils.py
--rw-rw-r--  2.0 unx    20853 b- defN 23-Jul-01 05:59 benchmark_simulator/simulator.py
--rw-rw-r--  2.0 unx     2544 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_base_wrapper.py
--rw-rw-r--  2.0 unx     2978 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_utils.py
--rw-rw-r--  2.0 unx    11790 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker.py
--rw-rw-r--  2.0 unx     3142 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker_manager.py
--rw-rw-r--  2.0 unx     8367 b- defN 23-Jul-01 05:59 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      307 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       51 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-01 06:48 mfhpo_simulator-1.2.2.dist-info/RECORD
-15 files, 81971 bytes uncompressed, 23675 bytes compressed:  71.1%
+-rw-rw-r--  2.0 unx    25336 b- defN 23-Jul-05 11:47 benchmark_simulator/simulator.py
+-rw-rw-r--  2.0 unx     2582 b- defN 23-Jul-04 07:45 benchmark_simulator/_simulator/_base_wrapper.py
+-rw-rw-r--  2.0 unx     2978 b- defN 23-Jul-04 16:11 benchmark_simulator/_simulator/_utils.py
+-rw-rw-r--  2.0 unx    11647 b- defN 23-Jul-04 16:12 benchmark_simulator/_simulator/_worker.py
+-rw-rw-r--  2.0 unx     3223 b- defN 23-Jul-04 10:43 benchmark_simulator/_simulator/_worker_manager.py
+-rw-rw-r--  2.0 unx     8290 b- defN 23-Jul-04 16:13 benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      307 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       51 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1401 b- defN 23-Jul-05 11:48 mfhpo_simulator-1.2.3.dist-info/RECORD
+15 files, 88386 bytes uncompressed, 24899 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: benchmark_simulator/_simulator/_worker_manager.py
 Comment: 
 
 Filename: benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py
 Comment: 
 
-Filename: mfhpo_simulator-1.2.2.dist-info/LICENSE
+Filename: mfhpo_simulator-1.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: mfhpo_simulator-1.2.2.dist-info/METADATA
+Filename: mfhpo_simulator-1.2.3.dist-info/METADATA
 Comment: 
 
-Filename: mfhpo_simulator-1.2.2.dist-info/WHEEL
+Filename: mfhpo_simulator-1.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: mfhpo_simulator-1.2.2.dist-info/top_level.txt
+Filename: mfhpo_simulator-1.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: mfhpo_simulator-1.2.2.dist-info/RECORD
+Filename: mfhpo_simulator-1.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## benchmark_simulator/__init__.py

```diff
@@ -1,12 +1,12 @@
 from benchmark_simulator._constants import AbstractAskTellOptimizer, ObjectiveFuncType
 from benchmark_simulator.simulator import ObjectiveFuncWrapper, get_multiple_wrappers
 
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/mfhpo-simulator"
```

## benchmark_simulator/_constants.py

```diff
@@ -31,32 +31,36 @@
 class _InfoPaths:
     proc_alloc: str
     result: str
     state_cache: str
     worker_cumtime: str
     timestamp: str
     timenow: str
+    config_tracker: str
 
 
 @dataclass(frozen=True)
 class _ResultData:
     cumtime: float
     eval_config: dict[str, Any]
     results: dict[str, float]
     fidels: dict[str, int | float]
     seed: int | None
+    prev_fidel: int | None
+    config_id: int | None
 
 
 class _SharedDataFileNames(Enum):
     proc_alloc: str = "proc_alloc.json"
     result: str = "results.json"
     state_cache: str = "state_cache.json"
     worker_cumtime: str = "simulated_cumtime.json"
     timestamp: str = "timestamp.json"
     timenow: str = "timenow.json"
+    config_tracker: str = "config_tracker.json"
 
 
 @dataclass(frozen=True)
 class _TimeValue:
     terminated: float = float(1 << 40)
     crashed: float = float(1 << 41)
 
@@ -72,14 +76,16 @@
     runtime_key: str
     fidel_keys: list[str] | None
     seed: int | None
     continual_max_fidel: int | None
     max_waiting_time: float
     check_interval_time: float
     store_config: bool
+    allow_parallel_sampling: bool
+    config_tracking: bool
 
     def validate(self) -> None:
         if self.n_actual_evals_in_opt < self.n_workers + self.n_evals:
             threshold = self.n_workers + self.n_evals
             # In fact, n_workers + n_evals - 1 is the real minimum threshold.
             raise ValueError(
                 "Cannot guarantee that optimziers will not hang. "
@@ -100,15 +106,15 @@
 
 
 _TIME_VALUES = _TimeValue()
 
 
 class AbstractAskTellOptimizer(metaclass=ABCMeta):
     @abstractmethod
-    def ask(self) -> tuple[dict[str, Any], dict[str, int | float] | None]:
+    def ask(self) -> tuple[dict[str, Any], dict[str, int | float] | None, int | None]:
         """
         The ask method to sample a configuration using an optimizer.
 
         Args:
             None
 
         Returns:
@@ -117,35 +123,51 @@
                     The configuration to evaluate.
                     The key is the hyperparameter name and its value is the corresponding hyperparameter value.
                     For example, when returning {"alpha": 0.1, "beta": 0.3}, the objective function evaluates
                     the hyperparameter configuration with alpha=0.1 and beta=0.3.
                 * fidels (dict[str, int | float] | None):
                     The fidelity parameters to be used for the evaluation of the objective function.
                     If not multi-fidelity optimization, simply return None.
+                * config_id (int | None):
+                    The identifier of configuration if needed for continual learning.
+                    Not used at all when continual_max_fidel=None.
+                    As we internally use a hash of eval_config, it may be unstable if eval_config has float.
+                    However, even if config_id is not provided, our simulator works without errors
+                    although we cannot guarantee that our simulator recognizes the same configs if a users' optimizer
+                    slightly changes the content of eval_config.
         """
         raise NotImplementedError
 
     @abstractmethod
     def tell(
         self,
         eval_config: dict[str, Any],
         results: dict[str, float],
         *,
-        fidels: dict[str, int | float] | None,
+        fidels: dict[str, int | float] | None = None,
+        config_id: int | None = None,
     ) -> None:
         """
         The tell method to register for a tuple of configuration, fidelity, and the results to an optimizer.
 
         Args:
             eval_config (dict[str, Any]):
-                The evaluated configuration.
+                The configuration to be used in the objective function.
             results (dict[str, float]):
                 The dict of the return values from the objective function.
-            fidels (dict[str, int | float] | None):
-                The fidelity parameters used in the evaluation.
+            fidels (dict[str, Union[float, int] | None):
+                The fidelities to be used in the objective function. Typically training epoch in deep learning.
+                If None, we assume that no fidelity is used.
+            config_id (int | None):
+                The identifier of configuration if needed for continual learning.
+                Not used at all when continual_max_fidel=None.
+                As we internally use a hash of eval_config, it may be unstable if eval_config has float.
+                However, even if config_id is not provided, our simulator works without errors
+                although we cannot guarantee that our simulator recognizes the same configs if a users' optimizer
+                slightly changes the content of eval_config.
 
         Returns:
             None
         """
         raise NotImplementedError
 
 
@@ -159,18 +181,18 @@
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         """The prototype of the objective function.
 
         Args:
             eval_config (dict[str, Any]):
                 The configuration to be used in the objective function.
-            fidels (Optional[dict[str, Union[float, int]]):
+            fidels (dict[str, Union[float, int] | None):
                 The fidelities to be used in the objective function. Typically training epoch in deep learning.
                 If None, we assume that no fidelity is used.
-            seed (Optional[int]):
+            seed (int | None):
                 The random seed to be used in the objective function.
             **data_to_scatter (Any):
                 Data to scatter across workers.
                 For example, when the objective function instance has a large file,
                 Dask, which is a typical module for parallel optimization, must serialize/deserialize
                 the objective function instances. It causes a significant bottleneck.
                 By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
```

## benchmark_simulator/_secure_proc.py

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import fcntl
 import os
 import time
 import warnings
+from typing import Any
 
 from benchmark_simulator._constants import (
     _SharedDataFileNames,
     _StateType,
     _TIME_VALUES,
     _TimeNowDictType,
 )
@@ -78,14 +79,22 @@
     with lock.edit(path) as f:
         record = json.load(f)
         record[worker_id] = prev_timestamp
         f.seek(0)
         json.dump(record, f, indent=4)
 
 
+def _record_existing_configs(path: str, config_id_str: str, config: dict[str, Any], lock: _SecureLock) -> None:
+    with lock.edit(path) as f:
+        existing_configs = json.load(f)
+        existing_configs[config_id_str] = config
+        f.seek(0)
+        json.dump(existing_configs, f, indent=4)
+
+
 def _cache_state(
     path: str, config_hash: int, new_state: _StateType, lock: _SecureLock, update_index: int | None = None
 ) -> None:
     with lock.edit(path) as f:
         config_hash_str = str(config_hash)
         cache = json.load(f)
         _new_state = [new_state.runtime, new_state.cumtime, new_state.fidel, new_state.seed]
@@ -136,14 +145,21 @@
 def _fetch_timestamps(path: str, lock: _SecureLock) -> dict[str, float]:
     with lock.read(path) as f:
         timestamps = json.load(f)
 
     return timestamps
 
 
+def _fetch_existing_configs(path: str, lock: _SecureLock) -> dict[str, dict[str, Any]]:
+    with lock.read(path) as f:
+        existing_configs = json.load(f)
+
+    return existing_configs
+
+
 def _fetch_proc_alloc(path: str, lock: _SecureLock) -> dict[int, int]:
     return _complete_proc_allocation(path=path, lock=lock)
 
 
 def _record_result(path: str, results: dict[str, float], lock: _SecureLock, fixed: bool = True) -> None:
     with lock.edit(path) as f:
         record = json.load(f)
```

## benchmark_simulator/simulator.py

```diff
@@ -96,14 +96,16 @@
     obj_keys: list[str] | None = None,
     runtime_key: str = "runtime",
     seed: int | None = None,
     continual_max_fidel: int | None = None,
     max_waiting_time: float = np.inf,
     check_interval_time: float = 1e-4,
     store_config: bool = False,
+    allow_parallel_sampling: bool = False,
+    config_tracking: bool = True,
 ) -> list[ObjectiveFuncWrapper]:
     """Return multiple wrapper instances.
 
     Args:
         obj_func (ObjectiveFuncType):
             A callable object that serves as the objective function.
             Args:
@@ -156,21 +158,29 @@
         max_waiting_time (float):
             The maximum waiting time to judge hang.
             If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
         store_config (bool):
             Whether to store all config/fidel information.
             The information is sorted chronologically.
             When you do large-scale experiments, this may incur too much storage consumption.
+        allow_parallel_sampling (bool):
+            Whether sampling can happen in parallel.
+            In many cases, sampler will not be run in parallel and then allow_parallel_sampling should be False.
+            The default value is False.
+        config_tracking (bool):
+            Whether to validate config_id provided from the user side.
+            It slows the simulation down when n_evals is large (> 3000),
+            but it is recommended to avoid unexpected bugs that could happen.
 
     Returns:
         wrappers (list[ObjectiveFuncWrapper]):
             A list of wrappers.
             It contains n_workers of worker wrappers.
     """
-    curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S")
+    curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S.%f")
     save_dir_name = save_dir_name if save_dir_name is not None else f"data-{curtime}"
 
     dir_name = os.path.join(DIR_NAME, save_dir_name)
     if os.path.exists(dir_name):
         raise FileExistsError(f"The directory `{dir_name}` already exists. Remove it first.")
 
     wrapper_kwargs = dict(
@@ -184,26 +194,65 @@
         obj_keys=obj_keys,
         runtime_key=runtime_key,
         seed=seed,
         continual_max_fidel=continual_max_fidel,
         max_waiting_time=max_waiting_time,
         check_interval_time=check_interval_time,
         store_config=store_config,
+        allow_parallel_sampling=allow_parallel_sampling,
+        config_tracking=config_tracking,
     )
     pool = Pool()
     results = []
     for _ in range(n_workers):
         results.append(pool.apply_async(ObjectiveFuncWrapper, kwds=wrapper_kwargs))
 
     pool.close()
     pool.join()
     return [result.get() for result in results]
 
 
 class ObjectiveFuncWrapper:
+    """Objective function wrapper API for users.
+
+    Please check more details at https://github.com/nabenabe0928/mfhpo-simulator/
+
+    Attributes:
+        dir_name (str):
+            The relative path where results will be stored.
+            In principle, it returns `./mfhpo-simulator/<save_dir_name>`.
+        obj_keys (list[str]):
+            The objective names that will be collected in results.
+            The returned dict from users' objective functions must contain these keys.
+            If you want to include the runtime in the results, you also need to include the runtime_key in obj_keys.
+        runtime_key (str):
+            The runtime name that will be used to define the runtime which the user objective function really took.
+            The returned dict from users' objective functions must contain this key.
+        fidel_keys (list[str]):
+            The fidelity names that will be used in users' objective functions.
+            `fidels` passed to the objective functions must contain these keys.
+            When `continual_max_fidel=True`, fidel_keys can contain only one key and this fidelity will be used for
+            the definition of continual learning.
+        n_actual_evals_in_opt (int):
+            The number of configuration evaluations during the actual optimization.
+            Note that even if some configurations are continuations from an existing config with lower fidelity,
+            they are counted as separated config evaluations.
+        n_workers (int):
+            The number of workers used in the user-defined optimizer.
+
+    Methods:
+        __call__(...) -> dict[str, float]:
+            The wrapped objective function used in the user-defined optimizer. Valid only if `ask_and_tell=False`.
+            Please check `ObjectiveFuncWrapper.__call__.__doc__` for more details.
+        simulate(opt: AbstractAskTellOptimizer) -> None:
+            The optimization loop for the wrapped objective function and the user-defined optimizer.
+            Valid only if `ask_and_tell=True`.
+            Please check `ObjectiveFuncWrapper.simulate.__doc__` for more details.
+    """
+
     def __init__(
         self,
         obj_func: ObjectiveFuncType,
         launch_multiple_wrappers_from_user_side: bool = False,
         ask_and_tell: bool = False,
         save_dir_name: str | None = None,
         n_workers: int = 4,
@@ -213,14 +262,16 @@
         obj_keys: list[str] | None = None,
         runtime_key: str = "runtime",
         seed: int | None = None,
         continual_max_fidel: int | None = None,
         max_waiting_time: float = np.inf,
         check_interval_time: float = 1e-4,
         store_config: bool = False,
+        allow_parallel_sampling: bool = False,
+        config_tracking: bool = True,
     ):
         """The initialization of a wrapper class.
 
         Both ObjectiveFuncWorker and CentralWorkerManager have the same interface and the same set of control params.
 
         Args:
             obj_func (ObjectiveFuncType):
@@ -287,30 +338,40 @@
             max_waiting_time (float):
                 The maximum waiting time to judge hang.
                 If any one of the workers does not do any updates for this amount of time, we raise TimeoutError.
             store_config (bool):
                 Whether to store all config/fidel information.
                 The information is sorted chronologically.
                 When you do large-scale experiments, this may incur too much storage consumption.
+            allow_parallel_sampling (bool):
+                Whether sampling can happen in parallel.
+                In many cases, sampler will not be run in parallel and then allow_parallel_sampling should be False.
+                The default value is False.
+            config_tracking (bool):
+                Whether to validate config_id provided from the user side.
+                It slows the simulation down when n_evals is large (> 3000),
+                but it is recommended to avoid unexpected bugs that could happen.
         """
-        curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S")
+        curtime = datetime.now().strftime("%Y-%m-%d-%H:%M:%S.%f")
         wrapper_vars = _WrapperVars(
             obj_func=obj_func,
             save_dir_name=save_dir_name if save_dir_name is not None else f"data-{curtime}",
             n_workers=n_workers,
             n_actual_evals_in_opt=n_actual_evals_in_opt,
             n_evals=n_evals,
             fidel_keys=fidel_keys,
             obj_keys=obj_keys if obj_keys is not None else ["loss"],
             runtime_key=runtime_key,
             seed=seed,
             continual_max_fidel=continual_max_fidel,
             max_waiting_time=max_waiting_time,
             check_interval_time=check_interval_time,
             store_config=store_config,
+            allow_parallel_sampling=allow_parallel_sampling,
+            config_tracking=config_tracking,
         )
 
         self._main_wrapper: _AskTellWorkerManager | _CentralWorkerManager | _ObjectiveFuncWorker
         self._validate(
             save_dir_name=save_dir_name,
             ask_and_tell=ask_and_tell,
             launch_multiple_wrappers_from_user_side=launch_multiple_wrappers_from_user_side,
@@ -363,42 +424,53 @@
             )
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
+        config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         """The meta-wrapper method of the objective function method in WorkerFunc instances.
 
         This method recognizes each WorkerFunc by process ID and call the corresponding worker based on the ID.
 
         Args:
             eval_config (dict[str, Any]):
-                The configuration to be used in the objective function.
+                The configuration to be used in the user-defined objective function.
+                This configuration will not be necessary for the processing in our API, but the storage purpose.
+                However, it will be directly passed to the user-defined objective function, hence we need it.
             fidels (dict[str, int | float] | None):
                 The fidelities to be used in the objective function. Typically training epoch in deep learning.
                 If None, no-fidelity opt.
+            config_id (int | None):
+                The identifier of configuration if needed for continual learning.
+                As we internally use a hash of eval_config, it may be unstable if eval_config has float.
+                However, even if config_id is not provided, our simulator works without errors
+                although we cannot guarantee that our simulator recognizes the same configs if a users' optimizer
+                slightly changes the content of eval_config.
             **data_to_scatter (Any):
                 Data to scatter across workers.
+                Users can pass any necessary information to the objective function,
+                but this variable will NOT be used by our API at all.
                 For example, when the objective function instance has a large file,
                 Dask, which is a typical module for parallel optimization, must serialize/deserialize
                 the objective function instances. It causes a significant bottleneck.
                 By using dask.scatter, we can avoid this problem and this kwargs serves for this purpose.
                 Note that since the handling of parallel workers vary depending on packages,
                 users must adapt by themselves.
 
         Returns:
             results (dict[str, float]):
                 The results of the objective function given the inputs.
                 It must have `objective metric` and `runtime` at least.
                 Otherwise, any other metrics are optional.
         """
-        return self._main_wrapper(eval_config=eval_config, fidels=fidels, **data_to_scatter)
+        return self._main_wrapper(eval_config=eval_config, fidels=fidels, config_id=config_id, **data_to_scatter)
 
     def simulate(self, opt: AbstractAskTellOptimizer) -> None:
         """
         Start the simulation using only the main process.
         Unlike the other worker wrappers, each objective function will not run in parallel.
         Instead, we internally simulate the cumulative runtime for each worker.
         For this sake, the optimizer must take so-called ask-and-tell interface.
```

## benchmark_simulator/_simulator/_base_wrapper.py

```diff
@@ -54,14 +54,15 @@
         raise NotImplementedError
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
+        config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         raise NotImplementedError(
             f"{self.__class__.__name__} is an optimizer wrapper, but not a function wrapper.\n"
             "It is not supposed to be called. If you want to use a function wrapper set `ask_and_tell = False`."
         )
```

## benchmark_simulator/_simulator/_worker.py

```diff
@@ -2,23 +2,19 @@
 
 import os
 import time
 from typing import Any
 
 from benchmark_simulator._constants import (
     INF,
-    _StateType,
     _TIME_VALUES,
     _TimeNowDictType,
     _WorkerVars,
 )
 from benchmark_simulator._secure_proc import (
-    _cache_state,
-    _delete_state,
-    _fetch_cache_states,
     _fetch_cumtimes,
     _fetch_timenow,
     _fetch_timestamps,
     _finish_worker_timer,
     _init_simulator,
     _is_simulator_terminated,
     _record_cumtime,
@@ -33,14 +29,16 @@
 from benchmark_simulator._simulator._base_wrapper import _BaseWrapperInterface
 from benchmark_simulator._simulator._utils import (
     _validate_fidel_args,
     _validate_fidels,
     _validate_fidels_continual,
     _validate_output,
 )
+from benchmark_simulator._trackers._config_tracker import _ConfigIDTracker
+from benchmark_simulator._trackers._state_tracker import _StateTracker
 from benchmark_simulator._utils import _generate_time_hash
 
 import numpy as np
 
 
 class _ObjectiveFuncWorker(_BaseWrapperInterface):
     """A worker class for each worker.
@@ -52,14 +50,18 @@
     """
 
     def __repr__(self) -> str:
         return f"Worker-{self._worker_vars.worker_id}"
 
     def _init_worker(self, worker_id: str) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
+        self._state_tracker = _StateTracker(
+            path=self._paths.state_cache, lock=self._lock, continual_max_fidel=self._wrapper_vars.continual_max_fidel
+        )
+        self._config_tracker = _ConfigIDTracker(path=self._paths.config_tracker, lock=self._lock)
         _init_simulator(dir_name=self.dir_name)
         _start_worker_timer(path=self._paths.worker_cumtime, worker_id=worker_id, lock=self._lock)
 
     def _alloc_index(self, worker_id: str) -> int:
         worker_id_to_index = _wait_all_workers(
             path=self._paths.worker_cumtime, n_workers=self._wrapper_vars.n_workers, lock=self._lock
         )
@@ -91,40 +93,14 @@
     def _validate(self) -> None:
         if self._crashed:
             raise InterruptedError(
                 "The simulation is interrupted due to deadlock or the dead of at least one of the workers.\n"
                 "This error could be avoided by increasing `max_waiting_time` (however, np.inf is discouraged).\n"
             )
 
-    def _get_cached_state_and_index(self, config_hash: int, fidel: int) -> tuple[_StateType, int | None]:
-        cached_states = _fetch_cache_states(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
-        intermediate_avail = [state.cumtime <= self._cumtime and state.fidel < fidel for state in cached_states]
-        cached_state_index = intermediate_avail.index(True) if any(intermediate_avail) else None
-        if cached_state_index is None:
-            # initial seed, note: 1 << 30 is a huge number that fits 32bit.
-            init_state = _StateType(seed=self._worker_vars.rng.randint(1 << 30))
-            return init_state, None
-        else:
-            return cached_states[cached_state_index], cached_state_index
-
-    def _update_state(
-        self,
-        config_hash: int,
-        fidel: int,
-        total_runtime: float,
-        seed: int | None,
-        cached_state_index: int | None,
-    ) -> None:
-        kwargs = dict(path=self._paths.state_cache, config_hash=config_hash, lock=self._lock)
-        if fidel != self._wrapper_vars.continual_max_fidel:  # update the cache data
-            new_state = _StateType(runtime=total_runtime, cumtime=self._cumtime, fidel=fidel, seed=seed)
-            _cache_state(new_state=new_state, update_index=cached_state_index, **kwargs)  # type: ignore[arg-type]
-        elif cached_state_index is not None:  # if None, newly start and train till the end, so no need to delete.
-            _delete_state(index=cached_state_index, **kwargs)  # type: ignore[arg-type]
-
     def _wait_other_workers(self) -> None:
         """
         Wait until the worker's cumulative runtime becomes the smallest.
         The smallest cumulative runtime implies that the order in the record will not disturbed
         even if the worker reports its results now.
         """
         _wait_until_next(
@@ -142,62 +118,80 @@
         )
 
     def _query_obj_func(
         self,
         eval_config: dict[str, Any],
         fidels: dict[str, int | float] | None,
         seed: int | None,
+        prev_fidel: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         if self._wrapper_vars.store_config:
             self._used_config = eval_config.copy()
-            self._used_config.update(**(fidels if fidels is not None else {}), seed=seed)
+            self._used_config.update(
+                **(fidels if fidels is not None else {}),
+                **({"prev_fidel": prev_fidel} if prev_fidel is not None else {}),
+                seed=seed,
+            )
 
         return self._wrapper_vars.obj_func(eval_config=eval_config, fidels=fidels, seed=seed, **data_to_scatter)
 
     def _proc_output_from_scratch(
         self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
     ) -> dict[str, float]:
         seed = self._worker_vars.rng.randint(1 << 30)
         results = self._query_obj_func(eval_config=eval_config, seed=seed, fidels=fidels, **data_to_scatter)
         _validate_output(results, stored_obj_keys=self._worker_vars.stored_obj_keys)
         self._cumtime += results[self.runtime_key]
         return {k: results[k] for k in self._worker_vars.stored_obj_keys}
 
     def _proc_output_from_existing_state(
-        self, eval_config: dict[str, Any], fidel: int, **data_to_scatter: Any
+        self, eval_config: dict[str, Any], fidel: int, config_id: int | None, **data_to_scatter: Any
     ) -> dict[str, float]:
-        config_hash: int = hash(str(eval_config))
-        cached_state, cached_state_index = self._get_cached_state_and_index(config_hash=config_hash, fidel=fidel)
+        config_hash: int = hash(str(eval_config)) if config_id is None else int(config_id)
+        cached_state, cached_state_index = self._state_tracker.get_cached_state_and_index(
+            config_hash=config_hash, fidel=fidel, cumtime=self._cumtime, rng=self._worker_vars.rng
+        )
         _fidels: dict[str, int | float] = {self._fidel_keys[0]: fidel}
         results = self._query_obj_func(
-            eval_config=eval_config, seed=cached_state.seed, fidels=_fidels, **data_to_scatter
+            eval_config=eval_config,
+            seed=cached_state.seed,
+            fidels=_fidels,
+            prev_fidel=cached_state.fidel,
+            **data_to_scatter,
         )
         _validate_output(results, stored_obj_keys=self._worker_vars.stored_obj_keys)
         total_runtime = results[self.runtime_key]
         actual_runtime = max(0.0, total_runtime - cached_state.runtime)
         self._cumtime += actual_runtime
-        self._update_state(
+        self._state_tracker.update_state(
+            cumtime=self._cumtime,
             total_runtime=total_runtime,
             cached_state_index=cached_state_index,
             seed=cached_state.seed,
             config_hash=config_hash,
             fidel=fidel,
         )
         return {**{k: results[k] for k in self._obj_keys}, self.runtime_key: actual_runtime}
 
     def _proc_output(
-        self, eval_config: dict[str, Any], fidels: dict[str, int | float] | None, **data_to_scatter: Any
+        self,
+        eval_config: dict[str, Any],
+        fidels: dict[str, int | float] | None,
+        config_id: int | None,
+        **data_to_scatter: Any,
     ) -> dict[str, float]:
         if not self._worker_vars.continual_eval:
             return self._proc_output_from_scratch(eval_config=eval_config, fidels=fidels, **data_to_scatter)
 
         # Otherwise, we try the continual evaluation
         fidel = _validate_fidels_continual(fidels)
-        return self._proc_output_from_existing_state(eval_config=eval_config, fidel=fidel, **data_to_scatter)
+        return self._proc_output_from_existing_state(
+            eval_config=eval_config, fidel=fidel, config_id=config_id, **data_to_scatter
+        )
 
     def _post_proc(self, results: dict[str, float]) -> None:
         # First, record the simulated cumulative runtime after calling the objective
         _record_cumtime(
             path=self._paths.worker_cumtime,
             worker_id=self._worker_vars.worker_id,
             cumtime=self._cumtime,
@@ -232,43 +226,53 @@
                 lock=self._lock,
             )
             return timestamp
 
         timenow_data = _fetch_timenow(path=self._paths.timenow, lock=self._lock)
         cumtime = _fetch_cumtimes(self._paths.worker_cumtime, lock=self._lock)[worker_id]
         # Consider the sampling time overlap
-        self._cumtime = max(cumtime, np.max(timenow_data["after_sample"][timenow_data["before_sample"] <= cumtime]))
+        self._cumtime = (
+            max(cumtime, np.max(timenow_data["after_sample"][timenow_data["before_sample"] <= cumtime]))
+            if not self._wrapper_vars.allow_parallel_sampling
+            else cumtime
+        )
         self._terminated = self._cumtime >= _TIME_VALUES.terminated - 1e-5
         self._crashed = self._cumtime >= _TIME_VALUES.crashed - 1e-5
         return timestamp_dict[worker_id]
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
+        config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         prev_timestamp = self._load_timestamps()
         self._validate()
         _validate_fidels(
             fidels=fidels,
             fidel_keys=self._fidel_keys,
             use_fidel=self._worker_vars.use_fidel,
             continual_eval=self._worker_vars.continual_eval,
         )
+        config_tracking = config_id is not None and self._wrapper_vars.config_tracking
+        if config_tracking:  # validate the config_id to ensure the user implementation is correct
+            assert config_id is not None  # mypy redefinition
+            self._config_tracker.validate(config=eval_config, config_id=config_id)
+
         if self._terminated:
             return {**{k: INF for k in self._obj_keys}, self.runtime_key: INF}
 
         sampling_time = max(0.0, time.time() - prev_timestamp)
         timenow_data = _TimeNowDictType(before_sample=self._cumtime, after_sample=self._cumtime + sampling_time)
         _record_timenow(path=self._paths.timenow, timenow_data=timenow_data, lock=self._lock)
 
         self._cumtime += sampling_time
-        results = self._proc_output(eval_config, fidels, **data_to_scatter)
+        results = self._proc_output(eval_config=eval_config, fidels=fidels, config_id=config_id, **data_to_scatter)
         self._post_proc(results)
         return results
 
     def _finish(self) -> None:
         """The method to close the worker instance.
         This method must be called before we finish the optimization.
         If not called, optimization modules are likely to hang.
```

## benchmark_simulator/_simulator/_worker_manager.py

```diff
@@ -56,14 +56,15 @@
             self._pid_to_index = _fetch_proc_alloc(path=path, lock=self._lock)
 
     def __call__(
         self,
         eval_config: dict[str, Any],
         *,
         fidels: dict[str, int | float] | None = None,
+        config_id: int | None = None,
         **data_to_scatter: Any,
     ) -> dict[str, float]:
         pid = os.getpid()
         pid = threading.get_ident() if pid == self._main_pid else pid
         if len(self._pid_to_index) != self._wrapper_vars.n_workers:
             self._init_alloc(pid)
 
@@ -72,9 +73,11 @@
                 f"An unknown process/thread with ID {pid} was specified.\n"
                 "It is likely that one of the workers crashed and a new worker was added or \n"
                 f"n_workers in ObjectiveFuncWrapper and your optimizer were incompatible.\n"
                 f"However, worker additions are not allowed in ObjectiveFuncWrapper."
             )
 
         worker_index = self._pid_to_index[pid]
-        results = self._workers[worker_index](eval_config=eval_config, fidels=fidels, **data_to_scatter)
+        results = self._workers[worker_index](
+            eval_config=eval_config, fidels=fidels, config_id=config_id, **data_to_scatter
+        )
         return results
```

## benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py

```diff
@@ -1,146 +1,137 @@
 from __future__ import annotations
 
-import json
 import os
 import time
 from typing import Any
 
 from benchmark_simulator._constants import AbstractAskTellOptimizer, _ResultData, _StateType, _WorkerVars
 from benchmark_simulator._simulator._base_wrapper import _BaseWrapperInterface
 from benchmark_simulator._simulator._utils import (
     _validate_fidel_args,
     _validate_fidels,
     _validate_fidels_continual,
     _validate_opt_class,
     _validate_output,
 )
+from benchmark_simulator._trackers._config_tracker import _AskTellConfigIDTracker
+from benchmark_simulator._trackers._state_tracker import _AskTellStateTracker
 
 import numpy as np
 
+import ujson as json  # type: ignore
+
 
 class _AskTellWorkerManager(_BaseWrapperInterface):
     def _init_wrapper(self) -> None:
         os.makedirs(self.dir_name, exist_ok=True)
         self._worker_vars = _WorkerVars(
             continual_eval=self._wrapper_vars.continual_max_fidel is not None,
             use_fidel=self._wrapper_vars.fidel_keys is not None,
             rng=np.random.RandomState(self._wrapper_vars.seed),
             stored_obj_keys=list(set(self.obj_keys + [self.runtime_key])),
             worker_id="",
             worker_index=-1,
         )
+        self._config_tracker = _AskTellConfigIDTracker()
+        self._state_tracker = _AskTellStateTracker(continual_max_fidel=self._wrapper_vars.continual_max_fidel)
 
         self._wrapper_vars.validate()
         _validate_fidel_args(continual_eval=self._worker_vars.continual_eval, fidel_keys=self._fidel_keys)
 
         self._timenow = 0.0
         self._cumtimes: np.ndarray = np.zeros(self._wrapper_vars.n_workers, dtype=np.float64)
-        self._intermediate_states: dict[int, list[_StateType]] = {}
         self._pending_results: list[_ResultData | None] = [None] * self._wrapper_vars.n_workers
         self._seen_config_keys: list[str] = []
         self._results: dict[str, list[Any]] = {"worker_index": [], "cumtime": []}
         self._results.update({k: [] for k in self._obj_keys})
         if self._wrapper_vars.store_config:
             self._results.update({k: [] for k in self._fidel_keys + ["seed"]})
-
-    def _fetch_prev_state_index(self, config_hash: int, fidel: int, worker_id: int) -> int | None:
-        states = self._intermediate_states.get(config_hash, [])
-        intermediate_avail = [state.cumtime <= self._cumtimes[worker_id] and state.fidel < fidel for state in states]
-        return intermediate_avail.index(True) if any(intermediate_avail) else None
-
-    def _fetch_prev_seed(self, config_hash: int, fidel: int, worker_id: int) -> int | None:
-        prev_state_index = self._fetch_prev_state_index(config_hash=config_hash, fidel=fidel, worker_id=worker_id)
-        if prev_state_index is None:
-            return self._worker_vars.rng.randint(1 << 30)
-        else:
-            return self._intermediate_states[config_hash][prev_state_index].seed
-
-    def _pop_old_state(self, config_hash: int, fidel: int, worker_id: int) -> _StateType | None:
-        prev_state_index = self._fetch_prev_state_index(config_hash=config_hash, fidel=fidel, worker_id=worker_id)
-        if prev_state_index is None:
-            return None
-
-        old_state = self._intermediate_states[config_hash].pop(prev_state_index)
-        if len(self._intermediate_states[config_hash]) == 0:
-            # Remove the empty set
-            self._intermediate_states.pop(config_hash)
-
-        return old_state
+            if self._wrapper_vars.continual_max_fidel is not None:
+                self._results["prev_fidel"] = []
 
     def _proc(
         self,
         eval_config: dict[str, Any],
         worker_id: int,
         fidels: dict[str, int | float] | None,
-    ) -> tuple[dict[str, float], int | None]:
-        continual_max_fidel = self._wrapper_vars.continual_max_fidel
+        config_id: int | None,
+    ) -> tuple[dict[str, float], int | None, int | None]:
         if not self._worker_vars.continual_eval:  # not continual learning
             seed = self._worker_vars.rng.randint(1 << 30)
             results = self._wrapper_vars.obj_func(eval_config=eval_config, fidels=fidels, seed=seed)
             _validate_output(results, stored_obj_keys=self._worker_vars.stored_obj_keys)
-            return results, seed
+            return results, seed, None
 
         fidel = _validate_fidels_continual(fidels)
         runtime_key = self._wrapper_vars.runtime_key
-        config_hash = int(hash(str(eval_config)))
-        seed = self._fetch_prev_seed(config_hash=config_hash, fidel=fidel, worker_id=worker_id)
+        config_hash = int(hash(str(eval_config))) if config_id is None else config_id
+        seed = self._state_tracker.fetch_prev_seed(
+            config_hash=config_hash,
+            fidel=fidel,
+            cumtime=self._cumtimes[worker_id],
+            rng=self._worker_vars.rng,
+        )
         results = self._wrapper_vars.obj_func(eval_config=eval_config, fidels=fidels, seed=seed)
         _validate_output(results, stored_obj_keys=self._worker_vars.stored_obj_keys)
-        old_state = self._pop_old_state(config_hash=config_hash, fidel=fidel, worker_id=worker_id)
+        old_state = self._state_tracker.pop_old_state(
+            config_hash=config_hash, fidel=fidel, cumtime=self._cumtimes[worker_id]
+        )
         old_state = _StateType(seed=seed) if old_state is None else old_state
 
         results[runtime_key] = max(0.0, results[runtime_key] - old_state.runtime)
-        assert continual_max_fidel is not None  # mypy redefinition
-        if fidel < continual_max_fidel:
-            new_state = _StateType(
-                runtime=results[runtime_key],
-                cumtime=self._cumtimes[worker_id],
-                fidel=fidel,
-                seed=old_state.seed,
-            )
-            if config_hash in self._intermediate_states:
-                self._intermediate_states[config_hash].append(new_state)
-            else:
-                self._intermediate_states[config_hash] = [new_state]
+        self._state_tracker.update_state(
+            config_hash=config_hash,
+            fidel=fidel,
+            runtime=results[runtime_key],
+            cumtime=self._cumtimes[worker_id],
+            seed=old_state.seed,
+        )
 
-        return results, seed
+        return results, seed, old_state.fidel
 
     def _proc_obj_func(
         self,
         eval_config: dict[str, Any],
         worker_id: int,
         fidels: dict[str, int | float] | None,
+        config_id: int | None,
     ) -> None:
         _validate_fidels(
             fidels=fidels,
             fidel_keys=self._fidel_keys,
             use_fidel=self._worker_vars.use_fidel,
             continual_eval=self._worker_vars.continual_eval,
         )
-        results, seed = self._proc(eval_config=eval_config, worker_id=worker_id, fidels=fidels)
+        results, seed, prev_fidel = self._proc(
+            eval_config=eval_config, worker_id=worker_id, fidels=fidels, config_id=config_id
+        )
         runtime_key = self._wrapper_vars.runtime_key
         self._cumtimes[worker_id] += results[runtime_key]
         self._pending_results[worker_id] = _ResultData(
             cumtime=self._cumtimes[worker_id],
             eval_config=eval_config,
             results=results,
             fidels=fidels if fidels is not None else {},
             seed=seed,
+            config_id=config_id,
+            prev_fidel=prev_fidel,
         )
 
     def _record_result_data(self, result_data: _ResultData, worker_id: int) -> None:
         prev_size = len(self._results["cumtime"])
         self._results["worker_index"].append(worker_id)
         self._results["cumtime"].append(result_data.cumtime)
         for k in self._obj_keys:
             self._results[k].append(result_data.results[k])
 
         if not self._wrapper_vars.store_config:
             return
+        if result_data.prev_fidel is not None:
+            self._results["prev_fidel"].append(result_data.prev_fidel)
 
         self._results["seed"].append(result_data.seed)
         for k in self._fidel_keys:
             self._results[k].append(result_data.fidels[k])
 
         eval_config = result_data.eval_config
         unseen_keys = [k for k in eval_config.keys() if k not in self._seen_config_keys]
@@ -152,38 +143,52 @@
             else:
                 self._results[k].append(val)
 
     def _ask_with_timer(
         self,
         opt: AbstractAskTellOptimizer,
         worker_id: int,
-    ) -> tuple[dict[str, Any], dict[str, int | float] | None]:
+    ) -> tuple[dict[str, Any], dict[str, int | float] | None, int | None]:
         start = time.time()
-        eval_config, fidels = opt.ask()
+        eval_config, fidels, config_id = opt.ask()
+        config_tracking = config_id is not None and self._wrapper_vars.config_tracking
+        if config_tracking:  # validate the config_id to ensure the user implementation is correct
+            assert config_id is not None  # mypy redefinition
+            self._config_tracker.validate(config=eval_config, config_id=config_id)
+
         sampling_time = time.time() - start
-        self._timenow = max(self._timenow, self._cumtimes[worker_id]) + sampling_time
-        self._cumtimes[worker_id] = self._timenow
-        return eval_config, fidels
+        if self._wrapper_vars.allow_parallel_sampling:
+            self._cumtimes[worker_id] = self._cumtimes[worker_id] + sampling_time
+        else:
+            self._timenow = max(self._timenow, self._cumtimes[worker_id]) + sampling_time
+            self._cumtimes[worker_id] = self._timenow
+
+        return eval_config, fidels, config_id
 
     def _tell_pending_result(self, opt: AbstractAskTellOptimizer, worker_id: int) -> None:
         result_data = self._pending_results[worker_id]
         if result_data is None:
             return
 
         self._record_result_data(result_data=result_data, worker_id=worker_id)
-        opt.tell(eval_config=result_data.eval_config, results=result_data.results, fidels=result_data.fidels)
+        opt.tell(
+            eval_config=result_data.eval_config,
+            results=result_data.results,
+            fidels=result_data.fidels,
+            config_id=result_data.config_id,
+        )
         self._pending_results[worker_id] = None
 
     def _save_results(self) -> None:
         with open(self._paths.result, mode="w") as f:
             json.dump({k: np.asarray(v).tolist() for k, v in self._results.items()}, f, indent=4)
 
     def simulate(self, opt: AbstractAskTellOptimizer) -> None:
         _validate_opt_class(opt)
         worker_id = 0
         for _ in range(self._wrapper_vars.n_evals + self._wrapper_vars.n_workers - 1):
-            eval_config, fidels = self._ask_with_timer(opt=opt, worker_id=worker_id)
-            self._proc_obj_func(eval_config=eval_config, worker_id=worker_id, fidels=fidels)
+            eval_config, fidels, config_id = self._ask_with_timer(opt=opt, worker_id=worker_id)
+            self._proc_obj_func(eval_config=eval_config, worker_id=worker_id, fidels=fidels, config_id=config_id)
             worker_id = np.argmin(self._cumtimes)
             self._tell_pending_result(opt=opt, worker_id=worker_id)
 
         self._save_results()
```

## Comparing `mfhpo_simulator-1.2.2.dist-info/LICENSE` & `mfhpo_simulator-1.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mfhpo_simulator-1.2.2.dist-info/RECORD` & `mfhpo_simulator-1.2.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-benchmark_simulator/__init__.py,sha256=e65JYj3YptJ3fbqs6Mg8jCw8Uph5ADdX6QLulYMgLTs,560
-benchmark_simulator/_constants.py,sha256=-dEdRbvQsWSaFm7jHlP2z9WCu5_Chh12A61zVzOJvHA,6127
-benchmark_simulator/_secure_proc.py,sha256=ZvJzKY6uwAIxXAlEwY9r271H5ZDSvplAIAreXkIIG20,11227
+benchmark_simulator/__init__.py,sha256=gcjgqYhs2r0tgv5fgrgZo8XUtjfDfS1uZ7nXTDUwabw,560
+benchmark_simulator/_constants.py,sha256=_9Whr7k-DDFxXoPHANgILWWLaYxKnfHobDkd_Ctql7o,7646
+benchmark_simulator/_secure_proc.py,sha256=Go1sN__3lsirYFUGOXm5Kgp0Lvkhc3TGd017bDoZHzI,11741
 benchmark_simulator/_utils.py,sha256=s2kwhhHIJbrT0VbNglmq-rlm0oE8OrqUBvDpCLEAsXk,1772
-benchmark_simulator/simulator.py,sha256=I-0ucvKzkE6U0EZRDevx7ZjaIB6Z9lrll53FTmAXrUA,20853
-benchmark_simulator/_simulator/_base_wrapper.py,sha256=dCvN1elNwyaMTdimCrJwRsVE1s0dhm8SZMizqPu501Y,2544
+benchmark_simulator/simulator.py,sha256=GkVnFY0Zepinp79s6vJOv9I_T9iXH9TVdgT8r7Z3fCk,25336
+benchmark_simulator/_simulator/_base_wrapper.py,sha256=HvK4Iq1vjCuD1HEcphY-hl4Wo_vo1d-N_FA9PFkYukA,2582
 benchmark_simulator/_simulator/_utils.py,sha256=eVQOty1X3ZfXb4Hr8oaRjaOMWYJQHi-YPmCDB91xhO4,2978
-benchmark_simulator/_simulator/_worker.py,sha256=mLzN1d1Z0RUL52bt5kfZyHbCBuE8uJr1uIwNKwYm0Rc,11790
-benchmark_simulator/_simulator/_worker_manager.py,sha256=A2AzmDRoKU5eZm9eVbQ9PKdHDWvnML9YfrhHuV71lQM,3142
-benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py,sha256=JOblB1eO48QqphDRU6YoENEI8KTmlwvOt8GUXNz7l_E,8367
-mfhpo_simulator-1.2.2.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
-mfhpo_simulator-1.2.2.dist-info/METADATA,sha256=TG70MKX8IQZ8Cr4CPq7Uqeb5TKDR9RTfS_2MnFXwfcw,307
-mfhpo_simulator-1.2.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-mfhpo_simulator-1.2.2.dist-info/top_level.txt,sha256=dkUhIqI2xJvV1NOS7bvMDWMNDJ1GGBwTnOBedLuz3OA,51
-mfhpo_simulator-1.2.2.dist-info/RECORD,,
+benchmark_simulator/_simulator/_worker.py,sha256=oE-vEJEgSu9LGNXIGE8Z7S8PCaivIGq9WWKDr8U-K-c,11647
+benchmark_simulator/_simulator/_worker_manager.py,sha256=hQXJR2GLrrKiTgCXoYDEs5bYRO1ASTF87ye37eGfKn8,3223
+benchmark_simulator/_simulator/_worker_manager_for_ask_and_tell.py,sha256=l3SK3Vv5_N4KrsNyTB-yWt3CfY453VFZ3z3iE7nmDN4,8290
+mfhpo_simulator-1.2.3.dist-info/LICENSE,sha256=auQsw_aAlfeXmKRQ_tmNBjUD2-wJojtRJPslgGyGqK4,10760
+mfhpo_simulator-1.2.3.dist-info/METADATA,sha256=W9-5rBtU34rEfmV_vZG60uUw93hGceRTreolOj4-now,307
+mfhpo_simulator-1.2.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+mfhpo_simulator-1.2.3.dist-info/top_level.txt,sha256=dkUhIqI2xJvV1NOS7bvMDWMNDJ1GGBwTnOBedLuz3OA,51
+mfhpo_simulator-1.2.3.dist-info/RECORD,,
```

