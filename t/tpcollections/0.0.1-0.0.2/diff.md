# Comparing `tmp/tpcollections-0.0.1.tar.gz` & `tmp/tpcollections-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpcollections-0.0.1.tar", last modified: Fri May  5 22:39:43 2023, max compression
+gzip compressed data, was "tpcollections-0.0.2.tar", last modified: Sat May  6 16:56:42 2023, max compression
```

## Comparing `tpcollections-0.0.1.tar` & `tpcollections-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     3078 2023-05-05 15:55:14.913102 tpcollections-0.0.1/.gitignore
--rw-r--r--   0        0        0      147 2023-05-05 15:55:15.002104 tpcollections-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-05 15:55:14.913102 tpcollections-0.0.1/LICENSE
--rw-r--r--   0        0        0    11401 2023-05-05 15:55:14.933103 tpcollections-0.0.1/LICENSE.apache
--rw-r--r--   0        0        0      188 2023-05-05 15:55:14.933103 tpcollections-0.0.1/LICENSE.rst
--rw-r--r--   0        0        0       52 2023-05-05 15:55:14.933103 tpcollections-0.0.1/Makefile
--rw-r--r--   0        0        0       78 2023-05-05 15:55:14.913102 tpcollections-0.0.1/README.md
--rw-r--r--   0        0        0     1105 2023-05-05 22:39:21.530638 tpcollections-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0     1327 2023-05-05 15:55:14.933103 tpcollections-0.0.1/run_all_tests.sh
--rw-r--r--   0        0        0      184 2023-05-05 22:30:45.095245 tpcollections-0.0.1/src/tpcollections/__init__.py
--rw-r--r--   0        0        0    11616 2023-05-05 22:32:01.065479 tpcollections-0.0.1/src/tpcollections/_db.py
--rw-r--r--   0        0        0    10099 2023-05-05 22:35:31.100892 tpcollections-0.0.1/src/tpcollections/_mapping.py
--rw-r--r--   0        0        0      932 2023-05-05 22:28:16.642844 tpcollections-0.0.1/src/tpcollections/_serializers.py
--rw-r--r--   0        0        0     1623 2023-05-05 21:48:43.010752 tpcollections-0.0.1/src/tpcollections/_util.py
--rw-r--r--   0        0        0        0 2023-05-05 15:55:14.934103 tpcollections-0.0.1/src/tpcollections/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 22:38:40.009963 tpcollections-0.0.1/test/__init__.py
--rw-r--r--   0        0        0    15450 2023-05-05 22:38:15.136559 tpcollections-0.0.1/test/test_mapping.py
--rw-r--r--   0        0        0     1093 1970-01-01 00:00:00.000000 tpcollections-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-05-05 19:11:26.352439 tpcollections-0.0.2/.gitignore
+-rw-r--r--   0        0        0      147 2023-05-05 19:11:26.352439 tpcollections-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE
+-rw-r--r--   0        0        0    11401 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE.apache
+-rw-r--r--   0        0        0      188 2023-05-05 19:11:26.352439 tpcollections-0.0.2/LICENSE.rst
+-rw-r--r--   0        0        0       52 2023-05-05 19:11:26.352439 tpcollections-0.0.2/Makefile
+-rw-r--r--   0        0        0     2679 2023-05-06 13:43:28.883045 tpcollections-0.0.2/README.md
+-rwxr-xr-x   0        0        0     2026 2023-05-06 16:53:33.707281 tpcollections-0.0.2/justfile
+-rw-r--r--   0        0        0     1105 2023-05-06 16:56:31.844943 tpcollections-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      188 2023-05-06 12:46:19.495293 tpcollections-0.0.2/src/tpcollections/__init__.py
+-rw-r--r--   0        0        0    12063 2023-05-06 16:15:09.267981 tpcollections-0.0.2/src/tpcollections/_db.py
+-rw-r--r--   0        0        0    13147 2023-05-06 16:16:37.751362 tpcollections-0.0.2/src/tpcollections/_mapping.py
+-rw-r--r--   0        0        0      925 2023-05-06 12:17:50.879505 tpcollections-0.0.2/src/tpcollections/_serializers.py
+-rw-r--r--   0        0        0     1623 2023-05-06 02:32:11.037046 tpcollections-0.0.2/src/tpcollections/_util.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:11:26.353439 tpcollections-0.0.2/src/tpcollections/py.typed
+-rw-r--r--   0        0        0        0 2023-05-06 02:32:11.037046 tpcollections-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0     6693 2023-05-06 16:13:48.868910 tpcollections-0.0.2/test/test_mapping.py
+-rw-r--r--   0        0        0     7748 2023-05-06 16:13:39.443550 tpcollections-0.0.2/test/test_ordered_mapping.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 tpcollections-0.0.2/PKG-INFO
```

### Comparing `tpcollections-0.0.1/.gitignore` & `tpcollections-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.1/LICENSE` & `tpcollections-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.1/LICENSE.apache` & `tpcollections-0.0.2/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `tpcollections-0.0.1/pyproject.toml` & `tpcollections-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'tpcollections'
 description = 'Persistent transactional Python collections'
-version = '0.0.1'
+version = '0.0.2'
 readme = 'README.md'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 1 - Planning',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

### Comparing `tpcollections-0.0.1/src/tpcollections/_db.py` & `tpcollections-0.0.2/src/tpcollections/_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,22 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import json
 import sqlite3
