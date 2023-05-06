# Comparing `tmp/pyxtension-1.15.0-py3-none-any.whl.zip` & `tmp/pyxtension-1.16.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 30371 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat    15389 b- defN 23-Apr-13 09:45 pyxtension/Json.py
--rw-rw-rw-  2.0 fat     1885 b- defN 23-Apr-13 09:45 pyxtension/__init__.py
--rw-rw-rw-  2.0 fat    11752 b- defN 23-Apr-13 09:45 pyxtension/fileutils.py
--rw-rw-rw-  2.0 fat     2647 b- defN 23-Apr-13 09:45 pyxtension/models.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-13 09:45 pyxtension/racelib.py
--rw-rw-rw-  2.0 fat    58818 b- defN 23-Apr-13 09:45 pyxtension/streams.py
--rw-rw-rw-  2.0 fat      775 b- defN 23-Apr-13 09:45 pyxtension/throttler.py
--rw-rw-rw-  2.0 fat      134 b- defN 23-Apr-12 22:39 pyxtension-1.15.0.data/data/requirements.txt
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17203 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1056 b- defN 23-Apr-13 09:45 pyxtension-1.15.0.dist-info/RECORD
-13 files, 113119 bytes uncompressed, 28619 bytes compressed:  74.7%
+Zip file size: 30649 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat    15389 b- defN 23-May-06 12:13 pyxtension/Json.py
+-rw-rw-rw-  2.0 fat     1885 b- defN 23-May-06 12:13 pyxtension/__init__.py
+-rw-rw-rw-  2.0 fat    11742 b- defN 23-May-06 12:15 pyxtension/fileutils.py
+-rw-rw-rw-  2.0 fat     2647 b- defN 23-May-06 12:13 pyxtension/models.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-May-06 12:13 pyxtension/racelib.py
+-rw-rw-rw-  2.0 fat    58757 b- defN 23-May-06 12:15 pyxtension/streams.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-06 12:14 pyxtension/throttler.py
+-rw-rw-rw-  2.0 fat      172 b- defN 23-May-06 12:17 pyxtension-1.16.0.data/data/requirements.txt
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-May-06 12:18 pyxtension-1.16.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    18277 b- defN 23-May-06 12:18 pyxtension-1.16.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 12:18 pyxtension-1.16.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-06 12:18 pyxtension-1.16.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1055 b- defN 23-May-06 12:18 pyxtension-1.16.0.dist-info/RECORD
+13 files, 113407 bytes uncompressed, 28897 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pyxtension/streams.py
 Comment: 
 
 Filename: pyxtension/throttler.py
 Comment: 
 
-Filename: pyxtension-1.15.0.data/data/requirements.txt
+Filename: pyxtension-1.16.0.data/data/requirements.txt
 Comment: 
 
-Filename: pyxtension-1.15.0.dist-info/LICENSE
+Filename: pyxtension-1.16.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyxtension-1.15.0.dist-info/METADATA
+Filename: pyxtension-1.16.0.dist-info/METADATA
 Comment: 
 
-Filename: pyxtension-1.15.0.dist-info/WHEEL
+Filename: pyxtension-1.16.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyxtension-1.15.0.dist-info/top_level.txt
+Filename: pyxtension-1.16.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyxtension-1.15.0.dist-info/RECORD
+Filename: pyxtension-1.16.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyxtension/fileutils.py

```diff
@@ -210,15 +210,15 @@
         self.update(self._seen_so_far + n, values)
 
     def __call__(self, el: _K) -> _K:
         """
         It's intended to be used from a mapper over a stream of values.
         It returns the same el
         # Example:
-        >>> from pyxtension.fileutils import Progbar
+        >>> from pyxtension import Progbar
         >>> stream(range(3)).map(Progbar(3)).size()
         1/3 [=========>....................] - ETA: 0s
         2/3 [===================>..........] - ETA: 0s
         3/3 [==============================] - 0s 100ms/step
         """
         self.add(1, None)
         return el
```

## pyxtension/streams.py

```diff
@@ -22,22 +22,22 @@
 from random import shuffle
 from types import GeneratorType
 from typing import AbstractSet, Any, BinaryIO, Callable, Dict, Generator, Iterable, Iterator, List, Mapping, MutableSet, \
     NamedTuple, Optional, overload, Set, Tuple, TypeVar, Union
 
 from tblib import pickling_support
 
-from pyxtension import validate, PydanticValidated
-from pyxtension.throttler import Throttler
+from pyxtension import validate, PydanticValidated, Json
+from pyxtension import Throttler
 
 ifilter = filter
 imap = map
 izip = zip
 xrange = range
-from pyxtension.fileutils import openByExtension
+from pyxtension import openByExtension
 
 from tqdm import tqdm
 
 __author__ = 'andrei.suiu@gmail.com'
 
 _K = TypeVar('_K')
 _V = TypeVar('_V')
@@ -679,15 +679,15 @@
             if k in res:
                 res[k] += v
             else:
                 res[k] = v
         return res
 
     def toJson(self) -> 'JsonList':
-        from pyxtension.Json import JsonList
+        from pyxtension import JsonList
         return JsonList(self)
 
     @overload
     def __getitem__(self, i: slice) -> 'stream[_K]':
         ...
 
     @overload
@@ -1441,15 +1441,14 @@
              postfix: Optional[dict] = None, gui: bool = False, **kwargs) -> 'stream[_K]':
         if total is None:
             total = self.size()
         return super().tqdm(desc, total, leave, file, ncols, mininterval, maxinterval, ascii, unit, unit_scale,
                             dynamic_ncols, smoothing, initial, position, postfix, gui, **kwargs)
 
     def toJson(self) -> 'sdict[_K,_V]':
-        from pyxtension.Json import Json
         return Json(self)
 
 
 class defaultstreamdict(sdict):
     @property
     def _itr(self):
         return ItrFromFunc(lambda: iter(self))
```

