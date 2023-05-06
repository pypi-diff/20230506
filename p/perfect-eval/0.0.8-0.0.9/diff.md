# Comparing `tmp/perfect-eval-0.0.8.tar.gz` & `tmp/perfect-eval-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfect-eval-0.0.8.tar", last modified: Wed Feb  8 08:14:49 2023, max compression
+gzip compressed data, was "perfect-eval-0.0.9.tar", last modified: Sat May  6 03:46:57 2023, max compression
```

## Comparing `perfect-eval-0.0.8.tar` & `perfect-eval-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-02-08 08:14:49.902560 perfect-eval-0.0.8/
--rw-r--r--   0 lumi       (501) admin       (80)     1057 2022-04-28 06:56:40.000000 perfect-eval-0.0.8/.gitignore
-drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-02-08 08:14:49.900532 perfect-eval-0.0.8/.idea/
--rw-r--r--   0 lumi       (501) admin       (80)       47 2022-11-02 07:57:23.000000 perfect-eval-0.0.8/.idea/.gitignore
--rw-r--r--   0 lumi       (501) admin       (80)    22729 2022-12-06 02:29:29.000000 perfect-eval-0.0.8/.idea/dbnavigator.xml
-drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-02-08 08:14:49.900928 perfect-eval-0.0.8/.idea/inspectionProfiles/
--rw-r--r--   0 lumi       (501) admin       (80)     9707 2022-11-02 07:57:33.000000 perfect-eval-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 lumi       (501) admin       (80)      174 2022-11-02 07:57:33.000000 perfect-eval-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 lumi       (501) admin       (80)      186 2022-11-02 11:21:13.000000 perfect-eval-0.0.8/.idea/misc.xml
--rw-r--r--   0 lumi       (501) admin       (80)      270 2022-11-02 07:57:33.000000 perfect-eval-0.0.8/.idea/modules.xml
--rw-r--r--   0 lumi       (501) admin       (80)      183 2022-11-02 07:57:33.000000 perfect-eval-0.0.8/.idea/vcs.xml
--rw-r--r--   0 lumi       (501) admin       (80)     1060 2022-04-28 02:53:13.000000 perfect-eval-0.0.8/LICENSE
--rw-r--r--   0 lumi       (501) admin       (80)       26 2022-04-28 02:53:13.000000 perfect-eval-0.0.8/MANIFEST.in
--rw-r--r--   0 lumi       (501) admin       (80)     2722 2023-02-08 08:14:49.902355 perfect-eval-0.0.8/PKG-INFO
--rw-r--r--   0 lumi       (501) admin       (80)     1889 2023-02-08 08:14:44.000000 perfect-eval-0.0.8/README.md
--rwxrwxrwx   0 lumi       (501) admin       (80)       91 2022-06-06 07:07:43.000000 perfect-eval-0.0.8/build.sh
-drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-02-08 08:14:49.901452 perfect-eval-0.0.8/perfect_eval/
--rw-r--r--   0 lumi       (501) admin       (80)      183 2022-10-31 02:06:34.000000 perfect-eval-0.0.8/perfect_eval/__init__.py
--rw-r--r--   0 lumi       (501) admin       (80)      219 2023-02-08 08:14:44.000000 perfect-eval-0.0.8/perfect_eval/__version__.py
--rw-r--r--   0 lumi       (501) admin       (80)    14595 2023-02-08 08:04:22.000000 perfect-eval-0.0.8/perfect_eval/eval.py
-drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-02-08 08:14:49.902126 perfect-eval-0.0.8/perfect_eval.egg-info/
--rw-r--r--   0 lumi       (501) admin       (80)     2722 2023-02-08 08:14:49.000000 perfect-eval-0.0.8/perfect_eval.egg-info/PKG-INFO
--rw-r--r--   0 lumi       (501) admin       (80)      462 2023-02-08 08:14:49.000000 perfect-eval-0.0.8/perfect_eval.egg-info/SOURCES.txt
--rw-r--r--   0 lumi       (501) admin       (80)        1 2023-02-08 08:14:49.000000 perfect-eval-0.0.8/perfect_eval.egg-info/dependency_links.txt
--rw-r--r--   0 lumi       (501) admin       (80)       13 2023-02-08 08:14:49.000000 perfect-eval-0.0.8/perfect_eval.egg-info/top_level.txt
--rw-r--r--   0 lumi       (501) admin       (80)       38 2023-02-08 08:14:49.902616 perfect-eval-0.0.8/setup.cfg
--rw-r--r--   0 lumi       (501) admin       (80)     3977 2023-02-08 08:14:44.000000 perfect-eval-0.0.8/setup.py
--rw-r--r--   0 lumi       (501) admin       (80)     1223 2023-02-08 08:14:44.000000 perfect-eval-0.0.8/test.py
+drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-05-06 03:46:57.246099 perfect-eval-0.0.9/
+-rw-r--r--   0 lumi       (501) admin       (80)     1057 2022-04-28 06:56:40.000000 perfect-eval-0.0.9/.gitignore
+drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-05-06 03:46:57.243562 perfect-eval-0.0.9/.idea/
+-rw-r--r--   0 lumi       (501) admin       (80)       47 2022-11-02 07:57:23.000000 perfect-eval-0.0.9/.idea/.gitignore
+-rw-r--r--   0 lumi       (501) admin       (80)    22729 2023-03-10 12:12:47.000000 perfect-eval-0.0.9/.idea/dbnavigator.xml
+drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-05-06 03:46:57.244044 perfect-eval-0.0.9/.idea/inspectionProfiles/
+-rw-r--r--   0 lumi       (501) admin       (80)     9707 2022-11-02 07:57:33.000000 perfect-eval-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 lumi       (501) admin       (80)      174 2022-11-02 07:57:33.000000 perfect-eval-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 lumi       (501) admin       (80)      186 2023-04-25 06:11:44.000000 perfect-eval-0.0.9/.idea/misc.xml
+-rw-r--r--   0 lumi       (501) admin       (80)      270 2022-11-02 07:57:33.000000 perfect-eval-0.0.9/.idea/modules.xml
+-rw-r--r--   0 lumi       (501) admin       (80)      183 2022-11-02 07:57:33.000000 perfect-eval-0.0.9/.idea/vcs.xml
+-rw-r--r--   0 lumi       (501) admin       (80)     1060 2022-04-28 02:53:13.000000 perfect-eval-0.0.9/LICENSE
+-rw-r--r--   0 lumi       (501) admin       (80)       26 2022-04-28 02:53:13.000000 perfect-eval-0.0.9/MANIFEST.in
+-rw-r--r--   0 lumi       (501) admin       (80)     2722 2023-05-06 03:46:57.245931 perfect-eval-0.0.9/PKG-INFO
+-rw-r--r--   0 lumi       (501) admin       (80)     1889 2023-03-10 12:12:47.000000 perfect-eval-0.0.9/README.md
+-rwxrwxrwx   0 lumi       (501) admin       (80)       91 2022-06-06 07:07:43.000000 perfect-eval-0.0.9/build.sh
+drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-05-06 03:46:57.244787 perfect-eval-0.0.9/perfect_eval/
+-rw-r--r--   0 lumi       (501) admin       (80)      183 2022-10-31 02:06:34.000000 perfect-eval-0.0.9/perfect_eval/__init__.py
+-rw-r--r--   0 lumi       (501) admin       (80)      219 2023-05-06 03:45:54.000000 perfect-eval-0.0.9/perfect_eval/__version__.py
+-rw-r--r--   0 lumi       (501) admin       (80)    14624 2023-05-06 03:44:07.000000 perfect-eval-0.0.9/perfect_eval/eval.py
+drwxr-xr-x   0 lumi       (501) admin       (80)        0 2023-05-06 03:46:57.245671 perfect-eval-0.0.9/perfect_eval.egg-info/
+-rw-r--r--   0 lumi       (501) admin       (80)     2722 2023-05-06 03:46:56.000000 perfect-eval-0.0.9/perfect_eval.egg-info/PKG-INFO
+-rw-r--r--   0 lumi       (501) admin       (80)      462 2023-05-06 03:46:57.000000 perfect-eval-0.0.9/perfect_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 lumi       (501) admin       (80)        1 2023-05-06 03:46:56.000000 perfect-eval-0.0.9/perfect_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 lumi       (501) admin       (80)       13 2023-05-06 03:46:56.000000 perfect-eval-0.0.9/perfect_eval.egg-info/top_level.txt
+-rw-r--r--   0 lumi       (501) admin       (80)       38 2023-05-06 03:46:57.246158 perfect-eval-0.0.9/setup.cfg
+-rw-r--r--   0 lumi       (501) admin       (80)     3977 2023-05-06 03:45:54.000000 perfect-eval-0.0.9/setup.py
+-rw-r--r--   0 lumi       (501) admin       (80)     1262 2023-05-06 03:44:59.000000 perfect-eval-0.0.9/test.py
```

### Comparing `perfect-eval-0.0.8/.gitignore` & `perfect-eval-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `perfect-eval-0.0.8/.idea/dbnavigator.xml` & `perfect-eval-0.0.9/.idea/dbnavigator.xml`

 * *Files identical despite different names*

