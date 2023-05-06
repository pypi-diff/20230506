# Comparing `tmp/preface-0.1.4.tar.gz` & `tmp/preface-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preface-0.1.4.tar", last modified: Mon Apr 10 16:52:42 2023, max compression
+gzip compressed data, was "preface-0.1.5.tar", last modified: Sat May  6 14:06:22 2023, max compression
```

## Comparing `preface-0.1.4.tar` & `preface-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      120 2023-04-10 16:52:08.131901 preface-0.1.4/.gitignore
--rw-r--r--   0        0        0     1081 2022-04-24 14:38:11.593494 preface-0.1.4/LICENSE
--rw-r--r--   0        0        0      449 2022-04-24 23:26:31.091106 preface-0.1.4/README.rst
--rw-r--r--   0        0        0     3973 2023-04-10 16:51:19.662901 preface-0.1.4/preface/__init__.py
--rw-r--r--   0        0        0     1149 2023-04-10 16:48:04.934428 preface-0.1.4/preface/concurrency.py
--rw-r--r--   0        0        0     2306 2022-09-15 04:02:14.210990 preface-0.1.4/preface/dict.py
--rw-r--r--   0        0        0        0 2022-04-24 17:49:39.575358 preface-0.1.4/preface/py.typed
--rw-r--r--   0        0        0      509 2022-09-15 04:14:08.661744 preface-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-10 16:51:54.101456 preface-0.1.4/requirements/dev.txt
--rw-r--r--   0        0        0       38 2022-04-25 00:15:06.344814 preface-0.1.4/requirements/docs.txt
--rw-r--r--   0        0        0       43 2022-09-15 04:13:47.071786 preface-0.1.4/setup.cfg
--rw-r--r--   0        0        0        0 2021-02-19 13:45:03.243430 preface-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      862 2022-09-15 04:04:41.365117 preface-0.1.4/tests/test_dict.py
--rw-r--r--   0        0        0     1374 2022-09-15 04:06:30.474925 preface-0.1.4/tests/test_preface.py
--rw-r--r--   0        0        0      377 2023-04-10 16:49:00.924969 preface-0.1.4/tox.ini
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 preface-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-05-04 13:31:10.697532 preface-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1081 2023-05-04 13:31:10.697601 preface-0.1.5/LICENSE
+-rw-r--r--   0        0        0      449 2023-05-04 13:31:10.697675 preface-0.1.5/README.rst
+-rw-r--r--   0        0        0     3973 2023-05-06 14:06:13.543266 preface-0.1.5/preface/__init__.py
+-rw-r--r--   0        0        0     1149 2023-05-04 13:31:10.697851 preface-0.1.5/preface/concurrency.py
+-rw-r--r--   0        0        0     2463 2023-05-06 14:04:21.422771 preface-0.1.5/preface/dict.py
+-rw-r--r--   0        0        0        0 2023-05-04 13:31:10.697939 preface-0.1.5/preface/py.typed
+-rw-r--r--   0        0        0      509 2023-05-04 13:31:10.698005 preface-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-04 13:31:10.698094 preface-0.1.5/requirements/dev.txt
+-rw-r--r--   0        0        0       38 2023-05-04 13:31:10.698150 preface-0.1.5/requirements/docs.txt
+-rw-r--r--   0        0        0       43 2023-05-04 13:31:10.698204 preface-0.1.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-04 13:31:10.698259 preface-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0     1141 2023-05-06 14:04:21.409389 preface-0.1.5/tests/test_dict.py
+-rw-r--r--   0        0        0     1395 2023-05-04 13:50:47.443056 preface-0.1.5/tests/test_preface.py
+-rw-r--r--   0        0        0      377 2023-05-04 13:31:10.698455 preface-0.1.5/tox.ini
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 preface-0.1.5/PKG-INFO
```

### Comparing `preface-0.1.4/LICENSE` & `preface-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `preface-0.1.4/preface/__init__.py` & `preface-0.1.5/preface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Some helper functions and classes that I want in nearly every project."""
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 
 import enum
 import sys
 from typing import (
     Iterable,
     Iterator,
     List,
```

### Comparing `preface-0.1.4/preface/concurrency.py` & `preface-0.1.5/preface/concurrency.py`

 * *Files identical despite different names*

### Comparing `preface-0.1.4/preface/dict.py` & `preface-0.1.5/preface/dict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 from typing import Any, Dict, Reversible, Union
 
 StrDict = Dict[str, object]
 Key = Union[str, Reversible[str]]
 Primitive = Union[str, int, float, bool, None]
 
 