-from collections.abc import MutableMapping
-from functools import wraps
-from contextlib import ExitStack, closing, contextmanager
-from datetime import timedelta
+from contextlib import closing, contextmanager
 from pathlib import Path
 from types import TracebackType
-from typing import Any, ContextManager, Generator, Iterable, Iterator, List, Optional, Reversible, Set, Tuple, Type, Union
-from weakref import finalize
+from typing import ContextManager, Generator, List, Optional, Set, Type
 from enum import auto, unique, Enum
 import warnings
 
 from ._util import Identifier
 
 @contextmanager
 def _savepoint(
     connection: sqlite3.Connection,
-    name: Identifier | str = Identifier('tpcollection'),
+    name: Identifier = Identifier('tpcollection'),
 ) -> Generator[None, None, None]:
-    if isinstance(name, str):
-        name = Identifier(name)
-
     with closing(connection.cursor()) as cursor:
         cursor.execute(f'SAVEPOINT {name}')
         try:
             yield
         except:
             cursor.execute(f'ROLLBACK TO {name}')
             raise
@@ -63,16 +52,16 @@
     # changes.  This connection may still establish locks, and therefore
     # might need to write to the filesystem. This mode is mostly useful
     # for performance reasons, as various read-only connections may read in
     # parallel.
     READ_ONLY = auto()
 
     # The database will not have any writes or locks done to it or its
-    # filesystem.  Other connections are expected to not write to the database
-    # at all.
+    # filesystem.  Only use this if you know the database will not be written to
+    # by any other process at all.
     IMMUTABLE = auto()
 
 def _uri(
     path: Optional[Path] = None,
     mode: Mode = Mode.READ_WRITE,
 ) -> str:
     if path is None:
@@ -83,14 +72,16 @@
         else:
             uri = 'file:' + str(path)
 
         if mode is Mode.READ_ONLY:
             uri += '?mode=ro'
         elif mode is Mode.IMMUTABLE:
             uri += '?immutable=1'
+        else:
+            uri += '?mode=rwc'
 
         return uri
 
 class Database:
     """
     A sqlite connection manager.
 
@@ -103,44 +94,48 @@
     """
 
     __slots__ = (
         '_uri',
         '_mode',
         '_connection',
         '_timeout',
-        '_wal',
+        '_memory',
         '__weakref__'
     )
 
     def __init__(self,
         path: Optional[Path] = None,
         mode: Mode = Mode.READ_WRITE,
-        wal: bool = False,
         timeout: float = 5.0,
         **kwargs,
     ) -> None:
