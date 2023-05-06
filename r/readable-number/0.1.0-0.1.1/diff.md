# Comparing `tmp/readable_number-0.1.0.tar.gz` & `tmp/readable_number-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readable_number-0.1.0.tar", last modified: Fri Apr 28 06:43:53 2023, max compression
+gzip compressed data, was "readable_number-0.1.1.tar", last modified: Sat May  6 00:02:52 2023, max compression
```

## Comparing `readable_number-0.1.0.tar` & `readable_number-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:43:53.401349 readable_number-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-28 06:43:42.000000 readable_number-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 06:43:42.000000 readable_number-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-28 06:43:53.401349 readable_number-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-28 06:43:42.000000 readable_number-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:43:53.401349 readable_number-0.1.0/readable_number/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-28 06:43:42.000000 readable_number-0.1.0/readable_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12094 2023-04-28 06:43:42.000000 readable_number-0.1.0/readable_number/readable_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:43:53.401349 readable_number-0.1.0/readable_number.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-28 06:43:53.000000 readable_number-0.1.0/readable_number.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 06:43:53.000000 readable_number-0.1.0/readable_number.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:43:53.000000 readable_number-0.1.0/readable_number.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 06:43:53.000000 readable_number-0.1.0/readable_number.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-28 06:43:53.401349 readable_number-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 06:43:42.000000 readable_number-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:43:53.401349 readable_number-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-04-28 06:43:42.000000 readable_number-0.1.0/tests/test_readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-06 00:02:41.000000 readable_number-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:02:41.000000 readable_number-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:02:52.825119 readable_number-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-06 00:02:41.000000 readable_number-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/readable_number/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-06 00:02:41.000000 readable_number-0.1.1/readable_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14705 2023-05-06 00:02:41.000000 readable_number-0.1.1/readable_number/readable_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/readable_number.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 00:02:52.000000 readable_number-0.1.1/readable_number.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-06 00:02:52.825119 readable_number-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-06 00:02:41.000000 readable_number-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 00:02:52.825119 readable_number-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20334 2023-05-06 00:02:41.000000 readable_number-0.1.1/tests/test_readable_number.py
```

### Comparing `readable_number-0.1.0/LICENSE` & `readable_number-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readable_number-0.1.0/PKG-INFO` & `readable_number-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: readable_number
-Version: 0.1.0
-Summary: A Python library to print numbers in human readable format
-Home-page: https://github.com/jsh9/readable-number
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # readable-number
 A Python library to print numbers in human readable format
 
 ## 1. Installation
 
 ```
 pip install readable-number
@@ -27,43 +10,78 @@
 This library does not depend on any third-party libraries, so installing it will not break your Python environment.
 
 ## 2. Usage
 
 ```python
 from readable_number import ReadableNumber
 
-# Print digit in groups
+### Print digit in groups
 str(ReadableNumber(-123))  # -123
 str(ReadableNumber(-1234))  # -1,234
 str(ReadableNumber(-123456789))  # -123,456,789
 str(ReadableNumber(-12345.6789))  # -12,345.6789
 str(ReadableNumber(-1.23456e18))  # -1,234,560,000,000,000,000
 
-# Custom grouping (in other locales)
+### Custom grouping (in other locales)
 str(ReadableNumber(-123456789, digit_group_size=4))  # -1,2345,6789
 str(ReadableNumber(-123456789, digit_group_delimiter='|'))  # -123|456|789
 
-# Convert to human-readable shortform (with k, M, B, and T as unit)
+### Convert to human-readable shortform (with k, M, B, and T as unit)
 str(ReadableNumber(12345, use_shortform=True))  # 12k
 str(ReadableNumber(12345, use_shortform=True, precision=1))  # 12.3k
 str(ReadableNumber(12345678, use_shortform=True))  # 12M
 str(ReadableNumber(12345678, use_shortform=True, precision=2))  # 12.35M
 
-# Numbers with small absolute values
+### Numbers with small absolute values
 str(ReadableNumber(0.12345))  # 0.12345
 str(ReadableNumber(0.0000012345))  # 0.0000012345
 str(ReadableNumber(0.12345, precision=None))  # 0.12345
 str(ReadableNumber(0.12345, precision=2))  # 0.12
 str(ReadableNumber(0.12345, precision=20))  # 0.123450000000000
 