### Comparing `perfect-eval-0.0.8/.idea/inspectionProfiles/Project_Default.xml` & `perfect-eval-0.0.9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `perfect-eval-0.0.8/LICENSE` & `perfect-eval-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `perfect-eval-0.0.8/PKG-INFO` & `perfect-eval-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-eval
-Version: 0.0.8
+Version: 0.0.9
 Summary: Safe execute expr code.
 Home-page: https://github.com/holbos-deng/perfect-eval
 Author: Holbos Deng
 Author-email: 2292861292@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `perfect-eval-0.0.8/README.md` & `perfect-eval-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `perfect-eval-0.0.8/perfect_eval/eval.py` & `perfect-eval-0.0.9/perfect_eval/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 import types
 import werkzeug
 import random
 from opcode import HAVE_ARGUMENT, opmap, opname
 from types import CodeType
 import dateutil
+import time
 
 unsafe_eval = eval
 
 __all__ = ['test_expr', 'eval_expr', 'const_eval']
 
 # The time module is usually already provided in the safe_eval environment
 # but some code, e.g. datetime.datetime.now() (Windows/Python 2.5.2, bug
@@ -290,14 +291,15 @@
     'range': range,
     'xrange': range,
     'zip': zip,
     'Exception': Exception,
     'random': random,
     'match': match,
     're': re,
