# Comparing `tmp/futured-1.3.tar.gz` & `tmp/futured-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "futured-1.3.tar", last modified: Sun Sep 12 18:00:45 2021, max compression
+gzip compressed data, was "futured-1.4.tar", last modified: Sat May  6 18:54:59 2023, max compression
```

## Comparing `futured-1.3.tar` & `futured-1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 18:00:45.142892 futured-1.3/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-09-12 18:00:14.000000 futured-1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2021-09-12 18:00:45.142892 futured-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2021-09-12 18:00:14.000000 futured-1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 18:00:45.142892 futured-1.3/futured/
--rw-r--r--   0 runner    (1001) docker     (121)     8975 2021-09-12 18:00:14.000000 futured-1.3/futured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-12 18:00:14.000000 futured-1.3/futured/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-12 18:00:45.142892 futured-1.3/futured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2021-09-12 18:00:45.000000 futured-1.3/futured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      237 2021-09-12 18:00:45.000000 futured-1.3/futured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-12 18:00:45.000000 futured-1.3/futured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-12 18:00:44.000000 futured-1.3/futured.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-09-12 18:00:45.000000 futured-1.3/futured.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-12 18:00:14.000000 futured-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2021-09-12 18:00:45.142892 futured-1.3/setup.cfg
+drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.327152 futured-1.4/
+-rw-r--r--   0 coady      (501) staff       (20)      576 2022-04-25 21:08:17.000000 futured-1.4/LICENSE.txt
+-rw-r--r--   0 coady      (501) staff       (20)     7227 2023-05-06 18:54:59.327034 futured-1.4/PKG-INFO
+-rw-r--r--   0 coady      (501) staff       (20)     5446 2023-05-06 18:19:03.000000 futured-1.4/README.md
+drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326251 futured-1.4/futured/
+-rw-r--r--   0 coady      (501) staff       (20)     8771 2023-05-06 18:36:26.000000 futured-1.4/futured/__init__.py
+-rw-r--r--   0 coady      (501) staff       (20)        0 2020-10-25 18:57:52.000000 futured-1.4/futured/py.typed
+drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326647 futured-1.4/futured.egg-info/
+-rw-r--r--   0 coady      (501) staff       (20)     7227 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/PKG-INFO
+-rw-r--r--   0 coady      (501) staff       (20)      215 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/SOURCES.txt
+-rw-r--r--   0 coady      (501) staff       (20)        1 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/dependency_links.txt
+-rw-r--r--   0 coady      (501) staff       (20)        8 2023-05-06 18:54:59.000000 futured-1.4/futured.egg-info/top_level.txt
+-rw-r--r--   0 coady      (501) staff       (20)     1491 2023-03-17 20:50:37.000000 futured-1.4/pyproject.toml
+-rw-r--r--   0 coady      (501) staff       (20)       38 2023-05-06 18:54:59.327185 futured-1.4/setup.cfg
+drwxr-xr-x   0 coady      (501) staff       (20)        0 2023-05-06 18:54:59.326758 futured-1.4/tests/
+-rw-r--r--   0 coady      (501) staff       (20)     4680 2022-11-19 03:19:34.000000 futured-1.4/tests/test_all.py
```

### Comparing `futured-1.3/LICENSE.txt` & `futured-1.4/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020 Aric Coady
+Copyright 2022 Aric Coady
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
      http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `futured-1.3/PKG-INFO` & `futured-1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,200 +1,217 @@
 Metadata-Version: 2.1
 Name: futured
-Version: 1.3
+Version: 1.4
 Summary: Functional interface for concurrent futures, including asynchronous I/O.
-Home-page: https://github.com/coady/futured
-Author: Aric Coady
-Author-email: aric.coady@gmail.com
-License: Apache Software License
-Project-URL: Documentation, https://coady.github.io/futured
-Description: [![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
-        ![image](https://img.shields.io/pypi/pyversions/futured.svg)
-        [![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
-        ![image](https://img.shields.io/pypi/status/futured.svg)
-        [![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
-        [![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
-        [![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
-        [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
-        [![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-        
-        Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
-        
-        ## Usage
-        ### threaded, processed
-        Transform any callable into one which runs in a thread or process pool, and returns a future.
-        
-        ```python
-        from futured import threaded, processed
-        import httpx
-        
-        fetch = threaded(httpx.Client().get)
-        fetch(url)  # return Future
-        
-        fs = (fetch(url + path) for path in paths)
-        threaded.results(fs)  # generate results from futures
-        threaded.results(fs, timeout=...)  # generate results as completed
-        
-        fetch.map(urls)  # generate results in order
-        fetch.map(urls, timeout=...)  # generate results as completed
-        fetch.mapzip(urls)  # generate (url, result) pairs as completed
-        ```
-        
-        Thread and process pool executors may be used as context managers, customized with options, and reused with different callables.
-        
-        ```python
-        threaded(max_workers=...)(func, ...)
-        processed(max_workers=...)(func, ...)
-        ```
-        
-        `futured` classes have a `waiting` context manager which collects results from tasks. Futures can be registered at creation, or appended to the list of tasks.
-        
-        ```python
-        with threaded.waiting(*fs) as tasks:
-            tasks.append(future)
-        tasks  # list of completed results
-        ```
-        
-        `futured` classes provide a `tasks` interface which generalizes `futures.as_completed` and `futures.wait`, while allowing the set of tasks to be modified, e.g., for retries.
-        
-        ```python
-        threaded.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
-        ```
-        
-        ### asynced
-        The same interface works for `asyncio`.
-        
-        ```python
-        from futured import asynced
-        import httpx
-        
-        fetch = asynced(httpx.AsyncClient().get)
-        fetch(url)  # return coroutine
-        
-        asynced.results(fs)  # generate results from futures
-        asynced.results(fs, timeout=...)  # generate results as completed
-        
-        fetch.map(urls)  # generate results in order
-        fetch.map(urls, timeout=...)  # generate results as completed
-        fetch.mapzip(urls)  # generate (url, result) pairs as completed
-        ```
-        
-        `asynced` provides utilities for calling coroutines from a synchronous context. `waiting` is similar to [trio's nursery](https://trio.readthedocs.io/en/latest/reference-core.html#nurseries-and-spawning), but returns results from a synchronous `with` block.
-        
-        ```python
-        asynced.run(async_func, ...)  # call and run until complete
-        asynced.run(async_gen, ...)  # call and run synchronous iterator
-        with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
-        asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
-        ```
-        
-        ### decorators
-        Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
-        
-        ```python
-        @threaded
-        def slow():
-           ...
-        
-        fetch = threaded(httpx.Client().get, url)
-        fetch(params=...)
-        ```
-        
-        Methods are supported, as well as a `decorated` utility for automatically subclassing.
-        
-        ```python
-        from futured import decorated
+Author-email: Aric Coady <aric.coady@gmail.com>
+License: Copyright 2022 Aric Coady
         
