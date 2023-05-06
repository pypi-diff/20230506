# Comparing `tmp/pydio-0.3.3.tar.gz` & `tmp/pydio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydio-0.3.3.tar", max compression
+gzip compressed data, was "pydio-0.4.0.tar", max compression
```

## Comparing `pydio-0.3.3.tar` & `pydio-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1094 2022-11-05 12:48:59.300964 pydio-0.3.3/LICENSE.txt
--rw-r--r--   0        0        0     3064 2022-11-05 12:48:59.300964 pydio-0.3.3/README.md
--rw-r--r--   0        0        0      525 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/__init__.py
--rw-r--r--   0        0        0      517 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/_compat.py
--rw-r--r--   0        0        0     2770 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/_factories.py
--rw-r--r--   0        0        0     2545 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/_unbound_factories.py
--rw-r--r--   0        0        0      845 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/api.py
--rw-r--r--   0        0        0     6251 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/base.py
--rw-r--r--   0        0        0     1765 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/exc.py
--rw-r--r--   0        0        0     6448 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/injector.py
--rw-r--r--   0        0        0     1663 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/keys.py
--rw-r--r--   0        0        0     4942 2022-11-05 12:48:59.300964 pydio-0.3.3/pydio/provider.py
--rw-r--r--   0        0        0     1568 2022-11-05 12:48:59.300964 pydio-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 pydio-0.3.3/setup.py
--rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 pydio-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-06 07:24:30.230336 pydio-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3064 2023-05-06 07:24:30.230336 pydio-0.4.0/README.md
+-rw-r--r--   0        0        0      525 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_compat.py
+-rw-r--r--   0        0        0     3458 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_factories.py
+-rw-r--r--   0        0        0     2545 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/_unbound_factories.py
+-rw-r--r--   0        0        0      845 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/api.py
+-rw-r--r--   0        0        0     7043 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/base.py
+-rw-r--r--   0        0        0     1765 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/exc.py
+-rw-r--r--   0        0        0     7221 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/injector.py
+-rw-r--r--   0        0        0     1663 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/keys.py
+-rw-r--r--   0        0        0     4942 2023-05-06 07:24:30.230336 pydio-0.4.0/pydio/provider.py
+-rw-r--r--   0        0        0     1568 2023-05-06 07:24:30.230336 pydio-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3764 1970-01-01 00:00:00.000000 pydio-0.4.0/setup.py
+-rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 pydio-0.4.0/PKG-INFO
```

### Comparing `pydio-0.3.3/LICENSE.txt` & `pydio-0.4.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `pydio-0.3.3/README.md` & `pydio-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pydio-0.3.3/pydio/__init__.py` & `pydio-0.4.0/pydio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ---------------------------------------------------------------------------
 # pydio/__init__.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 __released__ = 2021
 __author__ = 'Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>'
-__version__ = '0.3.3'
+__version__ = '0.4.0'
```

### Comparing `pydio-0.3.3/pydio/_compat.py` & `pydio-0.4.0/pydio/_compat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/_compat.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 from contextlib import AbstractAsyncContextManager
```

### Comparing `pydio-0.3.3/pydio/_factories.py` & `pydio-0.4.0/pydio/_factories.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/_factories.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 from .base import IFactory
@@ -21,22 +21,30 @@
         self._instance = _UNDEFINED
 
     def get_instance(self):
         if self._instance is _UNDEFINED:
             self._instance = next(self._generator)
         return self._instance
 
-    def close(self):
+    def close(self, exc_type=None, exc=None, tb=None):
         prev_instance = self._instance
         self._instance = None
         if prev_instance is not _UNDEFINED:
-            try:
-                next(self._generator)
-            except StopIteration:
-                pass
+            if exc_type is None:
+                try:
+                    next(self._generator)
+                except StopIteration:
+                    pass
+            else:
+                try:
+                    self._generator.throw(exc_type, exc, tb)
+                except StopIteration:
+                    raise exc
+                else:
+                    raise
 
 
 class AsyncGeneratorFactory(IFactory):
     awaitable = True
 
     def __init__(self, func):
         self._generator = func()
@@ -47,24 +55,30 @@
         async def async_get_instance():
             if self._instance is _UNDEFINED:
                 self._instance = await self._generator.__anext__()
             return self._instance
 
         return async_get_instance()
 
-    def close(self):
+    def close(self, exc_type=None, exc=None, tb=None):
 
         async def async_close():
             prev_instance = self._instance
             self._instance = None
             if prev_instance is not _UNDEFINED:
