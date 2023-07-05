# Comparing `tmp/clearml_session-0.4.0-py3-none-any.whl.zip` & `tmp/clearml_session-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 39932 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-11 21:21 clearml_session/__init__.py
--rw-r--r--  2.0 unx    49931 b- defN 23-Feb-11 21:21 clearml_session/__main__.py
--rw-r--r--  2.0 unx    37842 b- defN 23-Feb-11 21:21 clearml_session/interactive_session_task.py
--rw-r--r--  2.0 unx     4781 b- defN 23-Feb-11 21:21 clearml_session/single_thread_proxy.py
--rw-r--r--  2.0 unx    15948 b- defN 23-Feb-11 21:21 clearml_session/tcp_proxy.py
--rw-r--r--  2.0 unx       22 b- defN 23-Feb-11 21:21 clearml_session/version.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    17871 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1060 b- defN 23-Feb-11 21:21 clearml_session-0.4.0.dist-info/RECORD
-12 files, 138987 bytes uncompressed, 38126 bytes compressed:  72.6%
+Zip file size: 40551 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-05 05:49 clearml_session/__init__.py
+-rw-r--r--  2.0 unx    52386 b- defN 23-Jul-05 05:49 clearml_session/__main__.py
+-rw-r--r--  2.0 unx    37840 b- defN 23-Jul-05 05:49 clearml_session/interactive_session_task.py
+-rw-r--r--  2.0 unx     4781 b- defN 23-Jul-05 05:49 clearml_session/single_thread_proxy.py
+-rw-r--r--  2.0 unx    15948 b- defN 23-Jul-05 05:49 clearml_session/tcp_proxy.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-05 05:49 clearml_session/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18143 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1060 b- defN 23-Jul-05 05:49 clearml_session-0.6.0.dist-info/RECORD
+12 files, 141712 bytes uncompressed, 38745 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: clearml_session/tcp_proxy.py
 Comment: 
 
 Filename: clearml_session/version.py
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/LICENSE
+Filename: clearml_session-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/METADATA
+Filename: clearml_session-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/WHEEL
+Filename: clearml_session-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/entry_points.txt
+Filename: clearml_session-0.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/top_level.txt
+Filename: clearml_session-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: clearml_session-0.4.0.dist-info/RECORD
+Filename: clearml_session-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## clearml_session/__main__.py