-# Digits beyond double-precision limit are discarded
+### Digits beyond double-precision limit are discarded
 str(ReadableNumber(0.12345678901234567890, precision=90))  # 0.123456789012346
 str(ReadableNumber(1.23e-20, precision=90))  # 0.000000000000000
 
-# Print large/small numbers in exponantial notation
+### Print many numbers with the same config
+rn = ReadableNumber(precision=2, digit_group_size=4)
+rn.of(123456789)  # 1,2345,6789
+rn.of(0.123456789)  # 0.12
+rn.of(1e15)  # 1000,0000,0000,0000
+
+### Print large numbers in exponantial notation
 str(ReadableNumber(1234567890, use_exponent_for_large_numbers=True))  # 1.234568e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    precision=2,
+))  # 1.23e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    precision=None,
+))  # 1.23456789e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    large_number_threshold=1e20,  # only show in exp if we exceed this
+    precision=None,
+))  # 1,234,567,890
+
+### Print small numbers in exponential notation
 str(ReadableNumber(0.000000012, use_exponent_for_small_numbers=True))  # 1.200000e-08
+str(ReadableNumber(
+    -0.000000123456,
+    use_exponent_for_small_numbers=True,
+    precision=2,
+))  # -1.23e-07
+str(ReadableNumber(
+    -0.000012345,
+    use_exponent_for_small_numbers=True,
+    precision=None,
+    small_number_threshold=1e-2,
+))  # -1.2345e-05
 ```
 
 ## 3. Full API documentation
 
 Please visit this site: https://readable-number.readthedocs.io/en/stable/
```

### Comparing `readable_number-0.1.0/readable_number/readable_number.py` & `readable_number-0.1.1/readable_number/readable_number.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,16 +29,19 @@
 
 class ReadableNumber:
     """
     A class to hold a number for human-readable printing.
 
     Parameters
     ----------
-    num : numbers.Real
-        A number to be printed in a readable format.
+    num : numbers.Real or None
+        A number to be printed in a readable format.  If ``None``, it
+        means you are only initializing an "empty" object with printing
+        options. In that case, you can use the `of()` method later to
+        print the readable result.
     digit_group_size : int
         The size of the digit group (in the integer part).  For example,
         if 3, the number 123456789 will be printed as 123,456,789.
         If 0, no grouping will happen.  Only non-negative integers
         are allowed. (Default: 3)
     digit_group_delimiter : str
         The symbol to delimit the digit groups.  For example, if it
@@ -62,72 +65,97 @@
         (if ``precision`` is None, 2 digits will be used as per
         convention).
     use_shortform : bool
         If true, for large numbers, use notations such as "12.5k", "5.6M",
         etc. Currently, the largest supported unit is T (trillion). Numbers
         whose absolute values are larger than 1,000 trillion will be
         printed as something like "1535663T".
+    use_exponent_for_large_numbers : bool
+        Whether to use exponential notation (such as 1.2e+05) to represent
+        large numbers. Default: False.
+    large_number_threshold : int
+        If ``num``'s absolute value is beyond (≥) this cutoff value, we
+        consider it a large number. Default: 1,000,000.
+    use_exponent_for_small_numbers : bool
+        Whether to use exponential notation (such as 1.2e-05) to represent
+        small numbers. Default: False.
+    small_number_threshold : float
+        If ``num``'s absolute value is blow (≤) this cutoff value, we
+        consider it to be a small number. Default: 1 × 10⁻⁶.
 
     Examples
     --------
     >>> from readable_number import ReadableNumber
     >>> str(ReadableNumber(1234.567))
+    >>> rn = ReadableNumber()  # alternative way to print numbers
+    >>> rn.of(1234.567)
     """
 
     def __init__(
             self,
-            num: numbers.Real,
+            num: Optional[numbers.Real] = None,
             digit_group_size: int = 3,
             digit_group_delimiter: str = ',',
             decimal_symbol: str = '.',
             precision: Optional[int] = None,
             show_decimal_part_if_integer: bool = False,
             use_shortform: bool = False,
             use_exponent_for_large_numbers: bool = False,
+            large_number_threshold: int = 1_000_000,
             use_exponent_for_small_numbers: bool = False,
-    ):
-
-        self.num: numbers.Real = self._convert_to_num(num)
+            small_number_threshold: float = 1e-6,
+    ) -> None:
+        self.num: Optional[numbers.Real] = self._convert_to_num(num)
         self.digit_group_length = digit_group_size
         self.digit_group_delimiter = digit_group_delimiter
         self.decimal_symbol = decimal_symbol
         self.precision = precision
         self.show_decimal_part_if_integer = show_decimal_part_if_integer
         self.use_shortform = use_shortform
         self.use_exponent_for_large_numbers = use_exponent_for_large_numbers