-        FutureClient = decorated(httpx.Client, request=threaded)
-        
-         # equivalent to
-        class FutureClient(httpx.Client):
-            request = threaded(httpx.Client.request)
-        ```
-        
-        ### command
-        `command` wraps `subprocess.Popen` to provide a `Future` compatible interface.
-        
-        ```python
-        from futured import futured, command
-        
-        command('ls').result()  # return stdout or raises stderr
-        command('ls').pipe('wc')  # pipes into next command, or | ('wc',... )
-        for line in command('ls'):  # iterable lines
-        command.coroutine('ls')  # return coroutine
-        
-        futured(command, 'ls')  # supports `map` interface
-        asynced(command.coroutine, 'ls')  # supports `map` interface with timeout
-        ```
-        
-        ### forked
-        `forked` allows iteration in separate child processes.
-        
-        ```python
-        from futured import forked
-        
-        for value in forked(values, max_workers=...):
-            # in a child process
-         # in parent after children have exited
-        ```
-        
-        ## Installation
-        ```console
-        % pip install futured
-        ```
-        
-        ## Tests
-        100% branch coverage.
-        
-        ```console
-        % pytest [--cov]
-        ```
-        
-        ## Changes
-        1.3
-        
-        * Python >=3.7 required
-        * Python 3.10 event loop changes
-        * Streams replaced with tasks
-        
-        1.2
-        
-        * Python >=3.6 required
-        
-        1.1
-        
-        * Stream completed futures from a pending pool
-        
-        1.0
-        
-        * Executed functions are context managers
-        * `starmap` supported
-        
-        0.3
-        
-        * `forked` has optional maximum number of workers
-        * `waiting` context manager
-        * `command` pipes (`|`)
-        * `distributed.Client` support
-        
-        0.2
-        
-        * `command.coroutine` creates asyncio subprocesses
-        * `futured.mapzip` generates results zipped with arguments
-        * `asynced.run` supports asynchronous iterators
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+             http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
         
+Project-URL: Homepage, https://github.com/coady/futured
+Project-URL: Documentation, https://coady.github.io/futured
 Keywords: concurrent,futures,threads,processes,async,asyncio
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
+![image](https://img.shields.io/pypi/pyversions/futured.svg)
+[![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
+![image](https://img.shields.io/pypi/status/futured.svg)
+[![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
+[![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
+[![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
+[![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+
+Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
+
+## Usage
+### threaded, processed
+Transform any callable into one which runs in a thread or process pool, and returns a future.
+
+```python
+from futured import threaded, processed
+import httpx
+
+fetch = threaded(httpx.Client().get)
+fetch(url)  # return Future
+
+fs = (fetch(url + path) for path in paths)
+threaded.results(fs)  # generate results from futures
+threaded.results(fs, timeout=...)  # generate results as completed
+
+fetch.map(urls)  # generate results in order
+fetch.map(urls, timeout=...)  # generate results as completed
+fetch.mapzip(urls)  # generate (url, result) pairs as completed
+```
+
+Thread and process pool executors may be used as context managers, customized with options, and reused with different callables.
+
+```python
+threaded(max_workers=...)(func, ...)
+processed(max_workers=...)(func, ...)
+```
+
+`futured` classes have a `waiting` context manager which collects results from tasks. Futures can be registered at creation, or appended to the list of tasks.
+
+```python
+with threaded.waiting(*fs) as tasks:
+    tasks.append(future)
+tasks  # list of completed results
+```
+
+`futured` classes provide a `tasks` interface which generalizes `futures.as_completed` and `futures.wait`, while allowing the set of tasks to be modified, e.g., for retries.
+
+```python
+threaded.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
+```
+
+### asynced
+The same interface works for `asyncio`.
+
+```python
+from futured import asynced
+import httpx
+
+fetch = asynced(httpx.AsyncClient().get)
+fetch(url)  # return coroutine
+
+asynced.results(fs)  # generate results from futures
+asynced.results(fs, timeout=...)  # generate results as completed
+
+fetch.map(urls)  # generate results in order
+fetch.map(urls, timeout=...)  # generate results as completed
+fetch.mapzip(urls)  # generate (url, result) pairs as completed
+```
+
+`asynced` provides utilities for calling coroutines from a synchronous context. `waiting` is similar to [trio's nursery](https://trio.readthedocs.io/en/latest/reference-core.html#nurseries-and-spawning), but returns results from a synchronous `with` block.
+
+```python
+asynced.run(async_func, ...)  # call and run until complete
+asynced.run(async_gen, ...)  # call and run synchronous iterator
+with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
+asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
+```
+
+### decorators
+Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
+
+```python
+@threaded
+def slow():
+   ...
+
+fetch = threaded(httpx.Client().get, url)
+fetch(params=...)
+```
+
+Methods are supported, as well as a `decorated` utility for automatically subclassing.
+
+```python
+from futured import decorated
+
+FutureClient = decorated(httpx.Client, request=threaded)
+
+ # equivalent to
+class FutureClient(httpx.Client):
+    request = threaded(httpx.Client.request)
+```
+
+### command
+`command` wraps `subprocess.Popen` to provide a `Future` compatible interface.
+
+```python
+from futured import futured, command
+
+command('ls').result()  # return stdout or raises stderr
+command('ls').pipe('wc')  # pipes into next command, or | ('wc',... )
+for line in command('ls'):  # iterable lines
+command.coroutine('ls')  # return coroutine
+
+futured(command, 'ls')  # supports `map` interface
+asynced(command.coroutine, 'ls')  # supports `map` interface with timeout
+```
+
+### forked
+`forked` allows iteration in separate child processes.
+
+```python
+from futured import forked
+
+for value in forked(values, max_workers=...):
+    # in a child process
+ # in parent after children have exited
+```
+
+## Installation
+```console
+% pip install futured
+```
+
+## Tests
+100% branch coverage.
+
+```console
+% pytest [--cov]
+```
+
+## Changes
+1.4
+
+* Python >=3.8 required
+
+1.3
+
+* Python >=3.7 required
+* Python 3.10 event loop changes
+* Streams replaced with tasks
+
+1.2
+
+* Python >=3.6 required
+
+1.1
+
+* Stream completed futures from a pending pool
+
+1.0
+
+* Executed functions are context managers
+* `starmap` supported
+
+0.3
+
+* `forked` has optional maximum number of workers
+* `waiting` context manager
+* `command` pipes (`|`)
+* `distributed.Client` support
+
+0.2
+
+* `command.coroutine` creates asyncio subprocesses
+* `futured.mapzip` generates results zipped with arguments
+* `asynced.run` supports asynchronous iterators
```