## pyxtension/throttler.py

```diff
@@ -1,23 +1 @@
-from collections import deque
-import time
-from typing import Any, Callable
-
-
-class Throttler:
-    def __init__(self, max_req: int, period: float, time_func: Callable[[], float] = time.time) -> None:
-        self._max_req = max_req
-        self._period = period
-        self._request_timestamps = deque(maxlen=max_req)
-        self._req_cnt = 0
-        self._time_func = time_func
-
-    def throttle(self, val: Any) -> Any:
-        t1 = self._time_func()
-        self._req_cnt += 1
-        self._request_timestamps.append(t1)
-        if len(self._request_timestamps) >= self._max_req:
-            t0 = self._request_timestamps[0]
-            dt = t1 - t0
-            if dt < self._period:
-                time.sleep(self._period - dt)
-        return val
+from throttlex import *
```

## Comparing `pyxtension-1.15.0.dist-info/LICENSE` & `pyxtension-1.16.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyxtension-1.15.0.dist-info/METADATA` & `pyxtension-1.16.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,656 +1,536 @@
 Metadata-Version: 2.1
 Name: pyxtension
-Version: 1.15.0
+Version: 1.16.0
 Summary: Extension library for Python
 Home-page: https://github.com/asuiu/pyxtension
 Author: Andrei Suiu
 Author-email: andrei.suiu@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: json-composite-encoder (>=1.0.0)
+Requires-Dist: streamerate (>=1.0.0)
+Requires-Dist: throttlex (>=1.0.0)
 Requires-Dist: tqdm (>=4.62.0) ; python_version >= "3"
 Requires-Dist: pydantic (>=1.8.2) ; python_version >= "3"
 Requires-Dist: tblib (>=1.7.0) ; python_version >= "3"
 Provides-Extra: dev
-Requires-Dist: mock ; (python_version < "3") and extra == 'dev'
+Requires-Dist: twine (>=4.0.1) ; extra == 'dev'
+Requires-Dist: tsx (>=0.0.1) ; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: mock ; (python_version < "3") and extra == 'test'
-
-pyxtension
-==========
-
-| |build Status|
-| |Coverage Status|
-
-`pyxtension <https://github.com/asuiu/pyxtension>`__ is a pure Python
-MIT-licensed library that includes Scala-like streams, Json with
-attribute access syntax, and other common-use stuff.
-
-Installation
-------------
-
-::
-
-    pip install pyxtension
+Requires-Dist: twine (>=4.0.1) ; extra == 'test'
+Requires-Dist: tsx (>=0.0.1) ; extra == 'test'
 