+    'time': time
 }
 
 
 def eval_expr(expr, globals_dict=None, locals_dict=None, mode="eval", nocopy=False, locals_builtins=False,
               filename=None):
     """safe_eval(expression[, globals[, locals[, mode[, nocopy]]]]) -> result
```

### Comparing `perfect-eval-0.0.8/perfect_eval.egg-info/PKG-INFO` & `perfect-eval-0.0.9/perfect_eval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfect-eval
-Version: 0.0.8
+Version: 0.0.9
 Summary: Safe execute expr code.
 Home-page: https://github.com/holbos-deng/perfect-eval
 Author: Holbos Deng
 Author-email: 2292861292@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `perfect-eval-0.0.8/setup.py` & `perfect-eval-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = 'perfect-eval'
 DESCRIPTION = 'Safe execute expr code.'
 URL = 'https://github.com/holbos-deng/perfect-eval'
 EMAIL = '2292861292@qq.com'
 AUTHOR = 'Holbos Deng'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
 ]
 
 # What packages are optional?
 EXTRAS = {
```

### Comparing `perfect-eval-0.0.8/test.py` & `perfect-eval-0.0.9/test.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     print(eval_expr("f'{a} + {b} = {a + b}'", {"a": 123, "b": 456}))
     print(eval_expr("match(a, [(1, '11'), (2, '22'), (3, '33')], default='ooo')", {"a": 1}))
     print(eval_expr(r"re.sub(r'\d+', '很多', count)", {"count": '10个'}))
     print(eval_expr(
         """(x := random.randint(1, 10)) and (x <= 4 and random.choice(["好的", "好哦", "好呢"])) or (x <= 10 and "....")"""))
 
     print(eval_expr(
-        '''match(weather_condition, [("晴", "晴空万里"), ("多云", "浮云甚多"), ("阴", random.choice(["乌云密布", "乌云低垂"])), 
+        '''match(weather_condition, [("晴", "晴空万里"), ("多云", "浮云甚多"), ("阴", random.choice(["乌云密布", "乌云低垂"])),
         ("小雨", "落细雨"), ("中雨", "淅沥中雨"), ("大雨", "大雨滂沱")])''',
         {"weather_condition": "阴"}))
 
+    print(eval_expr("time.sleep(10)"))
+
     print(time.time() - t1)
 
 
 if __name__ == "__main__":
     test_eval()
```

