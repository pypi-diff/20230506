# Comparing `tmp/ensure-1.0.2.tar.gz` & `tmp/ensure-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensure-1.0.2.tar", last modified: Sun Dec  5 19:32:19 2021, max compression
+gzip compressed data, was "ensure-1.0.3.tar", last modified: Sat May  6 15:59:09 2023, max compression
```

## Comparing `ensure-1.0.2.tar` & `ensure-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2021-12-05 19:32:19.503743 ensure-1.0.2/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2021-12-05 18:42:32.000000 ensure-1.0.2/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2021-12-05 18:42:32.000000 ensure-1.0.2/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10277 2021-12-05 19:32:19.503933 ensure-1.0.2/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9269 2021-12-05 19:21:39.000000 ensure-1.0.2/README.rst
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2021-12-05 19:32:19.500956 ensure-1.0.2/ensure/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      287 2021-12-05 18:42:32.000000 ensure-1.0.2/ensure/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1051 2021-12-05 18:42:32.000000 ensure-1.0.2/ensure/_types.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    32226 2021-12-05 18:42:32.000000 ensure-1.0.2/ensure/main.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2021-12-05 19:32:19.502960 ensure-1.0.2/ensure.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10277 2021-12-05 19:32:19.000000 ensure-1.0.2/ensure.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      279 2021-12-05 19:32:19.000000 ensure-1.0.2/ensure.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2021-12-05 19:32:19.000000 ensure-1.0.2/ensure.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       36 2021-12-05 19:32:19.000000 ensure-1.0.2/ensure.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        7 2021-12-05 19:32:19.000000 ensure-1.0.2/ensure.egg-info/top_level.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       13 2021-12-05 18:42:32.000000 ensure-1.0.2/requirements.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      131 2021-12-05 19:32:19.504712 ensure-1.0.2/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1340 2021-12-05 19:31:38.000000 ensure-1.0.2/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2021-12-05 19:32:19.503386 ensure-1.0.2/test/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    17198 2021-12-05 19:07:26.000000 ensure-1.0.2/test/test.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-05-06 15:59:09.280455 ensure-1.0.3/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10273 2016-06-14 14:20:58.000000 ensure-1.0.3/LICENSE
+-rw-r--r--   0 kislyuk    (501) staff       (20)       41 2016-12-24 17:11:43.000000 ensure-1.0.3/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10276 2023-05-06 15:59:09.280298 ensure-1.0.3/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)     9269 2023-05-06 15:37:06.000000 ensure-1.0.3/README.rst
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-05-06 15:59:09.278962 ensure-1.0.3/ensure/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      203 2023-05-06 15:49:56.000000 ensure-1.0.3/ensure/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      857 2023-05-06 15:51:52.000000 ensure-1.0.3/ensure/_types.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    32022 2023-05-06 15:51:52.000000 ensure-1.0.3/ensure/main.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-05-06 15:59:09.279776 ensure-1.0.3/ensure.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10276 2023-05-06 15:59:09.000000 ensure-1.0.3/ensure.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)      284 2023-05-06 15:59:09.000000 ensure-1.0.3/ensure.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-05-06 15:59:09.000000 ensure-1.0.3/ensure.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       34 2023-05-06 15:59:09.000000 ensure-1.0.3/ensure.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        7 2023-05-06 15:59:09.000000 ensure-1.0.3/ensure.egg-info/top_level.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      187 2023-05-06 15:47:57.000000 ensure-1.0.3/pyproject.toml
+-rw-r--r--   0 kislyuk    (501) staff       (20)       13 2016-06-14 14:20:58.000000 ensure-1.0.3/requirements.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       38 2023-05-06 15:59:09.280489 ensure-1.0.3/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1328 2023-05-06 15:58:09.000000 ensure-1.0.3/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-05-06 15:59:09.279875 ensure-1.0.3/test/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    16722 2023-05-06 15:52:35.000000 ensure-1.0.3/test/test.py
```

### Comparing `ensure-1.0.2/LICENSE` & `ensure-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ensure-1.0.2/PKG-INFO` & `ensure-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: ensure
-Version: 1.0.2
+Version: 1.0.3
 Summary: Literate BDD assertions in Python with no magic
 Home-page: https://github.com/kislyuk/ensure
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
 ensure: Literate assertions in Python
 =====================================
 *ensure* is a set of simple assertion helpers that let you write more expressive, literate, concise, and readable
 Pythonic code for validating conditions. It's inspired by `should.js <https://github.com/shouldjs/should.js>`_,
@@ -263,9 +263,7 @@
         :target: https://github.com/kislyuk/ensure/actions
 .. image:: https://codecov.io/github/kislyuk/ensure/coverage.svg?branch=master
         :target: https://codecov.io/github/kislyuk/ensure?branch=master
 .. image:: https://img.shields.io/pypi/v/ensure.svg
         :target: https://pypi.python.org/pypi/ensure
 .. image:: https://img.shields.io/pypi/l/ensure.svg
         :target: https://pypi.python.org/pypi/ensure
