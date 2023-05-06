# Comparing `tmp/qgate_perf-0.1.7rc1-py3-none-any.whl.zip` & `tmp/qgate_perf-0.1.7rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15705 bytes, number of entries: 15
+Zip file size: 15758 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    11072 b- defN 23-May-06 06:12 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    11277 b- defN 23-May-06 07:32 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5424 b- defN 23-May-06 06:01 qgate_perf/parallel_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      218 b- defN 23-May-06 07:10 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      218 b- defN 23-May-06 07:29 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat     3274 b- defN 23-May-06 06:35 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6289 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1222 b- defN 23-May-06 07:11 qgate_perf-0.1.7rc1.dist-info/RECORD
-15 files, 47625 bytes uncompressed, 13683 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6289 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1222 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/RECORD
+15 files, 47830 bytes uncompressed, 13736 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.7rc1.dist-info/LICENSE
+Filename: qgate_perf-0.1.7rc2.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.7rc1.dist-info/METADATA
+Filename: qgate_perf-0.1.7rc2.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.7rc1.dist-info/WHEEL
+Filename: qgate_perf-0.1.7rc2.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.7rc1.dist-info/top_level.txt
+Filename: qgate_perf-0.1.7rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.7rc1.dist-info/RECORD
+Filename: qgate_perf-0.1.7rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -7,14 +7,15 @@
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
 import json
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.bundle_helper import BundleHelper
 from qgate_perf.executor_helper import ExecutorHelper
+from qgate_perf.parallel_return import ParallelReturn
 
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
     def __init__(self, func, label=None, detail_output=True, output_file=None):
         """ Setting of execution
             :param func:            function for parallel run
@@ -256,13 +257,21 @@
         self.run(processes=1,
                  threads=1,
                  run_setup=setup)
 
     def test_call(self, run_setup: RunSetup=None):
         """ Test call without parallel execution"""
 
-        key="no-parallel"
+        # init
+        key="test-no-parallel"
         dictionary={key: ""}
         run_setup.set_start_time()
+
+        # test call
         self._func(key, dictionary, run_setup)
 
+        # show output
+        ret=dictionary[key]
+        if ret:
+            print(ret.ToString())
+
     #TODO: create dir, if not exist
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.7rc1'
+__version__ = '0.1.7rc2'
```

## Comparing `qgate_perf-0.1.7rc1.dist-info/LICENSE` & `qgate_perf-0.1.7rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.7rc1.dist-info/METADATA` & `qgate_perf-0.1.7rc2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.7rc1
+Version: 0.1.7rc2
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.1.7rc1.dist-info/RECORD` & `qgate_perf-0.1.7rc2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=qJAErF7jPtMB5q7zEdplXQQSCvTmvdh2se-tzlRGlBk,5233
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=f2ods8Ju8JinNQvTsa9lZ1DJ88zyRwkFVXOLgD_hIu0,11072
+qgate_perf/parallel_executor.py,sha256=yhC3npsXNtfMRaQeiuiF3MFIz2-2YwivQB-mQUTyy3Y,11277
 qgate_perf/parallel_return.py,sha256=juWFud2q6rQDhBQMg4dGGp-_fzIedOSgMmW9RVkn-Pw,5424
 qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
-qgate_perf/version.py,sha256=vHD1krvDQh-II0yBgYUagVygpIq0JEDydARUg3Yhfwo,218
+qgate_perf/version.py,sha256=CL_zWZGYO_rMwlOPBg1M0h2yCZnineG20GvCK-rXYKQ,218
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_run.py,sha256=_sfjKemZx1ShKtKmlCL1CWT80uZpFKnXoK9EMhNLLi0,3274
-qgate_perf-0.1.7rc1.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.1.7rc1.dist-info/METADATA,sha256=A4pmzAk5BYD3xpCCZfBap7P5PctbMUgSfIeKV0WPSn4,6289
-qgate_perf-0.1.7rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.1.7rc1.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.1.7rc1.dist-info/RECORD,,
+qgate_perf-0.1.7rc2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.1.7rc2.dist-info/METADATA,sha256=yyRxGfetF6Uqgx_cpg1orhVEoGT2knU87iMrXj3DWKc,6289
+qgate_perf-0.1.7rc2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.1.7rc2.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.1.7rc2.dist-info/RECORD,,
```