-                try:
-                    await self._generator.__anext__()
-                except StopAsyncIteration:
-                    pass
+                if exc_type is None:
+                    try:
+                        await self._generator.__anext__()
+                    except StopAsyncIteration:
+                        pass
+                else:
+                    try:
+                        await self._generator.athrow(exc_type, exc, tb)
+                    except StopAsyncIteration:
+                        raise exc
 
         return async_close()
 
 
 class CoroutineFactory(IFactory):
     awaitable = True
 
@@ -77,15 +91,15 @@
         async def async_get_instance():
             if self._instance is _UNDEFINED:
                 self._instance = await self._awaitable
             return self._instance
 
         return async_get_instance()
 
-    def close(self):
+    def close(self, exc_type=None, exc=None, tb=None):
 
         async def async_close():
             self._instance = None
 
         return async_close()
 
 
@@ -94,22 +108,22 @@
 
     def __init__(self, func):
         self._instance = func()
 
     def get_instance(self):
         return self._instance
 
-    def close(self):
+    def close(self, exc_type=None, exc=None, tb=None):
         self._instance = None
 
 
 class InstanceFactory(IFactory):
     awaitable = False
 
     def __init__(self, value):
         self._value = value
 
     def get_instance(self):
         return self._value
 
-    def close(self):
+    def close(self, exc_type=None, exc=None, tb=None):
         self._value = None
```

### Comparing `pydio-0.3.3/pydio/_unbound_factories.py` & `pydio-0.4.0/pydio/_unbound_factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/_unbound_factories.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 import functools
```

### Comparing `pydio-0.3.3/pydio/api.py` & `pydio-0.4.0/pydio/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/api.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 """An all-in-one module for making imports easier.
```

### Comparing `pydio-0.3.3/pydio/base.py` & `pydio-0.4.0/pydio/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # ---------------------------------------------------------------------------
 # pydio/base.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 """Interface definitions."""
 
 import abc
 import contextlib
-import inspect
+import typing
 from typing import Awaitable, Hashable, Optional, TypeVar, Union
 
 from . import _compat
 
 T = TypeVar('T')
 
 
 class IInjector(
     contextlib.AbstractContextManager, _compat.AbstractAsyncContextManager
 ):
     """Definition of injector interface."""
 
-    def __exit__(self, *args):
-        self.close()
-
-    async def __aexit__(self, *args):
-        maybe_coroutine = self.close()
-        if inspect.iscoroutine(maybe_coroutine):
-            await maybe_coroutine
-
     @abc.abstractmethod
     def inject(self, key: Hashable) -> Union[T, Awaitable[T]]:
         """Create and return object for given hashable key.
 
         On success, this method returns created object or awaitable pointing
         to created object. On failure, it raises
         :exc:`pydio.exc.InjectorError`.
@@ -90,42 +82,77 @@
     """Interface for bound factories.
 
     Bound factories are managed by :class:`IInjector` objects and are
     responsible for construction of target object that is later returned by
     :meth:`IInjector.inject`. Each factory should wrap one kind of object
     factory function provided by user (f.e. normal function or a coroutine,
     but never both).
+
+    .. deprecated:: 0.4.0
+        This will be removed from the public interface.
     """
 
     @abc.abstractmethod
     def get_instance(self) -> Optional[Union[T, Awaitable[T]]]:
         """Create and return target object.
 
         Value returned by this method is later also returned by
         :meth:`IInjector.inject` method.
         """
 
     @abc.abstractmethod
-    def close(self):
+    def close(
+        self,
+        exc_type: typing.Type[BaseException] = None,
+        exc: BaseException = None,
+        tb=None
+    ):
         """Close this factory.
 
         When called, underlying instance is cleared and calling
         :meth:`get_instance` again will return None. This method may also
         invoke some additional custom-defined clearing actions (if supported
         by implementation).
+
+        :param exc_type:
+            Exception type.
+
+            This will be set with exception class object when underlying
+            factory is closed due to exception being raised.
+
+            .. versionadded:: 0.4.0
+
+        :param exc:
+            Exception object.
+
+            This will be set with exception instance when underlying factory is
+            closed due to exception being raised.
+
+            .. versionadded:: 0.4.0
+
+        :param tb:
+            Traceback object.
+
+            This will be set when underlying factory is closed due to exception
+            being raised.
+
+            .. versionadded:: 0.4.0
         """
 
 
 class IUnboundFactory(abc.ABC):
     """Interface for unbound factories.
 
     Unbound factories are created and managed by
     :class:`IUnboundFactoryRegistry` objects. The role of this class is to
     wrap user-specified factory functions that are being registered to
     providers.
+
+    .. deprecated:: 0.4.0
+        This will be removed from the public interface.
     """
 
     @property
     @abc.abstractmethod
     def scope(self) -> Optional[Hashable]:
         """Name of the scope assigned to this factory.
 
@@ -149,14 +176,17 @@
 
 class IUnboundFactoryRegistry(abc.ABC):
     """Interface for :class:`IUnboundFactory` objects registry.
 
     Factory registries are used by :class:`IInjector` objects to find
     :class:`IUnboundFactory` object that matches key that was given to
     :meth:`IInjector.inject` call.
