# Comparing `tmp/ilpy-0.3.0.tar.gz` & `tmp/ilpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilpy-0.3.0.tar", last modified: Wed May  3 13:44:00 2023, max compression
+gzip compressed data, was "ilpy-0.3.1.tar", last modified: Sat May  6 18:00:49 2023, max compression
```

## Comparing `ilpy-0.3.0.tar` & `ilpy-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.908895 ilpy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 13:43:48.000000 ilpy-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 13:43:48.000000 ilpy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:43:48.000000 ilpy-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:44:00.908895 ilpy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-03 13:43:48.000000 ilpy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/decl.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/config.h
--rw-r--r--   0 runner    (1001) docker     (123)    61557 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/gurobi_c.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.908895 ilpy-0.3.0/ilpy/impl/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/BackendPreference.h
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraint.h
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraints.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Constraints.h
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Objective.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Objective.h
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Relation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Sense.h
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Solution.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/Solution.h
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverBackend.h
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverFactory.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/SolverFactory.h
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/impl/solvers/VariableType.h
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-03 13:43:48.000000 ilpy-0.3.0/ilpy/wrapper.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:44:00.900895 ilpy-0.3.0/ilpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:44:00.000000 ilpy-0.3.0/ilpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-03 13:43:48.000000 ilpy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:44:00.908895 ilpy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-03 13:43:48.000000 ilpy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:49.660786 ilpy-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-06 18:00:37.000000 ilpy-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-06 18:00:37.000000 ilpy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 18:00:37.000000 ilpy-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-06 18:00:49.660786 ilpy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-06 18:00:37.000000 ilpy-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:49.656785 ilpy-0.3.1/ilpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/decl.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:49.656785 ilpy-0.3.1/ilpy/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)    61557 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/gurobi_c.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:49.660786 ilpy-0.3.1/ilpy/impl/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/BackendPreference.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Constraint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Constraint.h
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Constraints.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Constraints.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/CplexBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/CplexBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/GurobiBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/GurobiBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Objective.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Objective.h
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Relation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/ScipBackend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/ScipBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Sense.h
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Solution.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/Solution.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/SolverBackend.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/SolverFactory.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/SolverFactory.h
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/impl/solvers/VariableType.h
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-06 18:00:37.000000 ilpy-0.3.1/ilpy/wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-05-06 18:00:38.000000 ilpy-0.3.1/ilpy/wrapper.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:00:49.656785 ilpy-0.3.1/ilpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-06 18:00:49.000000 ilpy-0.3.1/ilpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-06 18:00:49.000000 ilpy-0.3.1/ilpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:00:49.000000 ilpy-0.3.1/ilpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-06 18:00:49.000000 ilpy-0.3.1/ilpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-06 18:00:49.000000 ilpy-0.3.1/ilpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-06 18:00:38.000000 ilpy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:00:49.660786 ilpy-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-06 18:00:38.000000 ilpy-0.3.1/setup.py
```

### Comparing `ilpy-0.3.0/CONTRIBUTING.md` & `ilpy-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/LICENSE` & `ilpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/PKG-INFO` & `ilpy-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrappers for popular MIP solvers.
 Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/funkelab/ilpy
 Project-URL: repository, https://github.com/funkelab/ilpy
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `ilpy-0.3.0/README.md` & `ilpy-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/__init__.py` & `ilpy-0.3.1/ilpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from . import wrapper
 from ._functional import solve
 from .expressions import Expression, Variable
 from .wrapper import *  # noqa: F403
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __all__ = [  # noqa: F405
     "Any",
     "Binary",
     "Constraint",
     "Constraint",
     "Constraints",
     "Continuous",
```

### Comparing `ilpy-0.3.0/ilpy/_functional.py` & `ilpy-0.3.1/ilpy/_functional.py`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/decl.pxd` & `ilpy-0.3.1/ilpy/decl.pxd`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/expressions.py` & `ilpy-0.3.1/ilpy/expressions.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,24 @@
             return self
         raise ValueError("Only quadratic variables are supported")
 
     def __hash__(self) -> int:
         # allow use as dict key
         return id(self)
 