-
-
```

### Comparing `ensure-1.0.2/README.rst` & `ensure-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `ensure-1.0.2/ensure/main.py` & `ensure-1.0.3/ensure/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,28 @@
-from __future__ import absolute_import, division, print_function, unicode_literals
-
-import sys
-import types
 import re
+import types
 from unittest.case import TestCase
+
 try:
-    from collections.abc import Mapping, Iterable
+    from collections.abc import Iterable, Mapping
 except ImportError:
     from collections import Mapping, Iterable
 
 from six import string_types
 
-from ._types import NumericString, NumericByteString, IntegerString, IntegerByteString
-
-USING_PYTHON2 = True if sys.version_info < (3, 0) else False
+from ._types import IntegerByteString, IntegerString, NumericByteString, NumericString
 
 try:
     from repr import Repr
 except ImportError:
     from reprlib import Repr
 
 _repr = Repr().repr
 
-unittest_case = TestCase(methodName='__init__')
+unittest_case = TestCase(methodName="__init__")
 
 
 def _format(message, *args):
     return message.format(*map(_repr, args))
 
 
 class EnsureError(AssertionError):
@@ -48,18 +44,20 @@
         self._args = []
         self._kwargs = {}
         self._call_subject = False
         return self
 
     def __repr__(self):
         desc = "<{module}.{classname} object at 0x{mem_loc:x} inspecting {subject}>"
-        return desc.format(module=self.__module__,
-                           classname=self.__class__.__name__,
-                           mem_loc=id(self),
-                           subject=_repr(self._orig_subject))
+        return desc.format(
+            module=self.__module__,
+            classname=self.__class__.__name__,
+            mem_loc=id(self),
+            subject=_repr(self._orig_subject),
+        )
 
     @property
     def _subject(self):
         if self._call_subject:
             return self._run(self._orig_subject, self._args, self._kwargs)
         else:
             return self._orig_subject
@@ -112,14 +110,15 @@
     @property
     def also(self):
         return Ensure(self._subject)
 
     def __repr__(self):
         return "{}: OK".format(Inspector.__repr__(self))
 
+
 class KeyInspector(Inspector):
     @property
     def whose_value(self):
         return Ensure(self._subject)
 
 
 class CallableInspector(Inspector):
@@ -133,45 +132,48 @@
         return getattr(self._subject, item)
 
 
 class MultiInspector(Inspector):
     """
     Calls a list of inspector objects on a single subject.
     """
+
     def _get_inspector(self, subject):
         return subject
 
     def __getattr__(self, item):
         # @functools.wraps(getattr(self._subject[0], item))
         def inspect(*args, **kwargs):
             sub_inspectors = []
             for subject in self._subject:
                 inspector = self._get_inspector(subject)
                 inspect_method = getattr(inspector, item)
                 sub_inspectors.append(inspect_method(*args, **kwargs))
             if not all(i is None for i in sub_inspectors):
                 return MultiInspector(sub_inspectors)
+
         return inspect
 
 
 class MultiEnsure(MultiInspector):
     """
     Maps a single Ensure object to an iterable of subjects.
     """
+
     def __init__(self, iterable, inspector):
         Inspector.__init__(self, iterable)
         self._inspector = inspector
         self._inspector(iterable).is_an(Iterable)
 
     def _get_inspector(self, subject):
         return self._inspector(subject)
 
 
 class Ensure(Inspector):
-    ''' Constructs a root-level inspector, which can perform a variety of checks (*predicates*) on subjects passed to
+    """Constructs a root-level inspector, which can perform a variety of checks (*predicates*) on subjects passed to
     it. If the checks do not pass, by default :class:`EnsureError` is raised. This can be configured by passing the
     ``error_factory`` keyword to the constructor.
 
     Subjects can be passed to the inspector at construction time or by calling the resulting object (each call resets
     the subject):
 
     .. code-block:: python
@@ -183,15 +185,16 @@
 
     Some predicates return child inspectors which can be chained into a series of predicates, for example:
 
     .. code-block:: python
 
         ensure({1: {2: "a"}}).has_key(1).whose_value.is_a(dict).of(int).to(str)
 
-    '''
+    """
+
     @classmethod
     def each_of(cls, iterable):
         """
         Applies subsequent predicate(s) to all items in *iterable*.
         """
         return MultiEnsure(iterable, cls())
 
@@ -250,16 +253,22 @@
 
     def contains_only(self, elements):
         """
         Ensures :attr:`subject` contains all of *elements*, which must be an iterable, and no other items.
         """
         for element in self._subject:
             if element not in elements:
-                raise self._error_factory(_format("Expected {} to have only {}, but it contains {}",
-                                                  self._subject, elements, element))
+                raise self._error_factory(
+                    _format(
+                        "Expected {} to have only {}, but it contains {}",
+                        self._subject,
+                        elements,
+                        element,
+                    )
+                )
         self.contains_all_of(elements)
         return ChainInspector(self._subject)
 
     def contains_some_of(self, elements):
         """
         Ensures :attr:`subject` contains at least one of *elements*, which must be an iterable.
         """
@@ -271,16 +280,22 @@
 
     def contains_all_of(self, elements):
         """
         Ensures :attr:`subject` contains all of *elements*, which must be an iterable.
         """
         for element in elements:
             if element not in self._subject:
-                raise self._error_factory(_format("Expected {} to have all of {}, but it does not contain {}",
-                                                  self._subject, elements, element))
+                raise self._error_factory(
+                    _format(
+                        "Expected {} to have all of {}, but it does not contain {}",
+                        self._subject,
+                        elements,
+                        element,
+                    )
+                )
         return ChainInspector(self._subject)
 
     def does_not_contain(self, element):
         """
         Ensures :attr:`subject` does not contain *element*.
         """
         self._run(unittest_case.assertNotIn, (element, self._subject))
@@ -403,15 +418,15 @@
         return ChainInspector(self._subject)
 
     def is_a(self, prototype):
         """
         Ensures :attr:`subject` is an object of class *prototype*.
         """
         self._run(unittest_case.assertIsInstance, (self._subject, prototype))
-        if hasattr(self._subject, '__iter__'):
+        if hasattr(self._subject, "__iter__"):
             return IterableInspector(self._subject)
         else:
             return ReferenceInspector(self._subject)
 
     is_an = is_a
     is_an_instance_of = is_a
 
@@ -526,17 +541,23 @@
         return self.is_an_iterable_of(prototype)
 
     def is_numeric(self):
         """
         Ensures :attr:`subject` is an int, float, or long.
         """
         from decimal import Decimal
-        numeric_types = (int, float, long, Decimal) if USING_PYTHON2 else (int, float, Decimal)  # noqa
+
+        numeric_types = (int, float, Decimal)
         if not isinstance(self._subject, numeric_types):
-            raise self._error_factory(_format("Expected {} to be numeric (int, float, long or Decimal)", self._subject))
+            raise self._error_factory(
+                _format(
+                    "Expected {} to be numeric (int, float, long or Decimal)",
+                    self._subject,
+                )
+            )
 
     def is_callable(self):
         """
         Ensures :attr:`subject` is a callable.
         """
         if not callable(self._subject):
             raise self._error_factory(_format("Expected {} to be callable", self._subject))
@@ -547,67 +568,73 @@
         *max* (if given).
         """
         unittest_case.assertFalse(length is None and min is None and max is None)
         my_length = len(self._subject)
         if length is not None:
             try:
                 unittest_case.assertTrue(my_length == length)
-            except self._catch as err:
+            except self._catch:
                 raise self._error_factory(_format("Expected {} to have length {}", self._subject, length))
         if min is not None:
             try:
                 unittest_case.assertTrue(my_length >= min)
-            except self._catch as err:
+            except self._catch:
                 raise self._error_factory(_format("Expected {} to have length at least {}", self._subject, min))
         if max is not None:
             try:
                 unittest_case.assertTrue(my_length <= max)
-            except self._catch as err:
+            except self._catch:
                 raise self._error_factory(_format("Expected {} to have length at most {}", self._subject, max))
         return ChainInspector(self._subject)
 
     def is_greater_than(self, other):
         """
         Ensures :attr:`subject` is greater than *other*.
         """
         try:
             unittest_case.assertTrue(self._subject > other)
-        except self._catch as err:
+        except self._catch:
             raise self._error_factory(_format("Expected {} to be greater than {}", self._subject, other))
         return ChainInspector(self._subject)
 
     exceeds = is_greater_than
 
     def is_less_than(self, other):
         """
         Ensures :attr:`subject` is less than *other*.
         """
         try:
             unittest_case.assertTrue(self._subject < other)
-        except self._catch as err:
+        except self._catch:
             raise self._error_factory(_format("Expected {} to be less than {}", self._subject, other))
         return ChainInspector(self._subject)
 
     def is_greater_than_or_equal_to(self, other):
         """
         Ensures :attr:`subject` is greater than or equal to *other*.
         """
         try:
             unittest_case.assertTrue(self._subject >= other)
-        except self._catch as err:
-            raise self._error_factory(_format("Expected {} to be greater than or equal to {}", self._subject, other))
+        except self._catch:
+            raise self._error_factory(
+                _format(
+                    "Expected {} to be greater than or equal to {}",
+                    self._subject,
+                    other,
+                )
+            )
         return ChainInspector(self._subject)
 
     def is_less_than_or_equal_to(self, other):
         """
         Ensures :attr:`subject` is less than or equal to *other*.
         """
         try:
             unittest_case.assertTrue(self._subject <= other)
-        except self._catch as err:
+        except self._catch:
             raise self._error_factory(_format("Expected {} to be less than or equal to {}", self._subject, other))
         return ChainInspector(self._subject)
 
     def called_with(self, *args, **kwargs):
         """
         Before evaluating subsequent predicates, calls :attr:`subject` with given arguments (but unlike a direct call,
         catches and transforms any exceptions that arise during the call).
@@ -626,16 +653,17 @@
         return unittest_case.assertRaises(expected_exception, self._orig_subject, *self._args, **self._kwargs)
 
     def raises_regex(self, expected_exception, expected_regexp):
         """
         Ensures preceding predicates (specifically, :meth:`called_with()`) result in *expected_exception* being raised,
         and the string representation of *expected_exception* must match regular expression *expected_regexp*.
         """
-        return unittest_case.assertRaisesRegexp(expected_exception, expected_regexp, self._orig_subject,
-                                                *self._args, **self._kwargs)
+        return unittest_case.assertRaisesRegexp(
+            expected_exception, expected_regexp, self._orig_subject, *self._args, **self._kwargs
+        )
 
     def is_a_numeric_string(self):
         return self.is_a(NumericString)
 
     def is_a_numeric_bytestring(self):
         return self.is_a(NumericByteString)
 
@@ -667,35 +695,40 @@
     #    self._run(jsonschema.validate, (self._subject, schema))
 
     def satisfies(self, predicate, *args, **kwargs):
         def run():
             if isinstance(predicate, string_types):
                 # `predicate` can be a string that names a method.
                 # In this case, look up the method and use that as the actual predicate.
-                if not predicate.startswith('.'):
-                    raise TypeError('Predicate must be a callable or method name, '
-                                    'and method names must start with ".": {}'.format(predicate))
+                if not predicate.startswith("."):
+                    raise TypeError(
+                        "Predicate must be a callable or method name, "
+                        'and method names must start with ".": {}'.format(predicate)
+                    )
                 method_name = predicate[1:]
 
                 def actual_predicate(subj, *args):
                     return getattr(subj, method_name)(*args, **kwargs)
+
                 predicate_name = predicate
             else:
                 # Otherwise assume `predicate` is some kind of callable
                 actual_predicate = predicate
-                predicate_name = getattr(predicate, '__name__', predicate)
+                predicate_name = getattr(predicate, "__name__", predicate)
 
             if not actual_predicate(self._subject, *args, **kwargs):
                 # Note the error message uses the original `predicate`
                 msg = _format("Expected {} to satisfy {}", self._subject, predicate_name)
                 if args:
                     msg += _format(" on args {}", args)
                 raise ValueError(msg)
+
         return self._run(run)
 
+
 class InspectorProxy(object):
     def __init__(self, *args, **kwargs):
         self._inspector = Ensure(*args, **kwargs)
         self._exception = None
 
     def __call__(self, *args, **kwargs):
         self.__init__(*args, **kwargs)
@@ -710,23 +743,26 @@
         def inspect(*args, **kwargs):
             if self._exception is None:
                 try:
                     self._inspector = inspect_method(*args, **kwargs)
                 except self._inspector._catch as e:
                     self._exception = e
             return self
+
         return inspect
 
+
 class Check(InspectorProxy):
     """
     Like Ensure, but if a check fails, saves the error instead of raising it immediately. The error can then be acted
     upon using :meth:`or_raise()` or :meth:`or_call()`.
 
     ``.each_of()`` is not supported by the **Check** inspector; all other methods are supported.
     """
+
     def or_raise(self, error_factory, message=None, *args, **kwargs):
         """
         Raises an exception produced by **error_factory** if a predicate fails.
 
         :param error_factory:
             Class or callable (e.g. :class:`Exception`) which will be invoked to produce the resulting exception.
             You can define a custom callable here; it will be given the underlying predicate's exception (AssertError)
@@ -753,31 +789,28 @@
             _callable(*args, **kwargs)
 
     def __bool__(self):
         return not self._exception
 
     __nonzero__ = __bool__  # Python 2 compatibility
 
+
 class NoOpInspector(InspectorProxy):
     """
     Goes through the motions of Ensure, but never raises on the error condition. For chaining with conditional
     predicates like ``is_none_or``.
     """
 
+
 def _check_default_argument(f, arg, value):
     if value is not None and arg in f.__annotations__:
         templ = f.__annotations__[arg]
         if not isinstance(value, templ):
-            msg = (
-                "Default argument {arg} of type {valt} to {f} "
-                "does not match annotation type {t}"
-            )
-            raise EnsureError(msg.format(
-                arg=arg, f=f, t=templ, valt=type(value)
-            ))
+            msg = "Default argument {arg} of type {valt} to {f} " "does not match annotation type {t}"
+            raise EnsureError(msg.format(arg=arg, f=f, t=templ, valt=type(value)))
 
 
 class WrappedFunction:
     """
     Wrapper for functions to check argument annotations
     """
 
@@ -792,21 +825,16 @@
                 value = args[pos]
             elif arg in kwargs:
                 value = kwargs[arg]
             else:
                 continue
 
             if not isinstance(value, templ):
-                msg = (
-                    "Argument {arg} of type {valt} to {f} "
-                    "does not match annotation type {t}"
-                )
-                raise EnsureError(msg.format(
-                    arg=arg, f=self.f, t=templ, valt=type(value)
-                ))
+                msg = "Argument {arg} of type {valt} to {f} " "does not match annotation type {t}"
+                raise EnsureError(msg.format(arg=arg, f=self.f, t=templ, valt=type(value)))
 
         return self.f(*args, **kwargs)
 
     def __getattr__(self, attr_name):
         return getattr(self.f, attr_name)
 
     def __repr__(self):
@@ -834,31 +862,21 @@
                 value = args[pos]
             elif arg in kwargs:
                 value = kwargs[arg]
             else:
                 continue
 
             if not isinstance(value, templ):
-                msg = (
-                    "Argument {arg} of type {valt} to {f} "
-                    "does not match annotation type {t}"
-                )
-                raise EnsureError(msg.format(
-                    arg=arg, f=self.f, t=templ, valt=type(value)
-                ))
+                msg = "Argument {arg} of type {valt} to {f} " "does not match annotation type {t}"
+                raise EnsureError(msg.format(arg=arg, f=self.f, t=templ, valt=type(value)))
 
         return_val = self.f(*args, **kwargs)
         if not isinstance(return_val, self.return_templ):
-            msg = (
-                "Return value of {f} of type {valt} "
-                "does not match annotation type {t}"
-            )
-            raise EnsureError(msg.format(
-                f=self.f, t=self.return_templ, valt=type(return_val)
-            ))
+            msg = "Return value of {f} of type {valt} " "does not match annotation type {t}"
+            raise EnsureError(msg.format(f=self.f, t=self.return_templ, valt=type(return_val)))
         return return_val
 
 
 def ensure_annotations(f):
     """
     Decorator to be used on functions with annotations. Runs type checks to enforce annotations. Raises
     :class:`EnsureError` if any argument passed to *f* is not of the type specified by the annotation. Also raises
@@ -904,16 +922,16 @@
         elif arg in f.__annotations__:
             templ = f.__annotations__[arg]
             if pos >= f.__code__.co_argcount:
                 arg_properties.append((arg, templ, None))
             else:
                 arg_properties.append((arg, templ, pos))
 
-    if 'return' in f.__annotations__:
-        return_templ = f.__annotations__['return']
+    if "return" in f.__annotations__:
+        return_templ = f.__annotations__["return"]
         return WrappedFunctionReturn(arg_properties, f, return_templ)
     else:
         return WrappedFunction(arg_properties, f)
 
 
 ensure = Ensure()
 check = Check()
```

