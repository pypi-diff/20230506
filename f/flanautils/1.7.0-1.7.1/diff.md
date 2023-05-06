# Comparing `tmp/flanautils-1.7.0.tar.gz` & `tmp/flanautils-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flanautils-1.7.0.tar", last modified: Tue Jan 10 22:46:09 2023, max compression
+gzip compressed data, was "flanautils-1.7.1.tar", last modified: Sat May  6 18:46:02 2023, max compression
```

## Comparing `flanautils-1.7.0.tar` & `flanautils-1.7.1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.475508 flanautils-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-01-10 22:45:52.000000 flanautils-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-10 22:46:09.475508 flanautils-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-01-10 22:45:52.000000 flanautils-1.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.467508 flanautils-1.7.0/flanautils/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/asyncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.471508 flanautils-1.7.0/flanautils/data_structures/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/data_structures/bi_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/data_structures/ordered_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/iterables.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/medias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.471508 flanautils-1.7.0/flanautils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/media.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/plotly_charts.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/score_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/models/time_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/oss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.471508 flanautils-1.7.0/flanautils/resources/
--rw-r--r--   0 runner    (1001) docker     (123)  3602215 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/resources/plotly_es.js
--rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-01-10 22:45:52.000000 flanautils-1.7.0/flanautils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 22:46:09.467508 flanautils-1.7.0/flanautils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-01-10 22:46:09.000000 flanautils-1.7.0/flanautils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-10 22:46:09.000000 flanautils-1.7.0/flanautils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 22:46:09.000000 flanautils-1.7.0/flanautils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-10 22:46:09.000000 flanautils-1.7.0/flanautils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-10 22:46:09.000000 flanautils-1.7.0/flanautils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-01-10 22:45:52.000000 flanautils-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-10 22:46:09.475508 flanautils-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.574962 flanautils-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-06 18:45:48.000000 flanautils-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-06 18:46:02.574962 flanautils-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-06 18:45:48.000000 flanautils-1.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/asyncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/bi_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/data_structures/ordered_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/iterables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/medias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25248 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/plotly_charts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/score_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/models/time_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/oss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)  3602215 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/resources/plotly_es.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14597 2023-05-06 18:45:48.000000 flanautils-1.7.1/flanautils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.570962 flanautils-1.7.1/flanautils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-06 18:46:02.000000 flanautils-1.7.1/flanautils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 18:45:48.000000 flanautils-1.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-06 18:46:02.574962 flanautils-1.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:46:02.574962 flanautils-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-06 18:45:48.000000 flanautils-1.7.1/tests/test_utils.py
```

### Comparing `flanautils-1.7.0/LICENSE` & `flanautils-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/PKG-INFO` & `flanautils-1.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanautils
-Version: 1.7.0
+Version: 1.7.1
 Summary: Set of utilities of all kinds to develop python projects.
 Home-page: https://github.com/AlberLC/flanautils
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanautils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanautils-1.7.0/README.rst` & `flanautils-1.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/constants.py` & `flanautils-1.7.1/flanautils/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import datetime
 import random
 from typing import Iterable, Sequence
 
 from flanautils.data_structures.bi_dict import BiDict
 from flanautils.data_structures.ordered_set import OrderedSet
 
+GOOGLE_BOT_USER_AGENTS = [
+    "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)",
+    "Googlebot/2.1 (+http://www.googlebot.com/bot.html)",
+    "Googlebot/2.1 (+http://www.google.com/bot.html)"
+]
 NUMBER_WORDS = {
     'es': BiDict({
         '+': 'mas',
         '-': 'menos',
         0: 'cero', 1: 'uno', 2: 'dos', 3: 'tres', 4: 'cuatro', 5: 'cinco', 6: 'seis', 7: 'siete', 8: 'ocho', 9: 'nueve',
         10: 'diez', 11: 'once', 12: 'doce', 13: 'trece', 14: 'catorce', 15: 'quince', 16: 'dieciséis',
         20: 'veinte', 30: 'treinta', 40: 'cuarenta', 50: 'cincuenta', 60: 'sesenta', 70: 'setenta', 80: 'ochenta', 90: 'noventa',
@@ -16,14 +21,15 @@
     })
 }
 NUMBERS_SCORE_MATCHING = 0.9
 SYMBOLS = ('!', '"', '#', '$', '%', '&', "'", '(', ')', '*', '+', ',', '-', '.', '/', ':', ';', '<', '=', '>', '?', '@',
            '[', '\\', ']', '^', '_', '`', '{', '|', '}', '~', '¡', '¨', 'ª', '¬', '´', '·', 'º', '¿', '€')
 TEXT_TO_NUMBER_MAX_WORD_LENGTH = 25
 TIME_UNITS_SCORE_MATCHING = 0.9