+# pyxtension
+[![build Status](https://travis-ci.org/asuiu/pyxtension.svg?branch=master)](https://travis-ci.org/asuiu/pyxtension)
+[![Coverage Status](https://coveralls.io/repos/asuiu/pyxtension/badge.svg?branch=master&service=github)](https://coveralls.io/github/asuiu/pyxtension?branch=master)
+
+[pyxtension](https://github.com/asuiu/pyxtension) is a pure Python MIT-licensed library that includes Scala-like streams (using [Fluent Interface pattern](https://en.wikipedia.org/wiki/Fluent_interface)), Json with attribute access syntax, and other common-use stuff.
+
+###### Note:
+
+**Drop support & maintenance for Python 2.x version, due to [Py2 death](https://www.python.org/doc/sunset-python-2/).**
+ 
+ Although Py2 version will remain in the repository, I won't update PyPi package, so the last Py2 version of the `pyxtension` available at [PyPi](https://pypi.org/project/pyxtension/) will remain [`1.12.7`](https://pypi.org/project/pyxtension/1.12.7/)
+
+Starting with [`1.13.0`](https://pypi.org/project/pyxtension/1.13.0/) I've migrated the packaging & distributing method to [Wheel](https://pythonwheels.com/).
+      
+## Installation
+```
+pip install pyxtension
+```
 or from Github:
-
-::
-
-    git clone https://github.com/asuiu/pyxtension.git
-    cd pyxtension
-    python setup.py install
-
+```
+git clone https://github.com/asuiu/pyxtension.git
+cd pyxtension
+python setup.py install
+```
 or
-
-::
-
-    git submodule add https://github.com/asuiu/pyxtension.git
-
-Modules overview
-----------------
-
-Json.py
-~~~~~~~
-
-Json
-^^^^
-
-| A ``dict`` subclass to represent a Json object. You should be able to
-  use this
-| absolutely anywhere you can use a ``dict``. While this is probably the
-  class you
-| want to use, there are a few caveats that follow from this being a
-  ``dict`` under
-| the hood.
+```
+git submodule add https://github.com/asuiu/pyxtension.git
+```
+
+## Modules overview
+### Json.py
+##### Json
+A `dict` subclass to represent a Json object. You should be able to use this
+absolutely anywhere you can use a `dict`. While this is probably the class you
+want to use, there are a few caveats that follow from this being a `dict` under
+the hood.
 
 **Never again will you have to write code like this**:
-
-.. code:: python
-
-            body = {
-                'query': {
-                    'filtered': {
-                        'query': {
-                            'match': {'description': 'addictive'}
-                        },
-                        'filter': {
-                            'term': {'created_by': 'ASU'}
-                        }
-                    }
-                }
+```python
+body = {
+    'query': {
+        'filtered': {
+            'query': {
+                'match': {'description': 'addictive'}
+            },
+            'filter': {
+                'term': {'created_by': 'ASU'}
             }
+        }
+    }
+}
+```
 
 From now on, you may simply write the following three lines:
+```python
+body = Json()
+body.query.filtered.query.match.description = 'addictive'
+body.query.filtered.filter.term.created_by = 'ASU'
+```
+### streams.py
+#### stream
+`stream` subclasses `collections.Iterable`. It's the same Python iterable, but with more added methods, suitable for multithreading and multiprocess processings.
+Used to create stream processing pipelines, similar to those used in [Scala](http://www.scala-lang.org/) and [MapReduce](https://en.wikipedia.org/wiki/MapReduce) programming model.
+Those who used [Apache Spark](http://spark.apache.org/) [RDD](http://spark.apache.org/docs/latest/programming-guide.html#rdd-operations) functions will find this model of processing very easy to use.
 
-.. code:: python
-
-            body = Json()
-            body.query.filtered.query.match.description = 'addictive'
-            body.query.filtered.filter.term.created_by = 'ASU'
-
-streams.py
-~~~~~~~~~~
-
-stream
-^^^^^^
-
-| ``stream`` subclasses ``collections.Iterable``. It's the same Python
-  iterable, but with more added methods, suitable for multithreading and
-  multiprocess processings.
-| Used to create stream processing pipelines, similar to those used in
-  `Scala <http://www.scala-lang.org/>`__ and
-  `MapReduce <https://en.wikipedia.org/wiki/MapReduce>`__ programming
-  model.
-| Those who used `Apache Spark <http://spark.apache.org/>`__
-  `RDD <http://spark.apache.org/docs/latest/programming-guide.html#rdd-operations>`__
-  functions will find this model of processing very easy to use.
-
-`streams <https://github.com/asuiu/pyxtension/blob/master/streams.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
+### [streams](https://github.com/asuiu/pyxtension/blob/master/streams.py)
 **Never again will you have to write code like this**:
+```python
+> lst = xrange(1,6)
+> reduce(lambda x, y: x * y, map(lambda _: _ * _, filter(lambda _: _ % 2 == 0, lst)))
+64
+```
+From now on, you may simply write the following lines:
+```python
+> the_stream = stream( xrange(1,6) )
+> the_stream.\
+    filter(lambda _: _ % 2 == 0).\
+    map(lambda _: _ * _).\
+    reduce(lambda x, y: x * y)
+64
+```
 
-.. code:: python
+#### A Word Count [Map-Reduce](https://en.wikipedia.org/wiki/MapReduce) naive example using multiprocessing map
+```python
+corpus = [
+    "MapReduce is a programming model and an associated implementation for processing and generating large data sets with a parallel, distributed algorithm on a cluster.",
+    "At Google, MapReduce was used to completely regenerate Google's index of the World Wide Web",
+    "Conceptually similar approaches have been very well known since 1995 with the Message Passing Interface standard having reduce and scatter operations."]
 
-    > lst = xrange(1,6)
-    > reduce(lambda x, y: x * y, map(lambda _: _ * _, filter(lambda _: _ % 2 == 0, lst)))
-    64
+def reduceMaps(m1, m2):
+    for k, v in m2.iteritems():
+        m1[k] = m1.get(k, 0) + v
+    return m1
 
-From now on, you may simply write the following lines:
+word_counts = stream(corpus).\
+    mpmap(lambda line: stream(line.lower().split(' ')).countByValue()).\
+    reduce(reduceMaps)
+```
 
-.. code:: python
+#### Basic methods
+###### **map(f)**
+Identic with builtin `map` but returns a stream
 
-    > the_stream = stream( xrange(1,6) )
-    > the_stream.\
-        filter(lambda _: _ % 2 == 0).\
-        map(lambda _: _ * _).\
-        reduce(lambda x, y: x * y)
-    64
 
-A Word Count `Map-Reduce <https://en.wikipedia.org/wiki/MapReduce>`__ naive example using multiprocessing map
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+###### **mpmap(self, f: Callable[[_K], _V], poolSize: int = cpu_count(), bufferSize: Optional[int] = None)**
+Parallel ordered map using `multiprocessing.Pool.imap()`.
 
-.. code:: python
+It can replace the `map` when need to split computations to multiple cores, and order of results matters.
 
-    corpus = [
-        "MapReduce is a programming model and an associated implementation for processing and generating large data sets with a parallel, distributed algorithm on a cluster.",
-        "At Google, MapReduce was used to completely regenerate Google's index of the World Wide Web",
-        "Conceptually similar approaches have been very well known since 1995 with the Message Passing Interface standard having reduce and scatter operations."]
+It spawns at most `poolSize` processes and applies the `f` function.
 
-    def reduceMaps(m1, m2):
-        for k, v in m2.iteritems():
-            m1[k] = m1.get(k, 0) + v
-        return m1
+It won't take more than `bufferSize` elements from the input unless it was already required by output, so you can use it with `takeWhile` on infinite streams and not be afraid that it will continue work in background.
 
-    word_counts = stream(corpus).\
-        mpmap(lambda line: stream(line.lower().split(' ')).countByValue()).\
-        reduce(reduceMaps)
+The elements in the result stream appears in the same order they appear in the initial iterable.
 
-Basic methods
-^^^^^^^^^^^^^
+```
+:type f: (T) -> V
+:rtype: `stream`
+```
 
-**map(f)**
-''''''''''
 
-Identic with builtin ``map`` but returns a stream
+###### **mpfastmap(self, f: Callable[[_K], _V], poolSize: int = cpu_count(), bufferSize: Optional[int] = None)**
+Parallel ordered map using `multiprocessing.Pool.imap_unordered()`.
 
-**mpmap(f, poolSize=16)**
-'''''''''''''''''''''''''
+It can replace the `map` when the ordered of results doesn't matter.
 
-Parallel ordered map using ``multiprocessing.Pool.imap()``.
+It spawns at most `poolSize` processes and applies the `f` function.
 
-It can replace the ``map`` when need to split computations to multiple
-cores, and order of results matters.
+It won't take more than `bufferSize` elements from the input unless it was already required by output, so you can use it with `takeWhile` on infinite streams and not be afraid that it will continue work in background.
 
-It spawns at most ``poolSize`` processes and applies the ``f`` function.
+The elements in the result stream appears in the unpredicted order.
 
-The elements in the result stream appears in the same order they appear
-in the initial iterable.
+```
+:type f: (T) -> V
+:rtype: `stream`
+```
 
-::
 
-    :type f: (T) -> V
-    :rtype: `stream`
+###### **fastmap(self, f: Callable[[_K], _V], poolSize: int = cpu_count(), bufferSize: Optional[int] = None)**
+Parallel unordered map using multithreaded pool.
+It can replace the `map` when the ordered of results doesn't matter.
 
-**mpfastmap(f, poolSize=16)**
-'''''''''''''''''''''''''''''
+It spawns at most `poolSize` threads and applies the `f` function.
 
-Parallel ordered map using ``multiprocessing.Pool.imap_unordered()``.
+The elements in the result stream appears in the **unpredicted** order.
 
-It can replace the ``map`` when the ordered of results doesn't matter.
+It won't take more than `bufferSize` elements from the input unless it was already required by output, so you can use it with `takeWhile` on infinite streams and not be afraid that it will continue work in background.
 
-It spawns at most ``poolSize`` processes and applies the ``f`` function.
+Because of CPython [GIL](https://wiki.python.org/moin/GlobalInterpreterLock) it's most usefull for I/O or CPU intensive consuming native functions, or on Jython or IronPython interpreters.
 
-The elements in the result stream appears in the unpredicted order.
-
-::
+:type f: (T) -> V
 
-    :type f: (T) -> V
-    :rtype: `stream`
+:rtype: `stream`
 
-**fastmap(f, poolSize=16)**
-'''''''''''''''''''''''''''
+###### **mtmap(self, f: Callable[[_K], _V], poolSize: int = cpu_count(), bufferSize: Optional[int] = None)**
+Parallel ordered map using multithreaded pool. 
+It can replace the `map` and the order of output stream will be the same as of the input.
 
-| Parallel unordered map using multithreaded pool.
-| It can replace the ``map`` when the ordered of results doesn't matter.
+It spawns at most `poolSize` threads and applies the `f` function.
 
-It spawns at most ``poolSize`` threads and applies the ``f`` function.
+The elements in the result stream appears in the **predicted** order.
 
-The elements in the result stream appears in the unpredicted order.
+It won't take more than `bufferSize` elements from the input unless it was already required by output, so you can use it with `takeWhile` on infinite streams and not be afraid that it will continue work in background.  
 
-Because of CPython
-`GIL <https://wiki.python.org/moin/GlobalInterpreterLock>`__ it's most
-usefull for I/O or CPU intensive consuming native functions, or on
-Jython or IronPython interpreters.
+Because of CPython [GIL](https://wiki.python.org/moin/GlobalInterpreterLock) it's most usefull for I/O or CPU intensive consuming native functions, or on Jython or IronPython interpreters.
 
 :type f: (T) -> V
 
-:rtype: ``stream``
+:rtype: `stream`
 
-\*\*flatMap(predicate=\_IDENTITY\_FUNC)\*\*
+
+###### **flatMap(predicate=_IDENTITY_FUNC)**
 :param predicate: is a function that will receive elements of self collection and return an iterable
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 By default predicate is an identity function
 
 :type predicate: (V)-> collections.Iterable[T]
 
 :return: will return stream of objects of the same type of elements from the stream returned by predicate()
 
 Example:
+```python
+stream([[1, 2], [3, 4], [4, 5]]).flatMap().toList() == [1, 2, 3, 4, 4, 5]
+```
 
-.. code:: python
-
-    stream([[1, 2], [3, 4], [4, 5]]).flatMap().toList() == [1, 2, 3, 4, 4, 5]
-
-**filter(predicate)**
-'''''''''''''''''''''
 
+###### **filter(predicate)**
 identic with builtin filter, but returns stream
 
-**reversed()**
-''''''''''''''
 
+###### **reversed()**
 returns reversed stream
 
-**exists(predicate)**
-'''''''''''''''''''''
 
-Tests whether a predicate holds for some of the elements of this
-sequence.
+###### **exists(predicate)**
+Tests whether a predicate holds for some of the elements of this sequence.
 
 :rtype: bool
 
 Example:
+```python
+stream([1, 2, 3]).exists(0) -> False
+stream([1, 2, 3]).exists(1) -> True
+```
 
-.. code:: python
 
-    stream([1, 2, 3]).exists(0) -> False
-    stream([1, 2, 3]).exists(1) -> True
-
-\*\*keyBy(keyfunc = \_IDENTITY\_FUNC)\*\*
+###### **keyBy(keyfunc = _IDENTITY_FUNC)**
 Transforms stream of values to a stream of tuples (key, value)
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
 :param keyfunc: function to map values to keys
 
 :type keyfunc: (V) -> T
 
 :return: stream of Key, Value pairs
 
 :rtype: stream[( T, V )]
 
 Example:
+```python
+stream([1, 2, 3, 4]).keyBy(lambda _:_ % 2) -> [(1, 1), (0, 2), (1, 3), (0, 4)]
+```
 
-.. code:: python
-
-    stream([1, 2, 3, 4]).keyBy(lambda _:_ % 2) -> [(1, 1), (0, 2), (1, 3), (0, 4)]
-
-**groupBy()**
-'''''''''''''
+###### **groupBy()**
+groupBy([keyfunc]) -> Make an iterator that returns consecutive keys and groups from the iterable.
 
-groupBy([keyfunc]) -> Make an iterator that returns consecutive keys and
-groups from the iterable.
-
-The iterable needs not to be sorted on the same key function, but the
-keyfunction need to return hasable objects.
+The iterable needs not to be sorted on the same key function, but the keyfunction need to return hasable objects.
 
 :param keyfunc: [Optional] The key is a function computing a key value for each element.
 
 :type keyfunc: (T) -> (V)
 
 :return: (key, sub-iterator) grouped by each value of key(value).
 
 :rtype: stream[ ( V, slist[T] ) ]
 
 Example:
+```python
+stream([1, 2, 3, 4]).groupBy(lambda _: _ % 2) -> [(0, [2, 4]), (1, [1, 3])]
+```
 
-.. code:: python
-
-    stream([1, 2, 3, 4]).groupBy(lambda _: _ % 2) -> [(0, [2, 4]), (1, [1, 3])]
-
-**countByValue()**
-''''''''''''''''''
-
+###### **countByValue()**
 Returns a collections.Counter of values
 
 Example
+```python
+stream(['a', 'b', 'a', 'b', 'c', 'd']).countByValue() == {'a': 2, 'b': 2, 'c': 1, 'd': 1}
+```
 
-.. code:: python
-
-    stream(['a', 'b', 'a', 'b', 'c', 'd']).countByValue() == {'a': 2, 'b': 2, 'c': 1, 'd': 1}
-
-**distinct()**
-''''''''''''''
-
+###### **distinct()**
 Returns stream of distinct values. Values must be hashable.
+```python
+stream(['a', 'b', 'a', 'b', 'c', 'd']).distinct() == {'a', 'b', 'c', 'd'}
+```
 
-.. code:: python
-
-    stream(['a', 'b', 'a', 'b', 'c', 'd']).distinct() == {'a', 'b', 'c', 'd'}
-
-**reduce(f, init=None)**
-''''''''''''''''''''''''
 
+###### **reduce(f, init=None)**
 same arguments with builtin reduce() function
 
-**toSet()**
-'''''''''''
 
+###### **toSet()**
 returns sset() instance
 
-**toList()**
-''''''''''''
 
+###### **toList()**
 returns slist() instance
 
-**toMap()**
-'''''''''''
 
+###### **toMap()**
 returns sdict() instance
 
-**sorted(key=None, cmp=None, reverse=False)**
-'''''''''''''''''''''''''''''''''''''''''''''
 
+###### **sorted(key=None, cmp=None, reverse=False)**
 same arguments with builtin sorted()
 
-**size()**
-''''''''''
 
+###### **size()**
 returns length of stream. Use carefully on infinite streams.
 
-**join(f)**
-'''''''''''
 
-Returns a string joined by f. Proivides same functionality as str.join()
-builtin method.
+###### **join(f)**
+Returns a string joined by f. Proivides same functionality as str.join() builtin method.
 
-if f is basestring, uses it to join the stream, else f should be a
-callable that returns a string to be used for join
+if f is basestring, uses it to join the stream, else f should be a callable that returns a string to be used for join
 
-**mkString(f)**
-'''''''''''''''
 
+###### **mkString(f)**
 identic with join(f)
 
-**take(n)**
-'''''''''''
-
-::
 
+###### **take(n)**
     returns first n elements from stream
 
-**head()**
-''''''''''
-
-::
 
+###### **head()**
     returns first element from stream
 
-**zip()**
-'''''''''
-
-::
 
+###### **zip()**
     the same behavior with itertools.izip()
 
-**throttle(max_req: int, interval: float)**
-'''''''''
-
-::
-
-    throttles to process at most max_req elements pe every 'interval' seconds.
-
-
-\*\*unique(predicate=\_IDENTITY\_FUNC)\*\*
-Returns a stream of unique (according to predicate) elements appearing in the same order as in original stream
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
-
-::
+###### **unique(predicate=_IDENTITY_FUNC)**
+    Returns a stream of unique (according to predicate) elements appearing in the same order as in original stream
 
     The items returned by predicate should be hashable and comparable.
 
-Statistics related methods
-^^^^^^^^^^^^^^^^^^^^^^^^^^
-
-**entropy()**
-'''''''''''''
 
+#### Statistics related methods
+###### **entropy()**
 calculates the Shannon entropy of the values from stream
 
-**pstddev()**
-'''''''''''''
 
+###### **pstddev()**
 Calculates the population standard deviation.
 
-**mean()**
-''''''''''
 
+###### **mean()**
 returns the arithmetical mean of the values
 
-**sum()**
-'''''''''
 
+###### **sum()**
 returns the sum of elements from stream
 
-\*\*min(key=\_IDENTITY\_FUNC)\*\*
+
+###### **min(key=_IDENTITY_FUNC)**
 same functionality with builtin min() funcion
-'''''''''''''''''''''''''''''''''''''''''''''
 
-\*\*min\_default(default, key=\_IDENTITY\_FUNC)\*\*
+
+###### **min_default(default, key=_IDENTITY_FUNC)**
 same functionality with min() but returns :default: when called on empty streams
-''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''''
 
-**max()**
-'''''''''
 
+###### **max()**
 same functionality with builtin max()
 
-\*\*maxes(key=\_IDENTITY\_FUNC)\*\*
-returns a stream of max values from stream
-''''''''''''''''''''''''''''''''''''''''''
-
-\*\*mins(key=\_IDENTITY\_FUNC)\*\*
-returns a stream of min values from stream
-''''''''''''''''''''''''''''''''''''''''''
-
-Other classes
-~~~~~~~~~~~~~
-
-slist
-^^^^^
-
-Inherits ``streams.stream`` and built-in ``list`` classes, and keeps in
-memory a list allowing faster index access
-
-sset
-^^^^
-
-Inherits ``streams.stream`` and built-in ``set`` classes, and keeps in
-memory the whole set of values
-
-sdict
-^^^^^
-
-Inherits ``streams.stream`` and built-in ``dict``, and keeps in memory
-the dict object.
-
-defaultstreamdict
-^^^^^^^^^^^^^^^^^
-
-Inherits ``streams.sdict`` and adds functionality of
-``collections.defaultdict`` from stdlib
-
-`throttler <https://github.com/asuiu/pyxtension/blob/master/throttler.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-Thread-safe time throttler that can be attached on a stream to limit the number of calls per time interval.
-Example:
-
-.. code:: python
-
-        > from pyxtension.throttler import Throttler
-        > throttler = Throttler(5, 10)
-        > stream(range(100)).map(throttler.throttle).map(print).to_list()
-
-
-it will throttle the stream to max 5 calls per every 10 seconds.
 
-`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-`Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__ is a
-module that provides mapping objects that allow their elements to be
-accessed both as keys and as attributes:
-
-.. code:: python
-
-        > from pyxtension.Json import Json
-        > a = Json({'foo': 'bar'})
-        > a.foo
-        'bar'
-        > a['foo']
-        'bar'
-
-Attribute access makes it easy to create convenient, hierarchical
-settings objects:
-
-.. code:: python
-
-        with open('settings.yaml') as fileobj:
-            settings = Json(yaml.safe_load(fileobj))
-
-        cursor = connect(**settings.db.credentials).cursor()
-
-        cursor.execute("SELECT column FROM table;")
-
-Basic Usage
-~~~~~~~~~~~
-
-| Json comes with two different classes, ``Json``, and ``JsonList``.
-| Json is fairly similar to native ``dict`` as it extends it an is a
-  mutable mapping that allow creating, accessing, and deleting key-value
-  pairs as attributes.
-| ``JsonList`` is similar to native ``list`` as it extends it and offers
-  a way to transform the ``dict`` objects from inside also in ``Json``
-  instances.
-
-Construction
-^^^^^^^^^^^^
-
-Directly from a JSON string
-'''''''''''''''''''''''''''
-
-.. code:: python
-
-    > Json('{"key1": "val1", "lst1": [1,2] }')
-    {u'key1': u'val1', u'lst1': [1, 2]}
-
-From ``tuple``\ s:
-''''''''''''''''''
-
-.. code:: python
-
-    > Json( ('key1','val1'), ('lst1', [1,2]) )
-    {'key1': 'val1', 'lst1': [1, 2]}
-    # keep in mind that you should provide at least two tuples with key-value pairs
-
-As a built-in ``dict``
-''''''''''''''''''''''
-
-.. code:: python
-
-    > Json( [('key1','val1'), ('lst1', [1,2])] )
-    {'key1': 'val1', 'lst1': [1, 2]}
+###### **maxes(key=_IDENTITY_FUNC)**
+returns a stream of max values from stream
 
-    Json({'key1': 'val1', 'lst1': [1, 2]})
-    {'key1': 'val1', 'lst1': [1, 2]}
 
-Convert to a ``dict``
-^^^^^^^^^^^^^^^^^^^^^
+###### **mins(key=_IDENTITY_FUNC)**
+returns a stream of min values from stream
 
-.. code:: python
 
-    > json = Json({'key1': 'val1', 'lst1': [1, 2]})
-    > json.toOrig()
-    {'key1': 'val1', 'lst1': [1, 2]}
+### Other classes
+##### slist
+Inherits `streams.stream` and built-in `list` classes, and keeps in memory a list allowing faster index access
+##### sset
+Inherits `streams.stream` and built-in `set` classes, and keeps in memory the whole set of values
+##### sdict
+Inherits `streams.stream` and built-in `dict`, and keeps in memory the dict object.
+##### defaultstreamdict
+Inherits `streams.sdict` and adds functionality  of `collections.defaultdict` from stdlib
+
+
+### [Json](https://github.com/asuiu/pyxtension/blob/master/Json.py)
+
+[Json](https://github.com/asuiu/pyxtension/blob/master/Json.py) is a module that provides mapping objects that allow their elements to be accessed both as keys and as attributes:
+
+```python
+    > from pyxtension import Json
+> a = Json({'foo': 'bar'})
+> a.foo
+'bar'
+> a['foo']
+'bar'
+```
+
+Attribute access makes it easy to create convenient, hierarchical settings objects:
+```python
+    with open('settings.yaml') as fileobj:
+        settings = Json(yaml.safe_load(fileobj))
+
+    cursor = connect(**settings.db.credentials).cursor()
+
+    cursor.execute("SELECT column FROM table;")
+```
+
+### Basic Usage
+
+Json comes with two different classes, `Json`, and `JsonList`.
+Json is fairly similar to native `dict` as it extends it an is a mutable mapping that allow creating, accessing, and deleting key-value pairs as attributes.
+`JsonList` is similar to native `list` as it extends it and offers a way to transform the `dict` objects from inside also in `Json` instances.
+
+#### Construction
+###### Directly from a JSON string
+```python
+> Json('{"key1": "val1", "lst1": [1,2] }')
+{u'key1': u'val1', u'lst1': [1, 2]}
+```
+###### From `tuple`s:
+```python
+> Json( ('key1','val1'), ('lst1', [1,2]) )
+{'key1': 'val1', 'lst1': [1, 2]}
+# keep in mind that you should provide at least two tuples with key-value pairs
+```
+###### As a built-in `dict`
+```python
+> Json( [('key1','val1'), ('lst1', [1,2])] )
+{'key1': 'val1', 'lst1': [1, 2]}
+
+Json({'key1': 'val1', 'lst1': [1, 2]})
+{'key1': 'val1', 'lst1': [1, 2]}
+```
+#### Convert to a `dict`
+```python
+> json = Json({'key1': 'val1', 'lst1': [1, 2]})
+> json.toOrig()
+{'key1': 'val1', 'lst1': [1, 2]}
+```
 
-Valid Names
-^^^^^^^^^^^
+#### Valid Names
 
 Any key can be used as an attribute as long as:
 
-#. The key represents a valid attribute (i.e., it is a string comprised
-   only of
-   alphanumeric characters and underscores that doesn't start with a
-   number)
-#. The key does not shadow a class attribute (e.g., get).
-
-Attributes vs. Keys
-^^^^^^^^^^^^^^^^^^^
-
-| There is a minor difference between accessing a value as an attribute
-  vs.
-| accessing it as a key, is that when a dict is accessed as an
-  attribute, it will
-| automatically be converted to a ``Json`` object. This allows you to
-  recursively
-| access keys::
-
-.. code:: python
-
-        > attr = Json({'foo': {'bar': 'baz'}})
-        > attr.foo.bar
-        'baz'
-
-| Relatedly, by default, sequence types that aren't ``bytes``, ``str``,
-  or ``unicode``
-| (e.g., ``list``\ s, ``tuple``\ s) will automatically be converted to
-  ``tuple``\ s, with any
-| mappings converted to ``Json``:
-
-.. code:: python
-
-        > attr = Json({'foo': [{'bar': 'baz'}, {'bar': 'qux'}]})
-        > for sub_attr in attr.foo:
-        >     print(sub_attr.bar)
-        'baz'
-        'qux'
-
-| To get this recursive functionality for keys that cannot be used as
-  attributes,
-| you can replicate the behavior by using dict syntax on ``Json``
-  object::
-
-
-.. code:: python
-
-        > json = Json({1: {'two': 3}})
-        > json[1].two
-        3
-
-``JsonList`` usage examples:
-
-.. code:: python
-
-    > json = Json('{"lst":[1,2,3]}')
-    > type(json.lst)
-    <class 'pyxtension.Json.JsonList'>
-
-    > json = Json('{"1":[1,2]}')
-    > json["1"][1]
-    2
+1. The key represents a valid attribute (i.e., it is a string comprised only of
+   alphanumeric characters and underscores that doesn't start with a number)
+2. The key does not shadow a class attribute (e.g., get).
+
+#### Attributes vs. Keys
+There is a minor difference between accessing a value as an attribute vs.
+accessing it as a key, is that when a dict is accessed as an attribute, it will
+automatically be converted to a `Json` object. This allows you to recursively
+access keys::
+```python
+    > attr = Json({'foo': {'bar': 'baz'}})
+    > attr.foo.bar
+    'baz'
+```
+Relatedly, by default, sequence types that aren't `bytes`, `str`, or `unicode`
+(e.g., `list`s, `tuple`s) will automatically be converted to `tuple`s, with any
+mappings converted to `Json`:
+```python
+    > attr = Json({'foo': [{'bar': 'baz'}, {'bar': 'qux'}]})
+    > for sub_attr in attr.foo:
+    >     print(sub_attr.bar)
+    'baz'
+    'qux'
+```
+To get this recursive functionality for keys that cannot be used as attributes,
+you can replicate the behavior by using dict syntax on `Json` object::
+```python
+> json = Json({1: {'two': 3}})
+> json[1].two
+3
+```
+`JsonList` usage examples:
+```
+> json = Json('{"lst":[1,2,3]}')
+> type(json.lst)
+<class 'pyxtension.Json.JsonList'>
+
+> json = Json('{"1":[1,2]}')
+> json["1"][1]
+2
+```
+
 
 Assignment as keys will still work::
+```python
+> json = Json({'foo': {'bar': 'baz'}})
+> json['foo']['bar'] = 'baz'
+> json.foo
+{'bar': 'baz'}
+```
+
+### frozendict
+`frozendict` is a simple immutable dictionary, where you can't change the internal variables of the class, and they are all immutable objects. Reinvoking `__init__` also doesn't alter the object.
+
+The API is the same as `dict`, without methods that can change the immutability. 
+
+`frozendict` is also hashable and can be used as keys for other dictionaries, of course with the condition that all values of the frozendict are also hashable.
+
+```python
+>>> from pyxtension import frozendict
+
+>>> fd = frozendict({"A": "B", "C": "D"})
+>>> print(fd)
+{'A': 'B', 'C': 'D'}
+
+>>> fd["A"] = "C"
+TypeError: object is immutable
+
+>>> hash(fd)
+-5063792767678978828
+```
+
+### License
+pyxtension is released under a GNU Public license.
+The idea for [Json](https://github.com/asuiu/pyxtension/blob/master/Json.py) module was inspired from [addict](https://github.com/mewwts/addict) and [AttrDict](https://github.com/bcj/AttrDict),
+but it has a better performance with lower memory consumption.
+
+### Alternatives
+There are other libraries that support Fluent Interface streams as alternatives to Pyxtension, but being much more poor in features for streaming:
+- https://pypi.org/project/lazy-streams/
+- https://pypi.org/project/pystreams/
+- https://pypi.org/project/fluentpy/
+- https://github.com/matthagy/scalaps
+- https://pypi.org/project/infixpy/ mentioned [here](https://stackoverflow.com/questions/49001986/left-to-right-application-of-operations-on-a-list-in-python3/62585964?noredirect=1#comment111806251_62585964)
+- https://github.com/sspipe/sspipe
 
-.. code:: python
 
-        > json = Json({'foo': {'bar': 'baz'}})
-        > json['foo']['bar'] = 'baz'
-        > json.foo
-        {'bar': 'baz'}
-
-License
-~~~~~~~
-
-| pyxtension is released under a GNU Public license.
-| The idea for
-  `Json <https://github.com/asuiu/pyxtension/blob/master/Json.py>`__
-  module was inspired from
-  `addict <https://github.com/mewwts/addict%3E>`__ and
-  `AttrDict <https://github.com/bcj/AttrDict>`__,
-| but it has a better performance with lower memory consumption.
-
-.. |build Status| image:: https://travis-ci.org/asuiu/pyxtension.svg?branch=master
-   :target: https://travis-ci.org/asuiu/pyxtension
-.. |Coverage Status| image:: https://coveralls.io/repos/asuiu/pyxtension/badge.svg?branch=master&service=github
-   :target: https://coveralls.io/github/asuiu/pyxtension?branch=master
+and something quite different from Fluent patterm, that makes kind of Piping: https://github.com/sspipe/sspipe and https://github.com/JulienPalard/Pipe
```