```diff
@@ -20,20 +20,30 @@
 import psutil
 from clearml import Task
 from clearml.backend_api.session.client import APIClient
 from clearml.config import config_obj
 from clearml.backend_api import Session
 from .tcp_proxy import TcpProxy
 from .single_thread_proxy import SingleThreadProxy
+from .version import __version__
 
+# noinspection PyBroadException
+try:
+    Session.add_client(__package__.partition(".")[0].replace("_", "-"), __version__)  # noqa
+except Exception:
+    pass
 
 system_tag = 'interactive'
 default_docker_image = 'nvidia/cuda:10.1-runtime-ubuntu18.04'
 
 
+class NonInteractiveError(Exception):
+    pass
+
+
 def _read_std_input(timeout):
     # wait for user input with timeout, return None if timeout or user input
     if sys.platform == 'win32':
         start_time = time()
         input_str = ''
         while True:
             if msvcrt.kbhit():
@@ -146,20 +156,21 @@
     with open(base_script_file, 'rt') as f:
         task_script['diff'] += '\n\n' + f.read()
 
     task_script['working_dir'] = '.'
     task_script['entry_point'] = 'interactive_session.py'
     task_script['requirements'] = {'pip': '\n'.join(
         ["clearml>=1.1.5"] +
-        (["jupyter", "jupyterlab", "jupyterlab_git", "traitlets"] if state.get('jupyter_lab') else []) +
+        (["jupyter", "jupyterlab", "traitlets"] if state.get('jupyter_lab') else []) +
         (['pylint'] if state.get('vscode_server') else []))}
 
     section, _, _ = _get_config_section_name()
 
     if Session.check_min_api_version('2.13'):
+        # noinspection PyProtectedMember
         _runtime_prop = dict(task._get_runtime_properties())
         _runtime_prop.update({
             "_user_key": '',
             "_user_secret": '',
             "_jupyter_token": '',
             "_ssh_password": "training",
         })
@@ -222,14 +233,15 @@
         (state.get('packages') or []) + ["clearml"] + \
         (["jupyter", "jupyterlab", "jupyterlab_git"] if state.get('jupyter_lab') else []) + \
         (['pylint'] if state.get('vscode_server') else [])
     task.update_task(task_state)
     section, _, _ = _get_config_section_name()
 
     if Session.check_min_api_version('2.13'):
+        # noinspection PyProtectedMember
         _runtime_prop = dict(task._get_runtime_properties())
         _runtime_prop.update({
             "_user_key": '',
             "_user_secret": '',
             "_jupyter_token": '',
             "_ssh_password": "training",
         })
@@ -338,14 +350,15 @@
             logging.getLogger().warning("could not locate project by the named '{}'".format(project_name))
             project_id = None
     return project_id
 
 
 def get_user_inputs(args, parser, state, client):
     default_needed_args = tuple()
+    assume_yes = args.yes
 
     user_args = sorted([a for a in args.__dict__ if not a.startswith('_')])
     # clear some states if we replace the base_task_id
     if 'base_task_id' in user_args and getattr(args, 'base_task_id', None) != state.get('base_task_id'):
         print('New base_task_id \'{}\', clearing previous packages & init_script'.format(
             getattr(args, 'base_task_id', None)))
         state.pop('init_script', None)
@@ -369,14 +382,17 @@
                 pass  # keep as is
         elif not v and a == 'remote_gateway':
             state.pop(a, None)
         elif v is not None:
             state[a] = v
 
         if a in default_needed_args and not state.get(a):
+            if assume_yes:
+                raise NonInteractiveError(
+                    "Using `--yes` but could not locate previously used value of '{}'".format(a))
             # noinspection PyProtectedMember
             state[a] = input(
                 "\nCould not locate previously used value of '{}', please provide it?"
                 "\n    Help: {}\n> ".format(
                     a, parser._option_string_actions['--{}'.format(a.replace('_', '-'))].help))
     # if no password was set, create a new random one
     if not state.get('password'):
@@ -388,18 +404,24 @@
         state['packages'] = (args.packages or []) + [
             p.strip() for p in args.requirements.readlines() if not p.strip().startswith('#')]
     elif args.packages is not None:
         state['packages'] = args.packages or []
 
     # allow to select queue
     ask_queues = not state.get('queue')
-    if state.get('queue'):
+
+    if assume_yes:
+        if ask_queues:
+            raise NonInteractiveError("Using `--yes` but no queue provided or previously used")
+        print("Using previous queue (resource) '{}'".format(state["queue"]))
+    elif state.get('queue'):
         choice = input('Use previous queue (resource) \'{}\' [Y]/n? '.format(state['queue']))
         if str(choice).strip().lower() in ('n', 'no'):
             ask_queues = True
+
     if ask_queues:
         print('Select the queue (resource) you request:')
         queues = None
         if not state.get('queue_include_tag') and not state.get('queue_excluded_tag'):
             # try default queue listing "interactive"
             queues = sorted([q.name for q in client.queues.get_all(system_tags=[str(system_tag)])])
 
@@ -418,14 +440,18 @@
             except (TypeError, ValueError, AssertionError):
                 pass
         state['queue'] = queues[int(choice)]
 
     print("\nInteractive session config:\n{}\n".format(
         json.dumps({k: v for k, v in state.items() if not str(k).startswith('__')}, indent=4, sort_keys=True)))
 
+    # no need to ask just return the value
+    if assume_yes:
+        return state
+
     choice = input('Launch interactive session [Y]/n? ')
     if str(choice).strip().lower() in ('n', 'no'):
         print('User aborted')
         exit(0)
 
     return state
 
@@ -448,16 +474,17 @@
 def load_state(state_file):
     # noinspection PyBroadException
     try:
         with open(state_file, 'rt') as f:
             state = json.load(f)
     except Exception:
         state = {}
-    # never reload --verbose state
+    # never reload --verbose and --yes states
     state.pop('verbose', None)
+    state.pop('yes', None)
     return state
 
 
 def clone_task(state, project_id=None):
     new_task = False
     if state.get('debugging_session'):
         print('Starting new debugging session to {}'.format(state.get('debugging_session')))
@@ -585,15 +612,15 @@
         print('.', end='', flush=True)
         if last_status is not None:
             sleep(2.)
             stopped_counter = (stopped_counter+1) if last_status == 'stopped' else 0
             if stopped_counter > 5:
                 break
         # noinspection PyProtectedMember
-        status, message = task._get_status()
+        status, message = task.get_status_message() if hasattr(task, "get_status_message") else task._get_status()
         status = str(status)
         if last_status != status or last_message != message:
             # noinspection PyProtectedMember
             print('Status [{}]{} {}'.format(status, ' - {}'.format(last_status) if last_status else '', message))
         last_status = status
         last_message = message
 
@@ -663,15 +690,15 @@
             task.get_status(), task.get_output_log_web_page()))
     print('\nRemote machine is ready')
 
     return task
 
 
 def start_ssh_tunnel(username, remote_address, ssh_port, ssh_password, local_remote_pair_list, debug=False):
-    print('Starting SSH tunnel')
+    print('Starting SSH tunnel to {}@{}, port {}'.format(username, remote_address, ssh_port))
     child = None
     args = ['-N', '-C',
             '{}@{}'.format(username, remote_address), '-p', '{}'.format(ssh_port),
             '-o', 'UserKnownHostsFile=/dev/null',
             '-o', 'Compression=yes',
             '-o', 'StrictHostKeyChecking=no',
             '-o', 'ServerAliveInterval=10',
@@ -715,15 +742,15 @@
                     ssh_password = input('Please enter password manually: ')
                     child.sendline(ssh_password)
                     child.expect([r'(?i)password:'], timeout=5)
                     print('{}Error: incorrect user input password'.format(fd.read() + '\n' if debug else ''))
                     raise ValueError('Incorrect password')
                 except pexpect.TIMEOUT:
                     pass
-    except Exception as ex:
+    except Exception:
         child.terminate(force=True)
         child = None
     print('\n')
     return child, ssh_password
 
 
 def monitor_ssh_tunnel(state, task):
@@ -889,14 +916,16 @@
 
 
 def setup_parser(parser):
     parser.add_argument('--version', action='store_true', default=None,
                         help='Display the clearml-session utility version')
     parser.add_argument('--attach', default=False, nargs='?',
                         help='Attach to running interactive session (default: previous session)')
+    parser.add_argument("--shutdown", "-S", default=None, const="", nargs="?",
+                        help="Shut down an active session (default: previous session)")
     parser.add_argument('--debugging-session', type=str, default=None,
                         help='Pass existing Task id (experiment), create a copy of the experiment on a remote machine, '
                              'and launch jupyter/ssh for interactive access. Example --debugging-session <task_id>')
     parser.add_argument('--queue', type=str, default=None,
                         help='Select the queue to launch the interactive session on (default: previously used queue)')
     parser.add_argument('--docker', type=str, default=None,
                         help='Select the docker image to use in the interactive session on '
@@ -964,14 +993,18 @@
                              '(default: `randomly-generated` or previously used one)')
     parser.add_argument('--username', type=str, default=None,
                         help='Advanced: Select ssh username for the interactive session '
                              '(default: `root` or previously used one)')
     parser.add_argument('--verbose', action='store_true', default=None,
                         help='Advanced: If set, print verbose progress information, '
                              'e.g. the remote machine setup process log')
+    parser.add_argument("--yes", "-y",
+                        action="store_true", default=False,
+                        help="Automatic yes to prompts; assume \"yes\" as answer "
+                             "to all prompts and run non-interactively",)
 
 
 def get_version():
     from .version import __version__
     return __version__
 
 
@@ -1003,16 +1036,28 @@
     state = load_state(state_file)
 
     if args.verbose:
         state['verbose'] = args.verbose
 
     client = APIClient()
 
+    if args.shutdown is not None:
+        task = _get_previous_session(
+            client, args, state, task_id=args.shutdown, verb="Shutting down",
+            question_verb="Shut down", ask_for_explicit_id=True
+        )
+        if not task:
+            print("No session to shut down, exiting")
+            return 1
+        task.mark_stopped()
+        print("Session #{} shut down, goodbye!".format(task.id))
+        return 0
+
     # get previous session, if it is running
-    task = _check_previous_session(client, args, state)
+    task = _get_previous_session(client, args, state, task_id=args.attach)
 
     if task:
         state['task_id'] = task.id
         save_state(state, state_file)
         if args.username:
             state['username'] = args.username
         if args.password:
@@ -1051,29 +1096,34 @@
     # launch ssh tunnel
     monitor_ssh_tunnel(state, task)
 
     # we are done
     print('Leaving interactive session')
 
 
-def _check_previous_session(client, args, state):
-    # now let's see if we have the requested Task
-    if args.attach:
-        task_id = args.attach
-        print('Checking previous session')
+def _get_previous_session(
+    client, args, state, task_id=None, verb="Connecting to", question_verb="Connect to", ask_for_explicit_id=False
+):
+    assume_yes = args.yes
+    if task_id:
+        print('Checking session #{}'.format(task_id))
         try:
             task = Task.get_task(task_id=task_id)
         except ValueError:
             task = None
         status = task.get_status() if task else None
         if status == 'in_progress':
             if not args.debugging_session or task.parent == args.debugging_session:
-                # only ask if we were not requested directly
-                print('Using active session id={}'.format(task_id))
-                return task
+                if assume_yes or not ask_for_explicit_id:
+                    print("{} active session id={}".format(verb, task_id))
+                    return task
+                choice = input("{} active session id={} [Y]/n? ".format(question_verb, task_id))
+                if str(choice).strip().lower() in ("y", "yes"):
+                    return task
+                return None
         raise ValueError('Could not connect to requested session id={} - status \'{}\''.format(
             task_id, status or 'Not Found'))
 
     # let's see if we have any other running sessions
     running_task_ids_created = _get_running_tasks(client, state.get('task_id'))
     if not running_task_ids_created:
         return None
@@ -1083,43 +1133,55 @@
         if not running_task_ids_created:
             print('No active task={} debugging session found'.format(args.debugging_session))
             return None
 
     # a single running session
     if len(running_task_ids_created) == 1:
         task_id = running_task_ids_created[0][0]
-        choice = input('Connect to active session id={} [Y]/n? '.format(task_id))
-        if str(choice).strip().lower() not in ('n', 'no'):
-            return Task.get_task(task_id=task_id)
+        if assume_yes:
+            print("{} active session {}".format(verb, task_id))
+        else:
+            choice = input("{} active session id={} [Y]/n? ".format(question_verb, task_id))
+            if str(choice).strip().lower() in ("y", "yes"):
+                return Task.get_task(task_id=task_id)
 
     # multiple sessions running
     print('Active sessions:')
     try:
         prev_task_id = state.get('task_id')
         default_i = next(i for i, (tid, _, _) in enumerate(running_task_ids_created) if prev_task_id == tid)
     except StopIteration:
         default_i = None
 
-    session_list = '\n'.join(
-        '{}{}] {} id={}'.format(i, '*' if i == default_i else '', dt.strftime("%Y-%m-%d %H:%M:%S"), tid)
-        for i, (tid, dt, _) in enumerate(running_task_ids_created))
-    while True:
-        try:
-            choice = input(session_list+'\nConnect to session [{}] or \'N\' to skip: '.format(
-                '0' if len(running_task_ids_created) <= 1 else '0-{}'.format(len(running_task_ids_created)-1)))
-            if choice.strip().lower().startswith('n'):
-                choice = None
-            elif default_i is not None and not choice.strip():
-                choice = default_i
-            else:
-                choice = int(choice)
-                assert 0 <= choice < len(running_task_ids_created)
-            break
-        except (TypeError, ValueError, AssertionError):
-            pass
+    session_list = "\n".join(
+        "{}{}] {} id={}".format(i, "*" if i == default_i else "", dt.strftime("%Y-%m-%d %H:%M:%S"), tid)
+        for i, (tid, dt, _) in enumerate(running_task_ids_created)
+    )
+    if assume_yes:
+        choice = 0
+    else:
+        while True:
+            try:
+                choice = input(
+                    session_list
+                    + "\n{} session [{}] or 'N' to skip: ".format(
+                        question_verb,
+                        "0" if len(running_task_ids_created) <= 1 else "0-{}".format(len(running_task_ids_created) - 1)
+                    )
+                )
+                if choice.strip().lower().startswith("n"):
+                    choice = None
+                elif default_i is not None and not choice.strip():
+                    choice = default_i
+                else:
+                    choice = int(choice)
+                    assert 0 <= choice < len(running_task_ids_created)
+                break
+            except (TypeError, ValueError, AssertionError):
+                pass
     if choice is None:
         return None
     return Task.get_task(task_id=running_task_ids_created[choice][0])
 
 
 def main():
     try:
```

