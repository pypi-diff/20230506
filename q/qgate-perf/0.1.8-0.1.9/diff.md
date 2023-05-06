# Comparing `tmp/qgate_perf-0.1.8-py3-none-any.whl.zip` & `tmp/qgate_perf-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,18 @@
-Zip file size: 17731 bytes, number of entries: 17
+Zip file size: 16109 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-May-06 11:51 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    11516 b- defN 23-May-06 12:24 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
--rw-rw-rw-  2.0 fat     5424 b- defN 23-May-06 06:01 qgate_perf/parallel_return.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 12:01 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 12:24 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat     3339 b- defN 23-May-06 11:56 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1372 b- defN 23-May-06 12:02 qgate_perf-0.1.8.dist-info/RECORD
-17 files, 53852 bytes uncompressed, 15483 bytes compressed:  71.2%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1286 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/RECORD
+16 files, 48583 bytes uncompressed, 13995 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -12,17 +12,14 @@
 
 Filename: qgate_perf/parallel_executor.py
 Comment: 
 
 Filename: qgate_perf/parallel_probe.py
 Comment: 
 
-Filename: qgate_perf/parallel_return.py
-Comment: 
-
 Filename: qgate_perf/run_return.py
 Comment: 
 
 Filename: qgate_perf/run_setup.py
 Comment: 
 
 Filename: qgate_perf/version.py
@@ -30,23 +27,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.8.dist-info/LICENSE
+Filename: qgate_perf-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.8.dist-info/METADATA
+Filename: qgate_perf-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.8.dist-info/WHEEL
+Filename: qgate_perf-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.8.dist-info/top_level.txt
+Filename: qgate_perf-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.8.dist-info/RECORD
+Filename: qgate_perf-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -8,14 +8,15 @@
 import concurrent.futures
 import json
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
 from qgate_perf.bundle_helper import BundleHelper
 from qgate_perf.executor_helper import ExecutorHelper
 from qgate_perf.parallel_probe import ParallelProbe
+from qgate_perf.run_return import RunReturn
 
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
     def __init__(self, func, label=None, detail_output=True, output_file=None):
         """ Setting of execution
             :param func:            function for parallel run
@@ -24,20 +25,22 @@
             :param output_file:     output to the file, defualt is without file
         """
         self._func = func
         self._detail_output = detail_output
         self._label =label
         self._output_file = output_file
 
+
     def _coreThreadClassPool(self, threads, return_key, return_dict, run_setup: RunSetup):
         with ThreadPoolExecutor(max_workers=threads) as executor:
             features = []
             for threadKey in range(threads):
+                run_return=RunReturn(f"{return_key}x{threadKey}", return_dict)
                 features.append(
-                    executor.submit(self._func, f"{return_key}x{threadKey}", return_dict, run_setup))
+                    executor.submit(self._func, run_return, run_setup))
 
             for future in concurrent.futures.as_completed(features):
                 future.result()
 
     def _coreThreadClass(self, threads, return_key, return_dict, run_setup):
         thrd = []
         for threadKey in range(threads):
@@ -77,30 +80,36 @@
                 features.append(
                     executor.submit(func, f"{return_key}x{thread_key}", return_dict, run_setup))
 
             for future in concurrent.futures.as_completed(features):
                 future.result()
 
     def _executeCore(self, run_setup: RunSetup, return_dict, processes=2, threads=2):
+
+        from qgate_perf.run_return import RunReturn
+
         proc = []
 
         # define synch time for run of all executors
         run_setup.set_start_time()
 
         if threads == 1:
             for process_key in range(processes):
+                run_return=RunReturn(process_key, return_dict)
                 p = Process(target=self._func,
-                            args=(process_key, return_dict, run_setup))
-#                            args=(run_setup))
+                            args=(run_return, run_setup))
+# oldversion                args=(process_key, return_dict, run_setup))
 
                 proc.append(p)
         else:
             for process_key in range(processes):
                 p = Process(target=self._coreThreadClassPool,
-                            args=(threads,process_key, return_dict, run_setup))
+                            args=(threads, process_key, return_dict, run_setup))
+# oldversion    p = Process(target=self._coreThreadClassPool,
+                #                p = Process(target=self._coreThreadClassPool,
                 # p = Process(target=self._coreThreadClass, args=(threads, process_key, return_dict, run_setup))
                 # p = Process(target=ParallelExecutor._coreThread, args=(self.func, threads, process_key, return_dict, run_setup))
                 # p = Process(target=ParallelExecutor._coreThreadPool, args=(self.func, threads, process_key, return_dict, run_setup))
                 proc.append(p)
 
         # start
         for p in proc:
@@ -142,15 +151,14 @@
             parallel_ret = return_dict[return_key]
             if (parallel_ret.counter > 0):
                 sum_time = sum_time + (parallel_ret.total_duration / parallel_ret.counter)
                 sum_deviation += parallel_ret.standard_deviation
                 sum_call += parallel_ret.counter
                 count += 1
             if (self._detail_output == True):
-                #                self._print(file, f"  Order:{return_key} {parallel_ret.ToString()}")
                 self._print(file, f"     {parallel_ret.ToString()}")
 
         if (count > 0):
             out = {
                 FileFormat.PRF_TYPE: FileFormat.PRF_CORE_TYPE,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR_ALL: processes * threads,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR: [processes, threads],
@@ -247,15 +255,14 @@
                 file.close()
 
     def one_shot(self):
         """ Run test, only one shot (execution) of test function """
 
         # setup minimalistic values
         setup = RunSetup(duration_second=0, start_delay=0, parameters=None)
-        setup.set_bulk(1,1)
 
         # run
         self.run(processes=1,
                  threads=1,
                  run_setup=setup)
 
     def test_call(self, run_setup: RunSetup=None):
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.8'
+__version__ = '0.1.9'
```

## Comparing `qgate_perf-0.1.8.dist-info/LICENSE` & `qgate_perf-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.8.dist-info/METADATA` & `qgate_perf-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.8
+Version: 0.1.9
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.1.8.dist-info/RECORD` & `qgate_perf-0.1.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=qJAErF7jPtMB5q7zEdplXQQSCvTmvdh2se-tzlRGlBk,5233
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=8Hx2bOANB2Vl7QEtjKpriEj-OP_rrCqWfsfu9a_h0lI,11275
+qgate_perf/parallel_executor.py,sha256=-hbQD5xxggyLlOAV8k_cqUZWTRdLgR-wsqrIzP5qVJM,11516
 qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
-qgate_perf/parallel_return.py,sha256=juWFud2q6rQDhBQMg4dGGp-_fzIedOSgMmW9RVkn-Pw,5424
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
-qgate_perf/version.py,sha256=rZoJQyfdmYs8ClZAslm2F1Zlc9Gj8yEs_4-rh-vSDN0,215
+qgate_perf/version.py,sha256=OihLCODldCFuoHsiS5g7v9O3WlewbjZKhlshBgY-Rg0,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_run.py,sha256=3AJwuRshkQ7b9jgVFlo82ABVxtoZc3ysB1V_VDP8zDc,3339
-qgate_perf-0.1.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.1.8.dist-info/METADATA,sha256=g7bqa6iGbqb_6lNBfqs6Tk6S6mX6xSJkq35xdYnlegM,6286
-qgate_perf-0.1.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.1.8.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.1.8.dist-info/RECORD,,
+qgate_perf-0.1.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.1.9.dist-info/METADATA,sha256=-ezHwp-s4lmplf3XWRweBc2sk4068dlHOCCK0zCJ-WM,6286
+qgate_perf-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.1.9.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.1.9.dist-info/RECORD,,
```

