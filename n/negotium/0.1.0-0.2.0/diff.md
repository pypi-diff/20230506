# Comparing `tmp/negotium-0.1.0.tar.gz` & `tmp/negotium-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negotium-0.1.0.tar", last modified: Thu May  4 11:15:38 2023, max compression
+gzip compressed data, was "negotium-0.2.0.tar", last modified: Sat May  6 00:31:21 2023, max compression
```

## Comparing `negotium-0.1.0.tar` & `negotium-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       51 2023-05-03 19:58:57.000000 negotium-0.1.0/.gitignore
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2463 2023-05-04 11:15:38.324810 negotium-0.1.0/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2296 2023-05-04 11:09:10.000000 negotium-0.1.0/README.md
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.320809 negotium-0.1.0/negotium/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.1.0/negotium/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3466 2023-05-04 10:25:21.000000 negotium-0.1.0/negotium/base.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium/mq/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.1.0/negotium/mq/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5472 2023-05-04 10:41:07.000000 negotium-0.1.0/negotium/mq/consumer.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1569 2023-05-03 21:22:40.000000 negotium-0.1.0/negotium/mq/publisher.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      510 2023-05-03 18:50:00.000000 negotium-0.1.0/negotium/settings.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      490 2023-05-03 12:19:38.000000 negotium-0.1.0/negotium/task.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium/utils/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.1.0/negotium/utils/__init__.py
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.1.0/negotium/utils/logger.py
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/negotium.egg-info/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2463 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/PKG-INFO
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      430 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/SOURCES.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/dependency_links.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      100 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/requires.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-04 11:15:38.000000 negotium-0.1.0/negotium.egg-info/top_level.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      405 2023-05-04 11:15:16.000000 negotium-0.1.0/pyproject.toml
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-03 19:02:07.000000 negotium-0.1.0/requirements.txt
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-04 11:15:38.324810 negotium-0.1.0/setup.cfg
-drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-04 11:15:38.324810 negotium-0.1.0/tests/
--rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.1.0/tests/__init__.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.970488 negotium-0.2.0/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       57 2023-05-06 00:17:07.000000 negotium-0.2.0/.gitignore
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3771 2023-05-06 00:31:21.970488 negotium-0.2.0/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3604 2023-05-06 00:30:37.000000 negotium-0.2.0/README.md
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.962485 negotium-0.2.0/negotium/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       27 2023-05-03 08:19:32.000000 negotium-0.2.0/negotium/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3603 2023-05-05 23:38:22.000000 negotium-0.2.0/negotium/base.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/mq/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:09:24.000000 negotium-0.2.0/negotium/mq/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     5985 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/mq/consumer.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     2947 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/mq/publisher.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1838 2023-05-06 00:25:28.000000 negotium-0.2.0/negotium/mq/trackers.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/schedules/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       29 2023-05-05 23:42:01.000000 negotium-0.2.0/negotium/schedules/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     1992 2023-05-06 00:23:30.000000 negotium-0.2.0/negotium/schedules/crontab.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      616 2023-05-06 00:27:04.000000 negotium-0.2.0/negotium/settings.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      867 2023-05-05 23:47:12.000000 negotium-0.2.0/negotium/task.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium/utils/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 08:08:36.000000 negotium-0.2.0/negotium/utils/__init__.py
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      687 2023-05-03 08:18:47.000000 negotium-0.2.0/negotium/utils/logger.py
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.966486 negotium-0.2.0/negotium.egg-info/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)     3771 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/PKG-INFO
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      515 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/SOURCES.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        1 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/dependency_links.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      117 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/requires.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        9 2023-05-06 00:31:21.000000 negotium-0.2.0/negotium.egg-info/top_level.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      429 2023-05-06 00:30:49.000000 negotium-0.2.0/pyproject.toml
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)      455 2023-05-06 00:28:29.000000 negotium-0.2.0/requirements.txt
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)       38 2023-05-06 00:31:21.970488 negotium-0.2.0/setup.cfg
+drwxrwxr-x   0 deestarks  (1000) deestarks  (1000)        0 2023-05-06 00:31:21.970488 negotium-0.2.0/tests/
+-rw-rw-r--   0 deestarks  (1000) deestarks  (1000)        0 2023-05-03 09:50:29.000000 negotium-0.2.0/tests/__init__.py
```

### Comparing `negotium-0.1.0/README.md` & `negotium-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,83 @@
+Metadata-Version: 2.1
+Name: negotium
+Version: 0.2.0
+Summary: A very simple asynchronous task/job queue
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # Negotium
 
 A simple, lightweight, and easy-to-use task or job queue for Python. It tries to mimic the implementation of celery and celery beat, but without the complexity and overhead. For now, it offers only a minimal set of features, which will be expanded. It also currently only supports Redis as the broker; however, it is planned to support other brokers in the future.
 
 ## Installation
 
 ```bash
 pip install negotium
 ```
 