## clearml_session/interactive_session_task.py

```diff
@@ -495,26 +495,26 @@
                 "CLEARML_API_ACCESS_KEY CLEARML_API_SECRET_KEY' >> /etc/ssh/sshd_config && "
                 'echo "export VISIBLE=now" >> /etc/profile && '
                 'echo "export PATH=$PATH" >> /etc/profile && '
                 'echo "ldconfig" 2>/dev/null >> /etc/profile && '
                 'echo "export CLEARML_CONFIG_FILE={trains_config_file}" >> /etc/profile'.format(
                     password=ssh_password,
                     port=port,
-                    trains_config_file=os.environ.get("CLEARML_CONFIG_FILE") or os.environ.get("CLEARML_CONFIG_FILE"),
+                    trains_config_file=os.environ.get("CLEARML_CONFIG_FILE") or os.environ.get("TRAINS_CONFIG_FILE"),
                 )
             )
             sshd_path = '/usr/sbin/sshd'
             ssh_config_path = '/etc/ssh/'
             custom_ssh_conf = None
         else:
             # check if sshd exists
             # noinspection PyBroadException
             try:
                 os.system('echo "export CLEARML_CONFIG_FILE={trains_config_file}" >> $HOME/.profile'.format(
-                    trains_config_file=os.environ.get("CLEARML_CONFIG_FILE") or os.environ.get("CLEARML_CONFIG_FILE"),
+                    trains_config_file=os.environ.get("CLEARML_CONFIG_FILE") or os.environ.get("TRAINS_CONFIG_FILE"),
                 ))
             except Exception:
                 print("warning failed setting ~/.profile")
 
             # check if shd is preinstalled
             # noinspection PyBroadException
             try:
```

