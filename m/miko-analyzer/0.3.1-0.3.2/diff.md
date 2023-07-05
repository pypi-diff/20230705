# Comparing `tmp/miko_analyzer-0.3.1.tar.gz` & `tmp/miko_analyzer-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miko_analyzer-0.3.1.tar", max compression
+gzip compressed data, was "miko_analyzer-0.3.2.tar", max compression
```

## Comparing `miko_analyzer-0.3.1.tar` & `miko_analyzer-0.3.2.tar`

### file list

```diff
@@ -1,23 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/LICENSE
--rw-r--r--   0        0        0      841 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/__init__.py
--rw-r--r--   0        0        0       97 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/__main__.py
--rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/cmdline/__init__.py
--rw-r--r--   0        0        0      280 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/cmdline/base.py
--rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/graph/__init__.py
--rw-r--r--   0        0        0     2472 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/graph/plotting.py
--rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/structure/__init__.py
--rw-r--r--   0        0        0     6812 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/structure/cluster.py
--rw-r--r--   0        0        0       62 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/__init__.py
--rw-r--r--   0        0        0       25 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/__init__.py
--rw-r--r--   0        0        0     3127 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/base.py
--rw-r--r--   0        0        0    26841 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/exploration.py
--rw-r--r--   0        0        0     4261 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/labeling.py
--rw-r--r--   0        0        0     2930 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/training.py
--rw-r--r--   0        0        0       54 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/__init__.py
--rw-r--r--   0        0        0       57 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/files.py
--rw-r--r--   0        0        0     1050 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/log_factory.py
--rw-r--r--   0        0        0       45 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/output.py
--rw-r--r--   0        0        0     1130 2023-06-25 10:10:57.927889 miko_analyzer-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 miko_analyzer-0.3.1/setup.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 miko_analyzer-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/LICENSE
+-rw-r--r--   0        0        0      841 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/__init__.py
+-rw-r--r--   0        0        0       97 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/cmdline/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/cmdline/base.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/graph/__init__.py
+-rw-r--r--   0        0        0     2472 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/graph/plotting.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/structure/__init__.py
+-rw-r--r--   0        0        0     6812 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/structure/cluster.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/__init__.py
+-rw-r--r--   0        0        0     1419 2023-07-05 14:11:20.297261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/exploration.py
+-rw-r--r--   0        0        0      537 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/labeling.py
+-rw-r--r--   0        0        0     1733 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/task.py
+-rw-r--r--   0        0        0     1432 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/ai2_kit/training.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/__init__.py
+-rw-r--r--   0        0        0    24683 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/exploration.py
+-rw-r--r--   0        0        0     4445 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/labeling.py
+-rw-r--r--   0        0        0      829 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/task.py
+-rw-r--r--   0        0        0     2787 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/base/training.py
+-rw-r--r--   0        0        0        0 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/__init__.py
+-rw-r--r--   0        0        0    11298 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/exploration.py
+-rw-r--r--   0        0        0      725 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/labeling.py
+-rw-r--r--   0        0        0     3353 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/task.py
+-rw-r--r--   0        0        0     2040 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/tesla/dpgen/training.py
+-rw-r--r--   0        0        0       54 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/__init__.py
+-rw-r--r--   0        0        0       57 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/files.py
+-rw-r--r--   0        0        0      524 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/lammps.py
+-rw-r--r--   0        0        0     1080 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/log_factory.py
+-rw-r--r--   0        0        0       45 2023-07-05 14:11:20.301261 miko_analyzer-0.3.2/miko/utils/output.py
+-rw-r--r--   0        0        0     1174 2023-07-05 14:19:05.164761 miko_analyzer-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 miko_analyzer-0.3.2/setup.py
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 miko_analyzer-0.3.2/PKG-INFO
```

### Comparing `miko_analyzer-0.3.1/LICENSE` & `miko_analyzer-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.1/README.md` & `miko_analyzer-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.1/miko/graph/plotting.py` & `miko_analyzer-0.3.2/miko/graph/plotting.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.1/miko/structure/cluster.py` & `miko_analyzer-0.3.2/miko/structure/cluster.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.1/miko/tesla/dpgen/base.py` & `miko_analyzer-0.3.2/miko/tesla/dpgen/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import json
-from abc import ABC
 from pathlib import Path
+from typing import Optional
 
-class DPTask(object):
+from miko.tesla.base.task import BaseTask, BaseAnalyzer
+
+
+class DPTask(BaseTask):
     """DPTask is a class reading a DP-GEN directory, where the DP-GEN task run.
     """
 
     def __init__(
         self,
         path: str,
         param_file: str = 'param.json',
         machine_file: str = 'machine.json',
-        record_file: str = 'record.dpgen',
-        deepmd_version: str = '2.0'
-    ):
+        record_file: str = 'record.dpgen'
+    ) -> None:
         """Generate a class of tesla task.
 
         Args:
             path (str): The path of the tesla task.
             param_file (str): The param json file name.
             machine_file (str): The machine json file name.
             record_file (str): The record file name.
             deepmd_version (str): DeepMD-kit version used. Default: 2.0.
         """
-        self.path = Path(path).resolve()
+        super().__init__(path)
+
         self.param_file = param_file
         self.machine_file = machine_file
         self.record_file = record_file
-        self.deepmd_version = deepmd_version
         self._load_task()
 
     def _load_task(self):
         """set properties for instance.
         """
         self._read_record()
         self._read_param_data()
@@ -67,34 +69,41 @@
             self.param_data = json.load(f)
 
     def _read_machine_data(self):
         _param_path = self.path / self.machine_file
         with open(_param_path) as f:
             self.machine_data = json.load(f)
 
-    @classmethod
-    def from_dict(cls, dp_task_dict: dict):
-        return cls(**dp_task_dict)
 
-
-class DPAnalyzer(ABC):
+class DPAnalyzer(BaseAnalyzer):
     """Base class to be implemented as analyzer for `DPTask`
     """
-    def __init__(self, dp_task: DPTask) -> None:
-        self.dp_task = dp_task
 
