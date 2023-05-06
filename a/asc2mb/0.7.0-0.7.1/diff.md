# Comparing `tmp/asc2mb-0.7.0.tar.gz` & `tmp/asc2mb-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asc2mb-0.7.0.tar", max compression
+gzip compressed data, was "asc2mb-0.7.1.tar", max compression
```

## Comparing `asc2mb-0.7.0.tar` & `asc2mb-0.7.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1077 2023-01-04 05:44:08.623819 asc2mb-0.7.0/LICENSE
--rw-r--r--   0        0        0     2327 2021-12-20 03:30:53.502175 asc2mb-0.7.0/README.md
--rw-r--r--   0        0        0        0 2021-12-08 10:10:14.401686 asc2mb-0.7.0/asc2mb/__init__.py
--rw-r--r--   0        0        0    16196 2023-05-05 03:38:11.938609 asc2mb-0.7.0/asc2mb/asc2mb.py
--rw-r--r--   0        0        0      606 2023-05-05 03:44:02.698247 asc2mb-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 asc2mb-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-01-04 05:44:08.623819 asc2mb-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2327 2021-12-20 03:30:53.502175 asc2mb-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2021-12-08 10:10:14.401686 asc2mb-0.7.1/asc2mb/__init__.py
+-rw-r--r--   0        0        0    16377 2023-05-06 03:39:18.549333 asc2mb-0.7.1/asc2mb/asc2mb.py
+-rw-r--r--   0        0        0      606 2023-05-06 03:42:04.545582 asc2mb-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 asc2mb-0.7.1/PKG-INFO
```

### Comparing `asc2mb-0.7.0/LICENSE` & `asc2mb-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asc2mb-0.7.0/README.md` & `asc2mb-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `asc2mb-0.7.0/asc2mb/asc2mb.py` & `asc2mb-0.7.1/asc2mb/asc2mb.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,30 +50,33 @@
     
 class Teacher(Json):
     """
     Special behavior for a teacher, where there is an email that might be in the xml file
     or it might not be. Some functionality is needed here to allow the end user define the pattern used to make the email
     for example by initials or firstname.lastname@example.com
     """
-    def __init__(self, data={}, default=''):
+    def __init__(self, data={}, default=None):
         if not data:
             data = {"name": "Unknown Teacher"}
+        if default is None:
+            default = '{".".join(teacher.name.split(' ')) + "@example.com"}'
         self.default = default
         Json.__init__(self, data, default)
 
     @property
     def email(self):
         """
         Conveniently override the email property to use an evaluated string
         """
+        #if 'email' in self.data and self.data.get('email'):
         if 'email' in self.data:
             return self.data.email
         teacher = self
         pattern = "f'" + (self.default or '') + "'"
-        return eval(pattern)
+        return eval(pattern).lower()
 
 # eval used 
 class_id_patterns = [
     {"p": "{class_.short}_{division.name}", "n":'default'},
     {"p":"{class_.short} {division.divisiontag if division.divisiontag!='0' else ''}{subject.short}", "n": "dar_al_marefa"},
     {'p': '{class_.name}', 'n':'name_only'}
 ]
@@ -210,14 +213,15 @@
             teacher_emails_list = []
             for teacher_id in teachers:
                 teacher = lookup.get('teachers').get(teacher_id)
                 teacher_obj = Teacher(teacher, teacher_email_pattern)
                 teacher_emails_list.append(teacher_obj)
             teacher_emails = "|".join([teacher.email if hasattr(teacher, 'email') else '' for teacher in teacher_emails_list])
 
+    
             combine = False
             if smart_combine and len(teachers) == 1 and largest > 1:
                 combine = True
 
             uniqs = []
             for index in range(largest):
                 group_id = groups[index]
```

### Comparing `asc2mb-0.7.0/pyproject.toml` & `asc2mb-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asc2mb"
-version = "0.7.0"
+version = "0.7.1"
 description = "Manage your timetable by pasing the XML export from asc and format into two files suitable for upload into ManageBac"
 authors = ["Adam Morris <adam.morris@fariaedu.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["ManageBac", "aSc", "timetable"]
 
 [tool.poetry.dependencies]
```

### Comparing `asc2mb-0.7.0/PKG-INFO` & `asc2mb-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asc2mb
-Version: 0.7.0
+Version: 0.7.1
 Summary: Manage your timetable by pasing the XML export from asc and format into two files suitable for upload into ManageBac
 License: MIT
 Keywords: ManageBac,aSc,timetable
 Author: Adam Morris
 Author-email: adam.morris@fariaedu.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