## clearml_session/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.4.0'
+__version__ = '0.6.0'
```

## Comparing `clearml_session-0.4.0.dist-info/LICENSE` & `clearml_session-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `clearml_session-0.4.0.dist-info/METADATA` & `clearml_session-0.6.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearml-session
-Version: 0.4.0
+Version: 0.6.0
 Summary: clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 Home-page: https://github.com/allegroai/clearml-session
 Author: Allegroai
 Author-email: clearml@allegro.ai
 License: Apache License 2.0
 Keywords: clearml mlops devops trains development machine deep learning version control machine-learning machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN
@@ -37,15 +37,15 @@
 ## **`clearml-session` </br> CLI for launching JupyterLab / VSCode on a remote machine**
 
 
 [![GitHub license](https://img.shields.io/github/license/allegroai/clearml-session.svg)](https://img.shields.io/github/license/allegroai/clearml-session.svg)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/clearml-session.svg)](https://img.shields.io/pypi/pyversions/clearml-session.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/clearml-session.svg)](https://img.shields.io/pypi/v/clearml-session.svg)
 [![PyPI status](https://img.shields.io/pypi/status/clearml-session.svg)](https://pypi.python.org/pypi/clearml-session/)
-[![Slack Channel](https://img.shields.io/badge/slack-%23clearml--community-blueviolet?logo=slack)](https://join.slack.com/t/allegroai-trains/shared_invite/zt-c0t13pty-aVUZZW1TSSSg2vyIGVPBhg)
+[![Slack Channel](https://img.shields.io/badge/slack-%23clearml--community-blueviolet?logo=slack)](https://joinslack.clear.ml)
 
 
 </div>
 
 **`clearml-session`** is a utility for launching detachable remote interactive sessions (MacOS, Windows, Linux)
 
 ### tl;dr 
@@ -247,14 +247,15 @@
 ``` bash
 clearml-session --help
 ```
 
 ``` console
 clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 usage: clearml-session [-h] [--version] [--attach [ATTACH]]
