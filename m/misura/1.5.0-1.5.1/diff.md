# Comparing `tmp/misura-1.5.0.tar.gz` & `tmp/misura-1.5.1.tar.gz`

## Comparing `misura-1.5.0.tar` & `misura-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.0/.gitattributes
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.5.0/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 misura-1.5.0/docs/docs.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/__main__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/exceptions.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/globals.py
--rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/quantities.py
--rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/tables.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/utilities.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 misura-1.5.0/tests/tests.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.0/LICENSE
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 misura-1.5.0/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 misura-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.1/.gitattributes
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.5.1/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 misura-1.5.1/docs/docs.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/__main__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/exceptions.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/globals.py
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/quantities.py
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/tables.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.1/src/misura/utilities.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 misura-1.5.1/tests/tests.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.1/LICENSE
+-rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 misura-1.5.1/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 misura-1.5.1/PKG-INFO
```

### Comparing `misura-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.5.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/.github/workflows/python-publish.yml` & `misura-1.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/docs/docs.md` & `misura-1.5.1/docs/docs.md`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,15 @@
 
 - `InitError`: raised on invalid quantity definition.
 - `UnitError`: raised on invalid `unit`.
 - `QuantityError`: raised on operations between incompatible quantities.
 - `ConversionError`: raised on errors during conversions.
 - `UnpackError`: raised on errors during unpacking.
 - `PackError`: raised on errors during packing.
+- `UncertaintyComparisonError`: raised on comparing quantities with uncertainty.
 - `DefinitionError`: raised on errors during unit definition.
 
 ## Examples
 
 [Go back to ToC](#table-of-contents)
 
 ### Quantities
```

### Comparing `misura-1.5.0/src/misura/__main__.py` & `misura-1.5.1/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/src/misura/exceptions.py` & `misura-1.5.1/src/misura/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,21 +25,21 @@
                 ", {}".format(uncertainty) if uAny(uncertainty) else "",
             )
         )
 
 
 class QuantityError(Exception):
     """
-    Raised on operations between incompatible quantities.
+    Raised on operators between incompatible quantities.
     """
 
-    def __init__(self, first, second, operation: str) -> None:
+    def __init__(self, first, second, operator: str) -> None:
         super().__init__(
             "unsupported operand unit(s) for {0}: '{1}' and '{2}'\nraised by: '{3}' {0} '{4}'".format(
-                operation, first.unit(), second.unit(), first, second
+                operator, first.unit(), second.unit(), first, second
             )
         )
 
 
 class ConversionError(Exception):
     """
     Raised on errors during conversions.
@@ -91,14 +91,27 @@
             super().__init__(
                 "cannot pack '{2}' to '{1}'\nraised by: '{0}'".format(
                     qnt, target, qnt.unit()
                 )
             )
 
 
+class UncertaintyComparisonError(Exception):
+    """
+    Raised on comparing quantities with uncertainty.
+    """
+
+    def __init__(self, first, second, operator: str) -> None:
+        super().__init__(
+            "cannot compare uncertain quantities\nraised by: '{}' {} '{}'".format(
+                first, operator, second
+            )
+        )
+
+
 class DefinitionError(Exception):
     """
     Raised on errors during unit definition.
     """
 
     # Custom error defined in tables.py.
     def __init__(self, error: str = "") -> None:
```

### Comparing `misura-1.5.0/src/misura/quantities.py` & `misura-1.5.1/src/misura/quantities.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .exceptions import (
     UnitError,
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
+    UncertaintyComparisonError,
 )
 from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
 from .utilities import dictFromUnit, unitFromDict, checkIter, uAll, uAny
 
 
 class quantity:
     """
@@ -439,70 +440,88 @@
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<")
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, "<")
+
         return self.value < other.value
 
     # Less or equal.
     def __le__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value <= other
 
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, "<=")
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, "<=")
+
         return self.value <= other.value
 
     # Greater than.
     def __gt__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value > other
 
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">")
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, ">")
+
         return self.value > other.value
 
     # Greater or equal.
     def __ge__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value >= other
 
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 other = convert(other, self.unit())
 
             else:
                 raise QuantityError(self, other, ">=")
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, ">=")
+
         return self.value >= other.value
 
     # Equal.
     def __eq__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value == other
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, "==")
+
         return self.value == other.value and self.unit() == other.unit()
 
     # Not equal.
     def __ne__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value != other
 
+        if uAny(self.uncertainty) or uAny(self.uncertainty):
+            raise UncertaintyComparisonError(self, other, "!=")
+
         return self.value != other.value or self.unit() != other.unit()
 
 
 # CONVERSION, UNPACKING AND PACKING
 
 
 # Conversion function.
```

### Comparing `misura-1.5.0/src/misura/tables.py` & `misura-1.5.1/src/misura/tables.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/src/misura/utilities.py` & `misura-1.5.1/src/misura/utilities.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/tests/tests.py` & `misura-1.5.1/tests/tests.py`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/LICENSE` & `misura-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.5.0/README.md` & `misura-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 
 **misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
-- Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons).
-- Uncertainty handling: [Example](#mathematical-operations). ![New feature](https://img.shields.io/badge/new-green)
-- Manual conversions: [Example](#manual-and-automatic-conversion).
-- Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
-- Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units).
-- User defined base and derived units: [Example](#user-defined-units-of-measure). ![New feature](https://img.shields.io/badge/new-green)
-- Large compatibility with other libraries: [Example](#working-with-other-libraries).
-- Custom exceptions: [Example](#comparisons).
+- Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons)
+- Uncertainty handling: [Example](#mathematical-operations) ![New feature](https://img.shields.io/badge/new-green)
+- Manual conversions: [Example](#manual-and-automatic-conversion)
+- Automatic conversions on operations: [Example](#manual-and-automatic-conversion)
+- Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units)
+- User defined base and derived units: [Example](#user-defined-units-of-measure) ![New feature](https://img.shields.io/badge/new-green)
+- Large compatibility with other libraries: [Example](#working-with-other-libraries)
+- Custom exceptions: [Example](#comparisons)
 
 ## Installation
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
```

### Comparing `misura-1.5.0/pyproject.toml` & `misura-1.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.5.0/PKG-INFO` & `misura-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: misura
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
 Project-URL: Homepage, https://github.com/diantonioandrea/misura
 Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
 Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
 Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -39,22 +39,22 @@
 
 **misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
-- Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons).
-- Uncertainty handling: [Example](#mathematical-operations). ![New feature](https://img.shields.io/badge/new-green)
-- Manual conversions: [Example](#manual-and-automatic-conversion).
-- Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
-- Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units).
-- User defined base and derived units: [Example](#user-defined-units-of-measure). ![New feature](https://img.shields.io/badge/new-green)
-- Large compatibility with other libraries: [Example](#working-with-other-libraries).
-- Custom exceptions: [Example](#comparisons).
+- Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons)
+- Uncertainty handling: [Example](#mathematical-operations) ![New feature](https://img.shields.io/badge/new-green)
+- Manual conversions: [Example](#manual-and-automatic-conversion)
+- Automatic conversions on operations: [Example](#manual-and-automatic-conversion)
+- Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units)
+- User defined base and derived units: [Example](#user-defined-units-of-measure) ![New feature](https://img.shields.io/badge/new-green)
+- Large compatibility with other libraries: [Example](#working-with-other-libraries)
+- Custom exceptions: [Example](#comparisons)
 
 ## Installation
 
 ### Installing misura
 
 **misura** can be installed from [PyPI](https://pypi.org) by:
```