+## Features
+
+- Asynchronous task execution
+- Scheduled task execution
+- Dynamic periodic task execution
+- Task cancellation: All tasks are cancellable using the UUID returned by the task execution methods: `delay`, `apply_async`, and `apply_periodic_async`
+
 ## Usage
 
 ```python
 # ---- main.py (app entry point) ----
 from negotium import Negotium
 
 app = Negotium(broker_url="redis://localhost:6379/0", app_name="my_app")
 app.start()
 
 @app.task
 def add(x, y):
     return x + y
+```
 
-# --- app.py (another module) ----
-from main import app
+#### Delayed task execution
 
-# Run the task asynchronously
+```python
 add.delay(1, 2)
+```
+
+#### Scheduled task execution
 
-# Schedule the task to run at a specific time
+```python
 add.apply_async(args=(1, 2), eta=datetime.datetime.now() + datetime.timedelta(seconds=10))
 ```
 
+#### Dynamic periodic task execution
+
+> Note: Periodic tasks are scheduled using `negotium.schedules.Crontab` object. The `Crontab` object takes the following arguments:
+> - `minute`: The minute to run the task at
+> - `hour`: The hour to run the task at
+> - `day`: The day of the week to run the task at
+> - `month`: The day of the month to run the task at
+> - `weekday`: The month of the year to run the task at
+> 
+> Or, you can pass a raw crontab expression as a string. For example: `* * * * *` will run the task every minute.
+
+
+```python
+from main import app
+from negotium.schedules import Crontab
+
+# run the task every minute
+task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(minute=1))
+
+# with a raw crontab expression
+task_id = add.apply_periodic_async(args=(1, 2), cron=Crontab(expression="* * * * *"))
+
+# to cancel, import the app object and call the `cancel` method
+app.cancel(task_id)
+```
+
 ### Using in a Django project
 
 - Create a `negotium.py` file in your Django project directory
 ```
 my_project/
     manage.py
     my_project/
@@ -70,20 +113,25 @@
     return x + y
 ```
 
 - In your views, you can run the task asynchronously
 ```python
 # --- example/views.py ---
 from example.tasks import add
+from negotium.schedules import Crontab
 
 def my_async_view(request):
     add.delay(1, 2) # <-- Run the task asynchronously
     return HttpResponse("Hello, world!")
 
 def my_scheduled_view(request):
     add.apply_async(
-        args=(1, 2), eta=datetime.datetime.now() + \
-            datetime.timedelta(seconds=10)) # <-- Schedule the task to run at a specific time
+        args=(1, 2), eta=datetime.datetime.now() + datetime.timedelta(seconds=10)
+    ) # <-- Schedule the task to run at a specific time
+    return HttpResponse("Hello, world!")
+
+def my_periodic_view(request):
+    add.apply_periodic_async(args=(1, 2), cron=Crontab(expression="* * * * *"))
     return HttpResponse("Hello, world!")
 ```
 
 You're all set! Now you can run the Django development server and start using negotium.
```

### Comparing `negotium-0.1.0/negotium/base.py` & `negotium-0.2.0/negotium/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 import inspect
 from functools import wraps
 
 from .settings import DEFAULT_HOST, DEFAULT_PORT, DEFAULT_LOGFILE
-from .task import _delay, _apply_async
+from .task import _delay, _apply_async, _apply_periodic_async
 from negotium.mq.consumer import _Consumer
 from negotium.mq.publisher import _Publisher
 from negotium.utils.logger import log
 
 
 class Negotium:
     """This class is the entry point to the negotium application.
@@ -72,28 +72,33 @@
             def add(x, y):
                 return x + y
         """
         @wraps(func)
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
-        wrapper.delay = lambda *args, **kwargs: _delay(self.publisher, {
+        d = {
             'app_name': self.app_name,
             'package_dir': '/'.join(inspect.getfile(func).split('/')[:-1]),
             'package_name': inspect.getfile(func).split('/')[-2],
             'module_name': inspect.getmodulename(inspect.getfile(func)),
             'function_name': func.__name__,
-            'args': args,
-            'kwargs': kwargs,
             'timestamp': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        })
-        wrapper.apply_async = lambda eta, args: _apply_async(self.publisher, {
-            'app_name': self.app_name,
-            'package_dir': '/'.join(inspect.getfile(func).split('/')[:-1]),
-            'package_name': inspect.getfile(func).split('/')[-2],
-            'module_name': inspect.getmodulename(inspect.getfile(func)),
-            'function_name': func.__name__,
-            'args': args,
-            'timestamp': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-        }, eta)
+        }
+        wrapper.delay = lambda *args, **kwargs: _delay(self.publisher, {**d, 'args': args, 'kwargs': kwargs})
+        wrapper.apply_async = lambda eta, args: _apply_async(self.publisher, {**d,'args': args}, eta)
+
+        def apply_periodic_async(cron, args):
+            uuid_ = _apply_periodic_async(self.publisher, {**d, 'args': args}, cron)
+            # restart the consumer to pick up the new periodic task
+            self.consumer._consume_periodic_tasks()
+            return uuid_
+        wrapper.apply_periodic_async = apply_periodic_async
         return wrapper
 
