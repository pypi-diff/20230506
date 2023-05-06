# Comparing `tmp/qgate_perf-0.1.6-py3-none-any.whl.zip` & `tmp/qgate_perf-0.1.7rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15679 bytes, number of entries: 15
+Zip file size: 15705 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
 -rw-rw-rw-  2.0 fat    11072 b- defN 23-May-06 06:12 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5424 b- defN 23-May-06 06:01 qgate_perf/parallel_return.py
--rw-rw-rw-  2.0 fat     1709 b- defN 23-May-06 06:12 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 06:22 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
+-rw-rw-rw-  2.0 fat      218 b- defN 23-May-06 07:10 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
--rw-rw-rw-  2.0 fat     3358 b- defN 23-May-06 06:01 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1207 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/RECORD
-15 files, 47692 bytes uncompressed, 13687 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat     3274 b- defN 23-May-06 06:35 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6289 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1222 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/RECORD
+15 files, 47625 bytes uncompressed, 13683 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.6.dist-info/LICENSE
+Filename: qgate_perf-0.1.7rc1.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.6.dist-info/METADATA
+Filename: qgate_perf-0.1.7rc1.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.6.dist-info/WHEEL
+Filename: qgate_perf-0.1.7rc1.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.6.dist-info/top_level.txt
+Filename: qgate_perf-0.1.7rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.6.dist-info/RECORD
+Filename: qgate_perf-0.1.7rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/run_setup.py

```diff
@@ -25,15 +25,15 @@
     def bulk_col(self):
         return self._bulk_col
 
     @property
     def when_start(self):
         return self._when_start
 
-    def parameter(self, key: str):
+    def param(self, key: str):
         """Return key parameter"""
         if self._parameters:
             return self._parameters[key]
         return None
 
     @property
     def duration_second(self):
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.6'
+__version__ = '0.1.7rc1'
```

## tests/test_run.py

```diff
@@ -14,29 +14,27 @@
         performance = ParallelReturn(run_setup)
 
         while (True):
 
             # START - performance measure for specific part of code
             performance.start()
 
-            for r in range(run_setup._bulk_row * run_setup._bulk_col):
+            for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
 
             # STOP - performance measure specific part of code
             if performance.stop():
                 break
 
         # return outputs
-        if return_dict is not None:
-            return_dict[return_key] = performance
+        return_dict[return_key] = performance
 
     except Exception as ex:
         # return outputs in case of error
-        if return_dict is not None:
-            return_dict[return_key] = ParallelReturn(None, ex)
+        return_dict[return_key] = ParallelReturn(None, ex)
 
 class TestCaseRun(unittest.TestCase):
 
     def setUp(self):
         pass
 
     def tearDown(self):
```

## Comparing `qgate_perf-0.1.6.dist-info/LICENSE` & `qgate_perf-0.1.7rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.6.dist-info/METADATA` & `qgate_perf-0.1.7rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.6
+Version: 0.1.7rc1
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.1.6.dist-info/RECORD` & `qgate_perf-0.1.7rc1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=qJAErF7jPtMB5q7zEdplXQQSCvTmvdh2se-tzlRGlBk,5233
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
 qgate_perf/parallel_executor.py,sha256=f2ods8Ju8JinNQvTsa9lZ1DJ88zyRwkFVXOLgD_hIu0,11072
 qgate_perf/parallel_return.py,sha256=juWFud2q6rQDhBQMg4dGGp-_fzIedOSgMmW9RVkn-Pw,5424
-qgate_perf/run_setup.py,sha256=UI1zsuXYZ3zeWcGL7MQuLqWkDjxmXPREdacsGl3r7jk,1709
-qgate_perf/version.py,sha256=3vQojhewunUhBEbe-r29QwJq9xnODPTgvWl4fGfeKl0,215
+qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
+qgate_perf/version.py,sha256=vHD1krvDQh-II0yBgYUagVygpIq0JEDydARUg3Yhfwo,218
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_run.py,sha256=1IwH3OhRoKkVKYEEeudi7VWOo_8mlYe8u43eet-gTqY,3358
-qgate_perf-0.1.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.1.6.dist-info/METADATA,sha256=tAiZ9bpEUgsz_76rNaSWMLOXtpfH_GSobt0aI5sg4jc,6286
-qgate_perf-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.1.6.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.1.6.dist-info/RECORD,,
+tests/test_run.py,sha256=_sfjKemZx1ShKtKmlCL1CWT80uZpFKnXoK9EMhNLLi0,3274
+qgate_perf-0.1.7rc1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.1.7rc1.dist-info/METADATA,sha256=A4pmzAk5BYD3xpCCZfBap7P5PctbMUgSfIeKV0WPSn4,6289
+qgate_perf-0.1.7rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.1.7rc1.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.1.7rc1.dist-info/RECORD,,
```

