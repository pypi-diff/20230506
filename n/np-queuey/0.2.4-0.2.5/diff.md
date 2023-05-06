# Comparing `tmp/np_queuey-0.2.4.tar.gz` & `tmp/np_queuey-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.2.4.tar", last modified: Sat May  6 06:53:03 2023, max compression
+gzip compressed data, was "np_queuey-0.2.5.tar", last modified: Sat May  6 07:14:34 2023, max compression
```

## Comparing `np_queuey-0.2.4.tar` & `np_queuey-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.4/README.md
--rw-r--r--   0        0        0     2607 2023-05-06 06:53:03.313737 np_queuey-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.4/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.4/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.4/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.4/src/np_queuey/hueys/qc.py
--rw-r--r--   0        0        0     4118 2023-05-06 06:34:16.154743 np_queuey-0.2.4/src/np_queuey/hueys/sorting.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.4/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.4/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.4/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.4/src/np_queuey/jobs/run_sorting.py
--rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.4/src/np_queuey/jobs/sorting.py
--rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.4/src/np_queuey/queues/__init__.py
--rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.4/src/np_queuey/queues/huey_job_queue.py
--rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.4/src/np_queuey/queues/peewee_job_queue.py
--rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.4/src/np_queuey/queues/pipeline_qc_queue.py
--rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.4/src/np_queuey/queues/pipeline_sorting_queue.py
--rw-r--r--   0        0        0    11399 2023-05-06 05:58:43.541175 np_queuey-0.2.4/src/np_queuey/queues/sqlite_isilon_queue.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.4/src/np_queuey/tasks.py
--rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.4/src/np_queuey/types.py
--rw-r--r--   0        0        0     3568 2023-05-06 04:43:39.240338 np_queuey-0.2.4/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.4/tests/test_huey.py
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 np_queuey-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.5/README.md
+-rw-r--r--   0        0        0     2607 2023-05-06 07:14:34.239599 np_queuey-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.5/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.5/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.5/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.5/src/np_queuey/hueys/qc.py
+-rw-r--r--   0        0        0     4118 2023-05-06 06:34:16.154743 np_queuey-0.2.5/src/np_queuey/hueys/sorting.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.5/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.5/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.5/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.5/src/np_queuey/jobs/run_sorting.py
+-rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.5/src/np_queuey/jobs/sorting.py
+-rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.5/src/np_queuey/queues/__init__.py
+-rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.5/src/np_queuey/queues/huey_job_queue.py
+-rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.5/src/np_queuey/queues/peewee_job_queue.py
+-rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.5/src/np_queuey/queues/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.5/src/np_queuey/queues/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0    11544 2023-05-06 07:13:48.049667 np_queuey-0.2.5/src/np_queuey/queues/sqlite_isilon_queue.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.5/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.5/src/np_queuey/types.py
+-rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.5/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.5/tests/test_huey.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 np_queuey-0.2.5/PKG-INFO
```

### Comparing `np_queuey-0.2.4/pyproject.toml` & `np_queuey-0.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.2.4"
+version = "0.2.5"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "peewee>=3.16.1",
```

### Comparing `np_queuey-0.2.4/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.5/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/hueys/qc.py` & `np_queuey-0.2.5/src/np_queuey/hueys/qc.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/hueys/sorting.py` & `np_queuey-0.2.5/src/np_queuey/hueys/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.5/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/jobs/sorting.py` & `np_queuey-0.2.5/src/np_queuey/jobs/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/queues/huey_job_queue.py` & `np_queuey-0.2.5/src/np_queuey/queues/huey_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/queues/peewee_job_queue.py` & `np_queuey-0.2.5/src/np_queuey/queues/peewee_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/queues/sqlite_isilon_queue.py` & `np_queuey-0.2.5/src/np_queuey/queues/sqlite_isilon_queue.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,19 @@
         
     def next(self) -> JobT | None:
         """
         Get the next job to process.
         Sorted by priority (desc), then date added (asc).
         """
         for job in self:
-            if not self.is_started(job):
+            if (
+                not self.is_started(job) 
+                and not job.finished
+                and not (job.error and job.hostname == np_config.HOSTNAME)
+            ):
                 return job
     
     def set_finished(self, session_or_job: SessionArgs | Job) -> None:
         """Mark a job as finished. May be irreversible, so be sure."""
         self.update(session_or_job, finished=1)
         
     def set_started(self, session_or_job: SessionArgs | Job) -> None:
```

### Comparing `np_queuey-0.2.4/src/np_queuey/types.py` & `np_queuey-0.2.5/src/np_queuey/types.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/src/np_queuey/utils.py` & `np_queuey-0.2.5/src/np_queuey/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     except BaseException as exc:
         if isinstance(exc, Exception):
             queue.set_errored(job, exc)
             logger.exception('Exception during processing %s %s', queue, job.session)
             return
         else: # KeyboardInterrupt, SystemExit etc:
             queue.set_queued(job)
+            logger.debug('Interrupted: job re-queued: %s %s', queue, job.session)
             raise
     else:
         queue.set_finished(job)
         logger.debug('Marked job finished: %s %s', queue, job.session)
 
 if __name__ == '__main__':
     import doctest
```

### Comparing `np_queuey-0.2.4/tests/test_huey.py` & `np_queuey-0.2.5/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.4/PKG-INFO` & `np_queuey-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

