# Comparing `tmp/np_queuey-0.2.5.tar.gz` & `tmp/np_queuey-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.2.5.tar", last modified: Sat May  6 07:14:34 2023, max compression
+gzip compressed data, was "np_queuey-0.2.6.tar", last modified: Sat May  6 07:26:53 2023, max compression
```

## Comparing `np_queuey-0.2.5.tar` & `np_queuey-0.2.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.5/README.md
--rw-r--r--   0        0        0     2607 2023-05-06 07:14:34.239599 np_queuey-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.5/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.5/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.5/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.5/src/np_queuey/hueys/qc.py
--rw-r--r--   0        0        0     4118 2023-05-06 06:34:16.154743 np_queuey-0.2.5/src/np_queuey/hueys/sorting.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.5/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.5/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.5/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.5/src/np_queuey/jobs/run_sorting.py
--rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.5/src/np_queuey/jobs/sorting.py
--rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.5/src/np_queuey/queues/__init__.py
--rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.5/src/np_queuey/queues/huey_job_queue.py
--rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.5/src/np_queuey/queues/peewee_job_queue.py
--rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.5/src/np_queuey/queues/pipeline_qc_queue.py
--rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.5/src/np_queuey/queues/pipeline_sorting_queue.py
--rw-r--r--   0        0        0    11544 2023-05-06 07:13:48.049667 np_queuey-0.2.5/src/np_queuey/queues/sqlite_isilon_queue.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.5/src/np_queuey/tasks.py
--rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.5/src/np_queuey/types.py
--rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.5/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.5/tests/test_huey.py
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 np_queuey-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-19 04:15:23.193498 np_queuey-0.2.6/README.md
+-rw-r--r--   0        0        0     2607 2023-05-06 07:26:53.877390 np_queuey-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 20:01:03.151595 np_queuey-0.2.6/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.6/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     9098 2023-04-25 20:53:23.800594 np_queuey-0.2.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0     1646 2023-05-06 05:36:41.042949 np_queuey-0.2.6/src/np_queuey/hueys/qc.py
+-rw-r--r--   0        0        0     4118 2023-05-06 06:34:16.154743 np_queuey-0.2.6/src/np_queuey/hueys/sorting.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.2.6/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6934 2023-04-24 19:51:13.132332 np_queuey-0.2.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.2.6/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0      224 2023-04-23 17:09:38.569310 np_queuey-0.2.6/src/np_queuey/jobs/run_sorting.py
+-rw-r--r--   0        0        0     1710 2023-05-05 19:56:33.188797 np_queuey-0.2.6/src/np_queuey/jobs/sorting.py
+-rw-r--r--   0        0        0      318 2023-05-06 03:57:55.539505 np_queuey-0.2.6/src/np_queuey/queues/__init__.py
+-rw-r--r--   0        0        0     3167 2023-05-05 20:05:28.178905 np_queuey-0.2.6/src/np_queuey/queues/huey_job_queue.py
+-rw-r--r--   0        0        0    10101 2023-05-06 01:49:49.463859 np_queuey-0.2.6/src/np_queuey/queues/peewee_job_queue.py
+-rw-r--r--   0        0        0      174 2023-05-06 03:43:50.132826 np_queuey-0.2.6/src/np_queuey/queues/pipeline_qc_queue.py
+-rw-r--r--   0        0        0      445 2023-05-06 06:51:03.263483 np_queuey-0.2.6/src/np_queuey/queues/pipeline_sorting_queue.py
+-rw-r--r--   0        0        0    11528 2023-05-06 07:23:22.330815 np_queuey-0.2.6/src/np_queuey/queues/sqlite_isilon_queue.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.2.6/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0     4952 2023-05-06 04:42:59.665481 np_queuey-0.2.6/src/np_queuey/types.py
+-rw-r--r--   0        0        0     3651 2023-05-06 07:05:03.336745 np_queuey-0.2.6/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-19 04:15:23.204497 np_queuey-0.2.6/tests/test_huey.py
+-rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 np_queuey-0.2.6/PKG-INFO
```

### Comparing `np_queuey-0.2.5/pyproject.toml` & `np_queuey-0.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.2.5"
+version = "0.2.6"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "peewee>=3.16.1",
```

### Comparing `np_queuey-0.2.5/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/hueys/qc.py` & `np_queuey-0.2.6/src/np_queuey/hueys/qc.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/hueys/sorting.py` & `np_queuey-0.2.6/src/np_queuey/hueys/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.2.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/jobs/sorting.py` & `np_queuey-0.2.6/src/np_queuey/jobs/sorting.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/queues/huey_job_queue.py` & `np_queuey-0.2.6/src/np_queuey/queues/huey_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/queues/peewee_job_queue.py` & `np_queuey-0.2.6/src/np_queuey/queues/peewee_job_queue.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/queues/sqlite_isilon_queue.py` & `np_queuey-0.2.6/src/np_queuey/queues/sqlite_isilon_queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,18 +282,19 @@
         self.update(session_or_job, started=None, hostname=None, finished=None, errored=None)
     
     def set_errored(self, session_or_job: SessionArgs | Job, error: str | Exception) -> None:
         self.update(session_or_job, error=str(error))
     
     def is_started(self, session_or_job: SessionArgs | Job) -> bool:
         """Whether the job has started processing, but not yet finished."""
+        job = self[session_or_job]
         return (
-            self[session_or_job].started
-            and not self[session_or_job].finished
-            and not self[session_or_job].error
+            job.started
+            and not job.finished
+            and not job.error
         )
 
 
 
 if __name__ == '__main__':
     import doctest
```

### Comparing `np_queuey-0.2.5/src/np_queuey/types.py` & `np_queuey-0.2.6/src/np_queuey/types.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/src/np_queuey/utils.py` & `np_queuey-0.2.6/src/np_queuey/utils.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/tests/test_huey.py` & `np_queuey-0.2.6/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.2.5/PKG-INFO` & `np_queuey-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.2.5
+Version: 0.2.6
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