+    def __int__(self) -> int:
+        if self.index is None:
+            raise TypeError(f"Variable {self!r} has no index")
+        return int(self.index)
+
+    __index__ = __int__
+
+    def __repr__(self) -> str:
+        return f"ilpy.Variable({self.id!r}, index={self.index!r})"
+
 
 # conversion between ast comparison operators and ilpy relations
 # TODO: support more less/greater than operators
 OPERATOR_MAP: dict[type[ast.cmpop], Relation] = {
     ast.LtE: Relation.LessEqual,
     ast.Eq: Relation.Equal,
     ast.GtE: Relation.GreaterEqual,
```

### Comparing `ilpy-0.3.0/ilpy/impl/gurobi_c.h` & `ilpy-0.3.1/ilpy/impl/gurobi_c.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Constraint.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/Constraint.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Constraint.h` & `ilpy-0.3.1/ilpy/impl/solvers/Constraint.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Constraints.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/Constraints.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Constraints.h` & `ilpy-0.3.1/ilpy/impl/solvers/Constraints.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/CplexBackend.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/CplexBackend.h` & `ilpy-0.3.1/ilpy/impl/solvers/CplexBackend.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/GurobiBackend.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/GurobiBackend.h` & `ilpy-0.3.1/ilpy/impl/solvers/GurobiBackend.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Objective.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/Objective.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Objective.h` & `ilpy-0.3.1/ilpy/impl/solvers/Objective.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/ScipBackend.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/ScipBackend.h` & `ilpy-0.3.1/ilpy/impl/solvers/ScipBackend.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/Solution.h` & `ilpy-0.3.1/ilpy/impl/solvers/Solution.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/SolverBackend.h` & `ilpy-0.3.1/ilpy/impl/solvers/SolverBackend.h`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/impl/solvers/SolverFactory.cpp` & `ilpy-0.3.1/ilpy/impl/solvers/SolverFactory.cpp`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/ilpy/wrapper.pyi` & `ilpy-0.3.1/ilpy/wrapper.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import IntEnum, auto
 from typing import TYPE_CHECKING, Iterable, Mapping, Sequence
 
 if TYPE_CHECKING:
     LinearCoeffs = Sequence[float] | Mapping[int, float]
     QCoeffs = Mapping[tuple[int, int], float] | Iterable[tuple[tuple[int, int], float]]
 
-from ilpy.expressions import Expression
+from ilpy.expressions import Expression, Variable
 
 class Preference(IntEnum):
     Any = auto()
     Scip = auto()
     Gurobi = auto()
     Cplex = auto()
 
@@ -43,28 +43,30 @@
 LessEqual = Relation.LessEqual
 Equal = Relation.Equal
 GreaterEqual = Relation.GreaterEqual
 
 class Solution:
     def __init__(self, size: int) -> None: ...
     def __len__(self) -> int: ...
-    def __getitem__(self, i: int) -> float: ...
-    def __setitem__(self, i: int, value: float) -> None: ...
+    def __getitem__(self, i: int | Variable) -> float: ...
+    def __setitem__(self, i: int | Variable, value: float) -> None: ...
     def resize(self, size: int) -> None: ...
     def get_value(self) -> float: ...
     def set_value(self, value: float) -> None: ...
     def get_status(self) -> str: ...
 
 class Objective:
     def __init__(self, size: int = 0) -> None: ...
     def set_constant(self, value: float) -> None: ...
     def get_constant(self) -> float: ...
-    def set_coefficient(self, i: int, value: float) -> None: ...
+    def set_coefficient(self, i: int | Variable, value: float) -> None: ...
     def get_coefficients(self) -> list[float]: ...
-    def set_quadratic_coefficient(self, i: int, j: int, value: float) -> None: ...
+    def set_quadratic_coefficient(
+        self, i: int | Variable, j: int | Variable, value: float
+    ) -> None: ...
     def get_quadratic_coefficients(self) -> dict[tuple[int, int], float]: ...
     def set_sense(self, sense: Sense) -> None: ...
     def get_sense(self) -> Sense: ...
     def resize(self, size: int) -> None: ...
     def __len__(self) -> int: ...
     @classmethod
     def from_coefficients(
@@ -73,17 +75,19 @@
         quadratic_coefficients: QCoeffs = (),
         constant: float = 0,
         sense: Sense = Sense.Minimize,
     ) -> Objective: ...
 
 class Constraint:
     def __init__(self) -> None: ...
-    def set_coefficient(self, i: int, value: float) -> None: ...
+    def set_coefficient(self, i: int | Variable, value: float) -> None: ...
     def get_coefficients(self) -> dict[int, float]: ...
-    def set_quadratic_coefficient(self, i: int, j: int, value: float) -> None: ...
+    def set_quadratic_coefficient(
+        self, i: int | Variable, j: int, value: float
+    ) -> None: ...
     def get_quadratic_coefficients(self) -> dict[tuple[int, int], float]: ...
     def set_relation(self, relation: Relation) -> None: ...
     def get_relation(self) -> Relation: ...
     def set_value(self, value: float) -> None: ...
     def get_value(self) -> float: ...
     def is_violated(self, solution: Solution) -> bool: ...
     @classmethod
@@ -94,15 +98,15 @@
         relation: Relation = Relation.LessEqual,
         value: float = 0,
     ) -> Constraint: ...
 
 class Constraints:
     def __init__(self) -> None: ...
     def clear(self) -> None: ...