### Comparing `ensure-1.0.2/ensure.egg-info/PKG-INFO` & `ensure-1.0.3/ensure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: ensure
-Version: 1.0.2
+Version: 1.0.3
 Summary: Literate BDD assertions in Python with no magic
 Home-page: https://github.com/kislyuk/ensure
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Provides-Extra: test
 License-File: LICENSE
 
 ensure: Literate assertions in Python
 =====================================
 *ensure* is a set of simple assertion helpers that let you write more expressive, literate, concise, and readable
 Pythonic code for validating conditions. It's inspired by `should.js <https://github.com/shouldjs/should.js>`_,
@@ -263,9 +263,7 @@
         :target: https://github.com/kislyuk/ensure/actions
 .. image:: https://codecov.io/github/kislyuk/ensure/coverage.svg?branch=master
         :target: https://codecov.io/github/kislyuk/ensure?branch=master
 .. image:: https://img.shields.io/pypi/v/ensure.svg
         :target: https://pypi.python.org/pypi/ensure
 .. image:: https://img.shields.io/pypi/l/ensure.svg
         :target: https://pypi.python.org/pypi/ensure
-
-
```

### Comparing `ensure-1.0.2/setup.py` & `ensure-1.0.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 #!/usr/bin/env python
 
 import os
-from setuptools import setup, find_packages
+
+from setuptools import find_packages, setup
 
 setup(
-    name='ensure',
-    version='1.0.2',
-    url='https://github.com/kislyuk/ensure',
-    license='Apache Software License',
-    author='Andrey Kislyuk',
-    author_email='kislyuk@gmail.com',
-    description='Literate BDD assertions in Python with no magic',
-    long_description=open('README.rst').read(),
-    python_requires='>=3.5',
-    install_requires=['six >= 1.11.0'],
-    extras_require={
-        'test': ['coverage', 'flake8']
-    },
-    packages=find_packages(exclude=['test']),
+    name="ensure",
+    version="1.0.3",
+    url="https://github.com/kislyuk/ensure",
+    license="Apache Software License",
+    author="Andrey Kislyuk",
+    author_email="kislyuk@gmail.com",
+    description="Literate BDD assertions in Python with no magic",
+    long_description=open("README.rst").read(),
+    python_requires=">=3.6",
+    install_requires=["six >= 1.11.0"],
+    extras_require={"test": ["coverage", "ruff"]},
+    packages=find_packages(exclude=["test"]),
     include_package_data=True,
-    platforms=['MacOS X', 'Posix'],
-    test_suite='test',
+    platforms=["MacOS X", "Posix"],
+    test_suite="test",
     classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: Apache Software License',
-        'Operating System :: MacOS :: MacOS X',
-        'Operating System :: POSIX',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Development Status :: 5 - Production/Stable',
-        'Topic :: Software Development :: Libraries :: Python Modules'
-    ]
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: POSIX",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Development Status :: 5 - Production/Stable",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
 )
