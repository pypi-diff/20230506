# Comparing `tmp/taskiq-0.4.1.tar.gz` & `tmp/taskiq-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.4.1.tar", max compression
+gzip compressed data, was "taskiq-0.4.2.tar", max compression
```

## Comparing `taskiq-0.4.1.tar` & `taskiq-0.4.2.tar`

### file list

```diff
@@ -1,58 +1,59 @@
--rw-r--r--   0        0        0     1075 2023-04-17 22:32:14.530082 taskiq-0.4.1/LICENSE
--rw-r--r--   0        0        0     1875 2023-04-17 22:32:14.530082 taskiq-0.4.1/README.md
--rw-r--r--   0        0        0     2888 2023-04-17 22:32:14.534082 taskiq-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1587 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/__init__.py
--rw-r--r--   0        0        0     2077 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/__init__.py
--rw-r--r--   0        0        0     9488 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     2997 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1375 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0       34 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2154 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3911 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1516 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     4286 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7498 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     5375 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/context.py
--rw-r--r--   0        0        0     2929 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/decor.py
--rw-r--r--   0        0        0      510 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/events.py
--rw-r--r--   0        0        0      778 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4315 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2005 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0     9641 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      476 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1519 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0     1071 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/state.py
--rw-r--r--   0        0        0     4139 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/task.py
--rw-r--r--   0        0        0      874 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/utils.py
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-06 15:09:29.858694 taskiq-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1875 2023-05-06 15:09:29.858694 taskiq-0.4.2/README.md
+-rw-r--r--   0        0        0     2884 2023-05-06 15:09:29.866694 taskiq-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1587 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/__init__.py
+-rw-r--r--   0        0        0     2077 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0    12063 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     2997 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1375 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0       34 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5874 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2197 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3911 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1516 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     4286 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7498 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     5375 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0      468 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/context.py
+-rw-r--r--   0        0        0     2929 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/decor.py
+-rw-r--r--   0        0        0      510 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/events.py
+-rw-r--r--   0        0        0      778 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2039 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0     9651 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      483 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1268 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1519 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0     1071 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/state.py
+-rw-r--r--   0        0        0     4139 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/task.py
+-rw-r--r--   0        0        0      874 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/utils.py
+-rw-r--r--   0        0        0      106 2023-05-06 15:09:29.866694 taskiq-0.4.2/taskiq/warnings.py
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.2/PKG-INFO
```

### Comparing `taskiq-0.4.1/LICENSE` & `taskiq-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/README.md` & `taskiq-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/pyproject.toml` & `taskiq-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.4.1"
+version = "0.4.2"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
@@ -43,15 +43,15 @@
 gitignore-parser = { version = "^0", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = { version = "^22.6.0", allow-prereleases = true }
 flake8 = "^4.0.1"
 isort = "^5.10.1"
-mypy = "^0.971"
+mypy = "^1"
 pre-commit = "^2.20.0"
 yesqa = "^1.3.0"
 autoflake = "^1.4"
 wemake-python-styleguide = "^0.16.1"
 coverage = "^6.4.2"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
```

### Comparing `taskiq-0.4.1/taskiq/__init__.py` & `taskiq-0.4.2/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/__main__.py` & `taskiq-0.4.2/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/abc/broker.py` & `taskiq-0.4.2/taskiq/abc/broker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import os
 import sys
+import warnings
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from functools import wraps
 from logging import getLogger
 from typing import (  # noqa: WPS235
     TYPE_CHECKING,
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
-    Coroutine,
     DefaultDict,
     Dict,
     List,
     Optional,
     TypeVar,
     Union,
     overload,
 )
 from uuid import uuid4
 
-from typing_extensions import ParamSpec, TypeAlias
+from typing_extensions import ParamSpec, Self, TypeAlias
 
 from taskiq.abc.middleware import TaskiqMiddleware
 from taskiq.decor import AsyncTaskiqDecoratedTask
 from taskiq.events import TaskiqEvents
 from taskiq.formatters.json_formatter import JSONFormatter
 from taskiq.message import BrokerMessage
 from taskiq.result_backends.dummy import DummyResultBackend
 from taskiq.state import TaskiqState
 from taskiq.utils import maybe_awaitable, remove_suffix
+from taskiq.warnings import TaskiqDeprecationWarning
 
 if TYPE_CHECKING:  # pragma: no cover
     from taskiq.abc.formatter import TaskiqFormatter
     from taskiq.abc.result_backend import AsyncResultBackend
 
 _T = TypeVar("_T")  # noqa: WPS111
 _FuncParams = ParamSpec("_FuncParams")
@@ -72,16 +73,28 @@
     def __init__(
         self,
         result_backend: "Optional[AsyncResultBackend[_T]]" = None,
         task_id_generator: Optional[Callable[[], str]] = None,
     ) -> None:
         if result_backend is None:
             result_backend = DummyResultBackend()
+        else:
+            warnings.warn(
+                "Setting result backend with constructor is deprecated. "
+                "Please use `with_result_backend` instead.",
+                TaskiqDeprecationWarning,
+            )
         if task_id_generator is None:
             task_id_generator = default_id_generator
+        else:
+            warnings.warn(
+                "Setting id generator with constructor is deprecated. "
+                "Please use `with_id_generator` instead.",
+                TaskiqDeprecationWarning,
+            )
         self.middlewares: "List[TaskiqMiddleware]" = []
         self.result_backend = result_backend
         self.decorator_class = AsyncTaskiqDecoratedTask
         self.formatter: "TaskiqFormatter" = JSONFormatter()
         self.id_generator = task_id_generator
         # Every event has a list of handlers.
         # Every handler is a function which takes state as a first argument.
@@ -128,14 +141,16 @@
         event = TaskiqEvents.CLIENT_STARTUP
         if self.is_worker_process:
             event = TaskiqEvents.WORKER_STARTUP
 
         for handler in self.event_handlers[event]:
             await maybe_awaitable(handler(self.state))
 
+        await self.result_backend.startup()
+
     async def shutdown(self) -> None:
         """
         Close the broker.
 
         This method is called,
         when broker is closig.
         """
@@ -143,14 +158,16 @@
         if self.is_worker_process:
             event = TaskiqEvents.WORKER_SHUTDOWN
 
         # Call all shutdown events.
         for handler in self.event_handlers[event]:
             await maybe_awaitable(handler(self.state))
 
+        await self.result_backend.shutdown()
+
     @abstractmethod
     async def kick(
         self,
         message: BrokerMessage,
     ) -> None:
         """
         This method is used to kick tasks out from current program.
@@ -289,15 +306,15 @@
 
         return handler
 
     def add_event_handler(
         self,
         event: TaskiqEvents,
         handler: EventHandler,
-    ) -> None:
+    ) -> None:  # pragma: no cover
         """
         Adds event handler.
 
         this function is the same as on_event.
 
         >>> broker.add_event_handler(TaskiqEvents.WORKER_STARTUP, my_startup)
 
@@ -307,7 +324,75 @@
         >>> async def my_startup(context: Context) -> None:
         >>>    ...
 
         :param event: Event to react to.
         :param handler: handler to call when event is started.
         """
         self.event_handlers[event].append(handler)
+
+    def with_result_backend(
+        self,
+        result_backend: "AsyncResultBackend[_T]",
+    ) -> "Self":  # pragma: no cover
+        """
+        Set a result backend and return updated broker.
+
+        :param result_backend: new result backend.
+        :return: self
+        """
+        self.result_backend = result_backend
+        return self
+
+    def with_id_generator(
+        self,
+        task_id_generator: Callable[[], str],
+    ) -> "Self":  # pragma: no cover
+        """
+        Set a new Id generator and return an updated broker.
+
+        :param task_id_generator: new generator function.
+        :return: self
+        """
+        self.id_generator = task_id_generator
+        return self
+
+    def with_middlewares(
+        self,
+        *middlewares: "TaskiqMiddleware",
+    ) -> "Self":  # pragma: no cover
+        """
+        Add middewares to broker.
+
+        This method adds new middlewares to broker
+        and returns and updated broker.
+
+        :param middlewares: list of middlewares.
+        :return: self
+        """
+        for middleware in middlewares:
+            if not isinstance(middleware, TaskiqMiddleware):
+                logger.warning(
+                    f"Middleware {middleware} is not an instance of TaskiqMiddleware. "
+                    "Skipping...",
+                )
+                continue
+            middleware.set_broker(self)
+            self.middlewares.append(middleware)
+        return self
+
+    def with_event_handlers(
+        self,
+        event: TaskiqEvents,
+        *handlers: EventHandler,
+    ) -> "Self":  # pragma: no cover
+        """
+        Set new event handlers.
+
+        It takes an event to handle, list of handlers
+        and sets it to broker, returning an updated broker.
+
+        :param event: event to handle.
+        :param handlers: event handlers.
+        :return: self
+        """
+        self.event_handlers[event].extend(handlers)
+        return self
```

### Comparing `taskiq-0.4.1/taskiq/abc/formatter.py` & `taskiq-0.4.2/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/abc/middleware.py` & `taskiq-0.4.2/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/abc/result_backend.py` & `taskiq-0.4.2/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/abc/schedule_source.py` & `taskiq-0.4.2/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/brokers/inmemory_broker.py` & `taskiq-0.4.2/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/brokers/shared_broker.py` & `taskiq-0.4.2/taskiq/brokers/shared_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import AsyncGenerator, Optional, TypeVar
 
+from typing_extensions import ParamSpec
+
 from taskiq.abc.broker import AsyncBroker
 from taskiq.decor import AsyncTaskiqDecoratedTask
 from taskiq.exceptions import TaskiqError
 from taskiq.kicker import AsyncKicker
 from taskiq.message import BrokerMessage
 
 _ReturnType = TypeVar("_ReturnType")
-_Params = TypeVar("_Params")
+_Params = ParamSpec("_Params")
 
 
 class SharedDecoratedTask(AsyncTaskiqDecoratedTask[_Params, _ReturnType]):
     """Decorator that is used with shared broker."""
 
     def kicker(self) -> AsyncKicker[_Params, _ReturnType]:
         """
```

### Comparing `taskiq-0.4.1/taskiq/brokers/zmq_broker.py` & `taskiq-0.4.2/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/scheduler/args.py` & `taskiq-0.4.2/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/scheduler/cmd.py` & `taskiq-0.4.2/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/scheduler/run.py` & `taskiq-0.4.2/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/utils.py` & `taskiq-0.4.2/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/watcher.py` & `taskiq-0.4.2/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/worker/args.py` & `taskiq-0.4.2/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/worker/cmd.py` & `taskiq-0.4.2/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/worker/log_collector.py` & `taskiq-0.4.2/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/worker/process_manager.py` & `taskiq-0.4.2/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/cli/worker/run.py` & `taskiq-0.4.2/taskiq/cli/worker/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/decor.py` & `taskiq-0.4.2/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/exceptions.py` & `taskiq-0.4.2/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/formatters/json_formatter.py` & `taskiq-0.4.2/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/funcs.py` & `taskiq-0.4.2/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/kicker.py` & `taskiq-0.4.2/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.4.2/taskiq/middlewares/prometheus_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/middlewares/retry_middleware.py` & `taskiq-0.4.2/taskiq/middlewares/retry_middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         :param message: Message that caused the error.
         :param result: execution result.
         :param exception: found exception.
         """
         retry_on_error = message.labels.get("retry_on_error")
         # Check if retrying is enabled for the task.
-        if retry_on_error != "True":
+        if retry_on_error is None or retry_on_error.lower() != "true":
             return
         new_msg = deepcopy(message)
         # Getting number of previous retries.
         retries = int(new_msg.labels.get("_retries", 0)) + 1
         new_msg.labels["_retries"] = str(retries)
         max_retries = int(new_msg.labels.get("max_retries", self.default_retry_count))
         if retries < max_retries:
```

### Comparing `taskiq-0.4.1/taskiq/receiver/params_parser.py` & `taskiq-0.4.2/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/receiver/receiver.py` & `taskiq-0.4.2/taskiq/receiver/receiver.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
             await dep_ctx.close()
 
         # Assemble result.
         result: "TaskiqResult[Any]" = TaskiqResult(
             is_err=found_exception is not None,
             log=None,
             return_value=returned,
-            execution_time=execution_time,
+            execution_time=round(execution_time, 2),
         )
         # If exception is found we execute middlewares.
         if found_exception is not None:
             for middleware in self.broker.middlewares:
                 if middleware.__class__.on_error != TaskiqMiddleware.on_error:
                     await maybe_awaitable(
                         middleware.on_error(
```

### Comparing `taskiq-0.4.1/taskiq/result_backends/dummy.py` & `taskiq-0.4.2/taskiq/result_backends/dummy.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,15 @@
         """
         Sets result.
 
         But actually it does nothing.
 
         :param task_id: current task id.
         :param result: result of execution.
-        :return: nothing.
         """
-        return await super().set_result(task_id, result)
 
     async def is_result_ready(self, task_id: str) -> bool:
         """
         Checks whether task is completed.
 
         Result is always ready,
         since it doesn't care about tasks.
```

### Comparing `taskiq-0.4.1/taskiq/schedule_sources/label_based.py` & `taskiq-0.4.2/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/scheduler/merge_functions.py` & `taskiq-0.4.2/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/scheduler/scheduler.py` & `taskiq-0.4.2/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/state.py` & `taskiq-0.4.2/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/task.py` & `taskiq-0.4.2/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/taskiq/utils.py` & `taskiq-0.4.2/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.1/PKG-INFO` & `taskiq-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.4.1
+Version: 0.4.2
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.4.1 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.4.2 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