-        assert not (path is None and mode is not Mode.READ_WRITE), (
-            'An in-memory database must be read-write'
-        )
+        if path is None:
+            self._mode = mode.READ_WRITE
+            self._memory = False
+        else:
+            self._mode = mode
+            self._memory = True
 
-        self._mode = mode
         self._uri = _uri(path, mode)
-        self._wal = wal
         self._timeout = timeout
 
     @property
     def read_only(self) -> bool:
         return self._mode is not Mode.READ_WRITE
 
+    @property
+    def memory(self) -> bool:
+        return self._memory
+
     def __call__(self) -> ContextManager['Connection']:
         return _connect(
-            self._uri,
-            self._mode,
-            self._wal,
-            self._timeout,
+            uri=self._uri,
+            mode=self._mode,
+            timeout=self._timeout,
+            memory=self._memory,
         )
 
     def __enter__(self) -> 'Connection':
         assert not hasattr(self, '_connection'), (
             'Database is not a nestable context manager, call it instead'
         )
         self._connection = self()
@@ -172,65 +167,69 @@
 if sqlite3.sqlite_version_info >= (3, 38):
     UNIXEPOCH = 'UNIXEPOCH()'
 else:
     UNIXEPOCH = "CAST(strftime('%s', 'now') AS INTEGER)"
 
 _APPLICATION_ID = -1238962565
 
-_STRICT_WITHOUT_ROWID = ', '.join(part for part in (STRICT, WITHOUT_ROWID) if part)
+STRICT_WITHOUT_ROWID = ', '.join(part for part in (STRICT, WITHOUT_ROWID) if part)
 
-class Connection(MutableMapping):
+class Connection:
     '''The actual connection object, as a MutableMapping[str, Any].
 
     Items are expired when a value is inserted or updated.  Deletion or
     postponement does not expire items.
     '''
 
     __slots__ = (
         '_connection',
         '_attachments',
         '_mode',
         '_transactions',
-        '_wal',
+        '_has_attachments',
+        '_memory',
         '__weakref__',
     )
 
     def __init__(self,
         connection: sqlite3.Connection,
         mode: Mode,
-        wal: bool,
+        memory: bool,
     ) -> None:
         self._connection = connection
         self._attachments: Set[str] = {'main'}
         self._mode = mode
         self._transactions: List[ContextManager[None]] = []
-        self._wal = wal
+        self._has_attachments = False
+        self._memory = memory
         self._init(Identifier('main'))
 
     def _init(self, database: Identifier) -> None:
+        '''Initialize a database or attachment.
+        '''
         with self.cursor() as cursor:
             application_id = next(cursor.execute('PRAGMA application_id'))[0]
             if application_id == 0:
-                cursor.execute(f'PRAGMA application_id = {_APPLICATION_ID}')
+                cursor.execute(f'PRAGMA {database}.application_id = {_APPLICATION_ID}')
             elif application_id != _APPLICATION_ID:
                 raise ValueError(f'illegal application ID {application_id}')
 
-            user_version = next(cursor.execute('PRAGMA user_version'))[0]
+            user_version = next(cursor.execute(f'PRAGMA {database}.user_version'))[0]
             if user_version == 0:
-                cursor.execute(f'PRAGMA user_version = 1')
+                cursor.execute(f'PRAGMA {database}.user_version = 1')
             elif user_version != 1:
-                raise ValueError(f'user_version was {user_version}')
+                raise ValueError(f'user_version for {database} was {user_version}')
 
             if not self.read_only:
                 cursor.execute(f'''
-                    CREATE TABLE IF NOT EXISTS main.tpcollections (
+                    CREATE TABLE IF NOT EXISTS {database}.tpcollections (
                         name TEXT PRIMARY KEY NOT NULL,
                         type TEXT NOT NULL,
                         version INTEGER NOT NULL
-                    ) {_STRICT_WITHOUT_ROWID}
+                    ) {STRICT_WITHOUT_ROWID}
                 ''')
 
     @property
     def connection(self) -> sqlite3.Connection:
         return self._connection
 
     @contextmanager
