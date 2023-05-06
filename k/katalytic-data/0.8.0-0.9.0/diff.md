# Comparing `tmp/katalytic-data-0.8.0.tar.gz` & `tmp/katalytic-data-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.8.0.tar", last modified: Fri May  5 17:31:25 2023, max compression
+gzip compressed data, was "katalytic-data-0.9.0.tar", last modified: Sat May  6 03:48:10 2023, max compression
```

## Comparing `katalytic-data-0.8.0.tar` & `katalytic-data-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.8.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.8.0/.gitignore
--rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.8.0/.gitlab-ci.yml
--rw-r--r--   0        0        0    12893 2023-05-05 17:31:03.370151 katalytic-data-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     1836 2023-04-30 14:20:58.779511 katalytic-data-0.8.0/README.md
--rw-r--r--   0        0        0     1236 2023-05-05 17:31:03.342151 katalytic-data-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    21439 2023-05-05 10:55:06.685464 katalytic-data-0.8.0/src/katalytic/data/__init__.py
--rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.8.0/src/katalytic/data/checks.py
--rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.8.0/tests/test_checks.py
--rw-r--r--   0        0        0    41654 2023-05-05 10:54:38.837287 katalytic-data-0.8.0/tests/test_data.py
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 katalytic-data-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.9.0/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.9.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    13305 2023-05-06 03:48:04.491993 katalytic-data-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     1836 2023-04-30 14:20:58.779511 katalytic-data-0.9.0/README.md
+-rw-r--r--   0        0        0     1236 2023-05-06 03:48:04.467993 katalytic-data-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    27212 2023-05-06 03:37:32.028261 katalytic-data-0.9.0/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.9.0/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.9.0/tests/test_checks.py
+-rw-r--r--   0        0        0    49962 2023-05-06 03:38:53.016355 katalytic-data-0.9.0/tests/test_data.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 katalytic-data-0.9.0/PKG-INFO
```

### Comparing `katalytic-data-0.8.0/.gitignore` & `katalytic-data-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/.gitlab-ci.yml` & `katalytic-data-0.9.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/CHANGELOG.md` & `katalytic-data-0.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.9.0 (2023-05-06)
+### feat
+- [[`1fddfe3`](https://gitlab.com/katalytic/katalytic-data/commit/1fddfe3b1910d55350c004003c808536f4999548)] pop_{min, max}, pop_{min, max}_by_dict_{keys,values}, swap_keys_and_values
+### fix
+- [[`75403ec`](https://gitlab.com/katalytic/katalytic-data/commit/75403ecb6d65ee217788438530d2ff666dc573cf)] exclude map from all_types_besides('iterables') and correct all_types('dict')
+
+
 ## 0.8.0 (2023-05-05)
 ### feat
 - [[`ae032f2`](https://gitlab.com/katalytic/katalytic-data/commit/ae032f23cf8e387387833a0648184ca6095bf9ed)] move katalytic-checks code into this repo
 ### fix
 - [[`ddc044f`](https://gitlab.com/katalytic/katalytic-data/commit/ddc044f3bdf1a872306cfbb090843e220d7222f5)] all_types()
```

### Comparing `katalytic-data-0.8.0/LICENSE.txt` & `katalytic-data-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/README.md` & `katalytic-data-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/pyproject.toml` & `katalytic-data-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.8.0"
+version = "0.9.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic-data-0.8.0/src/katalytic/data/__init__.py` & `katalytic-data-0.9.0/src/katalytic/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
 _UNDEFINED = object()
 
 
-def _generator(): yield 1
 def _function(): pass
+def _generator(): yield 1
 
 
 class _C:
     def __call__(self, *args, **kwargs):
         pass
 
 
+_map = map(int, [])
 _C_obj = _C()
 _obj = object()
 _lambda = lambda x: x
 _generator_expr = (x for x in [])
 _sequences = [[], (), range(0)]
 _dict_views = [{}.keys(), {}.values(), {}.items()]
-_iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
+_iterators = [_generator, _generator_expr, iter([]), _map, enumerate([]), zip([], [])]
 _iterables = [*_dict_views, *_iterators, *_sequences, set(), {}]
 _collections = [(), set(), frozenset([]), {}, []]
 _singletons = [None, True, False]
 _primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
 _callables = [_generator, _function, _lambda, _C_obj, _C]
 _numbers = [0, 0.0, 0j, Decimal('0'), Fraction(0, 1)]
 _objects = [_obj, _C_obj]
@@ -60,15 +61,15 @@
     'generator_expression': _generator_expr,
     'generator_function': _generator,
     'generators': _generators,
     'int': 0,
     'iterables': _iterables,
     'iterators': _iterators,
     'list': [],
-    'map': map(int, []),
+    'map': _map,
     'none': None,
     'numbers': _numbers,
     'objects': _objects,
     'path': Path(''),
     'primitives': _primitives,
     'sequences': _sequences,
     'set': set(),
@@ -93,15 +94,15 @@
 
     return _flatten(_types[t] for t in whitelist)
 
 
 def all_types_besides(blacklist):
     if isinstance(blacklist, str):
         blacklist = [blacklist]
-    if not is_iterable(blacklist):
+    elif not is_iterable(blacklist):
         raise TypeError(f'<blacklist> must be iterable. Got {type(blacklist).__name__}')
 
     blacklist = set(blacklist)
     unexpected = blacklist - set(_types.keys())
     if unexpected:
         raise ValueError(f'Unexpected types in <blacklist>: {unexpected}')
 
@@ -125,17 +126,15 @@
 
 def _flatten(iterable):
     if not is_iterable(iterable):
         raise TypeError(f'<iterable> expects an iterable. Got {type(iterable).__name__}')
 
     flat = []
     for x in iterable:
-        if is_generator(x):
-            flat.append(x)
-        elif is_iterable(x):
+        if isinstance(x, (dict, set, list, tuple)) and len(x):
             flat.extend(x)
         else:
             flat.append(x)
 
     return flat
 
 
@@ -386,14 +385,142 @@
 
     try:
         return next(filter(key, data))
     except StopIteration:
         return None
 
 
+def pop_min(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the minimum element from the collection.
+    If key is specified, the minimum element is determined by the key.
+    """
+    if not is_iterable(data):
+        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
+    elif isinstance(data, dict):
+        raise TypeError(f'<data> expects any iterable besides dict. For dict, use `pop_min_key` or `pop_min_value` instead')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    original_type = type(data)
+    data = [copy.deepcopy(item) for item in data]
+    found = min(data, key=key, default=_UNDEFINED)
+    if found is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty collection unless a default value is provided')
+
+    data.remove(found)
+    if original_type in (list, tuple, set, frozenset):
+        return found, original_type(data)
+    else:
+        return found, data
+
+
+def pop_max(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the maximum element from the collection.
+    If key is specified, the maximum element is determined by the key.
+    """
+    if not is_iterable(data):
+        raise TypeError(f'<data> expects an iterable. Got {type(data).__name__}: {data!r}')
+    elif isinstance(data, dict):
+        raise TypeError(f'<data> expects any iterable besides dict. For dict, use `pop_max_key` or `pop_max_value` instead')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    original_type = type(data)
+    data = [copy.deepcopy(item) for item in data]
+    found = max(data, key=key, default=_UNDEFINED)
+    if found is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty collection unless a default value is provided')
+
+    data.remove(found)
+    if original_type in (list, tuple, set, frozenset):
+        return found, original_type(data)
+    else:
+        return found, data
+
+
+def pop_max_by_dict_key(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the maximum (kay, value) pair from the dict based on the dict key.
+
+    If the <key> arg is specified, it will be used to calculate the maximum.
+    This key is the function by which to calculate the max, not the dict key
+    """
+    if not isinstance(data, dict):
+        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    data = copy.deepcopy(data)
+    dict_key = max(data.keys(), key=key, default=_UNDEFINED)
+    if dict_key is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+
+    value = data.pop(dict_key)
+    return (dict_key, value), data
+
+
+def pop_min_by_dict_key(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the minimum (kay, value) pair from the dict based on the dict key.
+
+    If the <key> arg is specified, it will be used to calculate the minimum.
+    This key is the function by which to calculate the min, not the dict key
+    """
+    if not isinstance(data, dict):
+        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    data = copy.deepcopy(data)
+    dict_key = min(data.keys(), key=key, default=_UNDEFINED)
+    if dict_key is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+
+    value = data.pop(dict_key)
+    return (dict_key, value), data
+
+
+def pop_max_by_dict_value(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the maximum (kay, value) pair from the dict based on the dict key.
+
+    If the <key> arg is specified, it will be used to calculate the maximum.
+    This key is the function by which to calculate the max, not the dict key
+    """
+    if not isinstance(data, dict):
+        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    data = copy.deepcopy(data)
+    item = max(data.items(), key=lambda kv: key(kv[1]), default=_UNDEFINED)
+    if item is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+
+    _ = data.pop(item[0])
+    return item, data
+
+
+def pop_min_by_dict_value(data, *, key=lambda x: x, default=_UNDEFINED):
+    """Removes and returns the minimum (kay, value) pair from the dict based on the dict key.
+
+    If the <key> arg is specified, it will be used to calculate the minimum.
+    This key is the function by which to calculate the min, not the dict key
+    """
+    if not isinstance(data, dict):
+        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}: {data!r}')
+    elif not callable(key):
+        raise TypeError(f'<key> expects a function. Got {type(key).__name__}: {key!r}')
+
+    data = copy.deepcopy(data)
+    item = min(data.items(), key=lambda kv: key(kv[1]), default=_UNDEFINED)
+    if item is _UNDEFINED and default is _UNDEFINED:
+        raise ValueError('Cannot pop from an empty dict unless a default value is provided')
+
+    _ = data.pop(item[0])
+    return item, data
+
+
 def pick_all(needles, haystack):
     if not is_iterable(needles):
         raise TypeError(f'<needles> expects an iterable. Got {type(needles).__name__}: {needles!r}')
     elif not is_iterable(haystack):
         raise TypeError(f'<haystack> expects an iterable. Got {type(haystack).__name__}: {haystack!r}')
 
     return [needle for needle in needles if is_any_of(needle, haystack)]
@@ -541,14 +668,21 @@
             return tuple(data)
         else:
             return data
     else:  # pragma: no cover
         raise AssertionError(f'Unexpected branch for <data> of type {type(data).__name__}')
 
 
+def swap_keys_and_values(data):
+    if not isinstance(data, dict):
+        raise TypeError(f'<data> expects a dict. Got {type(data).__name__}')
+
+    return {v: k for k, v in data.items()}
+
+
 def xor(*values, key=bool):
     if len(values) < 2:
         raise ValueError('<values> expects at least two values')
     elif not callable(key):
         raise TypeError(f'<key> expects a function. Got {type(key).__name__}')
 
     v = None
```

### Comparing `katalytic-data-0.8.0/src/katalytic/data/checks.py` & `katalytic-data-0.9.0/src/katalytic/data/checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/tests/test_checks.py` & `katalytic-data-0.9.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.8.0/tests/test_data.py` & `katalytic-data-0.9.0/tests/test_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from _decimal import Decimal
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
-from katalytic.data.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
+from katalytic.data.checks import is_generator, is_generator_function, is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
     _C, _C_obj, _callables, _collections, _dict_views, _flatten, _function, _functions, _generators, _iterables, _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
-    map_recursive, one, pick_all, pick_all_besides, pick_any, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
-    as_dict_of_lists, sort_recursive, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
+    map_recursive, one, pick_all, pick_all_besides, pick_any, pop_max, pop_max_by_dict_key, pop_max_by_dict_value, pop_min, pop_min_by_dict_key, pop_min_by_dict_value, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
+    as_dict_of_lists, sort_recursive, swap_keys_and_values, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
 
 
@@ -569,14 +569,220 @@
         {0, 1, 2, 3},
         {3, 2, 1, 0},
     ])
     def test_one_of_set(self, data):
         assert one(data) in data
 
 
+class Test_pop_min:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    def test_not_an_iterable(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min(wrong_type)
+
+    def test_dict(self):
+        with pytest.raises(TypeError):
+            pop_min({})
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min([1], key=wrong_type)
+
+    @pytest.mark.parametrize('data', all_types('iterables'))
+    def test_empty(self, data):
+        if isinstance(data, dict):
+            return
+        elif is_generator_function(data):
+            data = data()
+            next(data)
+
+        with pytest.raises(ValueError):
+            pop_min(data)
+
+    @pytest.mark.parametrize('data, expected', [
+        ([3,2,1,4], (1, [3,2,4])),
+        ((0,-1,3,4), (-1, (0,3,4))),
+        (map(float, (0,3,-4,5)), (-4, [0,3,5])),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_min(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ([3,2,1,4], (4, [3,2,1])),
+        ((0,-1,3,4), (4, (0,-1,3))),
+        (map(float, (0,3,-4,5)), (5, [0,3,-4])),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_min(data, key=lambda x: -x) == expected
+
+
+class Test_pop_max:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
+    def test_not_an_iterable(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max(wrong_type)
+
+    def test_dict(self):
+        with pytest.raises(TypeError):
+            pop_max({})
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max([1], key=wrong_type)
+
+    @pytest.mark.parametrize('data', all_types('iterables'))
+    def test_empty(self, data):
+        if isinstance(data, dict):
+            return
+        elif is_generator_function(data):
+            data = data()
+            next(data)
+
+        with pytest.raises(ValueError):
+            pop_max(data)
+
+    @pytest.mark.parametrize('data, expected', [
+        ([3,2,1,4], (4, [3,2,1])),
+        ((0,-1,3,4), (4, (0,-1,3))),
+        (map(float, (0,3,-4,5)), (5, [0,3,-4])),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_max(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ([3,2,1,4], (1, [3,2,4])),
+        ({0,-1,3,4}, (-1, {0,3,4})),
+        (map(float, (0,3,-4,5)), (-4, [0,3,5])),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_max(data, key=lambda x: -x) == expected
+
+
+class Test_pop_max_by_dict_key:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    def test_not_a_dict(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max_by_dict_key(wrong_type)
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max_by_dict_key({'1': 1}, key=wrong_type)
+
+    def test_empty(self):
+        with pytest.raises(ValueError):
+            pop_max_by_dict_key({})
+
+    @pytest.mark.parametrize('data, expected', [
+        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
+        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('d', 3), {'a': 0, 'b': -1, 'c': 4})),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_max_by_dict_key(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((1, 'c'), {3: 'a', 2: 'b', 4: 'd'})),
+        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((-1, 'b'), {0: 'a', 4: 'c', 3: 'd'})),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_max_by_dict_key(data, key=lambda x: -x) == expected
+
+
+class Test_pop_min_by_dict_key:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    def test_not_a_dict(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min_by_dict_key(wrong_type)
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min_by_dict_key({'1': 1}, key=wrong_type)
+
+    def test_empty(self):
+        with pytest.raises(ValueError):
+            pop_min_by_dict_key({})
+
+    @pytest.mark.parametrize('data, expected', [
+        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('a', 3), {'b': 2, 'c': 1, 'd': 4})),
+        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('a', 0), {'b': -1, 'c': 4, 'd': 3})),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_min_by_dict_key(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
+        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((4, 'c'), {0: 'a', -1: 'b', 3: 'd'})),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_min_by_dict_key(data, key=lambda x: -x) == expected
+
+
+class Test_pop_max_by_dict_value:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    def test_not_a_dict(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max_by_dict_value(wrong_type)
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_max_by_dict_value({'1': 1}, key=wrong_type)
+
+    def test_empty(self):
+        with pytest.raises(ValueError):
+            pop_max_by_dict_value({})
+
+    @pytest.mark.parametrize('data, expected', [
+        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('d', 4), {'a': 3, 'b': 2, 'c': 1})),
+        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('c', 4), {'a': 0, 'b': -1, 'd': 3})),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_max_by_dict_value(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((3, 'a'), {2: 'b', 1: 'c', 4: 'd'})),
+        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((0, 'a'), {-1: 'b', 4: 'c', 3: 'd'})),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_max_by_dict_value(data, key=lambda x: -ord(x)) == expected
+
+
+class Test_pop_min_by_dict_value:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    def test_not_a_dict(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min_by_dict_value(wrong_type)
+
+    @pytest.mark.parametrize('wrong_type', all_types_besides('callables'))
+    def test_key_is_not_a_function(self, wrong_type):
+        with pytest.raises(TypeError):
+            pop_min_by_dict_value({'1': 1}, key=wrong_type)
+
+    def test_empty(self):
+        with pytest.raises(ValueError):
+            pop_min_by_dict_value({})
+
+    @pytest.mark.parametrize('data, expected', [
+        ({'a': 3, 'b': 2, 'c': 1, 'd': 4}, (('c', 1), {'a': 3, 'b': 2, 'd': 4})),
+        ({'a': 0, 'b': -1, 'c': 4, 'd': 3}, (('b', -1), {'a': 0, 'c': 4, 'd': 3})),
+    ])
+    def test_no_key(self, data, expected):
+        assert pop_min_by_dict_value(data) == expected
+
+    @pytest.mark.parametrize('data, expected', [
+        ({3: 'a', 2: 'b', 1: 'c', 4: 'd'}, ((4, 'd'), {3: 'a', 2: 'b', 1: 'c'})),
+        ({0: 'a', -1: 'b', 4: 'c', 3: 'd'}, ((3, 'd'), {0: 'a', -1: 'b', 4: 'c'})),
+    ])
+    def test_with_key(self, data, expected):
+        assert pop_min_by_dict_value(data, key=lambda x: -ord(x)) == expected
+
+
 class Test_pick_all:
     @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
     def test_needles_should_be_iterable(self, wrong_type):
         with pytest.raises(TypeError):
             pick_all(wrong_type, [])
 
     @pytest.mark.parametrize('wrong_type', [object(), 1, True, False, None, ''])
@@ -1003,14 +1209,30 @@
     def test_sort_recursive(self, kwargs, expected):
         if is_iterator(expected):
             assert list(sort_recursive(**kwargs)) == list(expected)
         else:
             assert sort_recursive(**kwargs) == expected
 
 
+class Test_swap_keys_and_values:
+    @pytest.mark.parametrize('wrong_type', all_types_besides('dict'))
+    def test_wrong_type(self, wrong_type):
+        with pytest.raises(TypeError):
+            swap_keys_and_values(wrong_type)
+
+    @pytest.mark.parametrize('data, expected', [
+        ({1: 2}, {2: 1}),
+        ({1: 'a', 3: 'b'}, {'a': 1, 'b': 3}),
+        ({1: 2, 3: 2}, {2: 3}),
+        ({}, {})
+    ])
+    def test_simple(self, data, expected):
+        assert swap_keys_and_values(data) == expected
+
+
 class Test_xor:
     @pytest.mark.parametrize('wrong_type', [iter([]), map(lambda x: x, []), range(1), object(), [], {}, (), set(), 1, True, False, None, ''])
     def test_key_should_be_callable(self, wrong_type):
         with pytest.raises(TypeError):
             xor(1, 2, key=wrong_type)
 
     @pytest.mark.parametrize('values', [
```

### Comparing `katalytic-data-0.8.0/PKG-INFO` & `katalytic-data-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.8.0
+Version: 0.9.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