-    def _iteration_control_code(self, control_step, iteration=None):
+    def __init__(self, dp_task: DPTask, **kwargs) -> None:
+        super().__init__(dp_task)
+        if type(self.dp_task) is not DPTask:
+            self.dp_task = DPTask.from_dict(**self.dp_task.__dict__, **kwargs)
+
+    def _iteration_control_code(
+        self,
+        control_step: int,
+        iteration: Optional[int] = None
+    ):
         if iteration is None:
             if self.dp_task.step_code < control_step:
                 iteration = self.dp_task.iteration - 1
             else:
                 iteration = self.dp_task.iteration
         return iteration
 
     def _iteration_dir(self, **kwargs):
-        iteration = self._iteration_control_code(**kwargs)
+        control_step = kwargs.get('control_step', 2)
+        iteration = self._iteration_control_code(
+            control_step=control_step,
+            iteration=kwargs.get('iteration')
+        )
         return 'iter.' + str(iteration).zfill(6)
 
     @classmethod
     def setup_task(cls, **kwargs):
         task = DPTask(**kwargs)
         return cls(task)
```

### Comparing `miko_analyzer-0.3.1/miko/tesla/dpgen/exploration.py` & `miko_analyzer-0.3.2/miko/tesla/base/exploration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,107 @@
-import json
 import os
-from re import A
-import shutil
+
 from collections.abc import Iterable, Collection, Sized
-from glob import glob
 from pathlib import Path
 
-from typing import Optional, Union, List, Tuple, Dict
+from typing import Optional, Union, List, Tuple
 from matplotlib.figure import Figure
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
-from ase.io import read, write
 from matplotlib import pyplot as plt
 
 from miko.utils.log_factory import logger
-from miko.utils.files import count_lines
-from miko.graph.plotting import canvas_style, AxesInit, square_grid
-from miko.tesla.dpgen.base import DPAnalyzer
+from miko.graph.plotting import canvas_style, square_grid
+from miko.tesla.base.task import BaseAnalyzer
 
 
 def read_model_deviation(model_devi_path: Path):
     model_devi_path = model_devi_path.resolve()
     try:
         steps = np.loadtxt(model_devi_path, usecols=0)
         max_devi_f = np.loadtxt(model_devi_path, usecols=4)
-        max_devi_e = np.loadtxt(model_devi_path, usecols=3)
+        max_devi_v = np.loadtxt(model_devi_path, usecols=3)
     except FileNotFoundError as err:
         logger.error('Please select an existing model_devi.out')
         raise err
-    return steps, max_devi_f, max_devi_e
+    return steps, max_devi_f, max_devi_v
 
 
-class DPExplorationAnalyzer(DPAnalyzer):
+class ExplorationAnalyzer(BaseAnalyzer):
     """Analyzer for exploration tasks.
     """
 
-    def make_set(self, iteration: Optional[int] = None) -> List[dict]:
+    def _iteration_tasks(self, iteration: int) -> List[Path]:
+        ...
+        return []
+
+    def load_task_job_dict(self, task: Path) -> dict:
+        ...
+        return {}
+
+    def make_set(self, iteration: int, **kwargs) -> List[dict]:
         """Dump dataset for easy analysis as list of dict
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             List[dict]: all model deviation results
         """
-        n_iter = self._iteration_dir(control_step=2, iteration=iteration)
+
         all_data = []
-        for task in (self.dp_task.path / n_iter).glob('01.model_devi/task*'):
+        for task in self._iteration_tasks(iteration):
             # read model_devi.out
-            steps, max_devi_f, max_devi_e = \
+            steps, max_devi_f, max_devi_v = \
                 read_model_deviation(task / 'model_devi.out')
 
             # load job config
-            try:
-                with open(task / 'job.json', 'r') as f:
-                    job_dict = json.load(f)
-            except Exception as err:
-                logger.error(err)
-                job_dict = {}
+            job_dict = self.load_task_job_dict(task)
 
             # gather result_dict
             result_dict = {
-                'iteration': n_iter,
-                'max_devi_e': max_devi_e,
+                'iteration': self._iteration_dir(iteration=iteration, **kwargs),
+                'max_devi_v': max_devi_v,
                 'max_devi_f': max_devi_f,
                 'task_path': task,
                 'steps': steps
             }
             all_dict = {**result_dict, **job_dict}
             all_data.append(all_dict)
         return all_data
 
-    def get_cur_job(self, iteration: Optional[int]) -> dict:
-        """Get `cur_job.json` for the selected iteration
-
-        Args:
-            iteration (int, optional): the iteration to get
-
-        Returns:
-            dict: current job parameters
-        """
-        n_iter = self._iteration_dir(control_step=2, iteration=iteration)
-        try:
-            with open(
-                self.dp_task.path / n_iter / '01.model_devi' / 'cur_job.json', 'r'
-            ) as f:
-                job_dict = json.load(f)
-        except Exception as err:
-            logger.warning(err)
-            job_dict = {}
-        return job_dict
-
-    def make_set_dataframe(
-            self, iteration: Optional[int] = None) -> pd.DataFrame:
+    def make_set_dataframe(self, iteration: int) -> pd.DataFrame:
         """Dump dataset for easy analysis as `pandas.Dataframe`
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             pd.DataFrame: Dataframe containing all model deviation logs.
         """
         all_data = self.make_set(iteration=iteration)
         df = pd.DataFrame(all_data)
-        df = df.explode(["max_devi_e", "max_devi_f", "steps"])
+        df = df.explode(["max_devi_v", "max_devi_f", "steps"])
         return df
 
-    def make_set_pickle(self, iteration: Optional[int] = None) -> pd.DataFrame:
+    def make_set_pickle(self, iteration: int) -> pd.DataFrame:
         """Dump pickle from `self.make_set_dataframe` for quick load.
            Default to `<dpgen_task_path>/model_devi_each_iter/data_<iter>.pkl`
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             pd.DataFrame: DataFrame containing all model deviation logs.
         """
         df = self.make_set_dataframe(iteration=iteration)
         save_path = self.dp_task.path / 'model_devi_each_iter'
         os.makedirs(name=save_path, exist_ok=True)