### Comparing `futured-1.3/README.md` & `futured-1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,18 @@
 100% branch coverage.
 
 ```console
 % pytest [--cov]
 ```
 
 ## Changes
+1.4
+
+* Python >=3.8 required
+
 1.3
 
 * Python >=3.7 required
 * Python 3.10 event loop changes
 * Streams replaced with tasks
 
 1.2
```

### Comparing `futured-1.3/futured/__init__.py` & `futured-1.4/futured/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 import contextlib
 import itertools
 import operator
 import os
-import queue
 import subprocess
 import types
 from concurrent import futures
 from functools import partial
-from typing import AnyStr, AsyncIterable, Callable, Iterable, Iterator
+from typing import AnyStr, AsyncIterable, Callable, Iterable, Iterator, Optional
 
-__version__ = '1.3'
+__version__ = '1.4'
 
 
 class futured(partial):
     """A partial function which returns futures."""
 
     as_completed: Callable = NotImplemented
 
@@ -23,51 +22,51 @@
 
     @classmethod
     def results(cls, fs: Iterable, *, as_completed=False, **kwargs) -> Iterator:
         """Generate results concurrently from futures, by default in order.
 
         Args:
             fs: iterable of futures
-            as_completed, kwargs: generate results as completed with options, e.g., timeout
+            as_completed kwargs: generate results as completed with options, e.g., timeout
         """
         tasks = cls.as_completed(fs, **kwargs) if (as_completed or kwargs) else list(fs)
         return map(operator.methodcaller('result'), tasks)
 
     @classmethod
     def items(cls, pairs: Iterable, **kwargs) -> Iterator:
         """Generate key, result pairs as completed from futures.
 
         Args:
             pairs: key, future pairs
-            kwargs: as completed options, e.g., timeout
+            **kwargs: as completed options, e.g., timeout
         """
         keys = dict(map(reversed, pairs))  # type: ignore
         return ((keys[future], future.result()) for future in cls.as_completed(keys, **kwargs))
 
     def map(self, *iterables: Iterable, **kwargs) -> Iterator:
         """Asynchronously map function.
 
         Args:
-            kwargs: keyword options for [results][futured.futured.results]
+            **kwargs: keyword options for [results][futured.futured.results]
         """
         return self.results(map(self, *iterables), **kwargs)
 
     def starmap(self, iterable: Iterable, **kwargs) -> Iterator:
         """Asynchronously starmap function.
 
         Args:
-            kwargs: keyword options for [results][futured.futured.results]
+            **kwargs: keyword options for [results][futured.futured.results]
         """
         return self.results(itertools.starmap(self, iterable), **kwargs)
 
     def mapzip(self, iterable: Iterable, **kwargs) -> Iterator:
         """Generate arg, result pairs as completed.
 
         Args:
-            kwargs: keyword options for [items][futured.futured.items]
+            **kwargs: keyword options for [items][futured.futured.items]
         """
         return self.items(((arg, self(arg)) for arg in iterable), **kwargs)
 
     @classmethod
     @contextlib.contextmanager
     def waiting(cls, *fs, **kwargs):
         """Return context manager which waits on [results][futured.futured.results]."""
