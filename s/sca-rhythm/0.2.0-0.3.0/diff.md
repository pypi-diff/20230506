# Comparing `tmp/sca_rhythm-0.2.0.tar.gz` & `tmp/sca_rhythm-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.2.0.tar", max compression
+gzip compressed data, was "sca_rhythm-0.3.0.tar", max compression
```

## Comparing `sca_rhythm-0.2.0.tar` & `sca_rhythm-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.2.0/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.2.0/README.md
--rw-r--r--   0        0        0      358 2023-05-04 06:00:54.244474 sca_rhythm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    14934 2023-05-04 05:59:20.941469 sca_rhythm-0.2.0/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 sca_rhythm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.3.0/README.md
+-rw-r--r--   0        0        0      358 2023-05-05 23:08:41.312865 sca_rhythm-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    15235 2023-05-05 21:48:43.487039 sca_rhythm-0.3.0/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 sca_rhythm-0.3.0/PKG-INFO
```

### Comparing `sca_rhythm-0.2.0/LICENSE.md` & `sca_rhythm-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.2.0/README.md` & `sca_rhythm-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.2.0/sca_rhythm/__init__.py` & `sca_rhythm-0.3.0/sca_rhythm/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,49 +9,58 @@
 from celery import Task
 
 
 def duplicates(items):
     return list((Counter(items) - Counter(set(items))).keys())
 
 
+class WFNotFound(Exception):
+    pass
+
+
 class Workflow:
-    def __init__(self, celery_app, workflow_id=None, steps=None, name=None):
+    def __init__(self, celery_app, workflow_id=None, steps=None, name=None, project=None):
         self.app = celery_app
         db = self.app.backend.database
         self.wf_col = db.get_collection('workflow_meta')
 
+        assert workflow_id is not None or steps is not None, 'Either workflow_id or steps should not be None'
+
         if workflow_id is not None:
             # load from db
             res = self.wf_col.find_one({'_id': workflow_id})
             if res:
                 self.workflow = res
             else:
-                raise Exception(f'Workflow with id {workflow_id} is not found')
+                raise WFNotFound(f'Workflow with id {workflow_id} is not found')
         elif steps is not None:
             # create workflow object and save to db
             assert len(steps) > 0, 'steps is empty'
             for i, step in enumerate(steps):
                 assert 'name' in step, f'step - {i} does not have "name" key'
                 assert len(step['name']) > 0, f'step - {i} name is empty'
                 assert 'task' in step, f'step - {i} does not have "task" key'
                 # assert step['task'] in self.app.tasks, \
                 #     f'step - {i} Task {step["task"]} is not registered in the celery application'
             names = [step['name'] for step in steps]
             duplicate_names = duplicates(names)
             assert len(duplicate_names) == 0, f'Steps with duplicate names: {duplicate_names}'
 
+            assert name, 'name cannot be empty'
+            assert project, 'project cannot be empty'
             self.workflow = {
                 '_id': str(uuid.uuid4()),
                 'created_at': datetime.datetime.utcnow(),
                 'steps': steps,
-                'name': name
+                'name': name,
+                'project': project
             }
             self.wf_col.insert_one(self.workflow)
         else:
-            raise Exception('Either workflow_id or steps should not be None')
+            pass
 
     def start(self, *args, **kwargs):
         """
         Launches the task of the first step in this workflow.
 
         The task is called with given args and kwargs
         along with additional keyword args "workflow_id" and "step"
@@ -289,15 +298,15 @@
 
     def refresh(self):
         workflow_id = self.workflow['_id']
         res = self.wf_col.find_one({'_id': workflow_id})
         if res:
             self.workflow = res
         else:
-            raise Exception(f'Workflow with id {workflow_id} is not found')
+            raise WFNotFound(f'Workflow with id {workflow_id} is not found')
 
     def get_embellished_workflow(self, last_task_run=True, prev_task_runs=False):
         """
 
         :param last_task_run: include last run task for each step: boolean
         :param prev_task_runs: include previous task runs for each step: boolean
         :return:
@@ -322,14 +331,15 @@
             steps.append(emb_step)
 
         # number of steps done is same of index of the pending step
         # if all steps are complete pending_step_idx is None, then steps_done is len(steps)
         return {
             'id': self.workflow['_id'],
             'name': self.workflow.get('name', None),
+            'project': self.workflow.get('project', None),
             'created_at': self.workflow.get('created_at', None),
             'updated_at': self.workflow.get('updated_at', None),
             'status': status,
             'steps_done': pending_step_idx if pending_step_idx is not None else len(steps),
             'total_steps': len(steps),
             'steps': steps
         }
@@ -363,9 +373,7 @@
     def update_progress(self, progress_obj):
         # called_directly: This flag is set to true if the task was not executed by the worker.
         if not self.request.called_directly:
             print(f'updating progress for {self.name}', progress_obj)
             self.update_state(state='PROGRESS',
                               meta=progress_obj
                               )
-
-
```

### Comparing `sca_rhythm-0.2.0/PKG-INFO` & `sca_rhythm-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.7,<6.0.0)
```