-        if iteration is None:
-            iteration = self._iteration_control_code(
-                control_step=2, iteration=iteration)
         df.to_pickle(save_path / f'data_{str(iteration).zfill(6)}.pkl')
         return df
 
     def load_from_pickle(self, iteration: int) -> pd.DataFrame:
         """Load DataFrame from pickle file.
 
         Args:
@@ -139,15 +113,15 @@
         pkl_path = self.dp_task.path / \
             f'model_devi_each_iter/data_{str(iteration).zfill(6)}.pkl'
         df = pd.read_pickle(pkl_path)
         return df
 
     @staticmethod
     def _convert_group_by(
-        group_by: Optional[str] = None, 
+        group_by: Optional[str] = None,
         **kwargs
     ) -> Tuple[int, Union[List, Collection]]:
         if group_by is None:
             num_item = 1
             plot_items = [None]
         else:
             plot_items = kwargs.get(group_by)
@@ -191,98 +165,90 @@
             logger.error(f'Please choose existing iteration as input.')
             raise err
         return parts
 
     def _load_model_devi_dataframe(
             self,
             plot_item,
-            iteration=None,
+            iteration: int,
             group_by=None,
             select=None,
             select_value=None,
             **kwargs
     ) -> pd.DataFrame:
-        iteration_code = self._iteration_control_code(
-            control_step=2, iteration=iteration)
+        """Load model deviation DataFrame from tasks."""
         try:
-            df = self.load_from_pickle(iteration=iteration_code)
+            df = self.load_from_pickle(iteration=iteration)
         except FileNotFoundError:
-            df = self.make_set_pickle(iteration=iteration_code)
+            df = self.make_set_pickle(iteration=iteration)
 
         # select data frame of given select
         if all([select, select_value]):
             df = self.select_dataset(df, select, select_value)
 
         # extract data frame of given group
         if group_by:
             partdata = self.extract_group_dataset(df, plot_item, group_by)
         else:
             partdata = df
 
         # export data frame of given iteration
         parts = self.extract_iteration_dataset(
-            partdata, self._iteration_dir(
-                control_step=2, iteration=iteration
-            )
+            partdata, self._iteration_dir(iteration=iteration, **kwargs)
         )
         return parts
 
     def _data_prepareation(
             self,
             plot_item,
-            iteration=None,
+            iteration: int,
             group_by=None,
             select=None,
             select_value=None,
             **kwargs
     ):
-        iteration_code = self._iteration_control_code(
-            control_step=2, iteration=iteration)
         parts = self._load_model_devi_dataframe(
             plot_item, iteration, group_by, select, select_value, **kwargs
         )
 
         steps = parts['steps']
         mdf = parts['max_devi_f']
         label_unit = kwargs.get('label_unit')
         logger.info(
-            f"f_max = {mdf.max()} ev/Å at {group_by}={plot_item} {label_unit} at iter {iteration_code}.")
+            f"f_max = {mdf.max()} ev/Å at {group_by}={plot_item} {label_unit} at iter {iteration}.")
         return steps, mdf
 
     def _read_model_devi_trust_level(self, trust_level_key, iteration=None):
-        cur_job = self.get_cur_job(iteration)
-        trust_level = cur_job.get(trust_level_key)
-        if trust_level is None:
-            trust_level = self.dp_task.param_data[trust_level_key]
-        # Is average OK for different systems?
-        if isinstance(trust_level, Iterable):
-            trust_level = np.mean(trust_level)  # type: ignore
-        return trust_level
+        pass
 
     def plot_single_iteration(
             self,
-            iteration: Optional[int] = None,
+            iteration: int,
             *,
             x_limit: Optional[Union[float, List[float]]] = None,
             y_limit: Optional[Union[float, List[float]]] = None,
             use_log: bool = False,
             group_by: Optional[str] = None,
+            f_trust_lo: float = 0.1,
+            f_trust_hi: float = 0.3,
             select: Optional[str] = None,
             select_value: Optional[str] = None,
             **kwargs
     ) -> Figure:
         """Generate a plot of model deviation in each iteration.
 
         Args:
             iteration (int, optional): The iteration. Defaults to current iteration.
             x_limit (float, List[float], optional): Choose the limit of x axis. Defaults to None.
             y_limit (float, List[float], optional): Choose the limit of y axis. Defaults to None.
             use_log (bool, optional): Choose whether log scale used. Defaults to False.
             group_by (str, optional): Choose which the plots are grouped by, which should be included. 
                 Should be corresponding to keys in model_devi_job. Defaults to 'temps'.
+            f_trust_lo (float, optional): The lower limit of max_deviation_force. Defaults to 0.1.
+            f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to 0.3.
             select (str, optional): Choose which param selected as plot zone. Defaults to None.
             select_value (str, optional): The dependence of `select`. 
                 Different from `group_by`, please pass only one number. Defaults to None.
             kwargs (_type_, optional): Additional keyword arguments. Include other params, such as:
                 `temps`: please use the value of `group_by`, whose default input is `"temps"`.
                 `label_unit`: the unit of `select_value`, such as 'Å'.
                 Parameters of `canvas_style`: please refer to `miko.graph.plotting.canvas_style`.
@@ -299,72 +265,72 @@
         gs = fig.add_gridspec(num_item, 3)
 
         for i, plot_item in enumerate(plot_items):
             steps, mdf = self._data_prepareation(
                 plot_item, iteration, group_by, select, select_value, **kwargs)
 
             # left part
-            fig_left = fig.add_subplot(gs[i, :-1]) # type: ignore
+            fig_left = fig.add_subplot(gs[i, :-1])  # type: ignore
             fig_left_args = {
                 'x': steps,
                 'y': mdf,
                 'plot_item': plot_item,
                 'label_unit': kwargs.get('label_unit'),
                 'x_limit': x_limit,
                 'y_limit': y_limit,
                 'use_log': use_log,
-                'f_trust_lo': self._read_model_devi_trust_level("model_devi_f_trust_lo", iteration),
-                'f_trust_hi': self._read_model_devi_trust_level("model_devi_f_trust_hi", iteration),
+                'f_trust_lo': f_trust_lo,
+                'f_trust_hi': f_trust_hi,
                 'color': 'red',
                 'iteration': iteration,
             }
             PlottingExploartion.plot_mdf_time_curve(fig_left, fig_left_args)
             global_ylim = fig_left.get_ylim()
 
             # right part
