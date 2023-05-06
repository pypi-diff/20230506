# Comparing `tmp/datarec-0.2.0.tar.gz` & `tmp/datarec-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarec-0.2.0.tar", last modified: Mon Apr 24 05:09:41 2023, max compression
+gzip compressed data, was "datarec-0.3.0.tar", last modified: Sat May  6 05:33:00 2023, max compression
```

## Comparing `datarec-0.2.0.tar` & `datarec-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.864588 datarec-0.2.0/
--rw-rw-rw-   0        0        0    35285 2023-04-24 05:09:41.862585 datarec-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    34721 2023-04-24 05:06:54.000000 datarec-0.2.0/README.md
--rw-rw-rw-   0        0        0     1083 2023-04-23 22:56:24.000000 datarec-0.2.0/license
--rw-rw-rw-   0        0        0      666 2023-04-24 05:07:20.000000 datarec-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 05:09:41.865588 datarec-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.770118 datarec-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.791109 datarec-0.2.0/src/datarec/
--rw-rw-rw-   0        0        0      106 2023-04-23 22:56:24.000000 datarec-0.2.0/src/datarec/__init__.py
--rw-rw-rw-   0        0        0     5271 2023-04-24 04:46:53.000000 datarec-0.2.0/src/datarec/data.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.831123 datarec-0.2.0/src/datarec/tables/
--rw-rw-rw-   0        0        0      207 2023-04-23 22:56:24.000000 datarec-0.2.0/src/datarec/tables/__init__.py
--rw-rw-rw-   0        0        0     3467 2023-04-23 22:56:24.000000 datarec-0.2.0/src/datarec/tables/_is_close_numeric.py
--rw-rw-rw-   0        0        0     2449 2023-04-23 22:56:24.000000 datarec-0.2.0/src/datarec/tables/_is_equal.py
--rw-rw-rw-   0        0        0     2474 2023-04-23 22:56:24.000000 datarec-0.2.0/src/datarec/tables/_method_base.py
--rw-rw-rw-   0        0        0     3928 2023-04-23 23:49:47.000000 datarec-0.2.0/src/datarec/tables/_reconciler.py
--rw-rw-rw-   0        0        0     4479 2023-04-23 22:56:25.000000 datarec-0.2.0/src/datarec/tables/_summarizer.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.845583 datarec-0.2.0/src/datarec/utils/
--rw-rw-rw-   0        0        0      150 2023-04-23 22:56:25.000000 datarec-0.2.0/src/datarec/utils/__init__.py
--rw-rw-rw-   0        0        0      333 2023-04-23 22:56:25.000000 datarec-0.2.0/src/datarec/utils/_get_suffixed.py
--rw-rw-rw-   0        0        0      319 2023-04-23 22:56:25.000000 datarec-0.2.0/src/datarec/utils/_set_case.py
--rw-rw-rw-   0        0        0     5821 2023-04-23 22:56:25.000000 datarec-0.2.0/src/datarec/utils/functions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.810119 datarec-0.2.0/src/datarec.egg-info/
--rw-rw-rw-   0        0        0    35285 2023-04-24 05:09:41.000000 datarec-0.2.0/src/datarec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-04-24 05:09:41.000000 datarec-0.2.0/src/datarec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 05:09:41.000000 datarec-0.2.0/src/datarec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 05:09:41.000000 datarec-0.2.0/src/datarec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 05:09:41.000000 datarec-0.2.0/src/datarec.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 05:09:41.857586 datarec-0.2.0/tests/
--rw-rw-rw-   0        0        0     1756 2023-04-24 04:30:46.000000 datarec-0.2.0/tests/test_is_close.py
--rw-rw-rw-   0        0        0     1319 2023-04-24 04:45:32.000000 datarec-0.2.0/tests/test_is_equal.py
--rw-rw-rw-   0        0        0     3565 2023-04-24 04:52:14.000000 datarec-0.2.0/tests/test_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.467098 datarec-0.3.0/
+-rw-rw-rw-   0        0        0    35285 2023-05-06 05:33:00.465094 datarec-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    34721 2023-05-06 04:35:32.000000 datarec-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1083 2023-05-06 04:35:32.000000 datarec-0.3.0/license
+-rw-rw-rw-   0        0        0      666 2023-05-06 05:31:36.000000 datarec-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 05:33:00.468098 datarec-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.371102 datarec-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.397100 datarec-0.3.0/src/datarec/
+-rw-rw-rw-   0        0        0      106 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/__init__.py
+-rw-rw-rw-   0        0        0     5991 2023-05-06 05:30:21.000000 datarec-0.3.0/src/datarec/data.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.438100 datarec-0.3.0/src/datarec/tables/
+-rw-rw-rw-   0        0        0      207 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/__init__.py
+-rw-rw-rw-   0        0        0     3467 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_is_close_numeric.py
+-rw-rw-rw-   0        0        0     2449 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_is_equal.py
+-rw-rw-rw-   0        0        0     2474 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_method_base.py
+-rw-rw-rw-   0        0        0     3928 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/tables/_reconciler.py
+-rw-rw-rw-   0        0        0     4567 2023-05-06 05:21:50.000000 datarec-0.3.0/src/datarec/tables/_summarizer.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.452099 datarec-0.3.0/src/datarec/utils/
+-rw-rw-rw-   0        0        0      150 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/_get_suffixed.py
+-rw-rw-rw-   0        0        0      319 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/_set_case.py
+-rw-rw-rw-   0        0        0     5821 2023-05-06 04:35:32.000000 datarec-0.3.0/src/datarec/utils/functions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.417103 datarec-0.3.0/src/datarec.egg-info/
+-rw-rw-rw-   0        0        0    35285 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 05:33:00.000000 datarec-0.3.0/src/datarec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 05:33:00.462095 datarec-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1756 2023-05-06 04:35:32.000000 datarec-0.3.0/tests/test_is_close.py
+-rw-rw-rw-   0        0        0     1319 2023-05-06 04:35:32.000000 datarec-0.3.0/tests/test_is_equal.py
+-rw-rw-rw-   0        0        0     3585 2023-05-06 05:26:02.000000 datarec-0.3.0/tests/test_summarizer.py
```

### Comparing `datarec-0.2.0/PKG-INFO` & `datarec-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.2.0
+Version: 0.3.0
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.2.0/README.md` & `datarec-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/license` & `datarec-0.3.0/license`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/pyproject.toml` & `datarec-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "datarec"
 description = "utilities for reconciling data"
-version     = "0.2.0"
+version     = "0.3.0"
 readme      = "README.md"
 dependencies = [
   "polars",
 ]
 authors         = [
   { name = "Chris Mamon", email = "chrisam1993@live.com" },
 ]
```