```

### Comparing `ensure-1.0.2/test/test.py` & `ensure-1.0.3/test/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
+import collections
+import collections.abc
+import copy
 import os
+import re
 import sys
 import unittest
-import collections, collections.abc
-import copy
-import re
+
 from six import text_type as str
 
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
-from ensure import ensure, check, Ensure, Check, EnsureError, ensure_annotations
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+from ensure import Check, Ensure, EnsureError, check, ensure, ensure_annotations
 
 
 class TestEnsure(unittest.TestCase):
     def test_basic_ensure_statements(self):
         ensure(range(10)).contains(5)
         with self.assertRaises(EnsureError):
             ensure(range(10)).contains(-1)
@@ -26,138 +28,149 @@
             ensure(range(10)).is_in(-1)
 
         ensure("abc").matches("(abc|def)")
         with self.assertRaises(EnsureError):
             ensure(range(10)).is_in(-1)
 
         x = {x: x for x in range(10)}
-        ok_clauses = ('Ensure(x).contains(0)',
-                      'Ensure(x).contains_all_of(range(10))',
-                      'Ensure(x).contains_no(str)',
-                      'Ensure(x).contains_none_of(range(20, 30))',
-                      'Ensure(x).contains_one_of(range(1))',
-                      'Ensure(x).contains_some_of(range(2))',
-                      'Ensure(x).contains_only(range(10))',
-                      'Ensure(x).does_not_contain(-1)',
-                      'Ensure(x).does_not_equal(range(10))',
-                      'Ensure(x).has_attribute("__iter__")',
-                      'Ensure(x).has_length(10).also.is_nonempty()',
-                      'Ensure(x).has_length(length=10, min=9, max=10)',
-                      'Ensure(x).has_length(max=99.9)',
-                      'Ensure(x).is_nonempty().also.has_length(10)',
-                      'Ensure(x).is_a(collections.abc.Mapping)',
-                      'Ensure(x).is_a_dict_of(int).to(int)',
-                      'Ensure(x).is_a(collections.abc.Mapping).of(int).to(int)',
-                      'Ensure(6).is_greater_than(5)',
-                      'Ensure(6).exceeds(5)',
-                      'Ensure(1.1).is_greater_than_or_equal_to(1.1)',
-                      'Ensure(1.1).is_less_than_or_equal_to(1.1)',
-                      'Ensure(1).is_less_than(1.1)',
-                      'Ensure(1).is_positive()',
-                      'Ensure(1.1).is_a_positive(float)',
-                      'Ensure(-1).is_negative()',
-                      'Ensure(-1).is_a_negative(int)',
-                      'Ensure(0).is_nonnegative()',
-                      'Ensure(0).is_a_nonnegative(int)',
-                      'Ensure(1).is_a_positive(int).which.equals(1.0)',
-                      'Ensure((collections.namedtuple("Thing", ["x"]))(x={})).has_attribute("x").which.is_a(dict)',
-                      'Ensure({1:"a"}).has_key(1).whose_value.has_length(1)',
-                      'Ensure({1: "a", 2: "b", 3: "c"}).has_keys((1, 2))',
-                      'Ensure({1: "a", 2: "b", 3: "c"}).has_only_keys((1, 2, 3))',
-                      'Ensure({}).is_empty()',
-                      'Ensure(os.path.join).called_with("a", "b").returns(os.path.join("a", "b"))',
-                      'Ensure(int).called_with("1100101", base=2).returns(101)',
-                      'Ensure.each_of([1,2,3]).is_an(int)',
-                      'Ensure.each_of([lambda x: x, lambda y: y]).called_with(1).returns(1)',
-                      'Ensure(True).is_none_or.is_an(int)',  # See https://www.python.org/dev/peps/pep-0285/ (section 6)
-                      'Ensure(None).is_none_or.is_a_negative(int)',
-                      'Ensure(-5).is_none_or.is_a_negative(int)',
-                      'Ensure({"a": "b"}).is_none_or.has_key("a")',
-                      'Ensure([1,2,3]).is_sorted()',
-                      'Ensure([3,2,1]).is_sorted(key=lambda x: -x)',
-                      'Ensure("A").satisfies(str.isupper)',
-                      'Ensure("A").satisfies(".isupper")',
-                      'Ensure("ABC").satisfies(str.startswith, "AB")',
-                      'Ensure("ABC").satisfies(".startswith", "AB")',
-                      'Ensure(3).satisfies(lambda x, y: x < y, y=4)')
+        ok_clauses = (
+            "Ensure(x).contains(0)",
+            "Ensure(x).contains_all_of(range(10))",
+            "Ensure(x).contains_no(str)",
+            "Ensure(x).contains_none_of(range(20, 30))",
+            "Ensure(x).contains_one_of(range(1))",
+            "Ensure(x).contains_some_of(range(2))",
+            "Ensure(x).contains_only(range(10))",
+            "Ensure(x).does_not_contain(-1)",
+            "Ensure(x).does_not_equal(range(10))",
+            'Ensure(x).has_attribute("__iter__")',
+            "Ensure(x).has_length(10).also.is_nonempty()",
+            "Ensure(x).has_length(length=10, min=9, max=10)",
+            "Ensure(x).has_length(max=99.9)",
+            "Ensure(x).is_nonempty().also.has_length(10)",
+            "Ensure(x).is_a(collections.abc.Mapping)",
+            "Ensure(x).is_a_dict_of(int).to(int)",
+            "Ensure(x).is_a(collections.abc.Mapping).of(int).to(int)",
+            "Ensure(6).is_greater_than(5)",
+            "Ensure(6).exceeds(5)",
+            "Ensure(1.1).is_greater_than_or_equal_to(1.1)",
+            "Ensure(1.1).is_less_than_or_equal_to(1.1)",
+            "Ensure(1).is_less_than(1.1)",
+            "Ensure(1).is_positive()",
+            "Ensure(1.1).is_a_positive(float)",
+            "Ensure(-1).is_negative()",
+            "Ensure(-1).is_a_negative(int)",
+            "Ensure(0).is_nonnegative()",
+            "Ensure(0).is_a_nonnegative(int)",
+            "Ensure(1).is_a_positive(int).which.equals(1.0)",
+            'Ensure((collections.namedtuple("Thing", ["x"]))(x={})).has_attribute("x").which.is_a(dict)',
+            'Ensure({1:"a"}).has_key(1).whose_value.has_length(1)',
+            'Ensure({1: "a", 2: "b", 3: "c"}).has_keys((1, 2))',
+            'Ensure({1: "a", 2: "b", 3: "c"}).has_only_keys((1, 2, 3))',
+            "Ensure({}).is_empty()",
+            'Ensure(os.path.join).called_with("a", "b").returns(os.path.join("a", "b"))',
+            'Ensure(int).called_with("1100101", base=2).returns(101)',
+            "Ensure.each_of([1,2,3]).is_an(int)",
+            "Ensure.each_of([lambda x: x, lambda y: y]).called_with(1).returns(1)",
+            "Ensure(True).is_none_or.is_an(int)",  # See https://www.python.org/dev/peps/pep-0285/ (section 6)
+            "Ensure(None).is_none_or.is_a_negative(int)",
+            "Ensure(-5).is_none_or.is_a_negative(int)",
+            'Ensure({"a": "b"}).is_none_or.has_key("a")',
+            "Ensure([1,2,3]).is_sorted()",
+            "Ensure([3,2,1]).is_sorted(key=lambda x: -x)",
+            'Ensure("A").satisfies(str.isupper)',
+            'Ensure("A").satisfies(".isupper")',
+            'Ensure("ABC").satisfies(str.startswith, "AB")',
+            'Ensure("ABC").satisfies(".startswith", "AB")',
+            "Ensure(3).satisfies(lambda x, y: x < y, y=4)",
+        )
 
         for clause in ok_clauses:
             print("Testing OK clause", clause)
             eval(clause)