-            fig_right = fig.add_subplot(gs[i, -1]) # type: ignore
+            fig_right = fig.add_subplot(gs[i, -1])  # type: ignore
             fig_right_args = {
                 'data': mdf,
                 'plot_item': plot_item,
                 'label_unit': kwargs.get('label_unit'),
                 'y_limit': global_ylim,
                 'use_log': use_log,
-                'f_trust_lo': self._read_model_devi_trust_level("model_devi_f_trust_lo", iteration),
-                'f_trust_hi': self._read_model_devi_trust_level("model_devi_f_trust_hi", iteration),
+                'f_trust_lo': f_trust_lo,
+                'f_trust_hi': f_trust_hi,
                 'color': 'red',
                 'iteration': iteration,
             }
             PlottingExploartion.plot_mdf_distribution(
                 fig_right, fig_right_args, orientation='horizontal')
             fig_right.set_xticklabels([])
             fig_right.set_yticklabels([])
         return fig
 
     def plot_multiple_iterations(
             self,
             iterations: Iterable,
             group_by: Optional[str] = None,
-            f_trust_lo: float = 0.10,
-            f_trust_hi: float = 0.30,
+            f_trust_lo: float = 0.1,
+            f_trust_hi: float = 0.3,
             x_limit: Optional[Union[float, List[float]]] = None,
             y_limit: Optional[Union[float, List[float]]] = None,
             select: Optional[str] = None,
             select_value: Optional[str] = None,
             **kwargs
     ):
         """Analyse trajectories for different temperatures.
 
         Args:
             iterations (Iterabke): Iterations selected, which should be iterable.
             group_by (str, optional): Choose which the plots are grouped by, which should be included.
             For value of group_by, a list, int or str containing desired value(s) should be included as kwargs.
             For example, if `group_by='temps'`, then `temps=[100., 200., 300.]` should also be passed to this function.
             Default: "temps".
-            f_trust_lo (float, optional): The lower limit of max_deviation_force.. Defaults to 0.10.
-            f_trust_hi (float, optional): The higher limit of max_deviation_force.. Defaults to 0.30.
+            f_trust_lo (float, optional): The lower limit of max_deviation_force. Defaults to 0.1.
+            f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to 0.3.
             x_limit (_type_, optional): The limit of x scale. Defaults to None.
             y_limit (_type_, optional): The limit of y scale. Defaults to None.
             select (_type_, optional): Choose which param selected as plot zone.. Defaults to None.
             select_value (_type_, optional): _description_. Defaults to None.
 
         Returns:
             _type_: A plot for different iterations.
@@ -381,58 +347,58 @@
             try:
                 ax = axs.flatten()[i]
             except AttributeError:
                 ax = axs
             for iteration in iterations:
                 step, mdf = self._data_prepareation(
                     plot_item, iteration, group_by, select, select_value, **kwargs)
-                ax.scatter(step, mdf, s=80, alpha=0.3, # type: ignore
+                ax.scatter(step, mdf, s=80, alpha=0.3,  # type: ignore
                            label=f'iter {int(iteration)}', marker='o')
-            ax.axhline(f_trust_lo, linestyle='dashed') # type: ignore
-            ax.axhline(f_trust_hi, linestyle='dashed') # type: ignore
-            ax.set_ylabel(r"$\sigma_{f}^{max}$ (ev/Å)") # type: ignore
-            ax.set_xlabel('Simulation time (fs)') # type: ignore
-            ax.legend() # type: ignore
+            ax.axhline(f_trust_lo, linestyle='dashed')  # type: ignore
+            ax.axhline(f_trust_hi, linestyle='dashed')  # type: ignore
+            ax.set_ylabel(r"$\sigma_{f}^{max}$ (ev/Å)")  # type: ignore
+            ax.set_xlabel('Simulation time (fs)')  # type: ignore
+            ax.legend()  # type: ignore
             if x_limit is not None:
                 PlottingExploartion._plot_set_axis_limits(
-                    ax, x_limit, 'x_limit') # type: ignore
+                    ax, x_limit, 'x_limit')  # type: ignore
             if kwargs.get('use_log', False) == True:
-                ax.set_yscale('log') # type: ignore
+                ax.set_yscale('log')  # type: ignore
             else:
                 if y_limit is not None:
                     PlottingExploartion._plot_set_axis_limits(
-                        ax, y_limit, 'y_limit') # type: ignore
+                        ax, y_limit, 'y_limit')  # type: ignore
         for i in range(num_item, nrows * nrows):
             try:
                 fig.delaxes(axs.flatten()[i])
             except AttributeError:
                 pass
         return fig
 
     def plot_multi_iter_distribution(
             self,
             iterations: Iterable,
             group_by: Optional[str] = None,
+            f_trust_lo: float = 0.1,
+            f_trust_hi: float = 0.3,
             select: Optional[str] = None,
             select_value: Optional[str] = None,
-            f_trust_lo: Optional[float] = None,
-            f_trust_hi: Optional[float] = None,
             x_limit: Optional[Union[float, List[float]]] = None,
             y_limit: Optional[Union[float, List[float]]] = None,
             **kwargs
     ) -> Figure:
         """Draw distribution in histogram of model deviation for multiple iterations.
 
         Args:
             iterations (Iterable): _description_
             group_by (str, optional): _description_. Defaults to None.
             select (str, optional): _description_. Defaults to None.
             select_value (str, optional): _description_. Defaults to None.