+        self.large_number_threshold = large_number_threshold
         self.use_exponent_for_small_numbers = use_exponent_for_small_numbers
+        self.small_number_threshold = small_number_threshold
 
         self._validate_input_params()
 
     def __repr__(self):
         return str(self.num)
 
     def __str__(self):
+        if self.num is None:
+            raise ValueError(
+                'Please initialize the object with an actual number,'
+                ' or use the `of()` method to pass in a number.',
+            )
+
         if not math.isfinite(self.num):
             return str(self.num)
 
-        if self.use_exponent_for_small_numbers and 0 < abs(self.num) <= 1e-6:
-            return f'{self.num:e}'
+        if (
+            self.use_exponent_for_small_numbers
+            and 0 < abs(self.num) <= self.small_number_threshold
+        ):
+            return self._render_number_in_exponential()
 
-        if self.use_exponent_for_large_numbers and abs(self.num) >= 1e6:
-            return f'{self.num:e}'
+        if (
+            self.use_exponent_for_large_numbers
+            and abs(self.num) >= self.large_number_threshold
+        ):
+            return self._render_number_in_exponential()
 
         self.num_parts = self._get_integer_and_decimal_parts(self.num)
 
-        if (
-                self.use_shortform
-                and abs(self.num_parts.integer_part_int) > 1_000
-        ):
+        if self.use_shortform and abs(self.num_parts.integer_part_int) > 1_000:
             return self._render_integer_part_with_shortform()
 
         if self._is_integer():
             if self.show_decimal_part_if_integer:
                 decimal_part = (
-                    '00' if self.precision is None
-                    else '0'.zfill(self.precision)
+                    '00' if self.precision is None else '0'.zfill(self.precision)
                 )
                 return (
                     self._render_integer_part_in_groups()
                     + self.decimal_symbol
                     + decimal_part
                 )
 
@@ -142,14 +170,39 @@
         return (
             neg_sign
             + self._render_integer_part_in_groups(plus_1=should_carry_1_to_integer)
             + self.decimal_symbol
             + decimal_part
         )
 
+    def of(self, num: numbers.Real) -> str:
+        """
+        Print the number ``num`` in a readable format.  This method is
+        useful when you don't want to repeatedly specify the same options
+        when printing many numbers.
+
+        Parameters
+        ----------
+        num : numbers.Real
+            The number to be printed
+
+        Returns
+        -------
+        str
+            The number in a readable format
+
+        Examples
+        --------
+        >>> from readable_number import ReadableNumber
+        >>> rn = ReadableNumber()
+        >>> rn.of(1234.567)
+        """
+        self.num = num
+        return self.__str__()
+
     def _validate_input_params(self) -> None:
         if not isinstance(self.digit_group_length, int):
             raise TypeError('`digit_group_size` not an integer')
 
         if self.digit_group_length < 0:
             raise ValueError('`digit_group_size` should >= 0')
 
@@ -163,18 +216,15 @@
         if not isinstance(self.decimal_symbol, str):
             raise TypeError('`decimal_symbol` not a string')
 
         if self.decimal_symbol == '-':
             msg = 'Using "-" as `decimal_symbol` can cause ambiguity'
             raise ValueError(msg)
 
-        if (
-            self.precision is not None
-            and not isinstance(self.precision, int)
-        ):
+        if self.precision is not None and not isinstance(self.precision, int):
             msg = '`precision` not None and not int'
             raise TypeError(msg)
 
         if self.precision is not None and self.precision < 0:
             raise ValueError('`precision` should >= 0')
 
         if not isinstance(self.show_decimal_part_if_integer, bool):