-            if 'each_of' not in clause:
-                for sub in r'Check\1.otherwise(Exception)', r'Check\1.or_raise(Exception)', r'Check\1.or_call(self.assertTrue, False)':
-                    print("Testing OK clause", re.sub(r'^Ensure(.+)', sub, clause))
-                    eval(re.sub(r'^Ensure(.+)', sub, clause))
-
-                print("Testing OK clause", re.sub(r'Ensure(.+)', r'bool(Check\1)', clause))
-                self.assertEqual(eval(re.sub(r'Ensure(.+)', r'bool(Check\1)', clause)), True)
-
-
-        bad_clauses = ('Ensure(x).contains(-1)',
-                       'Ensure(x).has_length(10).also.is_empty()',
-                       'Ensure(x).contains_all_of(range(20))',
-                       'Ensure(x).contains_no(int)',
-                       'Ensure(x).contains_none_of(range(0, 30))',
-                       'Ensure(x).contains_one_of(range(2))',
-                       'Ensure(x).contains_some_of(range(20, 30))',
-                       'Ensure(x).contains_only(range(11))',
-                       'Ensure(x).does_not_contain(1)',
-                       'Ensure(x).does_not_equal(x)',
-                       'Ensure(x).does_not_equal(copy.deepcopy(x))',
-                       'Ensure(x).has_attribute("y")',
-                       'Ensure(x).has_length(1)',
-                       'Ensure(x).has_length(length=1, min=9, max=10)',
-                       'Ensure(x).has_length(min=11)',
-                       'Ensure(x).has_length(max=1.1)',
-                       'Ensure(x).is_a(str)',
-                       'Ensure(x).is_empty()',
-                       'Ensure(6).is_greater_than(7)',
-                       'Ensure(6).exceeds(7)',
-                       'Ensure(1).is_greater_than_or_equal_to(1.1)',
-                       'Ensure(None).is_greater_than_or_equal_to(1.1)',
-                       'Ensure(5).is_less_than_or_equal_to(1)',
-                       'Ensure(1).is_less_than(None)',
-                       'Ensure(0).is_positive()',
-                       'Ensure(1).is_a_positive(float)',
-                       'Ensure(1).is_negative()',
-                       'Ensure(-0).is_a_negative(int)',
-                       'Ensure(-0.1).is_nonnegative()',
-                       'Ensure(None).is_a_nonnegative(int)',
-                       'Ensure({1: "a"}).has_key(1).whose_value.has_length(2)',
-                       'Ensure({1: "a"}).has_keys((1, 2))',
-                       'Ensure({1: "a", 2: "b"}).has_only_keys([1])',
-                       'Ensure({1: "a", 2: "b"}).has_only_keys([1, 2, 3])',
-                       'Ensure([1, 2, 3]).has_only_keys([1, 2, 3])',
-                       'Ensure(os.path.join).called_with("a", "b").returns(None)',
-                       'Ensure(1).is_a_positive(int).which.equals(1.2)',
-                       'Ensure.each_of([lambda x: x, lambda y: y]).called_with(2).returns(1)',
-                       'Ensure(5).is_none_or.is_a_negative(int)',
-                       'Ensure(None).is_a_negative(int)',
-                       'Ensure([1,2,1]).is_sorted()',
-                       'Ensure([1,2,1]).is_sorted(key=lambda x: -x)',
-                       'Ensure(None).is_sorted()',
-                       'Ensure("a").satisfies(str.isupper)',
-                       'Ensure("a").satisfies(".isupper")',
-                       'Ensure("ABC").satisfies(str.startswith, "Z")',
-                       'Ensure("ABC").satisfies(".startswith", "Z")',
-                       'Ensure(5).satisfies(str.isupper)',
-                       'Ensure(5).satisfies(".isupper")')
+            if "each_of" not in clause:
+                for sub in (
+                    r"Check\1.otherwise(Exception)",
+                    r"Check\1.or_raise(Exception)",
+                    r"Check\1.or_call(self.assertTrue, False)",
+                ):
+                    print("Testing OK clause", re.sub(r"^Ensure(.+)", sub, clause))
+                    eval(re.sub(r"^Ensure(.+)", sub, clause))
+
+                print("Testing OK clause", re.sub(r"Ensure(.+)", r"bool(Check\1)", clause))
+                self.assertEqual(eval(re.sub(r"Ensure(.+)", r"bool(Check\1)", clause)), True)
+
+        bad_clauses = (
+            "Ensure(x).contains(-1)",
+            "Ensure(x).has_length(10).also.is_empty()",
+            "Ensure(x).contains_all_of(range(20))",
+            "Ensure(x).contains_no(int)",
+            "Ensure(x).contains_none_of(range(0, 30))",
+            "Ensure(x).contains_one_of(range(2))",
+            "Ensure(x).contains_some_of(range(20, 30))",
+            "Ensure(x).contains_only(range(11))",
+            "Ensure(x).does_not_contain(1)",
+            "Ensure(x).does_not_equal(x)",
+            "Ensure(x).does_not_equal(copy.deepcopy(x))",
+            'Ensure(x).has_attribute("y")',
+            "Ensure(x).has_length(1)",
+            "Ensure(x).has_length(length=1, min=9, max=10)",
+            "Ensure(x).has_length(min=11)",
+            "Ensure(x).has_length(max=1.1)",
+            "Ensure(x).is_a(str)",
+            "Ensure(x).is_empty()",
+            "Ensure(6).is_greater_than(7)",
+            "Ensure(6).exceeds(7)",
+            "Ensure(1).is_greater_than_or_equal_to(1.1)",
+            "Ensure(None).is_greater_than_or_equal_to(1.1)",
+            "Ensure(5).is_less_than_or_equal_to(1)",
+            "Ensure(1).is_less_than(None)",
+            "Ensure(0).is_positive()",
+            "Ensure(1).is_a_positive(float)",
+            "Ensure(1).is_negative()",
+            "Ensure(-0).is_a_negative(int)",
+            "Ensure(-0.1).is_nonnegative()",
+            "Ensure(None).is_a_nonnegative(int)",
+            'Ensure({1: "a"}).has_key(1).whose_value.has_length(2)',
+            'Ensure({1: "a"}).has_keys((1, 2))',
+            'Ensure({1: "a", 2: "b"}).has_only_keys([1])',
+            'Ensure({1: "a", 2: "b"}).has_only_keys([1, 2, 3])',
+            "Ensure([1, 2, 3]).has_only_keys([1, 2, 3])",
+            'Ensure(os.path.join).called_with("a", "b").returns(None)',
+            "Ensure(1).is_a_positive(int).which.equals(1.2)",
+            "Ensure.each_of([lambda x: x, lambda y: y]).called_with(2).returns(1)",
+            "Ensure(5).is_none_or.is_a_negative(int)",
+            "Ensure(None).is_a_negative(int)",
+            "Ensure([1,2,1]).is_sorted()",
+            "Ensure([1,2,1]).is_sorted(key=lambda x: -x)",
+            "Ensure(None).is_sorted()",
+            'Ensure("a").satisfies(str.isupper)',
+            'Ensure("a").satisfies(".isupper")',
+            'Ensure("ABC").satisfies(str.startswith, "Z")',
+            'Ensure("ABC").satisfies(".startswith", "Z")',
+            "Ensure(5).satisfies(str.isupper)",
+            'Ensure(5).satisfies(".isupper")',
+        )
 
         for clause in bad_clauses:
             print("Testing bad clause", clause)
             with self.assertRaises(EnsureError):
                 eval(clause)