-            f_trust_lo (float, optional): The lower limit of max_deviation_force. Defaults to None.
-            f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to None.
+            f_trust_lo (float, optional): The lower limit of max_deviation_force. Defaults to 0.1.
+            f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to 0.3.
             x_limit (Union[float, List[float]], optional): _description_. Defaults to None.
             y_limit (Union[float, List[float]], optional): _description_. Defaults to None.
 
         Returns:
             Figure: A figure containing distribution of model deviation for multiple iterations.
         """
         num_item, plot_items = self._convert_group_by(group_by, **kwargs)
@@ -440,74 +406,68 @@
 
         canvas_style(**kwargs)
 
         nrows = square_grid(num_item)
         fig, axs = plt.subplots(nrows, nrows, figsize=[
                                 12, 12], constrained_layout=True)
 
-        colors = plt.colormaps['viridis_r']( # type: ignore
-            np.linspace(0.15, 0.85, len(iterations)) # type: ignore
+        colors = plt.colormaps['viridis_r'](  # type: ignore
+            np.linspace(0.15, 0.85, len(iterations))  # type: ignore
         )
         for i, plot_item in enumerate(plot_items):
             try:
                 ax = axs.flatten()[i]
             except AttributeError:
                 ax = axs
             for j, iteration in enumerate(iterations):
                 step, mdf = self._data_prepareation(
                     plot_item, iteration, group_by, select, select_value, **kwargs)
-                if f_trust_lo is None:
-                    f_trust_lo = self._read_model_devi_trust_level(
-                        "model_devi_f_trust_lo", iteration)
-                if f_trust_hi is None:
-                    f_trust_hi = self._read_model_devi_trust_level(
-                        "model_devi_f_trust_hi", iteration)
                 ax_args = {
                     'data': mdf,
                     'plot_item': plot_item,
                     'label_unit': kwargs.get('label_unit'),
                     'f_trust_lo': f_trust_lo,
                     'f_trust_hi': f_trust_hi,
                     'iteration': iteration,
                     'x_limit': x_limit,
                     'y_limit': y_limit,
                     'color': colors[j],
                     'label': f'Iter {iteration}'
                 }
                 PlottingExploartion.plot_mdf_distribution(
-                    ax, ax_args, orientation='vertical') # type: ignore
-            ax.set_ylabel('Distribution') # type: ignore
-            ax.set_xlabel(r'$\sigma_{f}^{max}$ (ev/Å)') # type: ignore
-            ax.legend() # type: ignore
+                    ax, ax_args, orientation='vertical')  # type: ignore
+            ax.set_ylabel('Distribution')  # type: ignore
+            ax.set_xlabel(r'$\sigma_{f}^{max}$ (ev/Å)')  # type: ignore
+            ax.legend()  # type: ignore
         for i in range(num_item, nrows * nrows):
             try:
                 fig.delaxes(axs.flatten()[i])
             except AttributeError:
                 pass
         return fig
 
     def plot_ensemble_ratio_bar(
             self,
             iterations: Iterable,
             group_by: Optional[str] = None,
             select: Optional[str] = None,
             select_value: Optional[str] = None,
-            f_trust_lo: Optional[float] = None,
-            f_trust_hi: Optional[float] = None,
+            f_trust_lo: float = 0.1,
+            f_trust_hi: float = 0.3,
             **kwargs
     ) -> Figure:
         """Draw ensemble ratio bar for multiple iterations.
 
         Args:
             iterations (Iterable): _description_
             group_by (Optional[str], optional): _description_. Defaults to None.
             select (Optional[str], optional): _description_. Defaults to None.
             select_value (Optional[str], optional): _description_. Defaults to None.