@@ -100,15 +99,15 @@
             return self
 
         def __next__(self):
             return next(self.it)
 
 
 class executed(futured):
-    """Extensible base class for callables which require a ``submit`` method."""
+    """Extensible base class for callables which require a `submit` method."""
 
     as_completed = futures.as_completed
     Executor = futures.Executor
 
     def __new__(cls, *args, **kwargs):
         if args:
             return futured.__new__(cls, cls.Executor().submit, *args, **kwargs)
@@ -231,41 +230,36 @@
         return self.pipe(*other)
 
     def __iter__(self):
         """Return output lines."""
         return iter(self.result().splitlines())
 
 
-class Results(queue.Queue):
-    def put(self, pid, value):
-        pid, status = os.waitpid(pid, 0)
-        super().put((status, value))
-
-    def get(self):
-        status, value = super().get()
-        if status:
-            raise OSError(status, value)
-        return not status
-
-
-def forked(values: Iterable, max_workers: int = None) -> Iterator:
+def forked(values: Iterable, max_workers: Optional[int] = None) -> Iterator:
     """Generate each value in its own child process and wait in the parent."""
     max_workers = max_workers or os.cpu_count() or 1  # same default as ProcessPoolExecutor
-    workers, results = 0, Results()
-    task = threaded(max_workers=max_workers)(results.put)
+    workers: dict = {}
+
+    def wait():
+        pid, status = os.wait()
+        if pid in workers:
+            value = workers.pop(pid)
+            if status:
+                raise OSError(status, value)
+
     for value in values:
