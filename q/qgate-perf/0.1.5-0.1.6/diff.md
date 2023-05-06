# Comparing `tmp/qgate_perf-0.1.5-py3-none-any.whl.zip` & `tmp/qgate_perf-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 15391 bytes, number of entries: 15
+Zip file size: 15679 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
--rw-rw-rw-  2.0 fat      373 b- defN 23-May-05 17:10 qgate_perf/bundle_helper.py
--rw-rw-rw-  2.0 fat     4598 b- defN 23-May-05 17:10 qgate_perf/executor_helper.py
+-rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
+-rw-rw-rw-  2.0 fat     5233 b- defN 23-May-06 06:05 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    10991 b- defN 23-May-05 21:01 qgate_perf/parallel_executor.py
--rw-rw-rw-  2.0 fat     5424 b- defN 23-May-05 21:15 qgate_perf/parallel_return.py
--rw-rw-rw-  2.0 fat     1057 b- defN 23-May-05 19:53 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-05 21:17 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat    11072 b- defN 23-May-06 06:12 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat     5424 b- defN 23-May-06 06:01 qgate_perf/parallel_return.py
+-rw-rw-rw-  2.0 fat     1709 b- defN 23-May-06 06:12 qgate_perf/run_setup.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 06:22 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
--rw-rw-rw-  2.0 fat     3356 b- defN 23-May-05 19:57 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-05 21:17 qgate_perf-0.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6286 b- defN 23-May-05 21:17 qgate_perf-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 21:17 qgate_perf-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-05 21:17 qgate_perf-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1207 b- defN 23-May-05 21:17 qgate_perf-0.1.5.dist-info/RECORD
-15 files, 46267 bytes uncompressed, 13399 bytes compressed:  71.0%
+-rw-rw-rw-  2.0 fat     3358 b- defN 23-May-06 06:01 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6286 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1207 b- defN 23-May-06 06:22 qgate_perf-0.1.6.dist-info/RECORD
+15 files, 47692 bytes uncompressed, 13687 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.1.5.dist-info/LICENSE
+Filename: qgate_perf-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.1.5.dist-info/METADATA
+Filename: qgate_perf-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.1.5.dist-info/WHEEL
+Filename: qgate_perf-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.1.5.dist-info/top_level.txt
+Filename: qgate_perf-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.1.5.dist-info/RECORD
+Filename: qgate_perf-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/bundle_helper.py

```diff
@@ -1,9 +1,11 @@
 
 class BundleHelper:
     """ Predefines values for setting of bundle lists with pattern [[rows, columns], ..] """
     def __init__(self):
         pass
 
+    ROW_1_COL_10_100 = [[1, 10], [1, 50], [1, 100]]
+
     ROW_1_10k_COL_10 = [[1, 10], [100, 10], [1000, 10], [10000, 10]]
     ROW_1_10k_COL_50 = [[1, 50], [100, 50], [1000, 50], [10000, 50]]
     ROW_1_10k_COL_100 = [[1, 100], [100, 100], [1000, 100], [10000, 100]]
```

## qgate_perf/executor_helper.py