-            f_trust_lo (Optional[float], optional): _description_. Defaults to None.
-            f_trust_hi (Optional[float], optional): _description_. Defaults to None.
+            f_trust_lo (float, optional): _description_. Defaults to 0.1.
+            f_trust_hi (float, optional): _description_. Defaults to 0.3.
 
         Returns:
             Figure: _description_
         """
 
         num_item, plot_items = self._convert_group_by(group_by, **kwargs)
         nrows = square_grid(num_item)
@@ -515,29 +475,22 @@
         canvas_style(**kwargs)
 
         fig, axs = plt.subplots(nrows, nrows)
         for i, plot_item in enumerate(plot_items):
             if type(axs) is plt.Axes:
                 ax = axs
             else:
-                ax = axs.flatten()[i] # type: ignore
+                ax = axs.flatten()[i]  # type: ignore
 
-            ratios = np.zeros((len(iterations), 3)) # type: ignore
+            ratios = np.zeros((len(iterations), 3))  # type: ignore
 
             for j, iteration in enumerate(iterations):
                 df = self._load_model_devi_dataframe(
                     plot_item, iteration, group_by, select, select_value, **kwargs)
 
-                if f_trust_lo is None:
-                    f_trust_lo = self._read_model_devi_trust_level(
-                        "model_devi_f_trust_lo", iteration)
-                if f_trust_hi is None:
-                    f_trust_hi = self._read_model_devi_trust_level(
-                        "model_devi_f_trust_hi", iteration)
-
                 accu_count = (df['max_devi_f'] <= f_trust_lo).sum()
                 failed_count = (df['max_devi_f'] > f_trust_hi).sum()
                 candidate_count = (
                     (df['max_devi_f'] > f_trust_lo) &
                     (df['max_devi_f'] <= f_trust_hi)
                 ).sum()
 
@@ -551,15 +504,15 @@
                 'ratios': ratios,
                 'iterations': iterations,
             }
             PlottingExploartion.plot_ensemble_ratio_bar(ax, ax_args)
             handles, labels = ax.get_legend_handles_labels()
         fig.supxlabel('Iteration')
         fig.supylabel('Ratio')
-        fig.legend(handles, labels, loc='upper center', # type: ignore
+        fig.legend(handles, labels, loc='upper center',  # type: ignore
                    ncol=3, bbox_to_anchor=(0.5, 1.0))
         return fig
 
 
 class PlottingExploartion:
     @staticmethod
     def plot_mdf_time_curve(ax: plt.Axes, args):
@@ -583,46 +536,50 @@
         else:
             PlottingExploartion._plot_set_axis_limits(ax, y_limit, 'y_limit')
 
         if f_trust_lo is not None:
             ax.axhline(f_trust_lo, linestyle='dashed')
         if f_trust_hi is not None:
             ax.axhline(f_trust_hi, linestyle='dashed')
-        if ax.get_subplotspec().is_last_row(): # type: ignore
+        if ax.get_subplotspec().is_last_row():  # type: ignore
             ax.set_xlabel('Simulation Steps')
-        if ax.get_subplotspec().is_first_col(): # type: ignore
+        if ax.get_subplotspec().is_first_col():  # type: ignore
             ax.set_ylabel(r'$\sigma_{f}^{max}$ (ev/Å)')
         ax.legend()
         return ax
 
     @staticmethod
     def plot_mdf_distribution(ax: plt.Axes, args, orientation='vertical'):
-        #data = args.get('data')
+        # data = args.get('data')
         x_limit = args.get('x_limit')
         y_limit = args.get('y_limit')
         f_trust_lo = args.get('f_trust_lo')
         f_trust_hi = args.get('f_trust_hi')
         color = args.get('color')
         label = args.get('label')
 
         # draw the kernel density estimate plot
         if orientation == 'vertical':
             sns.kdeplot(
                 data=args, x="data", label=label, fill=True,
                 color=color, alpha=0.5, ax=ax,
             )
-            ax.axvline(f_trust_lo, linestyle='dashed')
-            ax.axvline(f_trust_hi, linestyle='dashed')
+            if f_trust_lo:
+                ax.axvline(f_trust_lo, linestyle='dashed')
+            if f_trust_hi:
+                ax.axvline(f_trust_hi, linestyle='dashed')
         elif orientation == 'horizontal':
             sns.kdeplot(
                 data=args, y="data", label=label, fill=True,
                 color=color, alpha=0.5, ax=ax
             )
-            ax.axhline(f_trust_lo, linestyle='dashed')
-            ax.axhline(f_trust_hi, linestyle='dashed')
+            if f_trust_lo:
+                ax.axhline(f_trust_lo, linestyle='dashed')
+            if f_trust_hi:
+                ax.axhline(f_trust_hi, linestyle='dashed')
         else:
             raise ValueError('Invalid orientation')
 
         PlottingExploartion._plot_set_axis_limits(ax, x_limit, 'x_limit')
         if args.get('use_log', False) == True:
             ax.set_yscale('log')
         else:
@@ -631,15 +588,15 @@
 
     @staticmethod
     def plot_ensemble_ratio_bar(ax: plt.Axes, args):
         data = args.get('ratios')
         labels = args.get('iterations')
         category_names = args.get('category_names')
 
-        category_colors = plt.colormaps['YlGnBu_r']( # type: ignore
+        category_colors = plt.colormaps['YlGnBu_r'](  # type: ignore
             np.linspace(0.15, 0.85, data.shape[1])
         )
         data_cum = data.cumsum(axis=1)
         for i, (colname, color) in enumerate(zip(category_names, category_colors)):
             widths = data[:, i]
             starts = data_cum[:, i] - widths
             ax.bar(labels, widths, width=0.5, bottom=starts,
@@ -659,13 +616,13 @@
             if isinstance(limitation, (int, float)):
                 _func(0, limitation)
             elif isinstance(limitation, Sized):
                 if len(limitation) > 2:
                     raise ValueError("Limitation should be a value \
                         or a set with no more than 2 elements.")
                 elif len(limitation) == 1:
-                    _func(0, limitation[0]) # type: ignore
+                    _func(0, limitation[0])  # type: ignore
                 else:
                     _func(limitation)
             else:
                 raise ValueError("Limitation should be a value \
                     or a set with no more than 2 elements.")
```

### Comparing `miko_analyzer-0.3.1/miko/tesla/dpgen/labeling.py` & `miko_analyzer-0.3.2/miko/tesla/base/labeling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 import os
 
 import numpy as np
 from pathlib import Path
+from typing import List, Literal
 
 from ase.io import read
 from matplotlib import pyplot as plt
 
 from miko.utils.log_factory import logger
 from miko.utils.log_factory import LogFactory
-from miko.tesla.dpgen.base import DPAnalyzer
+from miko.tesla.base.task import BaseTask, BaseAnalyzer
 from miko.graph.plotting import canvas_style
 
 
 
-class DPLabelingAnalyzer(DPAnalyzer):
+class LabelingAnalyzer(BaseAnalyzer):
+
+    def __init__(
+        self, dp_task: BaseTask, 
+        fp_style: Literal['vasp', 'cp2k'] = 'vasp'
+    ) -> None:
+        super().__init__(dp_task)
+        self.fp_style = fp_style
+    
+    def get_fp_tasks(self, iteration: int = 0) -> List[Path]:
+        ...
+        return []
 
     def fp_group_distance(self, iteration, atom_group, **kwargs):
         """
         Analyse the distance of selected structures.
         :param iteration: The iteration selected.
         :param atom_group:A tuple contains the index number of two selected atoms.
         :return: A plot of distance distribution.
         """
+        task_files = self.get_fp_tasks(iteration=iteration)
+
         dis_loc = []
         dis = []
-        place = self.dp_task.path / f'iter.{str(iteration).zfill(6)}/02.fp'
+
         _stc_name = self._fp_style()
-        for i in place.iterdir():
+        for i in task_files:
             stc_file_path = i / _stc_name # type: ignore
             if stc_file_path.exists():
                 dis_loc.append(i)
                 stc = read(stc_file_path) 
                 dis.append(stc.get_distance( # type: ignore
                     atom_group[0], atom_group[1], mic=True))
         diss = np.array(dis)
@@ -52,27 +66,28 @@
         Analyse the distance of selected structures.
         :param iteration: The iteration selected.
         :param ele_group:A tuple contains the index number of two selected elements.
         :return: A plot of distance distribution.
         """
         dis = []
         dis_loc = []
-        place = os.path.join(self.dp_task.path, 'iter.' +
-                             str(iteration).zfill(6), '02.fp')
-        _output_name = self._fp_style()
-        for i in os.listdir(place):
-            if os.path.exists(os.path.join(place, i, _output_name)):
+        task_files = self.get_fp_tasks(iteration=iteration)
+        _stc_name = self._fp_style()
+
+        for i in task_files:
+            stc_file_path = i / _stc_name # type: ignore
+            if stc_file_path.exists():
                 dis_loc.append(i)