### Comparing `datarec-0.2.0/src/datarec/data.py` & `datarec-0.3.0/src/datarec/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import yaml
+import json
 from pprint import pformat
 from typing import List
 import polars as pl
 from dataclasses import dataclass
 from .utils._set_case import SetCase
 from .utils._get_suffixed import GetSuffixed
 
@@ -28,27 +30,46 @@
         return [c for c in self.results.columns if "**left**" in c.lower()][0]
 
     @property
     def is_right_col(self) -> List[str]:
         return [c for c in self.results.columns if "**right**" in c.lower()][0]
 
     @property
+    def is_intersection_col(self) -> List[str]:
+        return [c for c in self.results.columns if "**both**" in c.lower()][0]
+
+    @property
     def validation_columns(self) -> List[str]:
         return [
             c for c in self.results.columns if "~*validation*~" in c.lower()
         ]
 
     @property
     def left_columns(self) -> List[str]:
         return [c for c in self.results.columns if " ~%s~" % self.left in c]
 
     @property
     def right_columns(self) -> List[str]:
         return [c for c in self.results.columns if " ~%s~" % self.right in c]
 
+    def get_results_union(self) -> pl.LazyFrame:
+        return self.results
+
+    def get_results_left(self) -> pl.LazyFrame:
+        return self.results.filter(pl.col(self.is_left_col))
+
+    def get_results_right(self) -> pl.LazyFrame:
+        return self.results.filter(pl.col(self.is_right_col))
+
+    def get_results_intersection(self) -> pl.LazyFrame:
+        return self.results.filter(pl.col(self.is_intersection_col))
+
+    def get_results_disjoint(self) -> pl.LazyFrame:
+        return self.results.filter(pl.col(self.is_intersection_col).is_not())
+
     def get_rows_left_only(self) -> pl.LazyFrame:
         return (
             self.results.filter(
                 pl.col(self.is_left_col) & pl.col(self.is_right_col).is_not()
             )
             .select(self.columns_indexes + self.left_columns)
             .rename(
@@ -91,15 +112,14 @@
     n_tested_rows: int
     n_tested_cols: int
     n_tested_entries: int
 
     n_tested_entries_passed: int
     n_tested_entries_failed: int
 
-    n_tested_rows: int
     n_tested_rows_passed: int
     n_tested_rows_passed_partially: int
     n_tested_rows_failed: int
 
     validation_ratio_entries: float
     validation_ratio_rows: float
 
@@ -126,27 +146,27 @@
     def flag(self):
         if self.PASS:
             return "PASSED"
         return "FAILED"
 
     def to_dict(self):
         return dict(
-            Totals=dict(
-                n_rows_left=self.n_total_rows_left,
-                n_rows_right=self.n_total_rows_right,
-                n_rows_intersecting=self.n_total_rows_intersecting,
-                n_rows_union=self.n_total_rows_union,
-            ),
             TestedMeta=dict(
-                passed=self.PASS,
                 flag=self.flag,
+                passed=self.PASS,
                 tested_rows=self.n_tested_rows,
                 tested_cols=self.n_tested_cols,
                 tested_entries=self.n_tested_entries,
             ),
+            Totals=dict(
+                n_rows_left=self.n_total_rows_left,
+                n_rows_right=self.n_total_rows_right,
+                n_rows_intersecting=self.n_total_rows_intersecting,
+                n_rows_union=self.n_total_rows_union,
+            ),
             TestedRows=dict(
                 n_tested_rows_passed=self.n_tested_rows_passed,
                 n_tested_rows_passed_partially=self.n_tested_rows_passed_partially,
                 n_tested_rows_failed=self.n_tested_rows_failed,
             ),
             TestedEntries=dict(
                 n_tested_entries_passed=self.n_tested_entries_passed,
```

### Comparing `datarec-0.2.0/src/datarec/tables/_is_close_numeric.py` & `datarec-0.3.0/src/datarec/tables/_is_close_numeric.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/src/datarec/tables/_is_equal.py` & `datarec-0.3.0/src/datarec/tables/_is_equal.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/src/datarec/tables/_method_base.py` & `datarec-0.3.0/src/datarec/tables/_method_base.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/src/datarec/tables/_reconciler.py` & `datarec-0.3.0/src/datarec/tables/_reconciler.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/src/datarec/tables/_summarizer.py` & `datarec-0.3.0/src/datarec/tables/_summarizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,26 +48,26 @@
 
     try:
         row_validation_ratio = n_rows_passed / rows
     except ZeroDivisionError:
         row_validation_ratio = 0
 
     return (
-        rows,
-        cols,
-        n_entries,
-        n_entries_passed,
-        n_entries_failed,
-        n_rows_passed,
-        n_rows_partially_passed,
-        n_rows_failed,
-        entry_validation_ratio,
-        row_validation_ratio,
-        avg_row_invalidations,
-        std_row_invalidations,
+        int(rows),
+        int(cols),
+        int(n_entries),
+        int(n_entries_passed),
+        int(n_entries_failed),
+        int(n_rows_passed),
+        int(n_rows_partially_passed),
+        int(n_rows_failed),
+        float(entry_validation_ratio),
+        float(row_validation_ratio),
+        float(avg_row_invalidations),
+        float(std_row_invalidations),
     )
 
 
 def _get_totals(lf: pl.LazyFrame):
     left_col = [c for c in lf.columns if "**left**" in c.lower()][0]
     right_col = [c for c in lf.columns if "**right**" in c.lower()][0]
     intersecting_col = [c for c in lf.columns if "**both**" in c.lower()][0]
@@ -75,18 +75,18 @@
     n_total_rows_right = lf.select(right_col).collect().to_numpy().sum()
     n_total_rows_intersection = (
         lf.select(intersecting_col).collect().to_numpy().sum()
     )
     n_total_rows_union = len(lf.select(left_col).collect())
 
     return (
-        n_total_rows_left,
-        n_total_rows_right,
-        n_total_rows_intersection,
-        n_total_rows_union,
+        int(n_total_rows_left),
+        int(n_total_rows_right),
+        int(n_total_rows_intersection),
+        int(n_total_rows_union),
     )
 
 
 def _shared_summarize(
     lf: pl.LazyFrame, filter_col: str
 ) -> TableReconciliationData:
     lf_original = lf
```

### Comparing `datarec-0.2.0/src/datarec/utils/functions.py` & `datarec-0.3.0/src/datarec/utils/functions.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/src/datarec.egg-info/PKG-INFO` & `datarec-0.3.0/src/datarec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarec
-Version: 0.2.0
+Version: 0.3.0
 Summary: utilities for reconciling data
 Author-email: Chris Mamon <chrisam1993@live.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `datarec-0.2.0/src/datarec.egg-info/SOURCES.txt` & `datarec-0.3.0/src/datarec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/tests/test_is_close.py` & `datarec-0.3.0/tests/test_is_close.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/tests/test_is_equal.py` & `datarec-0.3.0/tests/test_is_equal.py`

 * *Files identical despite different names*

### Comparing `datarec-0.2.0/tests/test_summarizer.py` & `datarec-0.3.0/tests/test_summarizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,58 +63,58 @@
 validation_no_index = validate_no_index()
 validation_with_index = validate_with_index()
 
 
 class TestSummarization:
     def test_left_no_index(self):
         summary = tables.summarize_reconciliation(validation_no_index, "left")
-        assert summary.validation_ratio_entries == 1, "failed"
+        assert summary.validation_ratio_entries == 0.8563, "failed"
 
     def test_right_no_index(self):
         summary = tables.summarize_reconciliation(validation_no_index, "right")
         assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
+            summary.validation_ratio_entries, 0.8155238095238095
         ), "failed"
 
     def test_inner_no_index(self):
         summary = tables.summarize_reconciliation(validation_no_index, "inner")
-        assert summary.validation_ratio_entries == 1, "failed"
+        assert summary.validation_ratio_entries == 0.8563, "failed"
 
     def test_outer_no_index(self):
         summary = tables.summarize_reconciliation(validation_no_index, "outer")
         assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
+            summary.validation_ratio_entries, 0.8155238095238095
         ), "failed"
 
     def test_left_with_index(self):
         summary = tables.summarize_reconciliation(
             validation_with_index, "left"
         )
-        assert summary.validation_ratio_entries == 1, "failed"
+        assert summary.validation_ratio_entries == 0.8563, "failed"
 
     def test_right_with_index(self):
         summary = tables.summarize_reconciliation(
             validation_with_index, "right"
         )
         assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
+            summary.validation_ratio_entries, 0.8155238095238095
         ), "failed"
 
     def test_inner_with_index(self):
         summary = tables.summarize_reconciliation(
             validation_with_index, "inner"
         )
-        assert summary.validation_ratio_entries == 1, "failed"
+        assert summary.validation_ratio_entries == 0.8563, "failed"
 
     def test_outer_with_index(self):
         summary = tables.summarize_reconciliation(
             validation_with_index, "outer"
         )
         assert np.isclose(
-            summary.validation_ratio_entries, 0.9523809523809523
+            summary.validation_ratio_entries, 0.8155238095238095
         ), "failed"
 
 
 if __name__ == "__main__":
     T = TestSummarization()
     T.test_right_no_index()
     T.test_left_no_index()
```