@@ -185,14 +235,25 @@
 
         if not isinstance(self.use_exponent_for_large_numbers, bool):
             raise TypeError('`use_exponent_for_large_numbers` not a boolean')
 
         if not isinstance(self.use_exponent_for_small_numbers, bool):
             raise TypeError('`use_exponent_for_small_numbers` not a boolean')
 
+    def _render_number_in_exponential(self) -> str:
+        if self.precision is not None:
+            return f'{self.num:.{self.precision}e}'
+
+        temp_result = f'{self.num:.16e}'  # 16: max precision in 64-bit system
+        base_part_str, exp_part_str = temp_result.split('e')
+        base_part_float = float(base_part_str)
+        assert abs(base_part_float) < 10, 'Internal error; please contact the authors'
+        processed = str(ReadableNumber(base_part_float, precision=None))
+        return processed + 'e' + exp_part_str
+
     def _render_integer_part_with_shortform(self) -> str:
         num_digits = len(str(abs(self.num_parts.integer_part_int)))
         tier = (num_digits - 1) // 3
         tier = min(tier, MAX_TIER)
         unit_name = METRIC_PREFIX_LOOKUP[tier]
 
         prec_: int = 0 if self.precision is None else self.precision
@@ -215,18 +276,15 @@
         integer_part_str = str(
             self.num_parts.integer_part_int + (1 if plus_1 else 0),
         )
 
         for char in integer_part_str[::-1]:
             counter += 1
             new_chars.append(char)
-            if (
-                    self.digit_group_length > 0
-                    and counter % self.digit_group_length == 0
-            ):
+            if self.digit_group_length > 0 and counter % self.digit_group_length == 0:
                 new_chars.append(self.digit_group_delimiter)
 
         if new_chars[-1] == '-' and new_chars[-2] == self.digit_group_delimiter:
             new_chars.pop(-2)
         elif new_chars[-1] == self.digit_group_delimiter:
             new_chars.pop(-1)
 
@@ -259,15 +317,15 @@
         return decimal_part, should_carry_1
 
     def _is_integer(self) -> bool:
         return int(self.num) == self.num
 
     @classmethod
     def _convert_to_num(cls, num: Any) -> numbers.Real:
-        if isinstance(num, (float, int)):
+        if isinstance(num, (float, int, type(None))):
             return num
 
         if isinstance(num, complex):
             raise TypeError('Complex numbers are not supported.')
 
         return float(num)  # it would naturally fail if `num` is not valid
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `readable_number-0.1.0/readable_number.egg-info/PKG-INFO` & `readable_number-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: readable-number
-Version: 0.1.0
+Name: readable_number
+Version: 0.1.1
 Summary: A Python library to print numbers in human readable format
 Home-page: https://github.com/jsh9/readable-number
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # readable-number
 A Python library to print numbers in human readable format
 
 ## 1. Installation
@@ -27,43 +28,78 @@
 This library does not depend on any third-party libraries, so installing it will not break your Python environment.
 
 ## 2. Usage
 
 ```python
 from readable_number import ReadableNumber
 
-# Print digit in groups
+### Print digit in groups
 str(ReadableNumber(-123))  # -123
 str(ReadableNumber(-1234))  # -1,234
 str(ReadableNumber(-123456789))  # -123,456,789
 str(ReadableNumber(-12345.6789))  # -12,345.6789
 str(ReadableNumber(-1.23456e18))  # -1,234,560,000,000,000,000
 
-# Custom grouping (in other locales)
+### Custom grouping (in other locales)
 str(ReadableNumber(-123456789, digit_group_size=4))  # -1,2345,6789
 str(ReadableNumber(-123456789, digit_group_delimiter='|'))  # -123|456|789
 
-# Convert to human-readable shortform (with k, M, B, and T as unit)
+### Convert to human-readable shortform (with k, M, B, and T as unit)
 str(ReadableNumber(12345, use_shortform=True))  # 12k
 str(ReadableNumber(12345, use_shortform=True, precision=1))  # 12.3k
 str(ReadableNumber(12345678, use_shortform=True))  # 12M
 str(ReadableNumber(12345678, use_shortform=True, precision=2))  # 12.35M
 