-            if 'each_of' not in clause:
-                for sub in r'Check\1.otherwise(Exception)', r'Check\1.or_raise(Exception)', r'Check\1.or_call(self.assertTrue, False)':
+            if "each_of" not in clause:
+                for sub in (
+                    r"Check\1.otherwise(Exception)",
+                    r"Check\1.or_raise(Exception)",
+                    r"Check\1.or_call(self.assertTrue, False)",
+                ):
                     with self.assertRaises(Exception):
-                        print("Testing bad clause", re.sub(r'^Ensure(.+)', sub, clause))
-                        eval(re.sub(r'^Ensure(.+)', sub, clause))
+                        print("Testing bad clause", re.sub(r"^Ensure(.+)", sub, clause))
+                        eval(re.sub(r"^Ensure(.+)", sub, clause))
 
-                print("Testing bad clause", re.sub(r'^Ensure(.+)', r'bool(Check\1)', clause))
-                self.assertEqual(eval(re.sub(r'^Ensure(.+)', r'bool(Check\1)', clause)), False)
+                print("Testing bad clause", re.sub(r"^Ensure(.+)", r"bool(Check\1)", clause))
+                self.assertEqual(eval(re.sub(r"^Ensure(.+)", r"bool(Check\1)", clause)), False)
 
         with self.assertRaises(EnsureError):
             Ensure(x).is_a_dict_of(int).to(str)
         with self.assertRaises(EnsureError):
             Ensure(x).is_a_dict_of(str).to(int)
         with self.assertRaises(EnsureError):
             Ensure(x).called_with().is_an(int)
