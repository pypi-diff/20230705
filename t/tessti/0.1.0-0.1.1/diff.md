# Comparing `tmp/tessti-0.1.0.tar.gz` & `tmp/tessti-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessti-0.1.0.tar", last modified: Fri Jun 16 13:10:20 2023, max compression
+gzip compressed data, was "tessti-0.1.1.tar", last modified: Wed Jul  5 14:54:52 2023, max compression
```

## Comparing `tessti-0.1.0.tar` & `tessti-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-06-16 13:10:20.527936 tessti-0.1.0/
--rw-r--r--   0 vedrenne (271197) images    (7000)     4765 2023-06-16 13:10:20.527936 tessti-0.1.0/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)     4108 2023-06-16 13:07:51.000000 tessti-0.1.0/README.md
--rw-r--r--   0 vedrenne (271197) images    (7000)       38 2023-06-16 13:10:20.527936 tessti-0.1.0/setup.cfg
--rw-r--r--   0 vedrenne (271197) images    (7000)     1602 2023-06-16 13:08:31.000000 tessti-0.1.0/setup.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-06-16 13:10:20.527936 tessti-0.1.0/tessti/
--rw-r--r--   0 vedrenne (271197) images    (7000)      138 2023-06-16 12:09:00.000000 tessti-0.1.0/tessti/__init__.py
--rw-r--r--   0 vedrenne (271197) images    (7000)     3501 2023-06-16 12:36:29.000000 tessti-0.1.0/tessti/main.py
--rw-r--r--   0 vedrenne (271197) images    (7000)     4980 2023-06-16 12:05:43.000000 tessti-0.1.0/tessti/scheduler.py
-drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-06-16 13:10:20.527936 tessti-0.1.0/tessti.egg-info/
--rw-r--r--   0 vedrenne (271197) images    (7000)     4765 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/PKG-INFO
--rw-r--r--   0 vedrenne (271197) images    (7000)      250 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/SOURCES.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/dependency_links.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        1 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/not-zip-safe
--rw-r--r--   0 vedrenne (271197) images    (7000)        5 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/requires.txt
--rw-r--r--   0 vedrenne (271197) images    (7000)        7 2023-06-16 13:10:20.000000 tessti-0.1.0/tessti.egg-info/top_level.txt
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-07-05 14:54:52.656009 tessti-0.1.1/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     6640 2023-07-05 14:54:52.656009 tessti-0.1.1/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)     5983 2023-07-05 14:53:45.000000 tessti-0.1.1/README.md
+-rw-r--r--   0 vedrenne (271197) images    (7000)       38 2023-07-05 14:54:52.656009 tessti-0.1.1/setup.cfg
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1690 2023-07-04 08:31:44.000000 tessti-0.1.1/setup.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-07-05 14:54:52.656009 tessti-0.1.1/tessti/
+-rw-r--r--   0 vedrenne (271197) images    (7000)       86 2023-07-05 14:50:46.000000 tessti-0.1.1/tessti/__init__.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)     3709 2023-07-05 14:25:54.000000 tessti-0.1.1/tessti/config.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)     1501 2023-07-05 14:45:45.000000 tessti-0.1.1/tessti/main.py
+-rw-r--r--   0 vedrenne (271197) images    (7000)     5011 2023-07-05 14:50:06.000000 tessti-0.1.1/tessti/scheduler.py
+drwxr-xr-x   0 vedrenne (271197) images    (7000)        0 2023-07-05 14:54:52.656009 tessti-0.1.1/tessti.egg-info/
+-rw-r--r--   0 vedrenne (271197) images    (7000)     6640 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/PKG-INFO
+-rw-r--r--   0 vedrenne (271197) images    (7000)      300 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/SOURCES.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/dependency_links.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)       43 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/entry_points.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        1 2023-06-16 13:10:20.000000 tessti-0.1.1/tessti.egg-info/not-zip-safe
+-rw-r--r--   0 vedrenne (271197) images    (7000)       22 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/requires.txt
+-rw-r--r--   0 vedrenne (271197) images    (7000)        7 2023-07-05 14:54:52.000000 tessti-0.1.1/tessti.egg-info/top_level.txt
```

### Comparing `tessti-0.1.0/setup.py` & `tessti-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 name = "tessti"
 url = f"https://github.com/ListIndexOutOfRange/{name}"
 
 with open("README.md", "r") as f:
     readme = f.read()
 
-install_requires = ["toml",]
+install_requires = ["fire", "prettytable", "toml"]
 
 setup(
     name=name,
     version=__version__,
     description="A tool to schedule SLURM jobs made as simple as possible.",
     long_description_content_type="text/markdown",
     long_description=readme,
@@ -32,14 +32,15 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
+    entry_points={"console_scripts": ['tessti=tessti.main:cli']},
     python_requires=">=3.7",
 )
 
 
 # _______________________________________________________________________________________________ #
 # Using this script:
 # >>> python setup.py sdist bdist_wheel