-# Numbers with small absolute values
+### Numbers with small absolute values
 str(ReadableNumber(0.12345))  # 0.12345
 str(ReadableNumber(0.0000012345))  # 0.0000012345
 str(ReadableNumber(0.12345, precision=None))  # 0.12345
 str(ReadableNumber(0.12345, precision=2))  # 0.12
 str(ReadableNumber(0.12345, precision=20))  # 0.123450000000000
 
-# Digits beyond double-precision limit are discarded
+### Digits beyond double-precision limit are discarded
 str(ReadableNumber(0.12345678901234567890, precision=90))  # 0.123456789012346
 str(ReadableNumber(1.23e-20, precision=90))  # 0.000000000000000
 
-# Print large/small numbers in exponantial notation
+### Print many numbers with the same config
+rn = ReadableNumber(precision=2, digit_group_size=4)
+rn.of(123456789)  # 1,2345,6789
+rn.of(0.123456789)  # 0.12
+rn.of(1e15)  # 1000,0000,0000,0000
+
+### Print large numbers in exponantial notation
 str(ReadableNumber(1234567890, use_exponent_for_large_numbers=True))  # 1.234568e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    precision=2,
+))  # 1.23e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    precision=None,
+))  # 1.23456789e+09
+str(ReadableNumber(
+    1234567890,
+    use_exponent_for_large_numbers=True,
+    large_number_threshold=1e20,  # only show in exp if we exceed this
+    precision=None,
+))  # 1,234,567,890
+
+### Print small numbers in exponential notation
 str(ReadableNumber(0.000000012, use_exponent_for_small_numbers=True))  # 1.200000e-08
+str(ReadableNumber(
+    -0.000000123456,
+    use_exponent_for_small_numbers=True,
+    precision=2,
+))  # -1.23e-07
+str(ReadableNumber(
+    -0.000012345,
+    use_exponent_for_small_numbers=True,
+    precision=None,
+    small_number_threshold=1e-2,
+))  # -1.2345e-05
 ```
 
 ## 3. Full API documentation
 
 Please visit this site: https://readable-number.readthedocs.io/en/stable/
```

### Comparing `readable_number-0.1.0/setup.cfg` & `readable_number-0.1.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [metadata]
 name = readable_number
-version = v0.1.0
+version = v0.1.1
 description = A Python library to print numbers in human readable format
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jsh9/readable-number
 license = MIT
 license_file = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 install_requires = 
-python_requires = >=3.8
+python_requires = >=3.7
 include_package_data = True
 
 [options.packages.find]
 exclude = 
 	tests*
 include = 
 	readable_number
```

### Comparing `readable_number-0.1.0/tests/test_readable_number.py` & `readable_number-0.1.1/tests/test_readable_number.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 comma = ','
 dot = '.'
 space = ' '
 
 long_num = 1.1234567890123456789012345
 
 test_cases = [
+    # fmt: off
+    (1e+500, 'inf', 0, comma, dot, 3, False, False),
+    (1e-500, '0', 0, comma, dot, 3, False, False),
+    # fmt: on
     (12345678, '12345678', 0, comma, dot, 3, False, False),
     (12345678, '12,345,678', 3, comma, dot, 3, False, False),
     (12345678, '12,345,678.0', 3, comma, dot, 1, True, False),
     (12345678, '12,345,678.00', 3, comma, dot, 2, True, False),
     (12345678, '12,345,678.000', 3, comma, dot, 3, True, False),
     (12345678, '1234,5678.000', 4, comma, dot, 3, True, False),
     (12345678, '123 45678.000', 5, space, dot, 3, True, False),
@@ -236,24 +240,28 @@
     (-12, '-12', 3, comma, dot, None, False, False),
     (-123, '-123', 3, comma, dot, None, False, False),
     (-1234, '-1,234', 3, comma, dot, None, False, False),
     (-0, '0', 3, comma, dot, None, False, False),
     (1.234568e-41, '0.000000000000000', 3, comma, dot, None, False, False),
     (1.234568e-41, '0.00', 3, comma, dot, 2, False, False),
     (
+        # fmt: off
         -0.000000000000000000001234e+30,
+        # fmt: on
         '1,234,000,000',
         3,
         comma,
         dot,
         2,
         False,
         False,
     ),
+    # fmt: off
     (-0.000000000000000000001234e+30, '-1.23B', 3, comma, dot, 2, False, True),
+    # fmt: on
 ]
 
 
 @pytest.mark.parametrize(
     'num,expected,grpSize,grpDelim,decSymb,precision,showDec,useShortform',
     test_cases,
 )
