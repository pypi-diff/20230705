# Comparing `tmp/kaiju_tasks-2.1.3-py3-none-any.whl.zip` & `tmp/kaiju_tasks-2.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,14 @@
-Zip file size: 18291 bytes, number of entries: 15
--rw-r--r--  2.0 unx      131 b- defN 23-Jul-02 13:03 kaiju_tasks/__init__.py
--rw-r--r--  2.0 unx    37494 b- defN 23-Jul-02 13:03 kaiju_tasks/services.py
--rw-r--r--  2.0 unx     4360 b- defN 23-Jul-02 13:03 kaiju_tasks/types.py
--rw-r--r--  2.0 unx       38 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/__init__.py
--rw-r--r--  2.0 unx     2011 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/models.py
--rw-r--r--  2.0 unx     4272 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/service.py
--rw-r--r--  2.0 unx      350 b- defN 23-Jul-02 13:03 kaiju_tasks/tasks_gui/validators.py
--rw-r--r--  2.0 unx       42 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/__init__.py
--rw-r--r--  2.0 unx     2058 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/fixtures.py
--rw-r--r--  2.0 unx    12224 b- defN 23-Jul-02 13:03 kaiju_tasks/tests/test_tasks.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2944 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-02 13:03 kaiju_tasks-2.1.3.dist-info/RECORD
-15 files, 67895 bytes uncompressed, 16199 bytes compressed:  76.1%
+Zip file size: 17446 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      150 b- defN 23-Jul-05 12:54 kaiju_tasks/__init__.py
+-rw-r--r--  2.0 unx     5345 b- defN 23-Jul-05 12:54 kaiju_tasks/gui.py
+-rw-r--r--  2.0 unx    37417 b- defN 23-Jul-05 12:54 kaiju_tasks/services.py
+-rw-r--r--  2.0 unx     4300 b- defN 23-Jul-05 12:54 kaiju_tasks/types.py
+-rw-r--r--  2.0 unx       42 b- defN 23-Jul-05 12:54 kaiju_tasks/tests/__init__.py
+-rw-r--r--  2.0 unx     2272 b- defN 23-Jul-05 12:54 kaiju_tasks/tests/fixtures.py
+-rw-r--r--  2.0 unx    12902 b- defN 23-Jul-05 12:54 kaiju_tasks/tests/test_tasks.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jul-05 12:54 kaiju_tasks-2.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3206 b- defN 23-Jul-05 12:54 kaiju_tasks-2.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-05 12:54 kaiju_tasks-2.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-05 12:54 kaiju_tasks-2.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-05 12:54 kaiju_tasks-2.1.4.dist-info/RECORD
+12 files, 67324 bytes uncompressed, 15808 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -1,46 +1,37 @@
 Filename: kaiju_tasks/__init__.py
 Comment: 
 
-Filename: kaiju_tasks/services.py
-Comment: 
-
-Filename: kaiju_tasks/types.py
-Comment: 
-
-Filename: kaiju_tasks/tasks_gui/__init__.py
-Comment: 
-
-Filename: kaiju_tasks/tasks_gui/models.py
+Filename: kaiju_tasks/gui.py
 Comment: 
 
-Filename: kaiju_tasks/tasks_gui/service.py
+Filename: kaiju_tasks/services.py
 Comment: 
 
-Filename: kaiju_tasks/tasks_gui/validators.py
+Filename: kaiju_tasks/types.py
 Comment: 
 
 Filename: kaiju_tasks/tests/__init__.py
 Comment: 
 
 Filename: kaiju_tasks/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_tasks/tests/test_tasks.py
 Comment: 
 
-Filename: kaiju_tasks-2.1.3.dist-info/LICENSE
+Filename: kaiju_tasks-2.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_tasks-2.1.3.dist-info/METADATA
+Filename: kaiju_tasks-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_tasks-2.1.3.dist-info/WHEEL
+Filename: kaiju_tasks-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_tasks-2.1.3.dist-info/top_level.txt
+Filename: kaiju_tasks-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_tasks-2.1.3.dist-info/RECORD
+Filename: kaiju_tasks-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_tasks/__init__.py