```

### Comparing `tessti-0.1.0/tessti/main.py` & `tessti-0.1.1/tessti/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,102 +1,122 @@
 from __future__ import annotations
-from typing import Any, Sequence
+from typing import TypeAlias, Any, Sequence
 import toml
 from pathlib import Path
-from argparse import ArgumentParser
-from .scheduler import HPCScheduler
+from prettytable import PrettyTable
 
 
-def parse_config_path_arg() -> str | None:
-    parser = ArgumentParser('Schedule multiple jobs or run a single job.')
-    # if config is specified, launch single run, else, schedule multi runs
-    parser.add_argument('--config', type=str, default=None)
-    return parser.parse_args().config
-
-
-def run(config_path: str | Path) -> None:
-    config = toml.load(config_path)
-    file = Path(config['run']['file'])
-    if file.suffix == '.py':
-        file = file.with_suffix('')
-    function = config['run']['function']
-    args = config['args']
-    exec(f'from {file} import {function}')
-    eval(f'{function}(**{args})')
+ConfigHPC: TypeAlias = dict[str: int | str | list[str]]
+CONFIG_PATH = Path(__file__).resolve().parent / '.config.toml'
+
+
+def create_hpc_config_file_if_required() -> None:
+    if CONFIG_PATH.exists():
+        return
+    f = open(CONFIG_PATH, 'w')
+    f.close()
+
+
+def save_hpc_config(config: ConfigHPC) -> None:
+    with open(CONFIG_PATH, 'w') as file:
+        toml.dump(config, file)
+
+
+def get_hpc_config() -> ConfigHPC:
+    return toml.load(CONFIG_PATH) if CONFIG_PATH.exists() else dict()
+
+
+def pretty_print_hpc_config(max_width: int = 40) -> None:
+    config = get_hpc_config()
+    table = PrettyTable(["Key", "Value"], max_width=max_width)
+    for k, v in config.items():
+        table.add_row([k, v])
+    table.title = 'HPC Configuration'
+    print(table)
+
+
+def set_hpc_config(
+    jobs_dir: str = None,
+    partition: str = None,
+    account: str = None,
+    node: int = None,
+    task: int = None,
+    cpu: int = None,
+    gpu: int = None,
+    ram: int = None,
+    constraint: str = None,
+    modules: list[str] = None,
+    commands: list[str] = None,
+) -> None:
+    params = parse(**locals())
+    new_config = {k: v for k, v in params.items() if v is not None}
+    create_hpc_config_file_if_required()
+    current_config = get_hpc_config()
+    updated_config = {**current_config, **new_config}
+    save_hpc_config(updated_config)
+
+
+def resolve_config(**kwargs: ConfigHPC) -> ConfigHPC:
+    """ Update a copy of the global SLURM config with given parameters for a single schedule. """
+    current_slurm_config = get_hpc_config()
+    for k in current_slurm_config.keys():
+        if kwargs[k] is not None:
+            current_slurm_config[k] = kwargs[k]
+    return current_slurm_config
 
 
 def create_configs(
     *,
     # ___________________________________ SLURM #
-    working_dir: str,
     jobs_dir: str,
     partition: str,
     account: str,
     node: int,
     task: int,
     cpu: int,
     gpu: int,
     ram: int,
     constraint: str,
     modules: list[str],
     commands: list[str],
     # _____________________________________ JOB #
     file: str,
     function: str,
-    args: dict[Any: Any] = dict(),
+    args: dict[Any: Any],
     # ________________________________ SCHEDULE #
     name: str,
-    schedule: dict[str: Sequence[Any]] = dict(),
-) -> None:
+    schedule: dict[str: Sequence[Any]],
+) -> Path:
+    # path handling
+    path = Path(file)
+    working_dir = path.resolve().parent
+    file = path.stem
+    # slurm config
+    slurm_config = resolve_config(**locals())
+    slurm_config['name'] = name
     # template config
     template_config = dict()
-    template_config['run'] = dict(file=file, function=function)
+    template_config['run'] = dict(working_dir=str(working_dir), file=file, function=function)
     template_config['args'] = args
-    with open((Path(working_dir) / 'template').with_suffix('.toml'), 'w') as config_file:
+    template_config_file = (working_dir / 'template').with_suffix('.toml')
+    with open(template_config_file, 'w') as config_file:
         toml.dump(template_config, config_file)
     # schedule config
     schedule_config = dict()
-    schedule_config['slurm'] = dict(name=name, working_dir=working_dir, jobs_dir=jobs_dir,
-                                    partition=partition, account=account,
-                                    node=node, task=task, cpu=cpu, gpu=gpu, ram=ram,
-                                    constraint=constraint, modules=modules, commands=commands)
+    schedule_config['slurm'] = slurm_config
     schedule_config['parameters'] = dict()
     for key, values in schedule.items():
         schedule_config['parameters'][key] = values
-    with open((Path(working_dir) / 'schedule').with_suffix('.toml'), 'w') as config_file:
+    schedule_config_file = (working_dir / 'schedule').with_suffix('.toml')
+    with open(schedule_config_file, 'w') as config_file:
         toml.dump(schedule_config, config_file)