+                       [--shutdown [SHUTDOWN]]
                        [--debugging-session DEBUGGING_SESSION] [--queue QUEUE]
                        [--docker DOCKER] [--docker-args DOCKER_ARGS]
                        [--public-ip [true/false]]
                        [--remote-ssh-port REMOTE_SSH_PORT]
                        [--vscode-server [true/false]]
                        [--vscode-version VSCODE_VERSION]
                        [--jupyter-lab [true/false]]
@@ -266,23 +267,26 @@
                        [--config-file CONFIG_FILE]
                        [--remote-gateway [REMOTE_GATEWAY]]
                        [--base-task-id BASE_TASK_ID] [--project PROJECT]
                        [--keepalive [true/false]]
                        [--queue-excluded-tag [QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]]]
                        [--queue-include-tag [QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]]]
                        [--skip-docker-network] [--password PASSWORD]
-                       [--username USERNAME] [--verbose]
+                       [--username USERNAME] [--verbose] [--yes]
 
 clearml-session - CLI for launching JupyterLab / VSCode on a remote machine
 
 optional arguments:
   -h, --help            show this help message and exit
   --version             Display the clearml-session utility version
   --attach [ATTACH]     Attach to running interactive session (default:
                         previous session)
+  --shutdown [SHUTDOWN], -S [SHUTDOWN]
+                        Shut down an active session (default: previous
+                        session)
   --debugging-session DEBUGGING_SESSION
                         Pass existing Task id (experiment), create a copy of
                         the experiment on a remote machine, and launch
                         jupyter/ssh for interactive access. Example
                         --debugging-session <task_id>
   --queue QUEUE         Select the queue to launch the interactive session on
                         (default: previously used queue)