-    def add(self, constraint: Constraint) -> None: ...
+    def add(self, constraint: Constraint | Expression) -> None: ...
     def add_all(self, constraints: Constraints) -> None: ...
     def __len__(self) -> int: ...
 
 class Solver:
     def __init__(
         self,
         num_variables: int,
```

### Comparing `ilpy-0.3.0/ilpy/wrapper.pyx` & `ilpy-0.3.1/ilpy/wrapper.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -52,21 +52,23 @@
     def __dealloc__(self):
         del self.p
 
     def __len__(self):
         return self.p.size()
 
     def __getitem__(self, i):
+        i = int(i)
         if i < 0 or i >= self.p.size():
-            raise IndexError()
+            raise IndexError(f"index {i!r} out of range for size {self.p.size()}")
         return self.p[0][i]
 
     def __setitem__(self, i, value):
+        i = int(i)
         if i < 0 or i >= self.p.size():
-            raise IndexError()
+            raise IndexError(f"index {i!r} out of range for size {self.p.size()}")
         self.p[0][i] = value
 
     def resize(self, size):
         self.p.resize(size)
 
     def get_value(self):
         return self.p.getValue()
@@ -221,16 +223,21 @@
 
     def __dealloc__(self):
         del self.p
 
     def clear(self):
         self.p.clear()
 
-    def add(self, Constraint constraint):
-        self.p.add(constraint.p[0])
+    def add(self, constraint: Constraint | Expression):
+        cdef Constraint const
+        if hasattr(constraint, "as_constraint"):
+            const = constraint.as_constraint()
+        else:
+            const = constraint
+        self.p.add(const.p[0])
 
     def add_all(self, Constraints constraints):
         self.p.addAll(constraints.p[0])
 
     def __len__(self):
         return self.p.size()
```

### Comparing `ilpy-0.3.0/ilpy.egg-info/PKG-INFO` & `ilpy-0.3.1/ilpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilpy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrappers for popular MIP solvers.
 Author-email: Jan Funke <funkej@janelia.hhmi.org>, Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/funkelab/ilpy
 Project-URL: repository, https://github.com/funkelab/ilpy
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `ilpy-0.3.0/ilpy.egg-info/SOURCES.txt` & `ilpy-0.3.1/ilpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/pyproject.toml` & `ilpy-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ilpy-0.3.0/setup.py` & `ilpy-0.3.1/setup.py`

 * *Files identical despite different names*