```diff
@@ -1,14 +1,23 @@
 import math
 
 class ExecutorHelper:
     """ Predefines values for setting of executor lists with pattern [[processes, threads, label], ..] """
     def __init__(self):
         pass
 
+    [[1, 1], [2, 2], [4, 1], [4, 2], [4, 4], [8, 1], [8, 2], [8, 4]]
+    PROCESS_2_8_THREAD_1_4 = [[2, 1, '1x thread'], [4, 1, '1x thread'], [8, 1, '1x thread'],
+                              [2, 2, '2x thread'], [4, 2, '2x thread'], [8, 2, '2x thread'],
+                              [2, 4, '4x thread'], [4, 4, '4x thread'], [8, 4, '4x thread']]
+
+    PROCESS_2_8_THREAD_1_4_SHORT = [[2, 1, '1x thread'], [2, 2, '2x thread'],
+                                                         [4, 2, '2x thread'], [4, 4, '4x thread'],
+                                                                              [8, 4, '4x thread']]
+
     PROCESS_1_8_THREAD_1 = [[1, 1, '1x thread'], [2, 1, '1x thread'], [4, 1, '1x thread'], [8, 1, '1x thread']]
     PROCESS_1_8_THREAD_2 = [[1, 2, '2x thread'], [2, 2, '2x thread'], [4, 2, '2x thread'], [8, 2, '2x thread']]
     PROCESS_1_8_THREAD_4 = [[1, 4, '4x thread'], [2, 4, '4x thread'], [4, 4, '4x thread'], [8, 4, '4x thread']]
     PROCESS_1_8_THREAD_8 = [[1, 8, '8x thread'], [2, 8, '8x thread'], [4, 8, '8x thread'], [8, 8, '8x thread']]
 
     PROCESS_1_16_THREAD_1 = [[1, 1, '1x thread'], [2, 1, '1x thread'], [4, 1, '1x thread'], [8, 1, '1x thread'],
                              [16, 1, '1x thread']]
```

## qgate_perf/parallel_executor.py

```diff
@@ -5,14 +5,16 @@
 import datetime
 import time
 from concurrent.futures import ThreadPoolExecutor
 import concurrent.futures
 import json
 from qgate_perf.file_format import FileFormat
 from qgate_perf.run_setup import RunSetup
+from qgate_perf.bundle_helper import BundleHelper
+from qgate_perf.executor_helper import ExecutorHelper
 
 class ParallelExecutor:
     """ Helper for parallel execution of defined function (via start new process with aim to avoid GIL) """
 
     def __init__(self, func, label=None, detail_output=True, output_file=None):
         """ Setting of execution
             :param func:            function for parallel run
@@ -115,15 +117,15 @@
 
     def _print_header(self, file, run_setup: RunSetup=None):
         self._start_tasks = datetime.datetime.utcnow()
         self._print(file, f"############### {self._start_tasks.isoformat(' ')} ###############")
         out = {
             FileFormat.PRF_TYPE: FileFormat.PRF_HDR_TYPE,
             FileFormat.PRF_HDR_LABEL: self._label if self._label is not None else "Noname",
-            FileFormat.PRF_HDR_BULK: [run_setup.bulk_row, run_setup.bulk_col],
+            FileFormat.PRF_HDR_BULK: [run_setup._bulk_row, run_setup._bulk_col],
             FileFormat.PRF_HDR_AVIALABLE_CPU: multiprocessing.cpu_count(),
             FileFormat.PRF_HDR_NOW: self._start_tasks.isoformat(' ')
         }
         self._print(file, json.dumps(out))
 
     def _print_footer(self, file):
         self._print(file,
@@ -152,23 +154,22 @@
                 FileFormat.PRF_CORE_PLAN_EXECUTOR_ALL: processes * threads,
                 FileFormat.PRF_CORE_PLAN_EXECUTOR: [processes, threads],
                 FileFormat.PRF_CORE_REAL_EXECUTOR: count,
                 FileFormat.PRF_CORE_GROUP: group,
                 FileFormat.PRF_CORE_TOTAL_CALL: sum_call,
                 FileFormat.PRF_CORE_AVRG_TIME: sum_time / count,
                 FileFormat.PRF_CORE_STD_DEVIATION: sum_deviation / count,
-                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count)==0 else (1 / (sum_time / count)) * count * run_setup.bulk_row,
+                FileFormat.PRF_CORE_TOTAL_CALL_PER_SEC: 0 if (sum_time / count)==0 else (1 / (sum_time / count)) * count * run_setup._bulk_row,
                 FileFormat.PRF_CORE_TIME_END: datetime.datetime.utcnow().isoformat(' ')
             }
             self._print(file, f"  {json.dumps(out)}")
 
-
     def run_bulk_executor(self,
-                              bulk_list=[[1, 1], [1, 2]],
-                              executor_list=[[1, 1], [2, 2], [4, 1], [4, 2], [4, 4], [8, 1], [8, 2], [8, 4]],
+                              bulk_list= BundleHelper.ROW_1_COL_10_100,
+                              executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                               run_setup: RunSetup=None,
                               sleep_between_bulks=0):
         """ Run cykle of bulks in cycle of sequences for function execution
         :param bulk_list:           list of bulks for execution in format [[rows, columns], ...]
         :param executor_list:       list of executors for execution in format [[processes, threads], ...]
         :param run_setup:           setup of execution
         :param sleep_between_bulks: sleep between bulks
@@ -177,15 +178,15 @@
             run_setup.set_bulk(bulk[0], bulk[1])
 
             # execute
             self.run_executor(executor_list, run_setup)
             time.sleep(sleep_between_bulks)
             gc.collect()
 
-    def run_executor(self, executor_list=[[1, 1], [2, 2], [4, 1], [4, 2], [4, 4], [8, 1], [8, 2], [8, 4]],
+    def run_executor(self, executor_list= ExecutorHelper.PROCESS_2_8_THREAD_1_4_SHORT,
                          run_setup: RunSetup=None):
         """ Run executor sequencies
             :param executor_list:       list of executors for execution in format [[processes, threads, 'label'], ...]
             :param run_setup:           setup of execution
         """
         file = None
         print('Execution...')
```