@@ -359,12 +363,14 @@
   --password PASSWORD   Advanced: Select ssh password for the interactive
                         session (default: `randomly-generated` or previously
                         used one)
   --username USERNAME   Advanced: Select ssh username for the interactive
                         session (default: `root` or previously used one)
   --verbose             Advanced: If set, print verbose progress information,
                         e.g. the remote machine setup process log
+  --yes, -y             Automatic yes to prompts; assume "yes" as answer to
+                        all prompts and run non-interactively
 
 Notice! all arguments are stored as new defaults for the next session
 ```
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clearml-session Version: 0.4.0 Summary: clearml-
+Metadata-Version: 2.1 Name: clearml-session Version: 0.6.0 Summary: clearml-
 session - CLI for launching JupyterLab / VSCode on a remote machine Home-page:
 https://github.com/allegroai/clearml-session Author: Allegroai Author-email:
 clearml@allegro.ai License: Apache License 2.0 Keywords: clearml mlops devops
 trains development machine deep learning version control machine-learning
 machinelearning deeplearning deep-learning experiment-manager jupyter vscode
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
@@ -25,16 +25,15 @@
 allegroai/clearml-session.svg) [![PyPI pyversions](https://img.shields.io/pypi/
    pyversions/clearml-session.svg)](https://img.shields.io/pypi/pyversions/
 clearml-session.svg) [![PyPI version shields.io](https://img.shields.io/pypi/v/
   clearml-session.svg)](https://img.shields.io/pypi/v/clearml-session.svg) [!
 [PyPI status](https://img.shields.io/pypi/status/clearml-session.svg)](https://
        pypi.python.org/pypi/clearml-session/) [![Slack Channel](https://
 img.shields.io/badge/slack-%23clearml--community-blueviolet?logo=slack)](https:
-        //join.slack.com/t/allegroai-trains/shared_invite/zt-c0t13pty-
-                            aVUZZW1TSSSg2vyIGVPBhg)
+                             //joinslack.clear.ml)
 **`clearml-session`** is a utility for launching detachable remote interactive
 sessions (MacOS, Windows, Linux) ### tl;dr CLI to launch remote sessions for
 JupyterLab / VSCode-server / SSH, inside any docker image! ### What does it do?
 Starting a clearml (ob)session from your local machine triggers the following:
 - ClearML allocates a remote instance (GPU) from your dedicated pool - On the
 allocated instance it will spin **jupyter-lab** + **vscode server** + **SSH**
 access for interactive usage (i.e., development) - ClearML will start
@@ -140,52 +139,54 @@
 allow you interactively execute and debug the experiment, on the allocated
 remote machine. In the `clearml` web UI, find the experiment (Task) you wish to
 debug. Click on the ID button next to the Task name, and copy the unique ID.
 ``` bash clearml-session --debugging-session  ``` Click on the JupyterLab/
 VSCode link, or connect directly to the SSH session ## CLI options ``` bash
 clearml-session --help ``` ``` console clearml-session - CLI for launching
 JupyterLab / VSCode on a remote machine usage: clearml-session [-h] [--version]
