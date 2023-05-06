# Comparing `tmp/qgate_perf-0.1.9-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 16109 bytes, number of entries: 16
+Zip file size: 16071 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
--rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
+-rw-rw-rw-  2.0 fat     5165 b- defN 23-May-06 14:38 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
 -rw-rw-rw-  2.0 fat    11516 b- defN 23-May-06 12:24 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 12:24 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 15:04 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat     3339 b- defN 23-May-06 11:56 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1286 b- defN 23-May-06 12:28 qgate_perf-0.1.9.dist-info/RECORD
-16 files, 48583 bytes uncompressed, 13995 bytes compressed:  71.2%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 15:05 qgate_perf-0.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6235 b- defN 23-May-06 15:05 qgate_perf-0.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 15:05 qgate_perf-0.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 15:05 qgate_perf-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1286 b- defN 23-May-06 15:05 qgate_perf-0.2.0.dist-info/RECORD
+16 files, 48464 bytes uncompressed, 13957 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.9.dist-info/LICENSE
+Filename: qgate_perf-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.9.dist-info/METADATA
+Filename: qgate_perf-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.9.dist-info/WHEEL
+Filename: qgate_perf-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.9.dist-info/top_level.txt
+Filename: qgate_perf-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.9.dist-info/RECORD
+Filename: qgate_perf-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/executor_helper.py

```diff
@@ -1,15 +1,12 @@
 import math
 
 class ExecutorHelper:
     """ Predefines values for setting of executor lists with pattern [[processes, threads, label], ..] """
-    def __init__(self):
-        pass
 
-    [[1, 1], [2, 2], [4, 1], [4, 2], [4, 4], [8, 1], [8, 2], [8, 4]]
     PROCESS_2_8_THREAD_1_4 = [[2, 1, '1x thread'], [4, 1, '1x thread'], [8, 1, '1x thread'],
                               [2, 2, '2x thread'], [4, 2, '2x thread'], [8, 2, '2x thread'],
                               [2, 4, '4x thread'], [4, 4, '4x thread'], [8, 4, '4x thread']]
 
     PROCESS_2_8_THREAD_1_4_SHORT = [[2, 1, '1x thread'], [2, 2, '2x thread'],
                                                          [4, 2, '2x thread'], [4, 4, '4x thread'],
                                                                               [8, 4, '4x thread']]
@@ -51,14 +48,17 @@
     PROCESS_1_128_THREAD_2 = [[1, 2, '2x thread'], [2, 2, '2x thread'], [4, 2, '2x thread'], [8, 2, '2x thread'],
                               [16, 2, '2x thread'], [32, 2, '2x thread'], [64, 2, '2x thread'], [128, 2, '2x thread']]
     PROCESS_1_128_THREAD_4 = [[1, 4, '4x thread'], [2, 4, '4x thread'], [4, 4, '4x thread'], [8, 4, '4x thread'],
                               [16, 4, '4x thread'], [32, 4, '4x thread'], [64, 4, '4x thread'], [128, 4, '4x thread']]
     PROCESS_1_128_THREAD_8 = [[1, 8, '8x thread'], [2, 8, '8x thread'], [4, 8, '8x thread'], [8, 8, '8x thread'],
                               [16, 8, '8x thread'], [32, 8, '8x thread'], [64, 8, '8x thread'], [128, 8, '8x thread']]
 
+    def __init__(self):
+        pass
+
     def ThreadGrow(label_thread=True, process=2, thread_pow_start=1, thread_pow_stop=6):
         pattern = []
         for i in range(thread_pow_start, thread_pow_stop):
             added = int(math.pow(2, i))
             label = f"{added}x thread" if label_thread else f"{process}x process"
             pattern.append([process, added, label])
         return pattern
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.9'
+__version__ = '0.2.0'
```

## Comparing `qgate_perf-0.1.9.dist-info/LICENSE` & `qgate_perf-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.9.dist-info/METADATA` & `qgate_perf-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.9
+Version: 0.2.0
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
@@ -17,54 +17,55 @@
 
 Performance test generator part of Quality Gate.
 
 ## Usage
 
 ```lang-python
 from qgate_perf.parallel_executor import ParallelExecutor
-from qgate_perf.parallel_return import ParallelReturn
+from qgate_perf.parallel_probe import ParallelProbe
 from qgate_perf.run_setup import RunSetup
+from qgate_perf.run_return import RunReturn
 import time
 
-def prf_GIL_impact(return_key, return_dict, run_setup: RunSetup):
+def prf_GIL_impact(run_return: RunReturn, run_setup: RunSetup):
     """ Function for performance testing"""
     try:
         # INIT - contain executor synchonization, if needed
-        performance = ParallelReturn(run_setup)
+        probe=ParallelProbe(run_setup)
 
         while (True):
 
-            # START - performance test, only for this specific code part
-            performance.start()
-            
+            # START - probe, only for this specific code part
+            probe.start()
+
             for r in range(run_setup.bulk_row * run_setup.bulk_col):
                 time.sleep(0)
-            
-            # STOP - performance test
-            if performance.stop():
+
+            # STOP - probe
+            if probe.stop():
                 break
 
-        # RETURN - data from performance
-        return_dict[return_key] = performance
-        
+        # RETURN - data from probe
+        run_return.probe=probe
+
     except Exception as ex:
         # RETURN - error
-        return_dict[return_key] = ParallelReturn(None, ex)
+        run_return.probe=ParallelProbe(None, ex)
 
 generator = ParallelExecutor(prf_GIL_impact,
                              label="GIL_impact",
                              detail_output=True,
                              output_file="prf_gil_impact_01.txt")
 
 generator.run_bulk_executor(bulk_list=[[1, 1]],
                             executor_list=[[16, 1, '1x thread'], [8, 2, '2x threads'],[4, 4,'4x threads']],
                             run_setup=RunSetup(duration_second=20,start_delay=0))
 ```
 