-                stc = read(os.path.join(place, i, _output_name))
-                symbol_list = stc.get_chemical_symbols()
+                stc = read(stc_file_path)
+                symbol_list = stc.get_chemical_symbols() # type: ignore
                 ele_list_1 = [i for i in range(
                     len(symbol_list)) if symbol_list[i] == ele_group[0]]
                 ele_list_2 = [i for i in range(
                     len(symbol_list)) if symbol_list[i] == ele_group[0]]
-                min_dis = min([stc.get_distance(ii, jj, mic=True)
+                min_dis = min([stc.get_distance(ii, jj, mic=True) # type: ignore
                                for ii in ele_list_1 for jj in ele_list_2])
                 dis.append(min_dis)
         diss = np.array(dis)
 
         fig, ax = plt.subplots()
         canvas_style(**kwargs)
 
@@ -80,40 +95,40 @@
                  label=f'iter {int(iteration)}')
         ax.legend(fontsize=16)
         ax.set_xlabel("d(Å)", fontsize=16)
         ax.set_xticks(np.arange(0, 6, step=0.5), fontsize=16)
         ax.set_yticks(fontsize=16)
         ax.set_title(
             f"Distibution of {ele_group[0]}-{ele_group[1]} distance", fontsize=16)
-        return plt
+        return fig
     
     def _fp_style(self):
         styles = {
             "vasp": "POSCAR",
             "cp2k": "coord.xyz",
         }
-        return styles.get(self.dp_task.param_data['fp_style'], None)
+        return styles.get(self.fp_style, None)
 
     def _fp_output_style(self):
         styles = {
             "vasp": "vasprun.xml",
             "cp2k": "coord.xyz",
         }
-        return styles.get(self.dp_task.param_data['fp_style'], None)
+        return styles.get(self.fp_style, None)
 
     def _fp_output_dpgen(self):
         styles = {
             "vasp": "OUTCAR",
             "cp2k": "output",
             "qe": "output",
             "siesta": "output",
             "gaussian": "output",
             "pwmat": "REPORT",
         }
-        return styles.get(self.dp_task.param_data['fp_style'], None)
+        return styles.get(self.fp_style, None)
 
     def _fp_output_format(self):
         styles = {
             "vasp": "vasp/outcar",
             "cp2k": "cp2k/output",
         }
-        return styles.get(self.dp_task.param_data['fp_style'], None)
+        return styles.get(self.fp_style, None)
```

### Comparing `miko_analyzer-0.3.1/miko/tesla/dpgen/training.py` & `miko_analyzer-0.3.2/miko/tesla/base/training.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,76 @@
+from pathlib import Path
+
 import numpy as np
 from matplotlib import pyplot as plt
 
 from miko.utils import logger
 from miko.graph.plotting import canvas_style
-from miko.tesla.dpgen.base import DPAnalyzer
+from miko.tesla.base.task import BaseAnalyzer, BaseTask
+
 
-class DPTrainingAnalyzer(DPAnalyzer):
+class TrainingAnalyzer(BaseAnalyzer):
     """Analyzer for training tasks.
     """
 
-    def load_lcurve(self, iteration=None, model=0):
-        n_iter = self._iteration_dir(control_step=2, iteration=iteration)
-        lcurve_path = self.dp_task.path / n_iter / \
-            f'00.train/{str(model).zfill(3)}/lcurve.out'
+    def __init__(
+        self,
+        dp_task: BaseTask,
+        validation: bool = False
+    ) -> None:
+        super().__init__(dp_task)
+        self.validation = validation
+
+    def get_lcurve_path(self, iteration: int, model=0) -> Path:
+        ...
+        return Path()
 
-        from distutils.version import LooseVersion
+    def load_lcurve(self, iteration: int, model=0):
+        lcurve_path = self.get_lcurve_path(iteration=iteration, model=model)
 
-        if LooseVersion(self.dp_task.deepmd_version) < LooseVersion('2.0'):
+        if self.validation is True:
             return {
                 'step': np.loadtxt(lcurve_path, usecols=0),
                 'energy_train': np.loadtxt(lcurve_path, usecols=4),
-                'energy_test': np.loadtxt(lcurve_path, usecols=3),
+                'energy_validation': np.loadtxt(lcurve_path, usecols=3),
                 'force_train': np.loadtxt(lcurve_path, usecols=6),
-                'force_test': np.loadtxt(lcurve_path, usecols=5),
+                'force_validation': np.loadtxt(lcurve_path, usecols=5),
             }
         else:
             return {
                 'step': np.loadtxt(lcurve_path, usecols=0),
                 'energy_train': np.loadtxt(lcurve_path, usecols=2),
                 'force_train': np.loadtxt(lcurve_path, usecols=3)
             }
 
-    def plot_lcurve(self, iteration=None, model=0, **kwargs):
+    def plot_lcurve(self, iteration: int, model=0, **kwargs):
         lcurve_data = self.load_lcurve(iteration=iteration, model=model)
 
         canvas_style(**kwargs)
         fig, axs = plt.subplots(2, 1)
-        fig.suptitle("DeepMD training and tests error")
 
         # energy figure
         step = lcurve_data['step']
         for key in lcurve_data.keys():
             if key.startswith('energy_'):
-                axs[0].scatter(step[10:], lcurve_data[key][10:],
-                               alpha=0.4, label=key.replace('energy_', ''))
-        axs[0].hlines(0.005, step[0], step[-1], linestyles='--',
-                      colors='red', label='5 meV')
-        axs[0].hlines(0.01, step[0], step[-1], linestyles='--',
-                      colors='blue', label='10 meV')
-        axs[0].hlines(0.05, step[0], step[-1], linestyles='--', label='50 meV')
+                axs[0].plot(step[10:], lcurve_data[key][10:],
+                            alpha=0.4, label=key.replace('energy_', ''))
+        axs[0].axhline(0.005, linestyle='dashed', color='red', label='5 meV')
+        axs[0].axhline(0.01, linestyle='dashed', color='blue', label='10 meV')
+        axs[0].axhline(0.05, linestyle='dashed', label='50 meV')
         axs[0].set_xlabel('Number of training batch')
         axs[0].set_ylabel('$E$(eV)')
         axs[0].legend()
 
         # force figure
         for key in lcurve_data.keys():
             if key.startswith('force_'):
-                axs[1].scatter(step[10:], lcurve_data[key][10:],
-                               alpha=0.4, label=key.replace('force_', ''))
-        axs[1].hlines(0.05, step[0], step[-1], linestyles='--',
-                      colors='red', label='50 meV/Å')
-        axs[1].hlines(0.1, step[0], step[-1], linestyles='--',
-                      colors='blue', label='100 meV/Å')
-        axs[1].hlines(0.2, step[0], step[-1],
-                      linestyles='--', label='200 meV/Å')
+                axs[1].plot(step[10:], lcurve_data[key][10:],
+                            alpha=0.4, label=key.replace('force_', ''))
+        axs[1].axhline(0.05, linestyle='dashed', color='red', label='50 meV/Å')
+        axs[1].axhline(0.1, linestyle='dashed', color='blue', label='100 meV/Å')
+        axs[1].axhline(0.2, linestyle='dashed', label='200 meV/Å')
         axs[1].set_xlabel('Number of training batch')
         axs[1].set_ylabel('$F$(eV/Å)')
         axs[1].legend()
 
         return fig
```

### Comparing `miko_analyzer-0.3.1/miko/utils/log_factory.py` & `miko_analyzer-0.3.2/miko/utils/log_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import os
+from pathlib import Path
 import logging
 
 
 class LogFactory(object):
     """
     For logging
     """
-    def __init__(self, logger=None, log_dir=""):
-        self.log_path = os.getcwd() if log_dir == "" else log_dir
+    def __init__(self, logger=None, log_dir=None, log_name="miko.log"):
+        self.log_path = Path.cwd() if log_dir is None else Path(log_dir)
         self.logger = logging.getLogger(logger)
         self.logger.setLevel(logging.DEBUG)
-        self.log_name = os.path.join(self.log_path, "miko.log")
+        self.log_name = self.log_path / log_name
 
         # create file handler which logs even debug messages
         file_handler = logging.FileHandler(self.log_name, delay=True)
         file_handler.setLevel(logging.DEBUG)
         # create console handler with a higher log level
         console_handler = logging.StreamHandler()
         console_handler.setLevel(logging.INFO)
```

### Comparing `miko_analyzer-0.3.1/pyproject.toml` & `miko_analyzer-0.3.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miko-analyzer"
-version = "0.3.1"
+version = "0.3.2"
 description = "Analyzing tool for deep learning based chemical research."
 authors = ["Cloudac7 <scottryuu@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cloudac7/miko-analysis"
 packages = [{include = "miko"}]
 
@@ -20,14 +20,16 @@
 dpdata = "*"
 dscribe = "*"
 dynaconf = "*"
 mdanalysis = "^2.2"
 scipy = "^1.10.1"
 seaborn = "*"
 tqdm = "^4.65.0"
+pymatgen = "^2023.5.10"
+ai2-kit = "^0.3.18"
 
 [tool.poetry.group.test.dependencies]
 flake8 = "*"
 pytest = "*"
 pytest-mock = "*"
 pytest-datadir = "*"
 coverage = "*"
```

### Comparing `miko_analyzer-0.3.1/setup.py` & `miko_analyzer-0.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,39 +3,43 @@
 
 packages = \
 ['miko',
  'miko.cmdline',
  'miko.graph',
  'miko.structure',
  'miko.tesla',
+ 'miko.tesla.ai2_kit',
+ 'miko.tesla.base',
  'miko.tesla.dpgen',
  'miko.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['ase>=3.21.1,<4.0.0',
+['ai2-kit>=0.3.18,<0.4.0',
+ 'ase>=3.21.1,<4.0.0',
  'dpdata',
  'dscribe',
  'dynaconf',
  'matplotlib>=3.7.1,<4.0.0',
  'mdanalysis>=2.2,<3.0',
  'numpy>=1.18,<1.24',
  'pandas>=1.3.3,<2.0.0',
+ 'pymatgen>=2023.5.10,<2024.0.0',
  'scipy>=1.10.1,<2.0.0',
  'seaborn',
  'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['miko = miko.cmdline.base:cli']}
 
 setup_kwargs = {
     'name': 'miko-analyzer',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'Analyzing tool for deep learning based chemical research.',
     'long_description': '# Miko-Analyzer\n\n[![Python package](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml)\n[![Coverage Status](https://coveralls.io/repos/github/Cloudac7/miko-analyzer/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/miko-analyzer?branch=master)\n\n> コードで占う巫女。\n> Miko using code to perform divinition.\n\nAn analysis plugin for [Deep Potential](https://github.com/deepmodeling/deepmd-kit) based chemical research.\n\nSupporting simple calculation workflow with the help of [DPDispatcher](https://github.com/deepmodeling/dpdispatcher).\n\n## Installation\n\nTo install, clone the repository:\n\n```\ngit clone https://github.com/cloudac7/miko-analyzer.git\n```\n\nand then install with `pip`:\n\n```\ncd miko-analyzer\npip install .\n```\n\n',
     'author': 'Cloudac7',
     'author_email': 'scottryuu@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cloudac7/miko-analysis',
```

### Comparing `miko_analyzer-0.3.1/PKG-INFO` & `miko_analyzer-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: miko-analyzer
-Version: 0.3.1
+Version: 0.3.2
 Summary: Analyzing tool for deep learning based chemical research.
 Home-page: https://github.com/cloudac7/miko-analysis
 License: Apache-2.0
 Author: Cloudac7
 Author-email: scottryuu@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ai2-kit (>=0.3.18,<0.4.0)
 Requires-Dist: ase (>=3.21.1,<4.0.0)
 Requires-Dist: dpdata
 Requires-Dist: dscribe
 Requires-Dist: dynaconf
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mdanalysis (>=2.2,<3.0)
 Requires-Dist: numpy (>=1.18,<1.24)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: pymatgen (>=2023.5.10,<2024.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/cloudac7/miko-analysis
 Description-Content-Type: text/markdown
 
 # Miko-Analyzer
```