@@ -285,58 +293,111 @@
 )
 def test_readableNumber_invalid_input(input_string):
     with pytest.raises(ValueError):
         ReadableNumber(input_string)
 
 
 @pytest.mark.parametrize(
-    'num, expected',
+    'num, expected, threshold, precision',
     [
-        (0, '0'),
-        (0.1, '0.1'),
-        (-0.01, '-0.01'),
-        (1234, '1,234'),
-        (123456, '123,456'),
-        (1234567, '1.234567e+06'),
-        (-1234567, '-1.234567e+06'),
-        (-12345678, '-1.234568e+07'),
-        (-123456789, '-1.234568e+08'),
-        (-123456789123456, '-1.234568e+14'),
-        (-123456789123456789123456789, '-1.234568e+26'),
-        (-1.234567e12, '-1.234567e+12'),
-        (-0.000000000000000000001234e+90, '-1.234000e+69'),
+        (0, '0', 1e6, 6),
+        (0.1, '0.100000', 1e6, 6),
+        (-0.01, '-0.010000', 1e6, 6),
+        (1234, '1,234', 1e6, 6),
+        (123456, '123,456', 1e6, 6),
+        (1234567, '1.234567e+06', 1e6, 6),
+        (-1234567, '-1.234567e+06', 1e6, 6),
+        (-12345678, '-1.234568e+07', 1e6, 6),
+        (-123456789, '-1.234568e+08', 1e6, 6),
+        (-123456789123456, '-1.234568e+14', 1e6, 6),
+        (-123456789123456789123456789, '-1.234568e+26', 1e6, 6),
+        (-1.234567e12, '-1.234567e+12', 1e6, 6),
+        (1234567890, '1,234,567,890', 1e100, 6),
+        # fmt: off
+        (-0.000000000000000000001234e90, '-1.234000e+69', 1e6, 6),
+        (-0.000000000000000000001234e+90, '-1.234000e+69', 1e6, 6),
+        # fmt: on
+        (-1234, '-1.234000e+03', 10, 6),
+        (-1234, '-1.234000e+03', 100, 6),
+        (-1234, '-1.234000e+03', 1000, 6),
+        (-1234, '-1.234000e+03', 1233, 6),
+        (-1234, '-1.234000e+03', 1234, 6),
+        (-1234, '-1,234', 1235, 6),
+        (-1234, '-1.234e+03', 10, None),
+        (-1234, '-1e+03', 10, 0),
+        (-1234, '-1.2e+03', 10, 1),
+        (-1234, '-1.23e+03', 10, 2),
+        (-1234, '-1.234e+03', 10, 3),
+        (-1234, '-1.23400000e+03', 10, 8),
+        (-1234, '-1.234000000000000000000000000000e+03', 10, 30),
+        (0.1, '0.1000', 1e6, 4),
+        (-0.01, '-0.0100', 1e6, 4),
+        (0.1, '0.1', 1e6, None),
+        (-0.01, '-0.01', 1e6, None),
+        # fmt: off
+        (-1.123e+123, '-1.123e+123', 1e6, None),
+        (-1.123e+456, '-inf', 1e6, None),
+        # fmt: on
     ],
 )