@@ -228,35 +241,44 @@
     '''Does some work'''
     return x * y
 """
         exec(f_code)
         self.assertEqual(f(1, 2.3), 3.3)
         self.assertEqual(f(1, y=2.3), 3.3)
         self.assertEqual(f(y=1.2, x=3), 4.2)
-        with self.assertRaisesRegex(
-                EnsureError, "Argument y of type <class 'int'> to <function f at .+> does not match annotation type <class 'float'>"):
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument y of type <class 'int'> to <function f at .+> does not match annotation type <class 'float'>",
+        ):
             self.assertEqual(f(1, 2), 3.3)
-        with self.assertRaisesRegex(EnsureError, "Argument y of type <class 'int'> to <function f at .+> does not match annotation type <class 'float'>"):
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument y of type <class 'int'> to <function f at .+> does not match annotation type <class 'float'>",
+        ):
             self.assertEqual(f(y=2, x=1), 3.3)
-        with self.assertRaisesRegex(EnsureError, "Return value of <function f at .+> does not match annotation type <class 'float'>"):
+        with self.assertRaisesRegexp(
+            EnsureError, "Return value of <function f at .+> does not match annotation type <class 'float'>"
+        ):
             self.assertEqual(f(1, -2.3), 4)
-        with self.assertRaisesRegex(EnsureError, "Return value of <function f at .+> does not match annotation type <class 'float'>"):
+        with self.assertRaisesRegexp(
+            EnsureError, "Return value of <function f at .+> does not match annotation type <class 'float'>"
+        ):
             self.assertEqual(f(x=1, y=-2.3), 4)
 
         # Test with mixtures of keyword and positional args
         self.assertEqual(g("the "), "the default")
         self.assertEqual(g("the ", "bomb"), "the bomb")
         self.assertEqual(g(y=g("the ", y="bomb"), x="somebody set up us "), "somebody set up us the bomb")
 
-        self.assertEqual('g', g.__name__)
-        self.assertEqual('Simply add numbers together', g.__doc__)
-        self.assertRegex(repr(g), '<function g at 0x[0-9a-fA-F]+>')
-        self.assertEqual('h', h.__name__)
-        self.assertEqual('Does some work', h.__doc__)
-        self.assertRegex(repr(h), '<function h at 0x[0-9a-fA-F]+>')
+        self.assertEqual("g", g.__name__)
+        self.assertEqual("Simply add numbers together", g.__doc__)
+        self.assertRegex(repr(g), "<function g at 0x[0-9a-fA-F]+>")
+        self.assertEqual("h", h.__name__)
+        self.assertEqual("Does some work", h.__doc__)
+        self.assertRegex(repr(h), "<function h at 0x[0-9a-fA-F]+>")
 
     @unittest.skipIf(sys.version_info < (3, 0), "Skipping test that requires Python 3 features")
     def test_annotations_with_bad_default(self):
         f_code = """
 from ensure import ensure_annotations
 
 global f, g