-# Outputs in text file
+# Outputs in text file 
 ```
 ############### 2023-05-05 06:30:36.194849 ###############
 {"type": "headr", "label": "GIL_impact", "bulk": [1, 1], "available_cpu": 12, "now": "2023-05-05 06:30:36.194849"}
   {"type": "core", "plan_executors": 4, "plan_executors_detail": [4, 1], "real_executors": 4, "group": "1x thread", "total_calls": 7590439, "avrg_time": 1.4127372338382197e-06, "std_deviation": 3.699171006877347e-05, "total_call_per_sec": 2831382.8673804617, "endexec": "2023-05-05 06:30:44.544829"}
   {"type": "core", "plan_executors": 8, "plan_executors_detail": [8, 1], "real_executors": 8, "group": "1x thread", "total_calls": 11081697, "avrg_time": 1.789265660825848e-06, "std_deviation": 4.164309967620533e-05, "total_call_per_sec": 4471107.994274894, "endexec": "2023-05-05 06:30:52.623666"}
   {"type": "core", "plan_executors": 16, "plan_executors_detail": [16, 1], "real_executors": 16, "group": "1x thread", "total_calls": 8677305, "avrg_time": 6.2560950624827455e-06, "std_deviation": 8.629422798757681e-05, "total_call_per_sec": 2557505.8946835063, "endexec": "2023-05-05 06:31:02.875799"}
   {"type": "core", "plan_executors": 8, "plan_executors_detail": [4, 2], "real_executors": 8, "group": "2x threads", "total_calls": 2761851, "avrg_time": 1.1906723084757647e-05, "std_deviation": 0.00010741937495211329, "total_call_per_sec": 671889.3135459893, "endexec": "2023-05-05 06:31:10.283786"}
@@ -81,12 +82,12 @@
      {"type": "detail", "processid": 8944, "calls": 1855611, "total": 2.5979537963867188, "avrg": 1.4000530264084008e-06, "min": 0.0, "max": 0.001207590103149414, "st-dev": 3.6889275786419565e-05, "initexec": "2023-05-05 07:01:21.466496", "startexec": "2023-05-05 07:01:21.466496", "endexec": "2023-05-05 07:01:26.466551"}
      {"type": "detail", "processid": 2108, "calls": 1943549, "total": 2.6283881664276123, "avrg": 1.3523652691172758e-06, "min": 0.0, "max": 0.0012514591217041016, "st-dev": 3.624462003401045e-05, "initexec": "2023-05-05 07:01:21.709203", "startexec": "2023-05-05 07:01:21.709203", "endexec": "2023-05-05 07:01:26.709298"}
      {"type": "detail", "processid": 19292, "calls": 1973664, "total": 2.6392557621002197, "avrg": 1.3372366127670262e-06, "min": 0.0, "max": 0.0041027069091796875, "st-dev": 3.620965943471147e-05, "initexec": "2023-05-05 07:01:21.840541", "startexec": "2023-05-05 07:01:21.840541", "endexec": "2023-05-05 07:01:26.841266"}
   {"type": "core", "plan_executors": 4, "plan_executors_detail": [4, 1], "real_executors": 4, "group": "1x thread", "total_calls": 7669236, "avrg_time": 1.3652863336090071e-06, "std_deviation": 3.645805510967187e-05, "total_call_per_sec": 2929788.3539391863, "endexec": "2023-05-05 07:01:26.891144"}
   ...
 ```
 
-# Next outputs generated from addition package qgate-graph
+# Graphs generated from qgate-graph based on text files from qgate-perf
 
 ![graph](https://fivekg.onrender.com/images/qgate/PRF-NoSQL_igz_nonprod-2023-04-23_14-41-18-bulk-100x50.png)
 ![graph](https://fivekg.onrender.com/images/qgate/EXE-NoSQL-2023-05-04_19-33-30-bulk-1x50-plan-8x2.png)
```

## Comparing `qgate_perf-0.1.9.dist-info/RECORD` & `qgate_perf-0.2.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
-qgate_perf/executor_helper.py,sha256=qJAErF7jPtMB5q7zEdplXQQSCvTmvdh2se-tzlRGlBk,5233
+qgate_perf/executor_helper.py,sha256=XtXNYJDUlrSk4MvQCQ4P6KSddJ-9jUQ8RNExKcFDV0U,5165
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
 qgate_perf/parallel_executor.py,sha256=-hbQD5xxggyLlOAV8k_cqUZWTRdLgR-wsqrIzP5qVJM,11516
 qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
 qgate_perf/run_setup.py,sha256=K06V_dsmOJnNQp7Mn1R8PXWIrYIhTn7IWnKnxyVeykc,1705
-qgate_perf/version.py,sha256=OihLCODldCFuoHsiS5g7v9O3WlewbjZKhlshBgY-Rg0,215
+qgate_perf/version.py,sha256=gMq86yppfPqRZlHkFy4T5klenrTd2zCVR9QEcqnv4V4,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_run.py,sha256=3AJwuRshkQ7b9jgVFlo82ABVxtoZc3ysB1V_VDP8zDc,3339
-qgate_perf-0.1.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.1.9.dist-info/METADATA,sha256=-ezHwp-s4lmplf3XWRweBc2sk4068dlHOCCK0zCJ-WM,6286
-qgate_perf-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.1.9.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.1.9.dist-info/RECORD,,
+qgate_perf-0.2.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.2.0.dist-info/METADATA,sha256=-kamKmUKX6Rpu0c8sUMiLkXWEgL5NxynK9W3vBWVQ1U,6235
+qgate_perf-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.2.0.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.2.0.dist-info/RECORD,,
```

