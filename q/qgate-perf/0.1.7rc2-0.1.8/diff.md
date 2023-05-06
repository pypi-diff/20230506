# Comparing `tmp/qgate_perf-0.1.7rc2-py3-none-any.whl.zip` & `tmp/qgate_perf-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,19 @@
-Zip file size: 15758 bytes, number of entries: 15
+Zip file size: 17731 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    11277 b- defN 23-May-06 07:32 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-May-06 11:51 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat     5424 b- defN 23-May-06 06:01 qgate_perf/parallel_return.py
+-rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      218 b- defN 23-May-06 07:29 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 12:01 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
--rw-rw-rw-  2.0 fat     3274 b- defN 23-May-06 06:35 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6289 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1222 b- defN 23-May-06 07:32 qgate_perf-0.1.7rc2.dist-info/RECORD
-15 files, 47830 bytes uncompressed, 13736 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat     3339 b- defN 23-May-06 11:56 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1372 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/RECORD
+17 files, 53852 bytes uncompressed, 15483 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -9,38 +9,44 @@
 
 Filename: qgate_perf/file_format.py
 Comment: 
 
 Filename: qgate_perf/parallel_executor.py
 Comment: 
 
+Filename: qgate_perf/parallel_probe.py
+Comment: 
+
 Filename: qgate_perf/parallel_return.py
 Comment: 
 
+Filename: qgate_perf/run_return.py
+Comment: 
+
 Filename: qgate_perf/run_setup.py
 Comment: 
 
 Filename: qgate_perf/version.py
 Comment: 
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.7rc2.dist-info/LICENSE
+Filename: qgate_perf-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.7rc2.dist-info/METADATA
+Filename: qgate_perf-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.7rc2.dist-info/WHEEL
+Filename: qgate_perf-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.7rc2.dist-info/top_level.txt
+Filename: qgate_perf-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.7rc2.dist-info/RECORD
+Filename: qgate_perf-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -7,15 +7,15 @@
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
 import json
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.bundle_helper import BundleHelper
 from qgate_perf.executor_helper import ExecutorHelper
-from qgate_perf.parallel_return import ParallelReturn
+from qgate_perf.parallel_probe import ParallelProbe
 
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
     def __init__(self, func, label=None, detail_output=True, output_file=None):
         """ Setting of execution
             :param func:            function for parallel run
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.7rc2'
+__version__ = '0.1.8'
```

## tests/test_run.py

```diff
@@ -1,40 +1,42 @@
 import unittest
 import logging
 from qgate_perf.parallel_executor import ParallelExecutor
-from qgate_perf.parallel_return import ParallelReturn
+from qgate_perf.parallel_probe import ParallelProbe
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.executor_helper import ExecutorHelper
+from qgate_perf.run_return import RunReturn
 import time
 
 
-def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+#def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+def prf_GIL_impact(run_return: RunReturn, run_setup: RunSetup):
     """ Function for performance testing"""
     try:
         # init (contain executor synchonization, if needed)
-        performance = ParallelReturn(run_setup)
+        probe = ParallelProbe(run_setup)
 
         while (True):
 
             # START - performance measure for specific part of code
-            performance.start()
+            probe.start()
 
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
 
             # STOP - performance measure specific part of code
-            if performance.stop():
+            if probe.stop():
                 break
 
         # return outputs
-        return_dict[return_key] = performance
+        run_return.probe=probe
 
     except Exception as ex:
         # return outputs in case of error
-        return_dict[return_key] = ParallelReturn(None, ex)
+        run_return.probe=ParallelProbe(None, ex)
 
 class TestCaseRun(unittest.TestCase):
 
     def setUp(self):
         pass
 
     def tearDown(self):
```

## Comparing `qgate_perf-0.1.7rc2.dist-info/LICENSE` & `qgate_perf-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.7rc2.dist-info/METADATA` & `qgate_perf-0.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.7rc2
+Version: 0.1.8
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