+    return schedule_config_file
 
 
-def schedule(
-    *,
-    # ___________________________________ SLURM #
-    working_dir: str = '.',
-    jobs_dir: str = 'jobs',
-    partition: str = 'publicgpu',
-    account: str = 'miv',
-    node: int = 1,
-    task: int = 1,
-    cpu: int = 1,
-    gpu: int = 1,
-    ram: int = 16,
-    constraint: str = 'gpua100|gpurtx6000|gpurtx5000|gpuv100',
-    modules: list[str] = ['python/Anaconda3-2019', 'cuda/cuda-11.8', 'gcc/gcc-11'],
-    commands: list[str] = ['source /usr/local/Anaconda/Anaconda3-2019.07/etc/profile.d/conda.sh',
-                           'conda deactivate',
-                           'conda activate torch2cu118'],
-    # _____________________________________ JOB #
-    file: str,
-    function: str,
-    args: dict[Any: Any] = dict(),
-    # ________________________________ SCHEDULE #
-    name: str,
-    schedule: dict[str: Sequence[Any]] = dict(),
-) -> None:
-    config_path = parse_config_path_arg()
-    if config_path is not None:
-        run(config_path)
-        return
-    params = locals()
-    params.pop('config_path')
-    create_configs(**params)
-    schedule_config_path = Path(working_dir).resolve() / 'schedule.toml'
-    HPCScheduler(config_path=schedule_config_path).run()
+def parse(**kwargs: ConfigHPC) -> ConfigHPC:
+    """ Handle string to list of strings or dict[str: Any]. """
+    for k, v in kwargs.items():
+        if k in ('modules', 'commands') and isinstance(v, str):
+            kwargs[k] = v[1:-1].split(',')
+        if k in ('args', 'schedule'):
+            kwargs[k] = eval(f'dict({kwargs[k]})')
+    return kwargs
```

### Comparing `tessti-0.1.0/tessti/scheduler.py` & `tessti-0.1.1/tessti/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
     @property
     def template_path(self) -> Path:
         return self.parent / 'template.toml'
 
     @property
     def slurm_script_params(self) -> tuple[str | int | list[str]]:
-        return (self.config['slurm']['working_dir'],
-                self.config['slurm']['jobs_dir'],
+        return (self.config['slurm']['jobs_dir'],
                 self.config['slurm']['partition'],
                 self.config['slurm']['account'],
                 self.config['slurm']['node'],
                 self.config['slurm']['task'],
                 self.config['slurm']['cpu'],
                 self.config['slurm']['gpu'],
                 self.config['slurm']['ram'],
@@ -67,16 +66,16 @@
     def prepare_jobs(self) -> list[Path]:
         self.setup_jobs_env()
         return self.write_configs()
 
     def write_slurm_job_files(self, config_paths: list[Path]) -> None:
         for config_path in config_paths:
             config = toml.load(config_path)
-            job_name = config['name']
-            script = get_slurm_script(job_name, *self.slurm_script_params)
+            working_dir, job_name = config['run']['working_dir'], config['name']
+            script = get_slurm_script(working_dir, job_name, *self.slurm_script_params)
             script_path = str(self.jobs_dir / f'{job_name}.job')
             with open(script_path, 'w') as file:
                 file.write(script)
 
     def submit_slurm_schedule(self) -> None:
         jobs_paths = list(self.jobs_dir.glob('*.job'))
         for path in jobs_paths:
@@ -89,31 +88,32 @@
         self.submit_slurm_schedule()
 
 
 # _______________________________________________________________________________________________ #
 
 
 def get_slurm_script(
-    job_name: str,
     working_dir: str,
+    job_name: str,
     jobs_dir: str,
     partition: str,
     account: str,
     node: int,
     task: int,
     cpu: int,
     gpu: int,
     ram: int,
     constraint: str,
     modules: list[str],
     commands: list[str],
 ) -> str:
-    working_dir = str(Path(working_dir).resolve())
-    stem = Path(jobs_dir) / job_name
-    config, output = f'{stem}.toml', f'{stem}.out'
+    working_dir = Path(working_dir).resolve()
+    stem = working_dir / Path(jobs_dir) / job_name
+    config = str(stem.with_suffix('.toml'))
+    output = str(stem.with_suffix('.out'))
     slurm = f"""#! /bin/bash
 
 
 # +------------------------------------------------------------------------------------+ #
 # |                                  SLURM PARAMETERS                                  | #
 # +------------------------------------------------------------------------------------+ #
 
@@ -139,10 +139,10 @@
         env += f"{command}\n"
     env += f"cd {working_dir}\n\n"
     run = f"""
 # +------------------------------------------------------------------------------------+ #
 # |                                 RUN PYTHON SCRIPT                                  | #
 # +------------------------------------------------------------------------------------+ #
 
-python schedule.py --config {config}
+tessti run {config}
 """
     return slurm + env + run
```