## qgate_perf/parallel_return.py

 * *Ordering differences only*

```diff
@@ -29,19 +29,19 @@
 
         if run_setup:
             # init incremental calculation of standard deviation
             self.stddev = self.StandardDeviation(ddof=0)
 
             # wait for other executors
             self._wait_for_others(run_setup.when_start)
+            self.duration_second = run_setup.duration_second
 
             # key part of init timer (import for stop parallel run)
             self.init_time = time.time()
             self.track_time[FileFormat.PRF_DETAIL_TIME_START] = datetime.datetime.utcnow()
-            self.duration_second = run_setup.duration_second
 
     def add_timetrack_only_label(self, label):
         self.track_time.append(label)
 
     def add_time_track(self, label):
         self.track_time.append(f"{label}: {datetime.datetime.now()}")
```

## qgate_perf/run_setup.py

```diff
@@ -2,24 +2,47 @@
 
 class RunSetup:
 
     def __init__(self, duration_second, start_delay: int, parameters: dict={}):
         """ Setup of execution
 
         :param duration_second:     parametrs for duration of atomic execution (it is up to function, if it will reflect the value)
-        :param start_delay:         maximal time for waiting/synchronization, before execution of all executors
+        :param start_delay:         maximal time for waiting/synchronization, before execution of all executors (0 = without synchronization)
         :param parameters:          addition parameters for execution
         """
-        self.duration_second=duration_second
-        self.bulk_row = 1
-        self.bulk_col = 10
-        self.start_delay=start_delay
+        self._duration_second=duration_second
+        self._bulk_row = 1
+        self._bulk_col = 10
+        self._start_delay=start_delay
+        self._when_start=None
 
         # collection of specific keys for project such as project_name, feature_set_name, etc.
-        self.parameters=parameters
+        self._parameters=parameters
+
+    @property
+    def bulk_row(self):
+        return self._bulk_row
+    @property
+    def bulk_col(self):
+        return self._bulk_col
+
+    @property
+    def when_start(self):
+        return self._when_start
+
+    def parameter(self, key: str):
+        """Return key parameter"""
+        if self._parameters:
+            return self._parameters[key]
+        return None
+
+    @property
+    def duration_second(self):
+        return self._duration_second
 
     def set_start_time(self):
-        self.when_start = datetime.datetime.now() + datetime.timedelta(seconds=self.start_delay)
+        """Define unique start time for all executors. The time has to be setup before executor start."""
+        self._when_start = datetime.datetime.now() + datetime.timedelta(seconds=self._start_delay)
 
     def set_bulk(self, bulk_row, bulk_column):
-        self.bulk_row = bulk_row if bulk_row > 0 else 1
-        self.bulk_col = bulk_column if bulk_column > 0 else 1
+        self._bulk_row = bulk_row if bulk_row > 0 else 1
+        self._bulk_col = bulk_column if bulk_column > 0 else 1
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.1.5'
+__version__ = '0.1.6'
```