```diff
@@ -1,6 +1,7 @@
 from .types import *
 from .services import *
+from .gui import *
 
-__version__ = '2.1.3'
+__version__ = '2.1.4'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_tasks/services.py

```diff
@@ -36,27 +36,26 @@
 
     service_name = 'tasks'
     table = sa.Table(
         'tasks',
         sa.MetaData(),
         sa.Column('id', sa_pg.TEXT, primary_key=True),
         # executor instructions
-        sa.Column('app', sa_pg.TEXT, nullable=False),
+        sa.Column('app_name', sa_pg.TEXT, nullable=False),
         sa.Column('commands', sa_pg.JSONB, nullable=False),
         sa.Column('kws', sa_pg.JSONB, nullable=False),
         # manager instructions
         sa.Column('enabled', sa_pg.BOOLEAN, nullable=False),
         sa.Column('cron', sa_pg.TEXT, nullable=True),
         sa.Column('max_exec_timeout', sa_pg.INTEGER, nullable=False),
         sa.Column('max_retries', sa_pg.INTEGER, nullable=False),
         sa.Column('restart_policy', sa_pg.TEXT, nullable=False),
         sa.Column('notify', sa_pg.BOOLEAN, nullable=False),
         sa.Column('next_task', sa.ForeignKey('tasks.id', ondelete='SET NULL'), nullable=True),
         # meta
-        sa.Column('name', sa_pg.TEXT, nullable=True),
         sa.Column('description', sa_pg.TEXT, nullable=True),
         sa.Column('meta', sa_pg.JSONB, nullable=False, default={}),
         # managed
         sa.Column('status', sa_pg.TEXT, nullable=False),
         sa.Column('result', sa_pg.JSONB, nullable=False),
         sa.Column('stage', sa_pg.INTEGER, nullable=False),
         sa.Column('stages', sa_pg.INTEGER, nullable=False),
@@ -87,24 +86,23 @@
     _task_command = j.Object(
         {'id': j.Integer(), 'method': j.String(), 'params': j.Object()}, additionalProperties=False, required=['method']
     )
 
     _task_validator = j.Object(
         {
             'id': j.String(minLength=1),
-            'app': j.String(),
+            'app_name': j.String(),
             'commands': j.Array(_task_command, minItems=1, maxItems=Limit.MAX_STAGES.value),
             'kws': j.Object(),
             'cron': j.String(),
             'max_exec_timeout': j.Integer(minimum=Limit.MIN_T.value, maximum=Limit.MAX_T.value),
             'max_retries': j.Integer(minimum=0, maximum=Limit.MAX_RETRIES.value),
             'restart_policy': j.Enumerated(enum=[RestartPolicy.CURRENT.value, RestartPolicy.FIRST.value]),
             'next_task': j.String(minLength=1),
             'notify': j.Boolean(),
-            'name': j.String(),
             'description': j.String(),
             'meta': j.Object(),
             'enabled': j.Boolean(default=True),
         },
         additionalProperties=False,
         required=['commands'],
     )
@@ -154,21 +152,20 @@
         return bool(restarted)
 
     def prepare_insert_data(self, data: dict):
         """Prepare task."""
         data = self._validate_data(data)
         task = Task(
             id=data.get('id', str(uuid4()).replace('-', '')),
-            app=data.get('app', self.app.name),
+            app_name=data.get('app', self.app.name),
             commands=data['commands'],
             kws=data.get('kws', {}),
             cron=data.get('cron'),
             max_exec_timeout=data.get('max_exec_timeout', Limit.DEFAULT_T.value),
             max_retries=data.get('max_retries', 0),
-            name=data.get('name'),
             description=data.get('description'),
             meta=data.get('meta', {}),
             notify=data.get('notify', False),
             restart_policy=data.get('restart_policy', RestartPolicy.CURRENT.value),
             enabled=data.get('enabled', True),
             status=TaskStatus.IDLE.value,
             stage=0,
@@ -280,15 +277,15 @@
 
     service_name = 'taskman'
     table = TaskService.table
 
     def __init__(
         self,
         app,
-        stream_client: StreamRPCClient,
+        stream_client: StreamRPCClient = None,
         database_service: DatabaseService = None,
         redis_transport: RedisTransportService = None,
         notification_service: NotificationService = None,
         scheduler_service: Scheduler = None,
         executor_topic: str = Topic.EXECUTOR,
         refresh_rate: int = 1,
         suspended_task_lifetime_hours: int = 24,
@@ -573,15 +570,15 @@
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
                 self.table.c.kws,
                 self.table.c.stage,
                 self.table.c.exec_deadline,
-                self.table.c.app,
+                self.table.c.app_name,
                 self.table.c.result,
                 self.table.c.job_id,
             )
         )
         async with self._db.begin() as conn:
             queued_tasks = await conn.execute(sql)
             queued_tasks = [r._asdict() for r in queued_tasks.all()]  # noqa
@@ -640,15 +637,15 @@
             )
             .returning(
                 self.table.c.id,
                 self.table.c.commands,
                 self.table.c.kws,
                 self.table.c.stage,
                 self.table.c.exec_deadline,
-                self.table.c.app,
+                self.table.c.app_name,
                 self.table.c.result,
                 self.table.c.job_id,
             )
         )
         async with self._db.begin() as conn:
             queued_tasks = await conn.execute(sql)
             queued_tasks = [r._asdict() for r in queued_tasks.all()]  # noqa
