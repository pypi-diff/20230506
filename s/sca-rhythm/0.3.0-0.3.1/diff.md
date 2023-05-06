# Comparing `tmp/sca_rhythm-0.3.0.tar.gz` & `tmp/sca_rhythm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.3.0.tar", max compression
+gzip compressed data, was "sca_rhythm-0.3.1.tar", max compression
```

## Comparing `sca_rhythm-0.3.0.tar` & `sca_rhythm-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.3.0/README.md
--rw-r--r--   0        0        0      358 2023-05-05 23:08:41.312865 sca_rhythm-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    15235 2023-05-05 21:48:43.487039 sca_rhythm-0.3.0/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 sca_rhythm-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.3.1/README.md
+-rw-r--r--   0        0        0      358 2023-05-06 00:00:30.340969 sca_rhythm-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    15364 2023-05-06 00:00:07.562543 sca_rhythm-0.3.1/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 sca_rhythm-0.3.1/PKG-INFO
```

### Comparing `sca_rhythm-0.3.0/LICENSE.md` & `sca_rhythm-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.3.0/README.md` & `sca_rhythm-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.3.0/sca_rhythm/__init__.py` & `sca_rhythm-0.3.1/sca_rhythm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class WFNotFound(Exception):
     pass
 
 
 class Workflow:
-    def __init__(self, celery_app, workflow_id=None, steps=None, name=None, project=None):
+    def __init__(self, celery_app, workflow_id=None, steps=None, name=None, project=None, description=None):
         self.app = celery_app
         db = self.app.backend.database
         self.wf_col = db.get_collection('workflow_meta')
 
         assert workflow_id is not None or steps is not None, 'Either workflow_id or steps should not be None'
 
         if workflow_id is not None:
@@ -48,15 +48,16 @@
             assert name, 'name cannot be empty'
             assert project, 'project cannot be empty'
             self.workflow = {
                 '_id': str(uuid.uuid4()),
                 'created_at': datetime.datetime.utcnow(),
                 'steps': steps,
                 'name': name,
-                'project': project
+                'project': project,
+                'description': description
             }
             self.wf_col.insert_one(self.workflow)
         else:
             pass
 
     def start(self, *args, **kwargs):
         """
@@ -332,14 +333,15 @@
 
         # number of steps done is same of index of the pending step
         # if all steps are complete pending_step_idx is None, then steps_done is len(steps)
         return {
             'id': self.workflow['_id'],
             'name': self.workflow.get('name', None),
             'project': self.workflow.get('project', None),
+            'description': self.workflow.get('description', None),
             'created_at': self.workflow.get('created_at', None),
             'updated_at': self.workflow.get('updated_at', None),
             'status': status,
             'steps_done': pending_step_idx if pending_step_idx is not None else len(steps),
             'total_steps': len(steps),
             'steps': steps
         }
```

### Comparing `sca_rhythm-0.3.0/PKG-INFO` & `sca_rhythm-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.3.0
+Version: 0.3.1
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=5.2.7,<6.0.0)
```