+    def cancel(self, uuid_: str):
+        """Cancel a scheduled task
+
+        Example:
+            negotium.cancel(uuid_)
+        """
+        self.consumer._delete_message(uuid_)
```

### Comparing `negotium-0.1.0/negotium/mq/publisher.py` & `negotium-0.2.0/negotium/mq/publisher.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,75 @@
 import datetime
 import json
 import redis
 
-from negotium.settings import DEFAULT_QUEUE, DEFAULT_SCHEDULER_QUEUE, DEFAULT_SCHEDULER_SORTED_SET
+from negotium.mq.trackers import _MessageTracker
+from negotium.mq.trackers import _COMMAND_ZREM, _COMMAND_LREM, _COMMAND_BLPOP
+from negotium.settings import (
+    _MESSAGE_MAIN, _MESSAGE_SCHEDULER, _MESSAGE_SCHEDULER_SORTED_SET, _MESSAGE_PERIODIC_TASKS
+)
+from negotium.schedules.crontab import Crontab
 from negotium.utils.logger import log
 
 class _Publisher:
     def __init__(self, db: int, host: str, port: int, app_name: str, logfile: str=None):
         self.connection = None
+        self._tracker = None
         self.db = db
         self.host = host
         self.port = port
         self.app_name = app_name
         self.logfile = logfile
 
     def _create_connection(self):
         """Create a connection to the message broker
         """
         self.connection = redis.Redis(db=self.db, host=self.host, port=self.port)
+        self._tracker = _MessageTracker(self.connection, self.app_name)
 
     def _close_connection(self):
         """Close the connection
         """
         self.connection.close()
 
-    def _publish(self, data: dict, eta: datetime.datetime=None):
-        """Publish a message to the queue
+    def _publish(self, data: dict, eta: datetime.datetime=None, cron: Crontab=None) -> str:
+        """Publish a message to the queue and return the message id
         """
         log(self.logfile, data.get('app_name'), f"Received task: {data.get('function_name')}")
         if eta:
             data = {
                 '_task': data,
                 '_eta': eta.strftime('%Y-%m-%d %H:%M:%S.%f')
             }
-            self.connection.rpush(DEFAULT_SCHEDULER_QUEUE + "__" + self.app_name, json.dumps(data))
-            # zadd
+            self.connection.rpush(_MESSAGE_SCHEDULER + "__" + self.app_name, json.dumps(data))
+            message_id = self._tracker._track(
+                name=_MESSAGE_SCHEDULER + "__" + self.app_name, 
+                identifier=json.dumps(data), 
+                command=_COMMAND_LREM
+            )
+
             timestamp = datetime.datetime.strptime(eta.strftime('%Y-%m-%d %H:%M:%S.%f'), '%Y-%m-%d %H:%M:%S.%f').timestamp()
-            self.connection.zadd(DEFAULT_SCHEDULER_SORTED_SET + "__" + self.app_name, {json.dumps(data): timestamp})
+            self.connection.zadd(_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name, {json.dumps(data): timestamp})
+            return self._tracker._track(
+                name=_MESSAGE_SCHEDULER_SORTED_SET + "__" + self.app_name,
+                identifier=json.dumps(data),
+                command=_COMMAND_ZREM,
+                uuid_=message_id
+            )
+        elif cron:
+            data = {
+                '_task': data,
+                '_cron': cron.__str__()
+            }
+            self.connection.rpush(_MESSAGE_PERIODIC_TASKS + "__" + self.app_name, json.dumps(data))
+            return self._tracker._track(
+                name=_MESSAGE_PERIODIC_TASKS + "__" + self.app_name,
+                identifier=json.dumps(data), 
+                command=_COMMAND_LREM
+            )
         else:
-            self.connection.rpush(DEFAULT_QUEUE + "__" + self.app_name, json.dumps(data))
+            self.connection.rpush(_MESSAGE_MAIN + "__" + self.app_name, json.dumps(data))
+            return self._tracker._track(
+                name=_MESSAGE_MAIN + "__" + self.app_name,
+                command=_COMMAND_BLPOP
+            )
```

### Comparing `negotium-0.1.0/negotium/utils/logger.py` & `negotium-0.2.0/negotium/utils/logger.py`

 * *Files identical despite different names*