@@ -722,29 +719,29 @@
                         result=task['result'][:stage],
                         exec_deadline=task['exec_deadline'],
                         stage=stage,
                         stages=len(task['commands']),
                         job_id=task['job_id'],
                     )
                 },
-                app=task['app'],
+                app=task['app_name'],
                 topic=self._executor_topic,
             )
 
 
 class TaskExecutor(ContextableService, PublicInterface):
     """Task executor receives and processes tasks from a manager."""
 
     service_name = 'executor'
     manager_service_name = TaskManager.service_name
 
     def __init__(
         self,
         app,
-        stream_client: StreamRPCClient,
+        stream_client: StreamRPCClient = None,
         manager_app: str = None,
         manager_topic: str = Topic.MANAGER,
         rpc_service: JSONRPCServer = None,
         scheduler: Scheduler = None,
         logger=None,
     ):
         """Initialize.
```

## kaiju_tasks/types.py

```diff
@@ -47,15 +47,15 @@
 class Task(TypedDict, total=False):
     """Task data."""
 
     id: str  #: generated / user-defined unique identifier
 
     # executor instructions
 
-    app: str  #: executor type (app.name)
+    app_name: str  #: executor type (app.name)
     commands: List[Union[TaskCommand, RPCRequest, List[TaskCommand], List[RPCRequest]]]  #: sequential list of stages
     kws: dict  #: additional kws template arguments
 
     # manager instructions
 
     enabled: bool  #: inactive tasks are not processed
     cron: str  #: cron instructions for periodic tasks
@@ -63,15 +63,14 @@
     max_retries: int  #: max retries for a failed task (0 for no retries)
     restart_policy: str  #: how the task will be restarted
     notify: bool  #: notify user about status changes
     next_task: Optional[str]  #: next task to run after finishing of this one
 
     # meta
 
-    name: Optional[str]  #: task short name, completely optional
     description: Optional[str]  #: task long description, completely optional
     meta: dict  #: task metadata, unused by the services
 
     # managed params
 
     status: str  #: current task status
     result: list  #: task execution result, a list of stage returns
```

## kaiju_tasks/tests/fixtures.py

```diff
@@ -1,12 +1,13 @@
 import pytest  # noqa: pycharm
 
 from kaiju_tasks.services import *
+from kaiju_tasks.gui import TaskGUI
 
-__all__ = ['task_service', 'notification_service', 'mock_task_executor', 'task_manager']
+__all__ = ['task_service', 'notification_service', 'mock_task_executor', 'task_manager', 'task_gui']
 
 
 @pytest.fixture
 def task_service(app, rpc, database_service) -> TaskService:
     rpc._use_annotation_parser = False
     service = TaskService(app=app, database_service=database_service)
     app.services.add_service(service)
@@ -60,7 +61,14 @@
         stream_client=redis_client,
         scheduler_service=scheduler,
         database_service=database_service,
         notification_service=notification_service,
     )
     app.services.add_service(service)
     return service
+
+
+@pytest.fixture
+def task_gui(app, task_service):
+    service = TaskGUI(app=app, task_service=task_service)
+    app.services.add_service(service)
+    return service
```

## kaiju_tasks/tests/test_tasks.py

```diff
@@ -7,16 +7,17 @@
 import pytest  # noqa: pycharm
 import pytest_asyncio
 
 from kaiju_db.tests.test_db import TestSQLService
 
 from kaiju_tasks.types import Task, Notification, TaskStatus, ExecutorTask, TaskCommand, RestartPolicy
 from kaiju_tasks.services import TaskService, NotificationService, TaskExecutor
+from kaiju_tasks.gui import TaskGUI
 
-__all__ = ['TestTaskService', 'TestNotificationService', 'TestTaskExecutor', 'TestTaskManager']
+__all__ = ['TestTaskService', 'TestNotificationService', 'TestTaskExecutor', 'TestTaskManager', 'TaskGUI']
 
 
 @pytest.mark.asyncio
 @pytest.mark.docker
 class TestTaskService(TestSQLService):
     """Test task service."""
 
@@ -281,7 +282,26 @@
         await task_service.update(task['id'], {'executor_id': new_executor, 'status': TaskStatus.EXECUTED.value})
         await _service.suspend_executor(new_executor)
         active = await _service.list_active_executors()
         assert str(new_executor).encode('utf-8') not in active
         task = await task_service.get(task['id'])
         assert task['status'] == TaskStatus.SUSPENDED.value
         assert task['executor_id'] is None
+
+
+@pytest.mark.asyncio
+@pytest.mark.docker
+class TestTaskGUI:
+    @pytest_asyncio.fixture
+    async def _service(self, app, rpc, task_gui):
+        rpc._enable_permissions = False
+        async with app.services:
+            yield task_gui
+
+    async def test_gui(self, task_service, _service: TaskGUI):
+        task = next(TestTaskService.get_rows(1))
+        await task_service.create(task)
+        await _service.update(task['id'], description='test test test')
+        data = await _service.get(task['id'])
+        _service.logger.debug(data)
+        data = await _service.grid(locale=None)
+        _service.logger.debug(data)
```

## Comparing `kaiju_tasks-2.1.3.dist-info/LICENSE` & `kaiju_tasks-2.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_tasks-2.1.3.dist-info/METADATA` & `kaiju_tasks-2.1.4.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-tasks
-Version: 2.1.3
+Version: 2.1.4
 Summary: Service and user task management
 Home-page: https://gitlab.com/kaiju-python/kaiju-tasks
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: croniter (>=1.4.1)
 Requires-Dist: kaiju-tools (<3,>=2)
 Requires-Dist: kaiju-db (<3,>=2)
 Requires-Dist: kaiju-redis (<3,>=2)
+Requires-Dist: kaiju-model (<3,>=2)
 Provides-Extra: dev
 Requires-Dist: bump2version (>=1.0) ; extra == 'dev'
 Requires-Dist: pyroma (>=4.1) ; extra == 'dev'
 Requires-Dist: bandit (>=1.7) ; extra == 'dev'
 Requires-Dist: black (>=22.12) ; extra == 'dev'
 Requires-Dist: flake8 (>=6.0) ; extra == 'dev'
 Requires-Dist: pyproject-flake8 ; extra == 'dev'
@@ -34,19 +35,24 @@
 Requires-Dist: setup-cfg-fmt (>=2.2) ; extra == 'dev'
 Requires-Dist: restructuredtext-lint (>=1.4) ; extra == 'dev'
 Requires-Dist: tox (>=3.28) ; extra == 'dev'
 Requires-Dist: tox-pyenv (>=1.1) ; extra == 'dev'
 Requires-Dist: pip-tools (>=6.13) ; extra == 'dev'
 Requires-Dist: towncrier (>=23.6) ; extra == 'dev'
 Requires-Dist: pyupgrade (>=3.4) ; extra == 'dev'
+Provides-Extra: docs
+Requires-Dist: sphinx ; extra == 'docs'
+Requires-Dist: python-docs-theme ; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: pytest (>=7.2) ; extra == 'test'
-Requires-Dist: pytest-asyncio (>=0.20) ; extra == 'test'
-Requires-Dist: docker (>=6.0) ; extra == 'test'
+Requires-Dist: pytest (>=7.4) ; extra == 'test'
+Requires-Dist: pytest-asyncio (>=0.21) ; extra == 'test'
+Requires-Dist: docker (>=6.1.3) ; extra == 'test'
 Requires-Dist: pytest-timeout (>=2.1) ; extra == 'test'
+Requires-Dist: pytest-aiohttp (>=1.0.4) ; extra == 'test'
+Requires-Dist: pytest-cov (>=4.1.0) ; extra == 'test'
 
 
 .. image:: https://badge.fury.io/py/kaiju-tasks.svg
     :target: https://pypi.org/project/kaiju-tasks
     :alt: Latest package version
 
 .. image:: https://readthedocs.org/projects/kaiju-tasks/badge/?version=latest
```

## Comparing `kaiju_tasks-2.1.3.dist-info/RECORD` & `kaiju_tasks-2.1.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-kaiju_tasks/__init__.py,sha256=27X9yp9XJDz9_Cm77AJ7szUnYjKOJghF8AHKDNpRYvs,131
-kaiju_tasks/services.py,sha256=UY3LvImaGK222lNdySKyJUo8D7lzJjqAFvkUSCvj--Q,37494
-kaiju_tasks/types.py,sha256=tp6fm6GJv8B5B6YhhiiZIbf00ahIBHUqaZNEQJFXEuw,4360
-kaiju_tasks/tasks_gui/__init__.py,sha256=_gDfM5r8uxCvydv3NOUN21imwJW_NW9R16UXWExQAE8,38
-kaiju_tasks/tasks_gui/models.py,sha256=iXqYnYYh8TJ7jkVxyEmMeykfpmoNfEfEERW-1jwzjsk,2011
-kaiju_tasks/tasks_gui/service.py,sha256=_qCURg-h6I9OI5uZdTGYCzJglXPXomcqAt6D7ODLRmU,4272
-kaiju_tasks/tasks_gui/validators.py,sha256=QybfHwKMWJq9AcGlXO7F5fuEGLssjHN2jcAV0UI6FPc,350
+kaiju_tasks/__init__.py,sha256=nH-UrtSfV9YuKVECOXZMDvOl9auX5iKJWhNYal8HQLg,150
+kaiju_tasks/gui.py,sha256=6QrPRCuVl_Axq6CacTY4S6IUBpXLBMhu08MRZsWsTvQ,5345
+kaiju_tasks/services.py,sha256=2pPLJ5Ur1I6a-B42KVwz6cvVPwndqglhGOBobUWitiY,37417
+kaiju_tasks/types.py,sha256=88ek-sF7tmV7frPxb-ZwMDA01P_qrXV1Cp5PQ7DANQ4,4300
 kaiju_tasks/tests/__init__.py,sha256=WlPruePOcaMi5ikqn6GheE1Z-zYcysb9M1dj6SteWGY,42
-kaiju_tasks/tests/fixtures.py,sha256=1WRWnb5aCklCpRo0iqp1rquZSB8qgKBULv5MhaO2rck,2058
-kaiju_tasks/tests/test_tasks.py,sha256=YvmLscWAwko7eQ2Jw4vXTrO7SkefFu_P8eOEMNT-lkk,12224
-kaiju_tasks-2.1.3.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
-kaiju_tasks-2.1.3.dist-info/METADATA,sha256=kWbYaN2uD1LzooXo7bX4T3LocT4vvz-tsoIH4_2fxwY,2944
-kaiju_tasks-2.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-kaiju_tasks-2.1.3.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
-kaiju_tasks-2.1.3.dist-info/RECORD,,
+kaiju_tasks/tests/fixtures.py,sha256=7hLaDyE3Sjibnt5zZ9YNNJ2586541NRPC4Y3qIQzI2s,2272
+kaiju_tasks/tests/test_tasks.py,sha256=7xJh_Pmbap-Z8pOW0o6DkMtotFLdYsyJIzqYp21LS0U,12902
+kaiju_tasks-2.1.4.dist-info/LICENSE,sha256=XIlN2qA8UqpBDA-PteoYP4hTU0qBW0G9PRB__khO2zc,610
+kaiju_tasks-2.1.4.dist-info/METADATA,sha256=vUhucDdBF7vO92N-PvkYtHrlrYQBx6-vvRAJwicZqO8,3206
+kaiju_tasks-2.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+kaiju_tasks-2.1.4.dist-info/top_level.txt,sha256=QyLogqOVVajJlalq6RfikGx5VGn_lLeTANJEsfZZlM0,12
+kaiju_tasks-2.1.4.dist-info/RECORD,,
```