@@ -265,15 +287,18 @@
 def f(x: int, y: float=None) -> float:
     return x+y if x+y > 0 else int(x+y)
 
 @ensure_annotations
 def g(x: str, y: str=5, z='untyped with default') -> str:
     return x+y+str(z)
 """
-        with self.assertRaisesRegex(EnsureError, "Default argument y of type <class 'int'> to <function g at .+> does not match annotation type <class 'str'>"):
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Default argument y of type <class 'int'> to <function g at .+> does not match annotation type <class 'str'>",
+        ):
             exec(f_code)
         # Make sure f still works as None should be excluded from default test
         self.assertEqual(f(1, 2.3), 3.3)
         self.assertEqual(f(1, y=2.3), 3.3)
         self.assertEqual(f(y=1.2, x=3), 4.2)
 
     @unittest.skipIf(sys.version_info < (3, 0), "Skipping test that requires Python 3 features")
@@ -292,16 +317,19 @@
 
 """
         exec(f_code)
         # Make sure f still works as None should be excluded from default test
         self.assertEqual(2.0, f(3, 4.0))
         self.assertEqual(62.0, f(3, 4.0, 10, 20, 30))
         self.assertEqual(66.0, f(3, 4.0, 10, 20, 30, z=1))
-        with self.assertRaisesRegex(EnsureError, "Argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>"):
-            self.assertEqual(66.0, f(3, 4.0, 10, 20, 30, z='hello world'))
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>",
+        ):
+            self.assertEqual(66.0, f(3, 4.0, 10, 20, 30, z="hello world"))
 
     @unittest.skipIf(sys.version_info < (3, 0), "Skipping test that requires Python 3 features")
     def test_annotations_with_varargs(self):
         f_code = """
 from ensure import ensure_annotations
 
 global f
@@ -314,20 +342,23 @@
         r = r + str(t - z) + s
 
     return r
 
 """
         exec(f_code)
         # Make sure f still works as None should be excluded from default test
-        self.assertEqual('', f(3, 4.0))
-        self.assertEqual('2.0abc', f(3, 4.0, 'abc'))
-        self.assertEqual('2.0abc2.0def', f(3, 4.0, 'abc', 'def'))
-        self.assertEqual('3.0abc3.0def', f(3, 4.0, 'abc', 'def', z=4))
-        with self.assertRaisesRegex(EnsureError, "Argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>"):
-            self.assertEqual('3.0abc3.0def', f(3, 4.0, 'abc', 'def', z='school'))
+        self.assertEqual("", f(3, 4.0))
+        self.assertEqual("2.0abc", f(3, 4.0, "abc"))
+        self.assertEqual("2.0abc2.0def", f(3, 4.0, "abc", "def"))
+        self.assertEqual("3.0abc3.0def", f(3, 4.0, "abc", "def", z=4))
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>",
+        ):
+            self.assertEqual("3.0abc3.0def", f(3, 4.0, "abc", "def", z="school"))
 
     @unittest.skipIf(sys.version_info < (3, 0), "Skipping test that requires Python 3 features")
     def test_annotations_with_vararg_bad_default(self):
         f_code = """
 from ensure import ensure_annotations
 
 global f
@@ -337,15 +368,18 @@
     t = x + y
     r = ''
     for s in args:
         r = r + str(t - z) + s
 
     return r
 """
-        with self.assertRaisesRegex(EnsureError, "Default argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>"):
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Default argument z of type <class 'str'> to <function f at .+> does not match annotation type <class 'int'>",
+        ):
             exec(f_code)
 
     @unittest.skipIf(sys.version_info < (3, 0), "Skipping test that requires Python 3 features")
     def test_annotations_on_bound_methods(self):
         f_code = """
 from ensure import ensure_annotations
 
@@ -359,23 +393,30 @@
     @ensure_annotations
     def g(self, x: int, y: float):
         return str(x+y)
 
 """
         exec(f_code)
         c = C()
-        self.assertEqual('3.3', c.f(1, 2.3))
-        self.assertRegex(repr(c.f), '<bound method C.f of <.+.C object at 0x[0-9a-fA-F]+>>')
-        with self.assertRaisesRegex(EnsureError, "Argument x of type <class 'float'> to <function (C.f|f) at .+> does not match annotation type <class 'int'>"):
+        self.assertEqual("3.3", c.f(1, 2.3))
+        self.assertRegex(repr(c.f), "<bound method C.f of <.+.C object at 0x[0-9a-fA-F]+>>")
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument x of type <class 'float'> to <function (C.f|f) at .+> does not match annotation type <class 'int'>",
+        ):
             g = C().f(3.2, 1)
 
-        self.assertEqual('3.3', c.g(1, 2.3))
-        self.assertRegex(repr(c.g), '<bound method C.g of <.+.C object at 0x[0-9a-fA-F]+>>')
-        with self.assertRaisesRegex(EnsureError, "Argument x of type <class 'float'> to <function (C.g|g) at .+> does not match annotation type <class 'int'>"):
+        self.assertEqual("3.3", c.g(1, 2.3))
+        self.assertRegex(repr(c.g), "<bound method C.g of <.+.C object at 0x[0-9a-fA-F]+>>")
+        with self.assertRaisesRegexp(
+            EnsureError,
+            "Argument x of type <class 'float'> to <function (C.g|g) at .+> does not match annotation type <class 'int'>",
+        ):
             g = C().g(3.2, 1)
 
     def test_error_formatting(self):
         with self.assertRaisesRegexp(Exception, "Major fail detected"):
             check(False).is_true().or_raise(KeyError, "{} {error} detected", "Major", error="fail")
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     unittest.main()
```