+
+    .. deprecated:: 0.4.0
+        This will be removed from the public interface.
     """
 
     @abc.abstractmethod
     def get(self,
             key: Hashable,
             env: Hashable = None) -> Optional[IUnboundFactory]:
         """Get :class:`IUnboundFactory` registered for given key and
```

### Comparing `pydio-0.3.3/pydio/exc.py` & `pydio-0.4.0/pydio/exc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/exc.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 """Base exception classes for PyDio."""
```

### Comparing `pydio-0.3.3/pydio/injector.py` & `pydio-0.4.0/pydio/injector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # ---------------------------------------------------------------------------
 # pydio/injector.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
+import inspect
 import threading
+import typing
 import weakref
 from typing import Awaitable, Hashable, Optional
 
 from . import exc
-from .base import IInjector, IUnboundFactoryRegistry
+from .base import IFactory, IInjector, IUnboundFactoryRegistry
 
 
 class Injector(IInjector):
     """Dependency injector main class.
 
     :param provider:
         Unbound factory provider to work on
@@ -31,20 +33,34 @@
 
         See :meth:`IUnboundFactoryRegistry.get` for more details.
     """
 
     def __init__(self, provider: IUnboundFactoryRegistry, env: Hashable = None):
         self._provider = provider
         self._env = env
-        self._cache = {}
+        self._cache: typing.Dict[typing.Any, IFactory] = {}
         self._lock = threading.RLock()
         self._scope = None
-        self._children = []
+        self._child_injectors: typing.List[Injector] = []
         self.__parent = None
 
+    def __exit__(self, exc_type, exc, tb):
+        if exc_type is None:
+            self.close()
+        else:
+            self._do_close(exc_type, exc, tb)
+
+    async def __aexit__(self, exc_type, exc, tb):
+        if exc_type is None:
+            maybe_coroutine = self.close()
+        else:
+            maybe_coroutine = self._do_close(exc_type, exc, tb)
+        if inspect.iscoroutine(maybe_coroutine):
+            await maybe_coroutine
+
     @property
     def _parent(self):
         if self.__parent is not None:
             return self.__parent()
         return None
 
     @_parent.setter
@@ -87,31 +103,37 @@
             if parent_env is not None and parent_env != env:
                 raise ValueError(
                     "scoped() got an invalid value for parameter 'env': expected {!r} or None, got {!r}"
                     .format(parent_env, env)
                 )
         with self._lock:
             injector = self.__class__(self._provider, env=env or self._env)
-            self._children.append(injector)
+            self._child_injectors.append(injector)
             injector._parent = self  # pylint: disable=protected-access
             injector._scope = scope  # pylint: disable=protected-access
             return injector
 
     def close(self) -> Optional[Awaitable[None]]:
         """See :meth:`pydio.base.IInjector.close`."""
+        return self._do_close()
+
+    def _do_close(self,
+                  exc_type=None,
+                  exc=None,
+                  tb=None) -> Optional[Awaitable[None]]:
         if self._provider is not None:
             with self._lock:
                 provider = self._provider
                 awaitables = []
-                for child in self._children:
-                    maybe_awaitable = child.close()
+                for child in self._child_injectors:
+                    maybe_awaitable = child._do_close(exc_type, exc, tb)
                     if maybe_awaitable is not None:
                         awaitables.append(maybe_awaitable)
                 for instance in self._cache.values():
-                    maybe_awaitable = instance.close()
+                    maybe_awaitable = instance.close(exc_type, exc, tb)
                     if maybe_awaitable is not None:
                         awaitables.append(maybe_awaitable)
                 if not provider.has_awaitables():
                     self._provider = None
                 else:
 
                     async def do_async_close(awaitables):
```

### Comparing `pydio-0.3.3/pydio/keys.py` & `pydio-0.4.0/pydio/keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/keys.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 import collections.abc
```

### Comparing `pydio-0.3.3/pydio/provider.py` & `pydio-0.4.0/pydio/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ---------------------------------------------------------------------------
 # pydio/provider.py
 #
-# Copyright (C) 2021 - 2022 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
+# Copyright (C) 2021 - 2023 Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>
 #
 # This file is part of PyDio library and is released under the terms of the
 # MIT license: http://opensource.org/licenses/mit-license.php.
 #
 # See LICENSE.txt for details.
 # ---------------------------------------------------------------------------
 import threading