## tests/test_run.py

```diff
@@ -14,15 +14,15 @@
         performance = ParallelReturn(run_setup)
 
         while (True):
 
             # START - performance measure for specific part of code
             performance.start()
 
-            for r in range(run_setup.bulk_row * run_setup.bulk_col):
+            for r in range(run_setup._bulk_row * run_setup._bulk_col):
                 time.sleep(0)
 
             # STOP - performance measure specific part of code
             if performance.stop():
                 break
 
         # return outputs
```

## Comparing `qgate_perf-0.1.5.dist-info/LICENSE` & `qgate_perf-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.1.5.dist-info/METADATA` & `qgate_perf-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.1.5
+Version: 0.1.6
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.1.5.dist-info/RECORD` & `qgate_perf-0.1.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
-qgate_perf/bundle_helper.py,sha256=UyUGOiAvtjSm4-TKhtz74b3DqLwlnBwy0PVLAU9GcjM,373
-qgate_perf/executor_helper.py,sha256=2SKt_C_hruPAwk1Owf4CmMeKlLnVVcVmxp7fWlA81UA,4598
+qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
+qgate_perf/executor_helper.py,sha256=qJAErF7jPtMB5q7zEdplXQQSCvTmvdh2se-tzlRGlBk,5233
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=BNEZqs1N5mseGwIauGEk_jykOjco1cmI836ft3wkYO4,10991
-qgate_perf/parallel_return.py,sha256=_hpmKYwyaOD3sMK_ikznpEUvnTfYnYqKkAANb2Kt9sU,5424
-qgate_perf/run_setup.py,sha256=_DvO0uhE0MoOaj6y_8jnIH9uTPDqG_Ku_iOlW83hPLg,1057
-qgate_perf/version.py,sha256=x2ibIZ0QvPi3JtXReRS6IJ6RnIQ56cR6XeTs_4R7WOY,215
+qgate_perf/parallel_executor.py,sha256=f2ods8Ju8JinNQvTsa9lZ1DJ88zyRwkFVXOLgD_hIu0,11072
+qgate_perf/parallel_return.py,sha256=juWFud2q6rQDhBQMg4dGGp-_fzIedOSgMmW9RVkn-Pw,5424
+qgate_perf/run_setup.py,sha256=UI1zsuXYZ3zeWcGL7MQuLqWkDjxmXPREdacsGl3r7jk,1709
+qgate_perf/version.py,sha256=3vQojhewunUhBEbe-r29QwJq9xnODPTgvWl4fGfeKl0,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tests/test_run.py,sha256=UAmMv55td1qYT3AJ9FEcNQcMJmFG3RPG4cbYyICmGrw,3356
-qgate_perf-0.1.5.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.1.5.dist-info/METADATA,sha256=yAT5JXc9M2ez71gDHxTBNRPxksR5aiZJ1bW0U-tr6ok,6286
-qgate_perf-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.1.5.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.1.5.dist-info/RECORD,,
+tests/test_run.py,sha256=1IwH3OhRoKkVKYEEeudi7VWOo_8mlYe8u43eet-gTqY,3358
+qgate_perf-0.1.6.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.1.6.dist-info/METADATA,sha256=tAiZ9bpEUgsz_76rNaSWMLOXtpfH_GSobt0aI5sg4jc,6286
+qgate_perf-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.1.6.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.1.6.dist-info/RECORD,,
```

