# Comparing `tmp/misura-1.4.1.tar.gz` & `tmp/misura-1.5.0.tar.gz`

## Comparing `misura-1.4.1.tar` & `misura-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.4.1/.gitattributes
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.4.1/Makefile
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.4.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 misura-1.4.1/docs/docs.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/__init__.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/__main__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/exceptions.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/globals.py
--rw-r--r--   0        0        0    19140 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/quantities.py
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/tables.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 misura-1.4.1/src/misura/utilities.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 misura-1.4.1/tests/tests.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.4.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.4.1/LICENSE
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 misura-1.4.1/README.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 misura-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 misura-1.5.0/.gitattributes
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 misura-1.5.0/Makefile
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 misura-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 misura-1.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 misura-1.5.0/docs/docs.md
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/__init__.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/__main__.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/exceptions.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/globals.py
+-rw-r--r--   0        0        0    22520 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/quantities.py
+-rw-r--r--   0        0        0    20506 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/tables.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 misura-1.5.0/src/misura/utilities.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 misura-1.5.0/tests/tests.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 misura-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 misura-1.5.0/LICENSE
+-rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 misura-1.5.0/README.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 misura-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 misura-1.5.0/PKG-INFO
```

### Comparing `misura-1.4.1/.github/ISSUE_TEMPLATE/feature_request.md` & `misura-1.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `misura-1.4.1/.github/workflows/python-publish.yml` & `misura-1.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `misura-1.4.1/docs/docs.md` & `misura-1.5.0/docs/docs.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,43 +22,46 @@
 - [Exceptions](#exceptions)
 - [Examples](#examples)
 
 ## Introduction
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
-**misura** is a Python library designed to simplify the _handling of units of measure_ for scientific and engineering applications. It provides a unified interface for _dealing with different units and their conversions_, allowing for quick and accurate calculations without the need for complex manual conversions.
+**misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
 
 **misura** is written in Python and developed by [Andrea Di Antonio](https://github.com/diantonioandrea).
 
 ## Quantities
 
 [Go back to ToC](#table-of-contents)
 
-Quantities are defined as `misura.quantity(value: any, unit: str)` objects.
+Quantities are defined as `misura.quantity(value: any, unit: str = "", uncertainty: any = 0)` objects.
 
 `values` stands for the value of the quantity itself, while `unit` represents its unit of measure.  
 `quantity(2, "kg")` is a well-defined quantity.
 
-`unit` must be a string in which the different units of measure must be _separated by a space_ and _followed by their exponent_, if different from `1`.  
+`unit` is a string in which the different units of measure must be _separated by a space_ and _followed by their exponent_, if different from `1`.  
 `quantity(3, "m s-1")` is a well-defined quantity.
 
+`uncertainty` stands for the quantity's uncertainty.  
+`quantity(3, "s", 0.5)` is a well-defined quantity.
+
 ### Methods
 
 `misura.quantity` objects implement the following methods:
 
 ```python
 def unit(self, print: bool = False) -> str
-def dimensionality(self) -> str
+def dimesion(self) -> str
 ```
 
 which:
 
 - `unit()`: Returns the units string of the quantity. It returns it in a fancier way if `print = True`.
-- `dimensionality()`: Returns the dimensionality string of the quantity if it is convertible.
+- `dimesion()`: Returns the dimesion string of the quantity if it is convertible.
 
 ### Operations
 
 `misura.quantity` objects implement the following dunder methods:
 
 ```python
 def __str__(self) -> str
@@ -69,27 +72,27 @@
 def __float__(self) -> float
 def __complex__(self) -> complex
 def __bool__(self) -> bool
 
 def __abs__(self) -> any
 def __pos__(self) -> any
 def __neg__(self) -> any
-def __invert__(self) -> any
+# def __invert__(self) -> any
 def __round__(self, number: int) -> any
 def __floor__(self, number: int) -> any
 def __ceil__(self, number: int) -> any
 def __trunc__(self, number: int) -> any
 
 def __add__(self, other: any) -> any
 def __sub__(self, other: any) -> any
 def __mul__(self, other: any) -> any
 def __truediv__(self, other: any) -> any
 def __floordiv__(self, other: any) -> any
 def __pow__(self, other: any) -> any
-def __mod__(self, other: any) -> any
+# def __mod__(self, other: any) -> any
 
 def __lt__(self, other: any) -> any
 def __le__(self, other: any) -> any
 def __gt__(self, other: any) -> any
 def __ge__(self, other: any) -> any
 def __eq__(self, other: any) -> any
 def __ne__(self, other: any) -> any
@@ -227,62 +230,65 @@
 
 ## Global options
 
 [Go back to ToC](#table-of-contents)
 
 **misura** implements the following global options:
 
-- `misura.style.unitHighlighting`, bool: Enables units of measure highlighting. Dafault: `True`.
+- `misura.style.quantityHighlighting`, bool: Enables units of measure highlighting. Dafault: `True`.
+- `misura.style.quantityPlusMinus`, string: "+-" symbol. Dafault: `" \u00b1 "`.
 
 Take a look at these [examples](#global-options-1)
 
 ## Exceptions
 
 [Go back to ToC](#table-of-contents)
 
 **misura** implements the following exceptions:
 
-- `UnitError`: raised on invalid `unit` passed to `quantity(value, unit)`.
+- `InitError`: raised on invalid quantity definition.
+- `UnitError`: raised on invalid `unit`.
 - `QuantityError`: raised on operations between incompatible quantities.
 - `ConversionError`: raised on errors during conversions.
 - `UnpackError`: raised on errors during unpacking.
 - `PackError`: raised on errors during packing.
 - `DefinitionError`: raised on errors during unit definition.
 
 ## Examples
 
 [Go back to ToC](#table-of-contents)
 
 ### Quantities
 
 ```python
 from misura import quantity
+import math
 import numpy
 
-num1 = quantity(7, "m s-1")
+num1 = quantity(7, "m s-1", 1)
 num2 = quantity(4, "km")
-num3 = numpy.array([quantity(2, "m"), quantity(4, "km")])
+num3 = numpy.array([quantity(2, "m", .5), quantity(4, "km", .1)])
 num4 = quantity(numpy.array([1, 2, 3]), "T")
 
 print(num1.unit(print=True))
-print(num1.dimensionality())
+print(num1.dimesion())
 print(num1 * 3)
 print(num2 ** 2 < 16)
-print(numpy.sum(num3))
+print(math.trunc(numpy.sum(num3)))
 print(num4)
 ```
 
 The output is:
 
 ```
 m / s
 [length / time]
-21 m / s
+21 ± 3 m / s
 False
-4002.0 m
+4002 ± 100 m
 [1 2 3] T
 ```
 
 ### Units of measure
 
 ```python
 from misura import quantity, convert, addUnit
@@ -335,21 +341,22 @@
 ### Global options
 
 ```python
 from misura import quantity
 from misura import style
 
 style.quantityHighlighting = False
+style.quantityPlusMinus = " +- "
 
 num1 = quantity(2, "m s-1")
-num2 = quantity(5, "s")
+num2 = quantity(5, "s", 1)
 
 print(num1)
 print(num2)
 ```
 
 The output is:
 
 ```
 2 [m / s]
-5 [s]
+5 +- 1 [s]
 ```
```

### Comparing `misura-1.4.1/src/misura/__main__.py` & `misura-1.5.0/src/misura/__main__.py`

 * *Files identical despite different names*

### Comparing `misura-1.4.1/src/misura/exceptions.py` & `misura-1.5.0/src/misura/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 # Exceptions.
 
 
 class UnitError(Exception):
     """
-    Raised on invalid unit passed to quantity(value: any, unit: str).
+    Raised on invalid units.
     """
 
     def __init__(self, unit: str) -> None:
+        super().__init__("invalid unit '{}'".format(unit))
+
+
+class InitError(Exception):
+    """
+    Raised on invalid parameters passed to quantity.__init__().
+    """
+
+    def __init__(self, value: any, unit: str = "", uncertainty: any = 0) -> None:
+        from .utilities import uAny
+
         super().__init__(
-            "unknown unit: {}".format(unit) if unit != "" else "empty unit"
+            "wrong parameters on quantity definition\nraised by: quantity({}{}{})".format(
+                value,
+                ", {}".format(unit) if unit else "",
+                ", {}".format(uncertainty) if uAny(uncertainty) else "",
+            )
         )
 
 
 class QuantityError(Exception):
     """
     Raised on operations between incompatible quantities.
     """
```

### Comparing `misura-1.4.1/src/misura/quantities.py` & `misura-1.5.0/src/misura/quantities.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,74 @@
+# Quantities.
 from __future__ import annotations
 
 from colorama import Style
+from math import sqrt
 
 from .exceptions import (
     UnitError,
     QuantityError,
     ConversionError,
     UnpackError,
     PackError,
 )
 from .tables import getBase, getDerived, getDerivedUnpacking, getFamily, getRep
-from .utilities import dictFromUnit, unitFromDict
-
-# QUANTITIES
+from .utilities import dictFromUnit, unitFromDict, checkIter, uAll, uAny
 
 
 class quantity:
     """
     The main class of misura, the class of quantities.
     """
 
-    def __init__(self, value: any, unit: str) -> None:
+    def __init__(self, value: any, unit: str = "", uncertainty: any = 0) -> None:
         """
         value: Can be anything that can be somewhat treated as a number.
         unit: A properly formatted string including all the units with their exponents. e.g. "m s-1".
         """
 
         try:
             assert isinstance(unit, str)
-            assert unit != ""
+            assert uAll(uncertainty >= 0) if uAny(uncertainty) else True
+            assert (
+                (checkIter(value) == checkIter(uncertainty))
+                if uAny(uncertainty)
+                else True
+            )
 
         except AssertionError:
-            raise UnitError(unit)
+            raise UnitError(value, unit, uncertainty)  # Needs a better exception.
 
         self.value: any = value
+        self.uncertainty = uncertainty
 
         table: dict = getBase()
         table.update(getDerived())
 
         # From unit: str to self.units: dict.
         self.units: dict = dictFromUnit(unit)
 
         # Checks whether the unit can be converted with the available units.
         self.convertible: bool = all(
             [any([unit in table[family] for family in table]) for unit in self.units]
         )
 
         # Define quantity's dimentsionality based on self.units.
-        self.dimensionalities: dict = (
+        self.dimesions: dict = (
             {getFamily(unit): self.units[unit] for unit in self.units}
             if self.convertible
             else dict()
         )
 
     def unit(self, print: bool = False) -> str:
         """
         Returns a readable version of the quantity's unit.
         print = True makes the output fancier.
         """
-        from .globals import style  # Unit highlighting.
+        from .globals import style
 
         # Fancy version.
         if print:
             # {"m": 1, "s": -1} -> "[m / s]".
             numerator = " ".join(
                 sorted(
                     [
@@ -110,145 +116,172 @@
                 )
 
             return "[" + numerator + denominator + "]" if numerator else ""
 
         # {"m": 1, "s": -1} -> "m s-1".
         return unitFromDict(self.units)
 
-    def dimensionality(self) -> str:
+    def dimesion(self) -> str:
         """
-        Returns a readable version of the quantity's dimensionality.
+        Returns a readable version of the quantity's dimesion.
         No fancy style.
         """
 
-        if not len(self.dimensionalities):
+        if not len(self.dimesions):
             return ""
 
         # {"length": 2, "time": -1} -> "[length(2) / time]".
         numerator = " * ".join(
             sorted(
                 [
                     dim
                     + (
-                        "({})".format(self.dimensionalities[dim])
-                        if self.dimensionalities[dim] != 1
+                        "({})".format(self.dimesions[dim])
+                        if self.dimesions[dim] != 1
                         else ""
                     )
-                    for dim in self.dimensionalities
-                    if self.dimensionalities[dim] > 0
+                    for dim in self.dimesions
+                    if self.dimesions[dim] > 0
                 ]
             )
         )
         denominator = (
             (
                 " / "
                 + " * ".join(
                     sorted(
                         [
                             dim
                             + (
-                                "({})".format(-1 * self.dimensionalities[dim])
-                                if self.dimensionalities[dim] != -1
+                                "({})".format(-1 * self.dimesions[dim])
+                                if self.dimesions[dim] != -1
                                 else ""
                             )
-                            for dim in self.dimensionalities
-                            if self.dimensionalities[dim] < 0
+                            for dim in self.dimesions
+                            if self.dimesions[dim] < 0
                         ]
                     )
                 )
             )
-            if len(
-                [dim for dim in self.dimensionalities if self.dimensionalities[dim] < 0]
-            )
+            if len([dim for dim in self.dimesions if self.dimesions[dim] < 0])
             else ""
         )
 
         if not numerator and denominator:
             numerator = "1"
 
         return "[" + numerator + denominator + "]" if numerator else ""
 
     # STRINGS.
 
     def __str__(self) -> str:
-        return (
-            "{} {}".format(self.value, self.unit(print=True))
-            if self.unit()
-            else str(self.value)
+        from .globals import style
+
+        return "{}{}{}".format(
+            self.value,
+            "{}{} ".format(style.quantityPlusMinus, self.uncertainty)
+            if uAny(self.uncertainty)
+            else " ",
+            self.unit(print=True) if self.units else "",
         )
 
     def __repr__(self) -> str:
         return str(self)
 
     def __format__(self, string) -> str:  # Unit highlighting works for print only.
+        from .globals import style
+
         # This works with print only.
-        return self.value.__format__(string) + (
-            " " + self.unit(print=True) if self.unit() else ""
+        return (
+            self.value.__format__(string)
+            + (
+                (style.quantityPlusMinus + self.uncertainty.__format__(string))
+                if uAny(self.uncertainty)
+                else ""
+            )
+            + (" " + self.unit(print=True) if self.unit() else "")
         )
 
     # PYTHON TYPES CONVERSION.
 
+    """
+    int, float and complex don't care about uncertainty.
+    """
+
     # Int.
     def __int__(self) -> int:
         return int(self.value)
 
     # Float.
     def __float__(self) -> float:
         return float(self.value)
 
     # Complex.
     def __complex__(self) -> complex:
         return complex(self.value)
 
     # Bool.
     def __bool__(self) -> bool:
-        return bool(self.value)
+        return bool(self.value or self.uncertainty)
 
     # MATH.
 
     # Abs.
     def __abs__(self) -> quantity:
-        return quantity(abs(self.value), self.unit())
+        # Since abs(number) cannot be negative, the uncertainty on this value gets modified.
+        return quantity(
+            abs(self.value),
+            self.unit(),
+            self.uncertainty if uAny(self.uncertainty) < self.value else self.value,
+        )
 
     # Positive.
     def __pos__(self) -> quantity:
-        return quantity(+self.value, self.unit())
+        return quantity(+self.value, self.unit(), self.uncertainty)
 
     # Negative.
     def __neg__(self) -> quantity:
-        return quantity(-self.value, self.unit())
+        return quantity(-self.value, self.unit(), self.uncertainty)
 
     # Invert.
-    def __invert__(self) -> quantity:
-        return quantity(~self.value, self.unit())
+    # def __invert__(self) -> quantity:
+    #     return quantity(~self.value, self.unit())
 
     # Round.
     def __round__(self, number: int) -> quantity:
-        return quantity(round(self.value, number), self.unit())
+        return quantity(
+            round(self.value, number), self.unit(), round(self.uncertainty, number + 1)
+        )
 
     # Floor.
     def __floor__(self) -> quantity:
         from math import floor
 
-        return quantity(floor(self.value), self.unit())
+        return quantity(floor(self.value), self.unit(), floor(self.uncertainty))
 
     # Ceil.
     def __ceil__(self) -> quantity:
         from math import ceil
 
-        return quantity(ceil(self.value), self.unit())
+        return quantity(ceil(self.value), self.unit(), ceil(self.uncertainty))
 
     # Trunc.
     def __trunc__(self) -> quantity:
         from math import trunc
 
-        return quantity(trunc(self.value), self.unit())
+        return quantity(trunc(self.value), self.unit(), trunc(self.uncertainty))
 
     # Addition.
-    def __add__(self, other: quantity) -> quantity:
+    def __add__(self, other: any) -> quantity:
+        if not isinstance(other, quantity):
+            if self.unit():
+                raise QuantityError(self, quantity(other, ""), "+")
+
+            return quantity(self.value + other, "", self.uncertainty)
+
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 # Chooses the one to convert.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
@@ -256,21 +289,31 @@
                     if len(first.unit()) < len(second.unit())
                     else (self, second)
                 )
 
             else:
                 raise QuantityError(self, other, "+")
 
-        return quantity(self.value + other.value, self.unit())
+        return quantity(
+            self.value + other.value,
+            self.unit(),
+            sqrt(self.uncertainty**2 + other.uncertainty**2),
+        )
 
     def __radd__(self, other: quantity) -> quantity:
         return self.__add__(other)
 
     # Subtraction.
-    def __sub__(self, other: quantity) -> quantity:
+    def __sub__(self, other: any) -> quantity:
+        if not isinstance(other, quantity):
+            if self.unit():
+                raise QuantityError(self, quantity(other, ""), "-")
+
+            return quantity(self.value - other, "", self.uncertainty)
+
         if self.unit() != other.unit():
             if self.convertible and other.convertible:
                 # Chooses the one to convert.
                 first = convert(self, other.unit())
                 second = convert(other, self.unit())
 
                 self, other = (
@@ -278,91 +321,117 @@
                     if len(first.unit()) < len(second.unit())
                     else (self, second)
                 )
 
             else:
                 raise QuantityError(self, other, "-")
 
-        return quantity(self.value - other.value, self.unit())
+        return quantity(
+            self.value - other.value,
+            self.unit(),
+            sqrt(self.uncertainty**2 + other.uncertainty**2),
+        )
 
     def __rsub__(self, other: quantity) -> quantity:
         return self.__sub__(other)
 
     # Multiplication.
     def __mul__(self, other: any) -> any:
         if not isinstance(other, quantity):
-            return quantity(self.value * other, self.unit())
+            return quantity(self.value * other, self.unit(), self.uncertainty * other)
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
         for unit in newUnits:
             if unit in other.units:
                 newUnits[unit] += other.units[unit]
 
         for unit in other.units:
             if unit not in newUnits:
                 newUnits[unit] = other.units[unit]
 
-        return (
-            quantity(self.value * other.value, unitFromDict(newUnits))
-            if unitFromDict(newUnits)
-            else self.value * other.value
+        return quantity(
+            self.value * other.value,
+            unitFromDict(newUnits),
+            sqrt(
+                (other.value * self.uncertainty) ** 2
+                + (self.value * other.uncertainty) ** 2
+            ),
         )
 
     def __rmul__(self, other: any) -> any:
         return self.__mul__(other)
 
     # Division.
     def __truediv__(self, other: any) -> any:
         if not isinstance(other, quantity):
-            return quantity(self.value / other, self.unit())
+            return quantity(self.value / other, self.unit(), self.uncertainty / other)
 
         newUnits = self.units.copy()
 
         if self.convertible and other.convertible:
             other = convert(other, self.unit(), partial=True)
 
         for unit in newUnits:
             if unit in other.units:
                 newUnits[unit] -= other.units[unit]
 
         for unit in other.units:
             if unit not in newUnits:
                 newUnits[unit] = -other.units[unit]
 
-        return (
-            quantity(self.value / other.value, unitFromDict(newUnits))
-            if unitFromDict(newUnits)
-            else self.value / other.value
+        return quantity(
+            self.value / other.value,
+            unitFromDict(newUnits),
+            sqrt(
+                (self.uncertainty / other.value) ** 2
+                + (self.value * other.uncertainty / (other.value**2)) ** 2
+            ),
         )
 
     def __floordiv__(self, other: any) -> quantity:
-        return quantity(self.value // other, self.unit())
+        return quantity(
+            self.value // other, self.unit(), self.uncertainty // other
+        )  # Check uncertainty.
 
     def __rtruediv__(self, other: any) -> any:
         return self**-1 * other
 
     # Power.
     def __pow__(self, other: any) -> quantity:
+        if isinstance(other, quantity):
+            raise QuantityError(self, other, "**")
+
         if other == 0:
-            return 1
+            return quantity(1 * bool(self.value), "", 1 * self.uncertainty != 0)
+
+        if other == 1:
+            return self
 
         newUnits = self.units.copy()
 
         for unit in newUnits:
             newUnits[unit] *= other
 
-        return quantity(self.value**other, unitFromDict(newUnits))
+        return quantity(
+            self.value**other,
+            unitFromDict(newUnits),
+            abs(other) * (self.value ** (other - 1)) * self.uncertainty,
+        )
+
+    def __rpow__(self, other: any) -> quantity:
+        if isinstance(other, quantity):
+            raise QuantityError(self, other, "**")
 
     # Modulo.
-    def __mod__(self, other: any) -> quantity:
-        return quantity(self.value % other, self.unit())
+    # def __mod__(self, other: any) -> quantity:
+    #     return quantity(self.value % other, self.unit())
 
     # COMPARISONS.
 
     # Less than.
     def __lt__(self, other: any) -> quantity:
         if not isinstance(other, quantity):
             return self.value < other
@@ -432,95 +501,103 @@
 
         return self.value != other.value or self.unit() != other.unit()
 
 
 # CONVERSION, UNPACKING AND PACKING
 
 
+# Conversion function.
 def convert(
     qnt: quantity, targets: str, partial: bool = False, un_pack: bool = True
 ) -> quantity:
     """
     Conversion function; converts the passed quantity object to the specified target units.
 
     "partial = True" converts only the specified units and "un_pack = True" enables automatic (un)packing.
     """
 
+    # Cannot convert non-convertible units.
     if not qnt.convertible:
         raise ConversionError(qnt, targets)
 
-    # Check dimensionality.
+    # Check dimesion.
     if not partial:
-        if (
-            unpack(qnt).dimensionality()
-            != unpack(quantity(1, targets)).dimensionality()
-        ):
+        if unpack(qnt).dimesion() != unpack(quantity(1, targets)).dimesion():
             raise ConversionError(qnt, targets)
 
-    # Automatic (un)packing.
-    # Version 1.
+    # Automatic (un)packing, version 1.
     if un_pack and not partial:
         try:
+            # Tries to pack qnt.
             return convert(pack(qnt, targets), targets, un_pack=False)
 
-        except ConversionError:
+        except (PackError, ConversionError):
             pass
 
+        # Completely unpacks units.
         return convert(
             unpack(qnt),
             unpack(quantity(1, targets)).unit(),
             un_pack=False,
         )
 
     factor: float = 1.0
-    units: dict = qnt.units.copy()
-    targetUnits: dict = dictFromUnit(targets)
+    tUnits: dict = dictFromUnit(targets)  # Target units.
 
-    partialTargets: dict = dict()
+    pTargets: dict = dict()  # Partial targets.
 
     table: dict = getBase()
     table.update(getDerived())
 
-    for unit in units.keys():
+    for unit in qnt.units.keys():
         family = getFamily(unit)
-        familyCounter = 0
 
-        for targetSym in targetUnits:
-            if targetSym in table[family]:
-                targetUnit = targetSym
-                familyCounter += 1
-
-        if familyCounter == 0:
-            if not partial:
-                raise ConversionError(qnt, targets)
+        # Number of corresponding families.
+        families = len([tgt for tgt in tUnits if tgt in table[family]])
 
-            partialTargets[unit] = units[unit]
+        # Check target presence if not partial.
+        if families == 0 and not partial:
+            raise ConversionError(qnt, targets)
+
+        # Partial conversion.
+        elif families == 0 and partial:
+            pTargets[unit] = qnt.units[unit]
             continue
 
-        elif familyCounter > 1:
+        # Target.
+        target = [tgt for tgt in tUnits if tgt in table[family]].pop()
+
+        # Too many units: errror.
+        if families > 1:
             raise ConversionError(qnt, targets)
 
-        elif unit != targetUnit:
-            if units[unit] != targetUnits[targetUnit]:
-                raise ConversionError(qnt, targets)
+        # Wrong power.
+        if unit != target and qnt.units[unit] != tUnits[target]:
+            raise ConversionError(qnt, targets)
 
-            factor *= (table[family][unit] / table[family][targetUnit]) ** units[unit]
-            partialTargets[targetUnit] = targetUnits[targetUnit]
+        # Conversion.
+        elif unit != target and qnt.units[unit] == tUnits[target]:
+            factor *= (table[family][unit] / table[family][target]) ** qnt.units[unit]
+            pTargets[target] = tUnits[target]
             continue
 
+        # Partial conversion.
         elif partial:
-            partialTargets[unit] = units[unit]
+            pTargets[unit] = qnt.units[unit]
 
     return (
-        quantity(qnt.value * factor, targets)
+        quantity(qnt.value * factor, targets, qnt.uncertainty * factor)
         if not partial
-        else quantity(qnt.value * factor, unitFromDict(partialTargets))
+        else quantity(
+            qnt.value * factor, unitFromDict(pTargets), qnt.uncertainty * factor
+        )
     )
 
 
+# Unpacking function.
 def unpack(qnt: quantity, targets: str = "") -> quantity:
     """
     Unpacking function; unpacks the passed targets units form the quantity object.
 
     'targets = ""' completely unpacks the quantity.
     """
 
@@ -532,38 +609,46 @@
             [unit for unit in qnt.units if getFamily(unit) in derivedTable]
         )
 
         if targets == "":
             return qnt
 
     for target in dictFromUnit(targets):
+        # Checks target.
         if getFamily(target) not in [getFamily(unit) for unit in qnt.units]:
             raise UnpackError(qnt, target)
 
-        conversionTarget = getRep(getFamily(target))
-        conversionTargetPower = [
+        cTarget = getRep(getFamily(target))  # Conversion target.
+        cTargetPower = [  # Conversion target's power.
             qnt.units[unit]
             for unit in qnt.units
             if getFamily(unit) == getFamily(target)
         ].pop()
 
+        # Raises an error if the program does not know how to unpack a unit.
+        if cTarget not in unpackTable:
+            raise UnpackError(qnt, target)
+
+        # Converts the quantity to an unpackable one.
         qnt = convert(
             qnt,
-            conversionTarget + str(conversionTargetPower),
+            cTarget + str(cTargetPower),
             partial=True,
             un_pack=False,
         )
 
-        if conversionTarget not in unpackTable:
-            raise UnpackError(qnt, target)
+        # Units that werent't involved in the previous conversion.
+        newUnits = {key: qnt.units[key] for key in qnt.units if key != cTarget}
 
-        newUnits = {key: qnt.units[key] for key in qnt.units if key != conversionTarget}
+        # Uncertainty should not vary on packing.
+        uncertainty = qnt.uncertainty
         qnt = (
             quantity(qnt.value, unitFromDict(newUnits)) if len(newUnits) else qnt.value
-        ) * (quantity(1, unpackTable[conversionTarget]) ** qnt.units[conversionTarget])
+        ) * (quantity(1, unpackTable[cTarget]) ** qnt.units[cTarget])
+        qnt.uncertainty = uncertainty
 
     return qnt
 
 
 # Packing function.
 def pack(qnt: quantity, targets: str, ignore: str = "", full: bool = False) -> quantity:
     """
@@ -578,22 +663,20 @@
     unitsTable.update(getDerived())
 
     if targets == "":
         raise PackError(qnt, "")
 
     # Simplify qnt -> base unit.
     for unit in qnt.units:
-        conversionTarget = [
+        cTarget = [
             unit
             for unit in unitsTable[getFamily(unit)]
             if unitsTable[getFamily(unit)][unit] == 1
         ].pop()
-        qnt = convert(
-            qnt, conversionTarget + str(qnt.units[unit]), partial=True, un_pack=False
-        )
+        qnt = convert(qnt, cTarget + str(qnt.units[unit]), partial=True, un_pack=False)
 
     # Unpack only relevant units.
     if ignore:
         for ignored in dictFromUnit(ignore):
             if getFamily(ignored) not in [getFamily(unit) for unit in qnt.units]:
                 raise PackError(qnt, targets, ignore)
 
@@ -637,24 +720,29 @@
             for targetUnit in targetUnits
             if targetUnit in qnt.units
         }
 
         if not len(powers):
             raise PackError(qnt, targets)
 
+        # Full packing is a stricter form of packing which
+        # requires that "no other units are produced from the packing process".
         if full:
             # Packability check.
             for targetUnit in targetUnits:
                 if targetUnit not in qnt.units:
                     raise PackError(qnt, targets, full=True)
 
                 if qnt.units[targetUnit] % targetUnits[targetUnit]:
                     raise PackError(qnt, targets, full=True)
 
             if min(powers) < max(powers) or max(powers) < 0:
                 raise PackError(qnt, targets, full=True)
 
+        # Uncertainty should not vary on packing.
+        uncertainty = qnt.uncertainty
         qnt *= (quantity(1, target) / quantity(1, unitFromDict(targetUnits))) ** max(
             powers
         )
+        qnt.uncertainty = uncertainty
 
     return qnt
```

### Comparing `misura-1.4.1/src/misura/tables.py` & `misura-1.5.0/src/misura/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# Tables.
 from .exceptions import DefinitionError
 from .utilities import dictFromUnit
 from .globals import defined
 
-# Utilities
+# Tables utilities
 
 
 def getRep(family: str) -> str:
     """
     Returns a reference unit given its family.
     """
 
@@ -66,14 +67,18 @@
     return table
 
 
 # Conversion tables.
 
 
 def addUnit(family: str, units: dict, unpacks: str = ""):
+    """
+    addUnit function, allows users to define new units.
+    """
+
     table = getBase()
     table.update(getDerived())
 
     try:
         assert isinstance(family, str)
         assert isinstance(units, dict)
         assert family != ""
```

### Comparing `misura-1.4.1/src/misura/utilities.py` & `misura-1.5.0/src/misura/utilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,41 @@
+# Utilities.
 from re import findall
 
-from .exceptions import UnitError
 
-# Utilities.
+def checkIter(obj: any) -> bool:
+    try:
+        _ = iter(obj)
+        return True
+
+    except TypeError:
+        return False
+
+
+def uAll(obj: any) -> bool:
+    """
+    Python's 'all' for (non)iterable objects.
+    """
+
+    return all(obj) if checkIter(obj) else bool(obj)
+
+
+def uAny(obj: any) -> bool:
+    """
+    Python's 'any' for (non)iterable objects.
+    """
+
+    return any(obj) if checkIter(obj) else bool(obj)
 
 
 def dictFromUnit(unit: str) -> dict:
+    from .exceptions import UnitError
+
     """
-    Returns the dictionary of units from a properly formatted string..
+    Returns the dictionary of units from a properly formatted string.
     """
 
     units = dict()
 
     for sym in unit.split(" "):
         candidate = findall(r"-?\d+\.?\d*", sym)
```

### Comparing `misura-1.4.1/tests/tests.py` & `misura-1.5.0/tests/tests.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 num5 = quantity(15, "H TT")
 num6 = quantity(12, "m2 s-2")
 num7 = quantity(3, "kg km2")
 num8 = quantity(13, "J")
 num9 = quantity(0.9, "mN km")
 num10 = quantity(3, "N m T")
 num11 = quantity(12, "kbnn")
+num12 = quantity(2, "kg", 0.5)
+num13 = quantity(0.7, "m3", 0.15)
 
 # Math.
 print(num0**0.5)
 
 # Logical.
 print(num0 > 10)
 print(num0**0.5 < num1)
 print(num0 < 0.02 * num1**2)
 print(num1 == num2)
 print(num1 != num2)
 
-# Conversions
+# Conversions.
 print(num0**0.5 + num1)
 print(convert(num0, "dm2"))
 print(convert(num1, "m"))
 print(convert(num2, "mA", partial=True))
 
 # Unpacking.
 print(unpack(num3))
@@ -44,9 +46,13 @@
 print(pack(num7, "J"))
 
 # Automatic conversion with (un)packing.
 print(num8 + num9)
 print(num9 + num8)
 print(pack(num10, "J", ignore="T"))
 
-# Custom units conversions.
+# Custom units of measure.
 print(convert(num11, "bnn"))
+
+# Uncertainty.
+print(num12**2)
+print(num12 / num13)
```

### Comparing `misura-1.4.1/LICENSE` & `misura-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `misura-1.4.1/README.md` & `misura-1.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: misura
+Version: 1.5.0
+Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
+Project-URL: Homepage, https://github.com/diantonioandrea/misura
+Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
+Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
+Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: colorama
+Requires-Dist: setuptools
+Description-Content-Type: text/markdown
+
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/misura)
 
 ![PyPI](https://img.shields.io/pypi/v/misura?label=misura%20on%20pypi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
 
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/diantonioandrea/misura)
@@ -9,32 +26,33 @@
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
->>> from misura import quantity as qnt
->>> (qnt(2, "m") + qnt(50, "cm")) / qnt(4, "s")
-0.625 m / s
+>>> from misura import quantity
+>>> quantity(7, "m", 1.5) / quantity(2, "s")
+3.5 ± 0.75 m / s
 ```
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
-**misura** is a Python library designed to simplify the _handling of units of measure_ for scientific and engineering applications. It provides a unified interface for _dealing with different units and their conversions_, allowing for quick and accurate calculations without the need for complex manual conversions.
+**misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
 - Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons).
+- Uncertainty handling: [Example](#mathematical-operations). ![New feature](https://img.shields.io/badge/new-green)
 - Manual conversions: [Example](#manual-and-automatic-conversion).
 - Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
 - Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units).
-- User defined base and derived units: [Example](#user-defined-units-of-measure).
+- User defined base and derived units: [Example](#user-defined-units-of-measure). ![New feature](https://img.shields.io/badge/new-green)
 - Large compatibility with other libraries: [Example](#working-with-other-libraries).
 - Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
@@ -118,31 +136,31 @@
 ### Mathematical operations
 
 ```python
 from misura import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
-num3 = quantity(2, "s")
+num3 = quantity(2, "s", .5)
 
 print(num1 + num2)
-print((num1 + num2).dimensionality())
+print((num1 + num2).dimesion())
 print(num1 * num2)
 print(num1 / num3)
 print(num3 ** 2)
 ```
 
 The output is:
 
 ```
 6 m / s
 [length / time]
 8 m(2) / s(2)
-1.0 m / s(2)
-4 s(2)
+1.0 ± 0.25 m / s(2)
+4 ± 2.0 s(2)
 ```
 
 ### Working with other libraries
 
 ```python
 from misura import quantity, convert
 from decimal import Decimal, getcontext
```

### Comparing `misura-1.4.1/pyproject.toml` & `misura-1.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "misura"
-version = "1.4.1"
+version = "1.5.0"
 authors = [
   { name="Andrea Di Antonio", email="mail@diantonioandrea.com" },
 ]
 description = "Python library for easy unit handling and conversion for scientific & engineering applications."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ["colorama", "setuptools"]
```

### Comparing `misura-1.4.1/PKG-INFO` & `misura-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: misura
-Version: 1.4.1
-Summary: Python library for easy unit handling and conversion for scientific & engineering applications.
-Project-URL: Homepage, https://github.com/diantonioandrea/misura
-Project-URL: Documentation, https://github.com/diantonioandrea/misura/blob/main/docs/docs.md
-Project-URL: Bug Tracker, https://github.com/diantonioandrea/misura/issues
-Author-email: Andrea Di Antonio <mail@diantonioandrea.com>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Requires-Dist: colorama
-Requires-Dist: setuptools
-Description-Content-Type: text/markdown
-
 ![GitHub](https://img.shields.io/github/license/diantonioandrea/misura)
 
 ![PyPI](https://img.shields.io/pypi/v/misura?label=misura%20on%20pypi)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/misura)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/misura)
 
 ![Libraries.io dependency status for GitHub repo](https://img.shields.io/librariesio/github/diantonioandrea/misura)
@@ -26,32 +9,33 @@
 ![GitHub Release Date](https://img.shields.io/github/release-date/diantonioandrea/misura)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # misura
 
 ```python
->>> from misura import quantity as qnt
->>> (qnt(2, "m") + qnt(50, "cm")) / qnt(4, "s")
-0.625 m / s
+>>> from misura import quantity
+>>> quantity(7, "m", 1.5) / quantity(2, "s")
+3.5 ± 0.75 m / s
 ```
 
 Python library for easy unit handling and conversion for scientific & engineering applications.
 
-**misura** is a Python library designed to simplify the _handling of units of measure_ for scientific and engineering applications. It provides a unified interface for _dealing with different units and their conversions_, allowing for quick and accurate calculations without the need for complex manual conversions.
+**misura** is a powerful Python library designed to streamline the *handling of units of measure for scientific and engineering applications*. It offers a unified interface for dealing with *different units and their conversions*, so you can quickly and accurately *perform calculations without the need for complex manual conversions*. Additionally, **misura** provides *uncertainty hadnling*, so *you can work with physical quantities and their associated uncertainties in a consistent and intuitive way*. On top of that, **misura** enables you to *define your own custom units of measure*, giving you the flexibility to work in your preferred units.
 
 Make sure to take a look at the [documentation](https://github.com/diantonioandrea/misura/blob/main/docs/docs.md), at the [contributing guidelines](https://github.com/diantonioandrea/.github/blob/main/CONTRIBUTING.md) and at the [examples](#examples).
 
 ### Features
 
 - Mathematical and logical operations between quantities: [Example](#mathematical-operations), [example](#comparisons).
+- Uncertainty handling: [Example](#mathematical-operations). ![New feature](https://img.shields.io/badge/new-green)
 - Manual conversions: [Example](#manual-and-automatic-conversion).
 - Automatic conversions on operations: [Example](#manual-and-automatic-conversion).
 - Unpack and pack derived units: [Example](#unpack-derived-units), [example](#pack-units).
-- User defined base and derived units: [Example](#user-defined-units-of-measure).
+- User defined base and derived units: [Example](#user-defined-units-of-measure). ![New feature](https://img.shields.io/badge/new-green)
 - Large compatibility with other libraries: [Example](#working-with-other-libraries).
 - Custom exceptions: [Example](#comparisons).
 
 ## Installation
 
 ### Installing misura
 
@@ -135,31 +119,31 @@
 ### Mathematical operations
 
 ```python
 from misura import quantity
 
 num1 = quantity(2, "m s-1")
 num2 = quantity(4, "m s-1")
-num3 = quantity(2, "s")
+num3 = quantity(2, "s", .5)
 
 print(num1 + num2)
-print((num1 + num2).dimensionality())
+print((num1 + num2).dimesion())
 print(num1 * num2)
 print(num1 / num3)
 print(num3 ** 2)
 ```
 
 The output is:
 
 ```
 6 m / s
 [length / time]
 8 m(2) / s(2)
-1.0 m / s(2)
-4 s(2)
+1.0 ± 0.25 m / s(2)
+4 ± 2.0 s(2)
 ```
 
 ### Working with other libraries
 
 ```python
 from misura import quantity, convert
 from decimal import Decimal, getcontext
```