-[--attach [ATTACH]] [--debugging-session DEBUGGING_SESSION] [--queue QUEUE] [--
-docker DOCKER] [--docker-args DOCKER_ARGS] [--public-ip [true/false]] [--
-remote-ssh-port REMOTE_SSH_PORT] [--vscode-server [true/false]] [--vscode-
-version VSCODE_VERSION] [--jupyter-lab [true/false]] [--git-credentials [true/
-false]] [--user-folder USER_FOLDER] [--packages [PACKAGES [PACKAGES ...]]] [--
-requirements REQUIREMENTS] [--init-script [INIT_SCRIPT]] [--config-file
-CONFIG_FILE] [--remote-gateway [REMOTE_GATEWAY]] [--base-task-id BASE_TASK_ID]
-[--project PROJECT] [--keepalive [true/false]] [--queue-excluded-tag
-[QUEUE_EXCLUDED_TAG [QUEUE_EXCLUDED_TAG ...]]] [--queue-include-tag
-[QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]]] [--skip-docker-network] [--
-password PASSWORD] [--username USERNAME] [--verbose] clearml-session - CLI for
-launching JupyterLab / VSCode on a remote machine optional arguments: -h, --
-help show this help message and exit --version Display the clearml-session
-utility version --attach [ATTACH] Attach to running interactive session
-(default: previous session) --debugging-session DEBUGGING_SESSION Pass existing
-Task id (experiment), create a copy of the experiment on a remote machine, and
-launch jupyter/ssh for interactive access. Example --debugging-session  --queue
-QUEUE Select the queue to launch the interactive session on (default:
-previously used queue) --docker DOCKER Select the docker image to use in the
-interactive session on (default: previously used docker image or `nvidia/cuda:
-10.1-runtime-ubuntu18.04`) --docker-args DOCKER_ARGS Add additional arguments
-for the docker image to use in the interactive session on (default: previously
-used docker-args) --public-ip [true/false] If True register the public IP of
-the remote machine. Set if running on the cloud. Default: false (use for local
-/ on-premises) --remote-ssh-port REMOTE_SSH_PORT Set the remote ssh server
-port, running on the agent`s machine. (default: 10022) --vscode-server [true/
-false] Install vscode server (code-server) on interactive session (default:
-true) --vscode-version VSCODE_VERSION Set vscode server (code-server) version,
-as well as vscode python extension version  (example: "3.7.4:
-2020.10.332292344") --jupyter-lab [true/false] Install Jupyter-Lab on
-interactive session (default: true) --git-credentials [true/false] If true,
-local .git-credentials file is sent to the interactive session. (default:
-false) --user-folder USER_FOLDER Advanced: Set the remote base folder (default:
-~/) --packages [PACKAGES [PACKAGES ...]] Additional packages to add, supports
-version numbers (default: previously added packages). examples: --packages
-torch==1.7 tqdm --requirements REQUIREMENTS Specify requirements.txt file to
-install when setting the interactive session. Requirements file is read and
-stored in `packages` section as default for the next sessions. Can be
+[--attach [ATTACH]] [--shutdown [SHUTDOWN]] [--debugging-session
+DEBUGGING_SESSION] [--queue QUEUE] [--docker DOCKER] [--docker-args
+DOCKER_ARGS] [--public-ip [true/false]] [--remote-ssh-port REMOTE_SSH_PORT] [--
+vscode-server [true/false]] [--vscode-version VSCODE_VERSION] [--jupyter-lab
+[true/false]] [--git-credentials [true/false]] [--user-folder USER_FOLDER] [--
+packages [PACKAGES [PACKAGES ...]]] [--requirements REQUIREMENTS] [--init-
+script [INIT_SCRIPT]] [--config-file CONFIG_FILE] [--remote-gateway
+[REMOTE_GATEWAY]] [--base-task-id BASE_TASK_ID] [--project PROJECT] [--
+keepalive [true/false]] [--queue-excluded-tag [QUEUE_EXCLUDED_TAG
+[QUEUE_EXCLUDED_TAG ...]]] [--queue-include-tag [QUEUE_INCLUDE_TAG
+[QUEUE_INCLUDE_TAG ...]]] [--skip-docker-network] [--password PASSWORD] [--
+username USERNAME] [--verbose] [--yes] clearml-session - CLI for launching
+JupyterLab / VSCode on a remote machine optional arguments: -h, --help show
+this help message and exit --version Display the clearml-session utility
+version --attach [ATTACH] Attach to running interactive session (default:
+previous session) --shutdown [SHUTDOWN], -S [SHUTDOWN] Shut down an active
+session (default: previous session) --debugging-session DEBUGGING_SESSION Pass
+existing Task id (experiment), create a copy of the experiment on a remote
+machine, and launch jupyter/ssh for interactive access. Example --debugging-
+session  --queue QUEUE Select the queue to launch the interactive session on
+(default: previously used queue) --docker DOCKER Select the docker image to use
+in the interactive session on (default: previously used docker image or
+`nvidia/cuda:10.1-runtime-ubuntu18.04`) --docker-args DOCKER_ARGS Add
+additional arguments for the docker image to use in the interactive session on
+(default: previously used docker-args) --public-ip [true/false] If True
+register the public IP of the remote machine. Set if running on the cloud.
+Default: false (use for local / on-premises) --remote-ssh-port REMOTE_SSH_PORT
+Set the remote ssh server port, running on the agent`s machine. (default:
+10022) --vscode-server [true/false] Install vscode server (code-server) on
+interactive session (default: true) --vscode-version VSCODE_VERSION Set vscode
+server (code-server) version, as well as vscode python extension version
+(example: "3.7.4:2020.10.332292344") --jupyter-lab [true/false] Install
+Jupyter-Lab on interactive session (default: true) --git-credentials [true/
+false] If true, local .git-credentials file is sent to the interactive session.
+(default: false) --user-folder USER_FOLDER Advanced: Set the remote base folder
+(default: ~/) --packages [PACKAGES [PACKAGES ...]] Additional packages to add,
+supports version numbers (default: previously added packages). examples: --
+packages torch==1.7 tqdm --requirements REQUIREMENTS Specify requirements.txt
+file to install when setting the interactive session. Requirements file is read
+and stored in `packages` section as default for the next sessions. Can be
 overridden by calling `--packages` --init-script [INIT_SCRIPT] Specify BASH
 init script file to be executed when setting the interactive session. Script
 content is read and stored as default script for the next sessions. To clear
 the init-script do not pass a file --config-file CONFIG_FILE Advanced: Change
 the configuration file used to store the previous state (default:
 ~/.clearml_session.json) --remote-gateway [REMOTE_GATEWAY] Advanced: Specify
 gateway ip/address:port to be passed to interactive session (for use with k8s
@@ -200,9 +201,11 @@
 [QUEUE_INCLUDE_TAG [QUEUE_INCLUDE_TAG ...]] Advanced: Only include queues with
 this specific tag from the selection --skip-docker-network Advanced: If set, `-
 -network host` is **not** passed to docker (assumes k8s network ingestion)
 (default: false) --password PASSWORD Advanced: Select ssh password for the
 interactive session (default: `randomly-generated` or previously used one) --
 username USERNAME Advanced: Select ssh username for the interactive session
 (default: `root` or previously used one) --verbose Advanced: If set, print
-verbose progress information, e.g. the remote machine setup process log Notice!
-all arguments are stored as new defaults for the next session ```
+verbose progress information, e.g. the remote machine setup process log --yes,
+-y Automatic yes to prompts; assume "yes" as answer to all prompts and run non-
+interactively Notice! all arguments are stored as new defaults for the next
+session ```
```

## Comparing `clearml_session-0.4.0.dist-info/RECORD` & `clearml_session-0.6.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 clearml_session/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-clearml_session/__main__.py,sha256=HS4NamSbK4lB7CxxcqdSDcQp8rUMQ8NudktfG28cDv0,49931
-clearml_session/interactive_session_task.py,sha256=5g-ijVSXeEdOcczK1LZvyu0ik3rHl6w_ksRyRi6qI28,37842
+clearml_session/__main__.py,sha256=REQjq07hpfk4dXkXq9RbxCYvBPq6ECoinI4SrUc68iM,52386
+clearml_session/interactive_session_task.py,sha256=lICmiXT41SIaZYUOGR2EEN5IMkh03ulgCBT8Q9OYpiA,37840
 clearml_session/single_thread_proxy.py,sha256=mOTRC0rca62C0EqhRkeXYEWbmDYwxBlE5_j_bMEb0nc,4781
 clearml_session/tcp_proxy.py,sha256=Oz6DNlbHtNRfhtSn3OYt_zNiasWZ_whHCk9KHIJr-2g,15948
-clearml_session/version.py,sha256=2eiWQI55fd-roDdkt4Hvl9WzrTJ4xQo33VzFud6D03U,22
-clearml_session-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-clearml_session-0.4.0.dist-info/METADATA,sha256=TUCfk3j7qs0z8XRKTpolgtn-65NI3kwemghjYo1UQpY,17871
-clearml_session-0.4.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-clearml_session-0.4.0.dist-info/entry_points.txt,sha256=-KMe29157dlUO8Vd4z5kYkLHS2nInJZj52SHA0E9SsU,67
-clearml_session-0.4.0.dist-info/top_level.txt,sha256=Gt2u68qTEiXZqnHSKJR6CRlY799su4rlKW7Y3tM2RzY,16
-clearml_session-0.4.0.dist-info/RECORD,,
+clearml_session/version.py,sha256=CBY3jsC-9HCm7eZ6CKD-sYLCejqOJ1pYWPQM4LGIXcI,22
+clearml_session-0.6.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+clearml_session-0.6.0.dist-info/METADATA,sha256=NvAPFO2QNmA7fpDg1LyyyCNWgSIHG6rM65vHwPIxaQY,18143
+clearml_session-0.6.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+clearml_session-0.6.0.dist-info/entry_points.txt,sha256=-KMe29157dlUO8Vd4z5kYkLHS2nInJZj52SHA0E9SsU,67
+clearml_session-0.6.0.dist-info/top_level.txt,sha256=Gt2u68qTEiXZqnHSKJR6CRlY799su4rlKW7Y3tM2RzY,16
+clearml_session-0.6.0.dist-info/RECORD,,
```