-def _index(dct: StrDict, key: str) -> StrDict:
-    new_dct = dct[key]
+def typesafeindex(dct: StrDict, key: str) -> StrDict:
+    obj = dct[key]
 
-    if not isinstance(new_dct, dict):
-        raise ValueError(f"Cannot index dct with key '{key}'")
+    if not isinstance(obj, dict):
+        raise KeyError(f"Dict does not contain a subdict at '{key}'.")
 
-    return new_dct
+    return obj
 
 
 def get(dct: StrDict, key: Key, sep: str = ".") -> Any:
     if isinstance(key, str):
         key = key.split(sep)
 
     key = list(reversed(key))
     while len(key) > 1:
-        dct = _index(dct, key.pop())
+        popped = key.pop()
+        dct = typesafeindex(dct, popped)
 
-    return dct[key[0]]
+    return dct[key.pop()]
 
 
 def contains(dct: StrDict, key: Key, sep: str = ".") -> bool:
     if isinstance(key, str):
         key = key.split(sep)
 
     key = list(reversed(key))
     while len(key) > 1:
         popped = key.pop()
         if popped not in dct:
             return False
-        dct = _index(dct, popped)
+
+        try:
+            dct = typesafeindex(dct, popped)
+        except KeyError:
+            return False
 
     return key[0] in dct
 
 
 def delete(dct: StrDict, key: Key, sep: str = ".") -> None:
     if isinstance(key, str):
         key = key.split(sep)
 
     key = list(reversed(key))
 
     while len(key) > 1:
-        dct = _index(dct, key.pop())
+        popped = key.pop()
+        dct = typesafeindex(dct, popped)
 
     del dct[key[0]]
 
 
 def set(dct: StrDict, key: Key, value: Any, sep: str = ".") -> None:
     if isinstance(key, str):
         key = key.split(sep)
@@ -59,15 +65,15 @@
 
     while len(key) > 1:
         k = key.pop()
 
         if k not in dct:
             dct[k] = {}
 
-        dct = _index(dct, k)
+        dct = typesafeindex(dct, k)
 
     dct[key[0]] = value
 
 
 def merge(*dcts: StrDict) -> StrDict:
     result: StrDict = {}
     for dct in dcts:
@@ -96,14 +102,14 @@
     """
     if isinstance(key, str):
         key = key.split(sep)
 
     key = list(reversed(key))
 
     while len(key) > 1:
-        dct = _index(dct, key.pop())
+        dct = typesafeindex(dct, key.pop())
 
     value = dct[key[0]]
 
     del dct[key[0]]
 
     return value
```

### Comparing `preface-0.1.4/tests/test_dict.py` & `preface-0.1.5/tests/test_dict.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 import preface
 
 
+def test_get_field_without_nested() -> None:
+    key = "a"
+    value = 1
+    dct = {key: value}
+
+    assert preface.dict.get(dct, key) == value
+
+
+def test_get_field_nested() -> None:
+    value = 1
+    dct = {"a": {"b": value}}
+
+    assert preface.dict.get(dct, "a.b") == value
+
+
 def test_set_dict_without_nested_dict() -> None:
     dct = {}
 
     key = "a.b.c"
 
     value = 1
```

### Comparing `preface-0.1.4/tests/test_preface.py` & `preface-0.1.5/tests/test_preface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hypothesis
 from hypothesis import strategies
 
 from preface import argsort, flattened, get, grouped, indexed
 
+integers = strategies.integers()
+
 
 @hypothesis.given(strategies.sets(strategies.integers(), min_size=1))
 def test_get(s):
     assert get(s) in s
 
 
 @hypothesis.given(strategies.lists(strategies.integers()))
@@ -29,15 +31,15 @@
 )
 def test_grouped(seq, size):
     for window in grouped(seq, size=size):
         assert len(window) == size
 
 
 @hypothesis.strategies.composite
-def list_and_indices(draw, elements=strategies.integers()):
+def list_and_indices(draw, elements=integers):
     lst = draw(strategies.lists(elements, min_size=1))
     indices = draw(
         strategies.lists(
             strategies.integers(min_value=0, max_value=len(lst) - 1), min_size=1
         )
     )
     return (lst, indices)
```

### Comparing `preface-0.1.4/PKG-INFO` & `preface-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preface
-Version: 0.1.4
+Version: 0.1.5
 Summary: Some helper functions and classes that I want in nearly every project.
 Author-email: Samuel Stevens <samuel.robert.stevens@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://github.com/samuelstevens/preface
 
 Python Preface
```