@@ -244,14 +243,15 @@
 
     def __enter__(self) -> None:
         if self._transactions:
             new_transaction = _savepoint(self._connection)
         else:
             new_transaction = _transaction(self._connection, self.read_only)
 
+        new_transaction.__enter__()
         self._transactions.append(new_transaction)
 
     def __exit__(
         self,
         type: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
@@ -268,46 +268,59 @@
 
         with closing(self._connection.cursor()) as cursor:
             if __debug__ and self._transactions:
                 warnings.warn(
                     'Attaching a database inside a transaction can prevent '
                     'transactions from being atomic.'
                 )
-            cursor.execute(f'ATTACH ? AS {database_id}', (uri,))
-            if self._wal and not self.read_only:
-                if __debug__:
-                    warnings.warn(
-                        'Attaching a database in wal mode can cause'
-                        ' non-atomic transactions:'
-                        ' https://www.sqlite.org/lang_attach.html'
-                    )
-                cursor.execute(f'PRAGMA {database_id}.journal_mode=WAL')
-                cursor.execute(f'PRAGMA {database_id}.synchronous=NORMAL')
 
-        self._init(database_id)
+            if not (self._memory or self._has_attachments or self.read_only):
+                # disable WAL mode when attaching databases
+                cursor.execute(f'PRAGMA main.journal_mode=DELETE')
+                cursor.execute(f'PRAGMA main.synchronous=FULL')
+                self._has_attachments = True
+
+            cursor.execute(f'ATTACH ? AS {database_id}', (uri,))
+            try:
+                if not (self.read_only or self._memory):
+                    cursor.execute(f'PRAGMA {database_id}.journal_mode=DELETE')
+                    cursor.execute(f'PRAGMA {database_id}.synchronous=FULL')
+
+                self._init(database_id)
+            except:
+                cursor.execute(f'DETACH {database_id}')
+                raise
 
 @contextmanager
 def _connect(
     uri: str,
     mode: Mode,
-    wal: bool,
     timeout: float,
+    memory: bool,
 ) -> Generator[Connection, None, None]:
-    with (
-        closing(sqlite3.connect(uri, timeout=timeout)) as connection,
-        closing(connection.cursor()) as cursor,
-    ):
+    with closing(sqlite3.connect(
+        uri,
+        timeout=timeout,
+        isolation_level=None,
+        check_same_thread=__debug__,
+        uri=True,
+        cached_statements=1024,
+    )) as connection, closing(connection.cursor()) as cursor:
         try:
-            if wal and mode is Mode.READ_WRITE:
+            if not memory and mode is Mode.READ_WRITE:
                 cursor.execute('PRAGMA main.journal_mode=WAL')
                 cursor.execute('PRAGMA main.synchronous=NORMAL')
 
-            yield Connection(connection, mode, wal)
+            yield Connection(
+                connection=connection,
+                mode=mode,
+                memory=memory,
+            )
         finally:
-            if mode is Mode.READ_WRITE:
+            if not memory and mode is Mode.READ_WRITE:
                 cursor.execute('PRAGMA analysis_limit=8192')
                 cursor.execute('PRAGMA optimize')
 
 class _Base:
     __slots__ = (
         '_connection',
         '_database',
@@ -330,15 +343,15 @@
                 SELECT type
                     FROM {database}.tpcollections
                     WHERE name = ?
             ''', (table.value,))
             row = cursor.fetchone()
             if row is None:
                 cursor.execute(
-                    'SELECT 1 FROM sqlite_master WHERE name = ?',
+                    f'SELECT 1 FROM {database}.sqlite_master WHERE name = ?',
                     (table.value,)
                 )
                 if cursor.fetchone() is not None:
                     raise NameError(f'table {table} already exists')
                 
                 cursor.execute(f'''
                     INSERT INTO {database}.tpcollections
```

### Comparing `tpcollections-0.0.1/src/tpcollections/_mapping.py` & `tpcollections-0.0.2/src/tpcollections/_mapping.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,123 +1,113 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-#
-# This code is distributed under the terms and conditions
-# from the Apache License, Version 2.0
-#
-# http://opensource.org/licenses/apache2.0.php
-#
-# This code was inspired by:
-#  * http://code.activestate.com/recipes/576638-draft-for-an-sqlite3-based-dbm/
-#  * http://code.activestate.com/recipes/526618/
-
-
-import json
 import sqlite3
-from collections.abc import MutableMapping
-from contextlib import ExitStack, closing, contextmanager
-from datetime import timedelta
-from types import TracebackType
-from typing import Any, Generator, Iterable, Iterator, Optional, Reversible, Tuple, Type, Union
-from weakref import finalize
+from typing import (
+    Any,
+    Generic,
+    ItemsView,
+    Iterable,
+    Iterator,
+    KeysView,
+    Reversible,
+    Tuple,
+    TypeVar,
+    ValuesView,
+    MutableMapping,
+)
 from enum import unique, Enum
 
 from ._util import Identifier
 
 from . import _db, _serializers
 
-@unique
-class MappingOrder(str, Enum):
-    '''An ordering enum for iteration methods.
-    '''
+Item = TypeVar('Item')
+Key = TypeVar('Key')
+Value = TypeVar('Value')
+
+class _ViewsBase(Reversible[Item], Iterable[Item]):
+    __slots__ = ()
+
+    _connection: _db.Connection
+    _database: Identifier
+    _table : Identifier
 
-    ID = 'id'
-    KEY = 'key'
+    def _iterator(self, order: str) -> Iterator[Item]:
+        raise NotImplementedError
 
-    def __str__(self) -> str:
-        return self.value
+    def __len__(self) -> int:
+        with self._connection.cursor() as cursor:
+            len, = cursor.execute(f'SELECT COUNT(*) FROM {self._database}.{self._table}').fetchone()
+            return len
 
-    def __format__(self, format_spec: str) -> str:
-        return self.value.__format__(format_spec)
+    def __iter__(self) -> Iterator[Item]:
+        return self._iterator('ASC')
 
-class _Keys(Reversible, Iterable[Any]):
+    def __reversed__(self) -> Iterator[Item]:
+        return self._iterator('DESC')
+
+class Keys(_ViewsBase[Key], KeysView[Key]):
     __slots__ = (
         '_connection',
         '_database',
         '_table',
         '_serializer',
         '_order',
     )
 
     def __init__(
         self,
         connection: _db.Connection,
         database: Identifier,
         table: Identifier,
         serializer: _serializers.Serializer,
-        order: MappingOrder,
+        order: str,
     ) -> None:
-
         self._connection = connection
         self._database = database
         self._table = table
         self._serializer = serializer
         self._order = order
     
-    def _iterator(self, order: str) -> Iterator[Any]:
+    def _iterator(self, order: str) -> Iterator[Key]:
         with self._connection.cursor() as cursor:
             for key, in cursor.execute(
                 f'SELECT key FROM {self._database}.{self._table} ORDER BY {self._order} {order}',
             ):
                 yield self._serializer.loads(key)
 
-    def __iter__(self) -> Iterator[Any]:
-        return self._iterator('ASC')
-
-    def __reversed__(self) -> Iterator[Any]:
-        return self._iterator('DESC')
-
-class _Values(Reversible, Iterable[Any]):
+class Values(_ViewsBase[Any], ValuesView[Value]):
     __slots__ = (
         '_connection',
         '_database',
         '_table',
         '_serializer',
         '_order',
     )
 
     def __init__(
         self,
         connection: _db.Connection,
         database: Identifier,
         table: Identifier,
         serializer: _serializers.Serializer,
-        order: MappingOrder,
+        order: str,
     ) -> None:
-
         self._connection = connection
         self._database = database
         self._table = table
         self._serializer = serializer
         self._order = order
 
-    def _iterator(self, order: str) -> Iterator[Any]:
+    def _iterator(self, order: str) -> Iterator[Value]:
         with self._connection.cursor() as cursor:
             for value, in cursor.execute(
                 f'SELECT value FROM {self._database}.{self._table} ORDER BY {self._order} {order}',
             ):
                 yield self._serializer.loads(value)
 
-    def __iter__(self) -> Iterator[Any]:
-        return self._iterator('ASC')
-
-    def __reversed__(self) -> Iterator[Any]:
-        return self._iterator('DESC')
-
-class _Items(Reversible, Iterable[Tuple[Any, Any]]):
+class Items(_ViewsBase[Tuple[Key, Value]], ItemsView[Key, Value]):
     __slots__ = (
         '_connection',
         '_database',
         '_table',
         '_key_serializer',
         '_value_serializer',
         '_order',
@@ -126,165 +116,142 @@
     def __init__(
         self,
         connection: _db.Connection,
         database: Identifier,
         table: Identifier,
         key_serializer: _serializers.Serializer,
         value_serializer: _serializers.Serializer,
-        order: MappingOrder,
+        order: str,
     ) -> None:
         self._connection = connection
         self._database = database
         self._table = table
         self._key_serializer = key_serializer
         self._value_serializer = value_serializer
         self._order = order
     
-    def _iterator(self, order: str) -> Iterator[Tuple[Any, Any]]:
+    def _iterator(self, order: str) -> Iterator[Tuple[Key, Value]]:
         with self._connection.cursor() as cursor:
             for key, value in cursor.execute(f'''
                 SELECT key, value FROM {self._database}.{self._table}
                     ORDER BY {self._order} {order}
             '''):
                 yield (
                     self._key_serializer.loads(key),
                     self._value_serializer.loads(value),
                 )
 
-    def __iter__(self) -> Iterator[Tuple[Any, Any]]:
-        return self._iterator('ASC')
-
-    def __reversed__(self) -> Iterator[Tuple[Any, Any]]:
-        return self._iterator('DESC')
-
-class Mapping(_db._Base, MutableMapping):
+class _MappingBase(_db._Base, MutableMapping[Key, Value]):
     '''A database mapping.
     '''
 
     __slots__ = (
         '_key_serializer',
         '_value_serializer',
     )
-
     def __init__(self,
         connection: _db.Connection,
-        database: str = 'main',
-        table: str = 'mapping',
-        key_serializer: _serializers.Serializer = _serializers.deterministic_json,
-        value_serializer: _serializers.Serializer = _serializers.pickle,
+        database: Identifier,
+        table: Identifier,
+        key_serializer,
+        value_serializer,
+        type: str,
     ) -> None:
-
-        super().__init__(connection, Identifier(database), Identifier(table), 'mapping')
+        super().__init__(connection, Identifier(database), Identifier(table), type)
 
         self._key_serializer = key_serializer
         self._value_serializer = value_serializer
 
-        version = self._version
-        previous_version = version
-
-        if version < 1:
-            with self._connection.cursor() as cursor:
-                cursor.execute(f'''
-                    CREATE TABLE {self._database}.{self._table} (
-                        id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
-                        key {_db.ANY} UNIQUE NOT NULL,
-                        value {_db.ANY} NOT NULL) {_db.STRICT}
-                ''')
-                version = 1
+    def __len__(self) -> int:
+        '''Get the count of keys in the table.
+        '''
 
-        if version > 1:
-            raise ValueError('tpcollections is not forward compatible')
+        with self._connection.cursor() as cursor:
+            len, = cursor.execute(f'SELECT COUNT(*) FROM {self._database}.{self._table}').fetchone()
+            return len
 
-        if version != previous_version:
-            self._version = version
 
     def __bool__(self) -> bool:
         '''Check if the table is not empty.'''
 
         return len(self) > 0
 
-    def keys(self, order: MappingOrder = MappingOrder.ID) -> Reversible[Any]:
+    def keys(self, order: str) -> Keys[Key]:
         '''Iterate over keys in the table.
         '''
 
-        return _Keys(
+        return Keys(
             connection=self._connection,
             database=self._database,
             table=self._table,
             serializer=self._key_serializer,
             order=order,
         )
 
-    def __iter__(self) -> Iterator[Any]:
-        return iter(self.keys())
-
-    def __reversed__(self) -> Iterator[Any]:
-        return reversed(self.keys())
-
-    def values(self, order: MappingOrder = MappingOrder.ID) -> Reversible[Any]:
+    def values(self, order: str) -> Values[Value]:
         '''Iterate over values in the table.
         '''
 
-        return _Values(
+        return Values(
             connection=self._connection,
             database=self._database,
             table=self._table,
             serializer=self._value_serializer,
             order=order,
         )
 
-    def items(self, order: MappingOrder = MappingOrder.ID) -> Reversible[Tuple[Any, Any]]:
+    def items(self, order: str) -> Items[Key, Value]:
         '''Iterate over keys and values in the table.
         '''
 
-        return _Items(
+        return Items(
             connection=self._connection,
             database=self._database,
             table=self._table,
             key_serializer=self._key_serializer,
             value_serializer=self._value_serializer,
             order=order,
         )
 
-    def __contains__(self, key: Any) -> bool:
+    def __contains__(self, key: Key) -> bool:
         '''Check if the table contains the given key.
         '''
 
         with self._connection.cursor() as cursor:
             cursor.execute(
                 f'SELECT 1 FROM {self._database}.{self._table} WHERE key = ?',
                 (self._key_serializer.dumps(key),),
             )
             return cursor.fetchone() is not None
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: Key) -> Value:
         '''Fetch the key.
         '''
 
         with self._connection.cursor() as cursor:
             for row in cursor.execute(
                 f'SELECT value FROM {self._database}.{self._table} WHERE key = ?',
                 (self._key_serializer.dumps(key),),
             ):
                 return self._value_serializer.loads(row[0])
         raise KeyError(key)
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: Key, value: Value) -> None:
         '''Set or replace the item.
 
         This also triggers cleaning up expired values.
         '''
 
         with self._connection.cursor() as cursor:
             if sqlite3.sqlite_version_info >= (3, 24):
                 cursor.execute(f'''
                         INSERT INTO {self._database}.{self._table} (key, value)
                             VALUES (?, ?)
                             ON CONFLICT (key) DO UPDATE
-                            SET value=excluded.valu
+                            SET value=excluded.value
                     ''',
                     (
                         self._key_serializer.dumps(key),
                         self._value_serializer.dumps(value),
                     ),
                 )
             elif key in self:
@@ -305,15 +272,15 @@
                     ''',
                     (
                         self._key_serializer.dumps(key),
                         self._value_serializer.dumps(value),
                     ),
                 )
 
-    def __delitem__(self, key: str) -> None:
+    def __delitem__(self, key: Key) -> None:
         '''Delete an item from the table.
         '''
 
         with self._connection.cursor() as cursor:
             cursor.execute(
                 f'DELETE FROM {self._database}.{self._table} WHERE key=?',
                 (self._key_serializer.dumps(key),),
@@ -323,7 +290,150 @@
 
     def clear(self) -> None:
         '''Delete all items from the table.
         '''
 
         with self._connection.cursor() as cursor:
             cursor.execute(f'DELETE FROM {self._database}.{self._table}')
+
+class OrderedMapping(_MappingBase[Key, Value]):
+    '''A database mapping.
+    '''
+
+    __slots__ = ()
+
+    @unique
+    class Order(str, Enum):
+        '''An ordering enum for iteration methods.
+        '''
+
+        ID = 'id'
+        KEY = 'key'
+
+        def __str__(self) -> str:
+            return self.value
+
+        def __format__(self, format_spec: str) -> str:
+            return self.value.__format__(format_spec)
+
+    def __init__(self,
+        connection: _db.Connection,
+        database: str = 'main',
+        table: str = 'orderedmapping',
+        key_serializer: _serializers.Serializer = _serializers.deterministic_json,
+        value_serializer: _serializers.Serializer = _serializers.pickle,
+    ) -> None:
+
+        super().__init__(
+            connection=connection,
+            database=Identifier(database),
+            table=Identifier(table),
+            type='orderedmapping',
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+        )
+
+        version = self._version
+        previous_version = version
+
+        if version < 1:
+            with self._connection.cursor() as cursor:
+                cursor.execute(f'''
+                    CREATE TABLE {self._database}.{self._table} (
+                        id INTEGER PRIMARY KEY AUTOINCREMENT NOT NULL,
+                        key {_db.ANY} UNIQUE NOT NULL,
+                        value {_db.ANY} NOT NULL) {_db.STRICT}
+                ''')
+                version = 1
+
+        if version > 1:
+            raise ValueError('tpcollections is not forward compatible')
+
+        if version != previous_version:
+            self._version = version
+
+    def keys(self, order: Order = Order.ID) -> Keys[Key]:
+        '''Iterate over keys in the table.
+        '''
+        return super().keys(order)
+
+    def __iter__(self) -> Iterator[Key]:
+        return iter(self.keys())
+
+    def __reversed__(self) -> Iterator[Key]:
+        return reversed(self.keys())
+
+    def values(self, order: Order = Order.ID) -> Values[Value]:
+        '''Iterate over values in the table.
+        '''
+        return super().values(order)
+
+    def items(self, order: Order = Order.ID) -> Items[Key, Value]:
+        '''Iterate over keys and values in the table.
+        '''
+        return super().items(order)
+
+class Mapping(_MappingBase[Key, Value]):
+    '''A database mapping ordered by key.
+
+    The table is smaller than OrderedMapping, which needs to keep a separate
+    index for the keys and can't use WITHOUT ROWID.  This does not remember
+    insertion order, and is always ordered by key insertion order.
+    '''
+
+    __slots__ = ()
+
+    def __init__(self,
+        connection: _db.Connection,
+        database: str = 'main',
+        table: str = 'mapping',
+        key_serializer: _serializers.Serializer = _serializers.deterministic_json,
+        value_serializer: _serializers.Serializer = _serializers.pickle,
+    ) -> None:
+
+        super().__init__(
+            connection=connection,
+            database=Identifier(database),
+            table=Identifier(table),
+            type='mapping',
+            key_serializer=key_serializer,
+            value_serializer=value_serializer,
+        )
+
+        version = self._version
+        previous_version = version
+
+        if version < 1:
+            with self._connection.cursor() as cursor:
+                cursor.execute(f'''
+                    CREATE TABLE {self._database}.{self._table} (
+                        key {_db.ANY} PRIMARY KEY UNIQUE NOT NULL,
+                        value {_db.ANY} NOT NULL) {_db.STRICT_WITHOUT_ROWID}
+                ''')
+                version = 1
+
+        if version > 1:
+            raise ValueError('tpcollections is not forward compatible')
+
+        if version != previous_version:
+            self._version = version
+
+    def keys(self) -> Keys[Key]:
+        '''Iterate over keys in the table.
+        '''
+        return super().keys('key')
+
+    def __iter__(self) -> Iterator[Key]:
+        return iter(self.keys())
+
+    def __reversed__(self) -> Iterator[Key]:
+        return reversed(self.keys())
+
+    def values(self) -> Values[Value]:
+        '''Iterate over values in the table.
+        '''
+        return super().values('key')
+
+    def items(self) -> Items[Key, Value]:
+        '''Iterate over keys and values in the table.
+        '''
+        return super().items('key')
```

### Comparing `tpcollections-0.0.1/src/tpcollections/_serializers.py` & `tpcollections-0.0.2/src/tpcollections/_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json as _json
-from typing import Callable, NamedTuple, Union, Any
+from typing import Callable, NamedTuple, Any
 from functools import partial
 import pickle as _pickle
 
 class Serializer(NamedTuple):
     loads: Callable[[Any], Any]
     dumps: Callable[[Any], Any]
```

### Comparing `tpcollections-0.0.1/src/tpcollections/_util.py` & `tpcollections-0.0.2/src/tpcollections/_util.py`

 * *Files identical despite different names*