```

### Comparing `pydio-0.3.3/pyproject.toml` & `pydio-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyDio"
-version = "0.3.3"
+version = "0.4.0"
 description = "Simple and functional dependency injection toolkit for Python"
 authors = [
     "Maciej Wiatrzyk <maciej.wiatrzyk@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://pydio.readthedocs.io"
@@ -41,15 +41,15 @@
 twine = "^4.0.1"
 toml = "^0.10.2"
 tox = "^3.27.0"
 myst-parser = "^0.18.1"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.3.3"
+version = "0.4.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 bump_message = "bump: $current_version -> $new_version [skip ci]"
 version_files = [
     "pydio/__init__.py",
     "pyproject.toml"
 ]
```

### Comparing `pydio-0.3.3/setup.py` & `pydio-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['pydio']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'pydio',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'Simple and functional dependency injection toolkit for Python',
     'long_description': "![PyPI](https://img.shields.io/pypi/v/pydio)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pydio)\n![PyPI - License](https://img.shields.io/pypi/l/pydio)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/pydio)\n[![codecov](https://codecov.io/gh/mwiatrzyk/pydio/branch/master/graph/badge.svg?token=Y6DJDSOR6M)](https://codecov.io/gh/mwiatrzyk/pydio)\n\n# PyDio\n\nSimple and functional dependency injection toolkit for Python.\n\n## About\n\nPyDio aims to be simple, yet still powerful, allowing you to feed\ndependencies inside your application in a flexible way. PyDio design is based\non simple assumption, that dependency injection can be achieved using simple\n**key-to-function** map, where **key** specifies **type of object** you want\nto inject and **function** is a **factory** function that creates\n**instances** of that type.\n\nIn PyDio, this is implemented using **providers** and **injectors**. You use\nproviders to configure your **key-to-function** mapping, and then you use\ninjectors to perform a **lookup** of a specific key and creation of the final\nobject.\n\nHere's a simple example:\n\n```python\nimport abc\n\nfrom pydio.api import Provider, Injector\n\nprovider = Provider()\n\n@provider.provides('greet')\ndef make_greet():\n    return 'Hello, world!'\n\ndef main():\n    injector = Injector(provider)\n    greet_message = injector.inject('greet')\n    print(greet_message)\n\nif __name__ == '__main__':\n    main()\n```\n\nNow you can save the snippet from above as ``example.py`` file and execute\nto see the output:\n\n```shell\n$ python example.py\nHello, world!\n```\n\n## Key features\n\n* Support for any hashable keys: class objects, strings, ints etc.\n* Support for any type of object factories: function, coroutine, generator,\n  asynchronous generator.\n* Automatic resource management via generator-based factories\n  (similar to pytest's fixtures)\n* Multiple environment support: testing, development, production etc.\n* Limiting created object's lifetime to user-defined scopes: global,\n  application, use-case etc.\n* No singletons used, so there is no global state...\n* ...but you still can create global injector on your own if you need it :-)\n\n## Installation\n\nYou can install PyDio using one of following methods:\n\n1) From PyPI (for stable releases):\n\n    ```shell\n    $ pip install PyDio\n    ```\n\n2) From test PyPI (for stable and development releases):\n\n    ```shell\n    $ pip install -i https://test.pypi.org/simple/ PyDio\n    ```\n\n3) Directly from source code repository (for all releases):\n\n    ```shell\n    $ pip install git+https://gitlab.com/zef1r/PyDio.git@[branch-or-tag]\n    ```\n\n## Documentation\n\nYou have two options available:\n\n1) Visit [PyDio's ReadTheDocs](https://pydio.readthedocs.io/en/latest/) site.\n\n2) Take a tour around [functional tests](https://github.com/mwiatrzyk/pydio/tree/master/tests/functional).\n\n## License\n\nThis project is released under the terms of the MIT license.\n\nSee [LICENSE.txt](https://github.com/mwiatrzyk/pydio/blob/master/LICENSE.txt) for more details.\n\n## Author\n\nMaciej Wiatrzyk <maciej.wiatrzyk@gmail.com>\n",
     'author': 'Maciej Wiatrzyk',
     'author_email': 'maciej.wiatrzyk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mwiatrzyk/pydio',
```

### Comparing `pydio-0.3.3/PKG-INFO` & `pydio-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydio
-Version: 0.3.3
+Version: 0.4.0
 Summary: Simple and functional dependency injection toolkit for Python
 Home-page: https://github.com/mwiatrzyk/pydio
 License: MIT
 Keywords: dependency,injection,di,framework,toolkit,tool,library
 Author: Maciej Wiatrzyk
 Author-email: maciej.wiatrzyk@gmail.com
 Requires-Python: >=3.7.2,<4
```