+USER_AGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/102.0.0.0 Safari/537.36'
 WEEKS_IN_A_MONTH = 4.34524
 WEEKS_IN_A_YEAR = WEEKS_IN_A_MONTH * 12
 
 
 class CommonWords:
     common_words = {
         'en': {
```

### Comparing `flanautils-1.7.0/flanautils/data_structures/bi_dict.py` & `flanautils-1.7.1/flanautils/data_structures/bi_dict.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/data_structures/ordered_set.py` & `flanautils-1.7.1/flanautils/data_structures/ordered_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,32 +23,33 @@
     """
 
     FLATTEN_DEPTH = 1
 
     T = TypeVar('T', bound='OrdereSet')
 
     def __init__(self, *args: Any):
-        self._elements_dict = {element: None for element in iterables.flatten_iterator(*args, depth=self.FLATTEN_DEPTH)}
+        self._elements_dict = {element: None for element in iterables.flatten(*args, depth=self.FLATTEN_DEPTH, lazy=True)}
 
     def __add__(self, other: Any) -> OrderedSet[E]:
         return self | other
 
-    def __iadd__(self, other: Any):
+    def __iadd__(self, other: Any) -> OrderedSet[E]:
         return self.__ior__(other)
 
     def __radd__(self, other: Any) -> OrderedSet[E]:
         return other | self
 
     def __and__(self, other: Any) -> OrderedSet[E]:
-        return OrderedSet(value for value in self if value in self.ordered_set_if_not_set(other))
-
-    def __iand__(self, other: Any):
-        for value in (self - self.ordered_set_if_not_set(other)):
-            self.discard(value)
-        return self
+        # the super implementation reverses the order so the code is the same but reversed to maintain the order
+        # noinspection PyUnresolvedReferences
+        return self._from_iterable(value for value in self if value in self.ordered_set_if_not_set(other))
+
+    def __iand__(self, other: Any) -> OrderedSet[E]:
+        # noinspection PyTypeChecker
+        return super().__iand__(self.ordered_set_if_not_set(other))
 
     def __rand__(self, other: Any) -> OrderedSet[E]:
         return self.ordered_set_if_not_set(other) & self
 
     def __contains__(self, element: Any) -> bool:
         return element in self._elements_dict
 
@@ -64,15 +65,16 @@
 
         for self_element, other_element in itertools.zip_longest(self, other):
             if self_element != other_element:
                 return False
         return True
 
     def __getitem__(self, item) -> E | OrderedSet[E]:
-        ordered_set = OrderedSet()
+        # noinspection PyUnresolvedReferences
+        ordered_set = self._from_iterable(())
         len_self = len(self)
 
         if isinstance(item, slice):
             step = 1 if item.step is None else item.step
             if step > 0:
                 if item.start is None:
                     start = 0
@@ -146,59 +148,47 @@
     def __iter__(self) -> Iterator[E]:
         return iter(self._elements_dict)
 
     def __len__(self) -> int:
         return len(self._elements_dict)
 
     def __or__(self, other: Any) -> OrderedSet[E]:
-        return OrderedSet(super().__or__(self.ordered_set_if_not_set(other)))
+        # noinspection PyTypeChecker
+        return super().__or__(self.ordered_set_if_not_set(other))
 
-    def __ior__(self, other: Any):
-        for value in self.ordered_set_if_not_set(other):
-            self.add(value)
-        return self
+    def __ior__(self, other: Any) -> OrderedSet[E]:
+        # noinspection PyTypeChecker
+        return super().__ior__(self.ordered_set_if_not_set(other))
 
     def __ror__(self, other: Any) -> OrderedSet[E]:
         return self.ordered_set_if_not_set(other) | self
 
     def __repr__(self) -> str:
         return str(self)
 
     def __reversed__(self) -> Iterator[E]:
         return reversed(self._elements_dict)
 
     def __str__(self) -> str:
         return f"#{{{', '.join(repr(element) for element in self)}}}"
 
     def __sub__(self, other: Any) -> OrderedSet[E]:
-        return OrderedSet(super().__sub__(self.ordered_set_if_not_set(other)))
+        # noinspection PyTypeChecker
+        return super().__sub__(self.ordered_set_if_not_set(other))
 
-    def __isub__(self, other: Any):
-        if other is self:
-            self.clear()
-        else:
-            for value in self.ordered_set_if_not_set(other):
-                self.discard(value)
-        return self
+    def __isub__(self, other: Any) -> OrderedSet[E]:
+        # noinspection PyTypeChecker
+        return super().__isub__(self.ordered_set_if_not_set(other))
 
     def __rsub__(self, other: Any) -> OrderedSet[E]:
         return self.ordered_set_if_not_set(other) - self
 
     def _json_repr(self) -> Any:
         return [json.loads(element.to_json()) if isinstance(element, JSONBASE) else pickle.dumps(element) for element in self]
 
-    def positive_index(self, index_: int) -> int:
-        if index_ < 0:
-            index_ += len(self)
-        return index_
-
-    @classmethod
-    def ordered_set_if_not_set(cls: Type[T], arg: Any) -> AbstractSet | T:
-        return arg if isinstance(arg, AbstractSet) else cls(iterables.flatten_iterator(arg))
-
     def add(self, element: Any):
         self._elements_dict[element] = None
 
     def add_many(self, elements: Iterable):
         for element in elements:
             self.add(element)
 
@@ -206,23 +196,25 @@
         try:
             while True:
                 self.pop()
         except IndexError:
             pass
 
     def copy(self) -> OrderedSet[E]:
-        return OrderedSet(self)
+        # noinspection PyUnresolvedReferences
+        return self._from_iterable(self)
 
     def difference(self, *args: Iterable) -> OrderedSet[E]:
-        new_ordered_set = OrderedSet(self)
+        # noinspection PyUnresolvedReferences
+        new_ordered_set = self._from_iterable(self)
         new_ordered_set.difference_update(*args)
         return new_ordered_set
 
     def difference_update(self, *args: Iterable):
-        self.discard_many(iterables.flatten_iterator(*args, depth=self.FLATTEN_DEPTH))
+        self.discard_many(iterables.flatten(*args, depth=self.FLATTEN_DEPTH, lazy=True))
 
     def discard(self, element: Any):
         try:
             self._elements_dict.pop(element, None)
         except TypeError:
             pass
 
@@ -248,77 +240,86 @@
         if raise_exception:
             raise ValueError(f'{element} is not in the OrderedSet')
 
     def insert(self, i, element):
         if element in self:
             return
 
-        i = self.positive_index(i)
-
         deleted_elements = []
-        for i_, element_ in enumerate(list(self)):
-            if i <= i_:
-                self.discard(element_)
-                deleted_elements.append(element_)
+        for element_ in list(self)[i:]:
+            self.discard(element_)
+            deleted_elements.append(element_)
 
         self.add(element)
         self.add_many(deleted_elements)
 
     def intersection(self, *args: Iterable) -> OrderedSet[E]:
-        new_ordered_set = OrderedSet(self)
+        # noinspection PyUnresolvedReferences
+        new_ordered_set = self._from_iterable(self)
         new_ordered_set.intersection_update(*args)
         return new_ordered_set
 
     def intersection_update(self, *args: Iterable):
         elements_to_delete = []
         for element in self:
             for arg in args:
-                if element not in iterables.flatten_iterator(arg, depth=self.FLATTEN_DEPTH):
+                if element not in iterables.flatten(arg, depth=self.FLATTEN_DEPTH, lazy=True):
                     elements_to_delete.append(element)
                     break
 
         self.discard_many(elements_to_delete)
 
     def is_disjoint(self, other) -> bool:
         return not (self & other)
 
     def is_subset(self, other) -> bool:
         return self <= other
 
     def is_superset(self, other) -> bool:
         return self >= other
 
+    @classmethod
+    def ordered_set_if_not_set(cls: Type[T], arg: Any) -> AbstractSet | T:
+        return arg if isinstance(arg, AbstractSet) else cls(iterables.flatten(arg, lazy=True))
+
     def pop(self, index=-1) -> E:
         element = self[index]
         self.discard(element)
         return element
 
+    def positive_index(self, index_: int) -> int:
+        if index_ < 0:
+            index_ += len(self)
+        return index_
+
     def reverse(self):
         reversed_self = list(reversed(self))
         self.clear()
         self.add_many(reversed_self)
 
     def sort(self, key=None, reverse=False):
         sorted_values = sorted(self, key=key, reverse=reverse)
         self.clear()
         self.add_many(sorted_values)
 
     def symmetric_difference(self, *args: Iterable) -> OrderedSet[E]:
-        new_ordered_set = OrderedSet(self)
+        # noinspection PyUnresolvedReferences
+        new_ordered_set = self._from_iterable(self)
         new_ordered_set.symmetric_difference_update(*args)
         return new_ordered_set
 
     def symmetric_difference_update(self, *args: Iterable):
         for arg in args:
             other_minus_self = self.ordered_set_if_not_set(arg) - self
             self.difference_update(arg)
             self.update(other_minus_self)
 
     def union(self, *args: Iterable) -> OrderedSet[E]:
-        new_ordered_set = OrderedSet(self)
+        # noinspection PyUnresolvedReferences
+        new_ordered_set = self._from_iterable(self)
         new_ordered_set.update(*args)
         return new_ordered_set
 
     def update(self, *args: Iterable):
-        self.add_many(iterables.flatten_iterator(*args, depth=self.FLATTEN_DEPTH))
+        self.add_many(iterables.flatten(*args, depth=self.FLATTEN_DEPTH, lazy=True))
 
     union_update = update
```

### Comparing `flanautils-1.7.0/flanautils/iterables.py` & `flanautils-1.7.1/flanautils/iterables.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 # noinspection PyShadowingNames
 def find(elements: Iterable, target: Any = None, condition: Callable[..., bool] = None, cast_numbers=False) -> Any:
     """
     Smart function that find anything in an iterable (classes, objects, ...).
 
     If condition is not None, return the first element that matches it.
 
-    Return None if nothing matches.
+    Returns None if nothing matches.
 
     >>> elements = [1, 2, '3', 4, 'hola', '6.6']
 
     >>> find(elements, 2)
     2
     >>> find(elements, int)
     1
@@ -105,68 +105,71 @@
     >>> find(elements, float, cast_numbers=True)
     6.6
     """
 
     return next(filter(elements, target, condition, cast_numbers, lazy=True), None)
 
 
-def flatten_iterator(*args: Iterable, depth=None) -> Iterator:
+def flatten(*args: Iterable, depth=None, lazy=False) -> Iterator | list:
     """
     Iterates and flattens iterables recursively according to the specified depth.
 
     If depth=None (the default) it flattens recursively until it finds no iterable.
 
-    >>> type(flatten_iterator([1, 2, [3, 4, ['cinco']]]))
+    >>> type(flatten([1, 2, [3, 4, ['cinco']]]))
+    <class 'list'>
+    >>> type(flatten([1, 2, [3, 4, ['cinco']]], lazy=True))
     <class 'generator'>
-    >>> list(flatten_iterator([1, 2, [3, 4, ['cinco']]]))
+    >>> flatten([1, 2, [3, 4, ['cinco']]])
     [1, 2, 3, 4, 'cinco']
-    >>> list(flatten_iterator([1, 2, [3, 4, ['cinco']]], depth=1))
+    >>> flatten([1, 2, [3, 4, ['cinco']]], depth=1)
     [1, 2, [3, 4, ['cinco']]]
-    >>> list(flatten_iterator([1, 2, [3, 4, ['cinco']]], depth=2))
+    >>> flatten([1, 2, [3, 4, ['cinco']]], depth=2)
     [1, 2, 3, 4, ['cinco']]
     """
 
     current_depth = -1
 
-    def flatten_iterator_(*args_: Iterable, depth_=None) -> Iterator:
+    def flatten_generator(*args_: Iterable, depth_=None) -> Iterator:
         nonlocal current_depth
 
         if depth_ is not None:
             current_depth += 1
 
         for arg_ in args_:
             if (
                     isinstance(arg_, Iterable)
                     and
                     not isinstance(arg_, (str, bytes))
                     and
                     (depth_ is None or current_depth < depth_)
             ):
-                yield from flatten_iterator_(*arg_, depth_=depth_)
+                yield from flatten_generator(*arg_, depth_=depth_)
                 if depth_ is not None:
                     current_depth -= 1
             else:
                 yield arg_
 
-    return flatten_iterator_(*args, depth_=depth)
+    generator_ = flatten_generator(*args, depth_=depth)
+    return generator_ if lazy else list(generator_)
 
 
 @overload
 def frange(start: float = 0, stop: float = float('inf'), step: float = 1, include_last=False) -> Iterator[float]:
     pass
 
 
 @overload
 def frange(stop: float = 0, include_last=False) -> Iterator[float]:
     pass
 
 
 def frange(start: float = None, stop: float = None, step: float = 1, include_last=False) -> Iterator[float]:
     """
-    Return a Generator that works like range but with floats.
+    Returns a Generator that works like range but with floats.
 
     Can generate infinite numerical series.
 
     >>> type(frange(5))
     <class 'generator'>
     >>> list(frange(5))
     [0.0, 1.0, 2.0, 3.0, 4.0]
```

### Comparing `flanautils-1.7.0/flanautils/medias.py` & `flanautils-1.7.1/flanautils/medias.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/models/bases.py` & `flanautils-1.7.1/flanautils/models/bases.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,18 +432,15 @@
             kwargs['skip'] = skip
         if limit is not None:
             kwargs['limit'] = limit
         cursor: pymongo.cursor.Cursor = cls.collection.find(query, **kwargs)
         if sort_keys:
             cursor.sort(sort_keys)
 
-        if lazy:
-            return find_generator()
-        else:
-            return [cls.from_dict(document) for document in cursor]
+        return find_generator() if lazy else list(find_generator())
 
     def find_in_database_by_id(self, object_id: ObjectId) -> dict | None:
         """Find an object in all database collections by its ObjectId."""
 
         if self.database is None:
             return
```

### Comparing `flanautils-1.7.0/flanautils/models/database.py` & `flanautils-1.7.1/flanautils/models/database.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/models/enums.py` & `flanautils-1.7.1/flanautils/models/enums.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/models/media.py` & `flanautils-1.7.1/flanautils/models/media.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/models/plotly_charts.py` & `flanautils-1.7.1/flanautils/models/plotly_charts.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/models/score_match.py` & `flanautils-1.7.1/flanautils/models/score_match.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/oss.py` & `flanautils-1.7.1/flanautils/oss.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import os
 import pathlib
 import pkgutil
 import subprocess
+import sys
 from collections.abc import Iterator
 from contextlib import contextmanager
 
 from flanautils import strings
 
 
 def find_paths_by_stem(
@@ -65,22 +66,62 @@
             subprocess.run(f'setx /m {k} {v}')
     else:
         for k, v in variables.items():
             os.environ[k] = v
 
 
 @contextmanager
+def suppress_low_level_stderr():
+    """A context manager that redirects low level stderr to devnull."""
+
+    with open(os.devnull, 'w') as err_null_file:
+        stderr_fileno = sys.stderr.fileno()
+        old_stderr_fileno = os.dup(sys.stderr.fileno())
+        old_stderr = sys.stderr
+
+        os.dup2(err_null_file.fileno(), stderr_fileno)
+        sys.stderr = err_null_file
+
+        try:
+            yield
+        finally:
+            sys.stderr = old_stderr
+            os.dup2(old_stderr_fileno, stderr_fileno)
+
+            os.close(old_stderr_fileno)
+
+
+@contextmanager
+def suppress_low_level_stdout():
+    """A context manager that redirects low level stdout to devnull."""
+
+    with open(os.devnull, 'w') as out_null_file:
+        stdout_fileno = sys.stdout.fileno()
+        old_stdout_fileno = os.dup(sys.stdout.fileno())
+        old_stdout = sys.stdout
+
+        os.dup2(out_null_file.fileno(), stdout_fileno)
+        sys.stdout = out_null_file
+
+        try:
+            yield
+        finally:
+            sys.stdout = old_stdout
+            os.dup2(old_stdout_fileno, stdout_fileno)
+
+            os.close(old_stdout_fileno)
+
+
+@contextmanager
 def suppress_stderr():
     """A context manager that redirects stderr to devnull."""
 
-    with open(os.devnull, 'w') as fnull:
-        with contextlib.redirect_stderr(fnull) as err:
-            yield err
+    with open(os.devnull, 'w') as null_file, contextlib.redirect_stderr(null_file):
+        yield
 
 
 @contextmanager
 def suppress_stdout():
     """A context manager that redirects stdout to devnull."""
 
-    with open(os.devnull, 'w') as fnull:
-        with contextlib.redirect_stdout(fnull) as out:
-            yield out
+    with open(os.devnull, 'w') as null_file, contextlib.redirect_stdout(null_file):
+        yield
```

### Comparing `flanautils-1.7.0/flanautils/resources/plotly_es.js` & `flanautils-1.7.1/flanautils/resources/plotly_es.js`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils/strings.py` & `flanautils-1.7.1/flanautils/strings.py`

 * *Files identical despite different names*

### Comparing `flanautils-1.7.0/flanautils.egg-info/PKG-INFO` & `flanautils-1.7.1/flanautils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: flanautils
-Version: 1.7.0
+Version: 1.7.1
 Summary: Set of utilities of all kinds to develop python projects.
 Home-page: https://github.com/AlberLC/flanautils
 Author: AlberLC
-Author-email: alberlc@outlook.com
 Project-URL: Bug Tracker, https://github.com/AlberLC/flanautils/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `flanautils-1.7.0/flanautils.egg-info/SOURCES.txt` & `flanautils-1.7.1/flanautils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 flanautils/constants.py
 flanautils/decorators.py
 flanautils/exceptions.py
 flanautils/iterables.py
 flanautils/maths.py
 flanautils/medias.py
 flanautils/oss.py
+flanautils/requests.py
 flanautils/strings.py
 flanautils.egg-info/PKG-INFO
 flanautils.egg-info/SOURCES.txt
 flanautils.egg-info/dependency_links.txt
 flanautils.egg-info/requires.txt
 flanautils.egg-info/top_level.txt
 flanautils/data_structures/__init__.py
@@ -24,8 +25,9 @@
 flanautils/models/bases.py
 flanautils/models/database.py
 flanautils/models/enums.py
 flanautils/models/media.py
 flanautils/models/plotly_charts.py
 flanautils/models/score_match.py
 flanautils/models/time_units.py
-flanautils/resources/plotly_es.js
+flanautils/resources/plotly_es.js
+tests/test_utils.py
```

### Comparing `flanautils-1.7.0/setup.cfg` & `flanautils-1.7.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [metadata]
 name = flanautils
-version = v1.7.0
+version = v1.7.1
 author = AlberLC
-author_email = alberlc@outlook.com
 description = Set of utilities of all kinds to develop python projects.
 long_description = file: README.rst
 url = https://github.com/AlberLC/flanautils
 project_urls = 
 	Bug Tracker = https://github.com/AlberLC/flanautils/issues
 classifiers = 
 	Programming Language :: Python :: 3.10
```