-        while workers >= max_workers:
-            workers -= results.get()
+        while len(workers) >= max_workers:
+            wait()
         pid = os.fork()
         if pid:
-            workers += bool(task(pid, value))
+            workers[pid] = value
         else:  # pragma: no cover
             yield value
             os._exit(0)
     while workers:
-        workers -= results.get()
+        wait()
 
 
 def decorated(base: type, **decorators: Callable) -> type:
     """Return subclass with decorated methods."""
     namespace = {name: decorators[name](getattr(base, name)) for name in decorators}
     return type(base.__name__, (base,), namespace)
```

### Comparing `futured-1.3/futured.egg-info/PKG-INFO` & `futured-1.4/futured.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,200 +1,217 @@
 Metadata-Version: 2.1
 Name: futured
-Version: 1.3
+Version: 1.4
 Summary: Functional interface for concurrent futures, including asynchronous I/O.
-Home-page: https://github.com/coady/futured
-Author: Aric Coady
-Author-email: aric.coady@gmail.com
-License: Apache Software License
-Project-URL: Documentation, https://coady.github.io/futured
-Description: [![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
-        ![image](https://img.shields.io/pypi/pyversions/futured.svg)
-        [![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
-        ![image](https://img.shields.io/pypi/status/futured.svg)
-        [![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
-        [![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
-        [![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
-        [![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
-        [![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
-        
-        Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
-        
-        ## Usage
-        ### threaded, processed
-        Transform any callable into one which runs in a thread or process pool, and returns a future.
-        
-        ```python
-        from futured import threaded, processed
-        import httpx
-        
-        fetch = threaded(httpx.Client().get)
-        fetch(url)  # return Future
-        
-        fs = (fetch(url + path) for path in paths)
-        threaded.results(fs)  # generate results from futures
-        threaded.results(fs, timeout=...)  # generate results as completed
-        
-        fetch.map(urls)  # generate results in order
-        fetch.map(urls, timeout=...)  # generate results as completed
-        fetch.mapzip(urls)  # generate (url, result) pairs as completed
-        ```
-        
-        Thread and process pool executors may be used as context managers, customized with options, and reused with different callables.
-        
-        ```python
-        threaded(max_workers=...)(func, ...)
-        processed(max_workers=...)(func, ...)
-        ```
-        
-        `futured` classes have a `waiting` context manager which collects results from tasks. Futures can be registered at creation, or appended to the list of tasks.
-        
-        ```python
-        with threaded.waiting(*fs) as tasks:
-            tasks.append(future)
-        tasks  # list of completed results
-        ```
-        
-        `futured` classes provide a `tasks` interface which generalizes `futures.as_completed` and `futures.wait`, while allowing the set of tasks to be modified, e.g., for retries.
-        
-        ```python
-        threaded.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
-        ```
-        
-        ### asynced
-        The same interface works for `asyncio`.
-        
-        ```python
-        from futured import asynced
-        import httpx
-        
-        fetch = asynced(httpx.AsyncClient().get)
-        fetch(url)  # return coroutine
-        
-        asynced.results(fs)  # generate results from futures
-        asynced.results(fs, timeout=...)  # generate results as completed
-        
-        fetch.map(urls)  # generate results in order
-        fetch.map(urls, timeout=...)  # generate results as completed
-        fetch.mapzip(urls)  # generate (url, result) pairs as completed
-        ```
-        
-        `asynced` provides utilities for calling coroutines from a synchronous context. `waiting` is similar to [trio's nursery](https://trio.readthedocs.io/en/latest/reference-core.html#nurseries-and-spawning), but returns results from a synchronous `with` block.
-        
-        ```python
-        asynced.run(async_func, ...)  # call and run until complete
-        asynced.run(async_gen, ...)  # call and run synchronous iterator
-        with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
-        asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
-        ```
-        
-        ### decorators
-        Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
-        
-        ```python
-        @threaded
-        def slow():
-           ...
-        
-        fetch = threaded(httpx.Client().get, url)
-        fetch(params=...)
-        ```
-        
-        Methods are supported, as well as a `decorated` utility for automatically subclassing.
-        
-        ```python
-        from futured import decorated
+Author-email: Aric Coady <aric.coady@gmail.com>
+License: Copyright 2022 Aric Coady
         
-        FutureClient = decorated(httpx.Client, request=threaded)
-        
-         # equivalent to
-        class FutureClient(httpx.Client):
-            request = threaded(httpx.Client.request)
-        ```
-        
-        ### command
-        `command` wraps `subprocess.Popen` to provide a `Future` compatible interface.
-        
-        ```python
-        from futured import futured, command
-        
-        command('ls').result()  # return stdout or raises stderr
-        command('ls').pipe('wc')  # pipes into next command, or | ('wc',... )
-        for line in command('ls'):  # iterable lines
-        command.coroutine('ls')  # return coroutine
-        
-        futured(command, 'ls')  # supports `map` interface
-        asynced(command.coroutine, 'ls')  # supports `map` interface with timeout
-        ```
-        
-        ### forked
-        `forked` allows iteration in separate child processes.
-        
-        ```python
-        from futured import forked
-        
-        for value in forked(values, max_workers=...):
-            # in a child process
-         # in parent after children have exited
-        ```
-        
-        ## Installation
-        ```console
-        % pip install futured
-        ```
-        
-        ## Tests
-        100% branch coverage.
-        
-        ```console
-        % pytest [--cov]
-        ```
-        
-        ## Changes
-        1.3
-        
-        * Python >=3.7 required
-        * Python 3.10 event loop changes
-        * Streams replaced with tasks
-        
-        1.2
-        
-        * Python >=3.6 required
-        
-        1.1
-        
-        * Stream completed futures from a pending pool
-        
-        1.0
-        
-        * Executed functions are context managers
-        * `starmap` supported
-        
-        0.3
-        
-        * `forked` has optional maximum number of workers
-        * `waiting` context manager
-        * `command` pipes (`|`)
-        * `distributed.Client` support
-        
-        0.2
-        
-        * `command.coroutine` creates asyncio subprocesses
-        * `futured.mapzip` generates results zipped with arguments
-        * `asynced.run` supports asynchronous iterators
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+             http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
         
+Project-URL: Homepage, https://github.com/coady/futured
+Project-URL: Documentation, https://coady.github.io/futured
 Keywords: concurrent,futures,threads,processes,async,asyncio
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![image](https://img.shields.io/pypi/v/futured.svg)](https://pypi.org/project/futured/)
+![image](https://img.shields.io/pypi/pyversions/futured.svg)
+[![image](https://pepy.tech/badge/futured)](https://pepy.tech/project/futured)
+![image](https://img.shields.io/pypi/status/futured.svg)
+[![image](https://github.com/coady/futured/workflows/build/badge.svg)](https://github.com/coady/futured/actions)
+[![image](https://codecov.io/gh/coady/futured/branch/main/graph/badge.svg)](https://codecov.io/github/coady/futured)
+[![image](https://github.com/coady/futured/workflows/codeql/badge.svg)](https://github.com/coady/futured/security/code-scanning)
+[![image](https://img.shields.io/badge/code%20style-black-000000.svg)](https://pypi.org/project/black/)
+[![image](http://mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
+
+Futured provides a consistent interface for concurrent functional programming in Python. It wraps any callable to return a `concurrent.futures.Future`, wraps any async coroutine to return an `asyncio.Future`, and provides concurrent iterators and context managers for futures.
+
+## Usage
+### threaded, processed
+Transform any callable into one which runs in a thread or process pool, and returns a future.
+
+```python
+from futured import threaded, processed
+import httpx
+
+fetch = threaded(httpx.Client().get)
+fetch(url)  # return Future
+
+fs = (fetch(url + path) for path in paths)
+threaded.results(fs)  # generate results from futures
+threaded.results(fs, timeout=...)  # generate results as completed
+
+fetch.map(urls)  # generate results in order
+fetch.map(urls, timeout=...)  # generate results as completed
+fetch.mapzip(urls)  # generate (url, result) pairs as completed
+```
+
+Thread and process pool executors may be used as context managers, customized with options, and reused with different callables.
+
+```python
+threaded(max_workers=...)(func, ...)
+processed(max_workers=...)(func, ...)
+```
+
+`futured` classes have a `waiting` context manager which collects results from tasks. Futures can be registered at creation, or appended to the list of tasks.
+
+```python
+with threaded.waiting(*fs) as tasks:
+    tasks.append(future)
+tasks  # list of completed results
+```
+
+`futured` classes provide a `tasks` interface which generalizes `futures.as_completed` and `futures.wait`, while allowing the set of tasks to be modified, e.g., for retries.
+
+```python
+threaded.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
+```
+
+### asynced
+The same interface works for `asyncio`.
+
+```python
+from futured import asynced
+import httpx
+
+fetch = asynced(httpx.AsyncClient().get)
+fetch(url)  # return coroutine
+
+asynced.results(fs)  # generate results from futures
+asynced.results(fs, timeout=...)  # generate results as completed
+
+fetch.map(urls)  # generate results in order
+fetch.map(urls, timeout=...)  # generate results as completed
+fetch.mapzip(urls)  # generate (url, result) pairs as completed
+```
+
+`asynced` provides utilities for calling coroutines from a synchronous context. `waiting` is similar to [trio's nursery](https://trio.readthedocs.io/en/latest/reference-core.html#nurseries-and-spawning), but returns results from a synchronous `with` block.
+
+```python
+asynced.run(async_func, ...)  # call and run until complete
+asynced.run(async_gen, ...)  # call and run synchronous iterator
+with asynced.waiting(*fs) as tasks:  # concurrent coroutines completed in a block
+asynced.tasks(fs, timeout=...)  # mutable set of running tasks which iterate as completed
+```
+
+### decorators
+Naturally `futured` wrappers can be used as decorators, but arguments can also be partially bound.
+
+```python
+@threaded
+def slow():
+   ...
+
+fetch = threaded(httpx.Client().get, url)
+fetch(params=...)
+```
+
+Methods are supported, as well as a `decorated` utility for automatically subclassing.
+
+```python
+from futured import decorated
+
+FutureClient = decorated(httpx.Client, request=threaded)
+
+ # equivalent to
+class FutureClient(httpx.Client):
+    request = threaded(httpx.Client.request)
+```
+
+### command
+`command` wraps `subprocess.Popen` to provide a `Future` compatible interface.
+
+```python
+from futured import futured, command
+
+command('ls').result()  # return stdout or raises stderr
+command('ls').pipe('wc')  # pipes into next command, or | ('wc',... )
+for line in command('ls'):  # iterable lines
+command.coroutine('ls')  # return coroutine
+
+futured(command, 'ls')  # supports `map` interface
+asynced(command.coroutine, 'ls')  # supports `map` interface with timeout
+```
+
+### forked
+`forked` allows iteration in separate child processes.
+
+```python
+from futured import forked
+
+for value in forked(values, max_workers=...):
+    # in a child process
+ # in parent after children have exited
+```
+
+## Installation
+```console
+% pip install futured
+```
+
+## Tests
+100% branch coverage.
+
+```console
+% pytest [--cov]
+```
+
+## Changes
+1.4
+
+* Python >=3.8 required
+
+1.3
+
+* Python >=3.7 required
+* Python 3.10 event loop changes
+* Streams replaced with tasks
+
+1.2
+
+* Python >=3.6 required
+
+1.1
+
+* Stream completed futures from a pending pool
+
+1.0
+
+* Executed functions are context managers
+* `starmap` supported
+
+0.3
+
+* `forked` has optional maximum number of workers
+* `waiting` context manager
+* `command` pipes (`|`)
+* `distributed.Client` support
+
+0.2
+
+* `command.coroutine` creates asyncio subprocesses
+* `futured.mapzip` generates results zipped with arguments
+* `asynced.run` supports asynchronous iterators
```