-def test_readableNumber_exponent_large_number(num, expected):
+def test_readableNumber_exponent_large_number(num, expected, threshold, precision):
     number = ReadableNumber(
         num=num,
         use_exponent_for_large_numbers=True,
+        large_number_threshold=threshold,
+        precision=precision,
     )
     assert str(number) == expected
 
 
 @pytest.mark.parametrize(
-    'num, expected',
+    'num, expected, threshold, precision',
     [
-        (0, '0'),
-        (0.1, '0.1'),
-        (-0.01, '-0.01'),
-        (123456789, '123,456,789'),
-        (0.00001, '0.00001'),
-        (0.000001, '1.000000e-06'),
-        (-0.0000001, '-1.000000e-07'),
-        (-0.0000000000000000000123, '-1.230000e-20'),
-        (-0.000075e-10, '-7.500000e-15'),
-        (1234567890e-50, '1.234568e-41'),
+        (0, '0', 1e-6, 6),
+        (0.1, '0.100000', 1e-6, 6),
+        (-0.01, '-0.010000', 1e-6, 6),
+        (123456789, '123,456,789', 1e-6, 6),
+        (0.00001, '0.000010', 1e-6, 6),
+        (0.000001, '1.000000e-06', 1e-6, 6),
+        (-0.0000001, '-1.000000e-07', 1e-6, 6),
+        (-0.0000000000000000000123, '-1.230000e-20', 1e-6, 6),
+        (-0.000075e-10, '-7.500000e-15', 1e-6, 6),
+        (1234567890e-50, '1.234568e-41', 1e-6, 6),
+        (-0.000123, '-1.230000e-04', 1e-1, 6),
+        (-0.000123, '-1.230000e-04', 1e-2, 6),
+        (-0.000123, '-1.230000e-04', 1e-3, 6),
+        (-0.000123, '-1.230000e-04', 0.000124, 6),
+        (-0.000123, '-1.230000e-04', 0.000123, 6),
+        (-0.000123, '-0.000123', 0.000122, 6),
+        (-0.000123, '-0.000123', 1e-4, 6),
+        (-0.000123, '-0.000123', 1e-5, 6),
+        (-0.0000000000123, '-0.0000000000123', 1e-20, None),
+        (-0.00012345, '-1e-04', 1e-1, 0),
+        (-0.00012345, '-1.2e-04', 1e-1, 1),
+        (-0.00012345, '-1.23e-04', 1e-1, 2),
+        (-0.00012345, '-1.234e-04', 1e-1, 3),
+        (-0.00012345, '-1.2345e-04', 1e-1, 4),
+        (-0.00012345, '-1.23450e-04', 1e-1, 5),
+        (-0.00012345, '-1.234500e-04', 1e-1, 6),
+        (-0.00012345, '-1.2345000e-04', 1e-1, 7),
+        (-0.00012345, '-1.2345000000e-04', 1e-1, 10),
+        (-0.00012345, '-1.234500000000000e-04', 1e-1, 15),
+        (-0.00012345, '-0.000123450000000', 1e-20, 15),
+        (-0.00012345, '-1.2345e-04', 1e-1, None),
+        (-0.00012345, '-0.00012345', 1e-10, None),
+        (-1.123e-123, '-1.123e-123', 1e6, None),
+        (-1.123e-999, '0', 1e6, None),
     ],
 )
-def test_readableNumber_exponent_small_number(num, expected):
+def test_readableNumber_exponent_small_number(num, expected, threshold, precision):
     number = ReadableNumber(
         num=num,
         use_exponent_for_small_numbers=True,
+        small_number_threshold=threshold,
+        precision=precision,
     )
     assert str(number) == expected
 
 
 @pytest.mark.parametrize(
     'param, val, expected_error',
     [
@@ -358,7 +419,28 @@
         ('use_shortform', 1, TypeError),
     ],
 )
 def test_readableNumber_invalid_params(param, val, expected_error):
     kwarg = {param: val}
     with pytest.raises(expected_error):
         ReadableNumber(1.2345, **kwarg)
+
+
+@pytest.mark.parametrize(
+    'num, options, expected',
+    [
+        (
+            12345678,
+            {'use_exponent_for_large_numbers': True, 'precision': 4},
+            '1.2346e+07',
+        ),
+        (
+            -0.000000123456789,
+            {'use_exponent_for_small_numbers': True, 'precision': None},
+            '-1.23456789e-07',
+        ),
+        (1234567890, {}, '1,234,567,890'),
+    ],
+)
+def test_of_method(num, options, expected):
+    rn = ReadableNumber(**options)
+    assert rn.of(num) == expected
```

