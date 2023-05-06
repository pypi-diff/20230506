# Comparing `tmp/ats_case-0.6.9.tar.gz` & `tmp/ats_case-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.6.9.tar", last modified: Sat May  6 07:58:11 2023, max compression
+gzip compressed data, was "ats_case-0.7.0.tar", last modified: Sat May  6 09:09:23 2023, max compression
```

## Comparing `ats_case-0.6.9.tar` & `ats_case-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.262022 ats_case-0.6.9/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.9/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-06 07:58:11.260028 ats_case-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:10.840645 ats_case-0.6.9/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.9/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.065626 ats_case-0.6.9/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.9/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17450 2023-05-04 06:36:02.000000 ats_case-0.6.9/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.9/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.6.9/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.6.9/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.140737 ats_case-0.6.9/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.9/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.9/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.6.9/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.209888 ats_case-0.6.9/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.9/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.6.9/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.6.9/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.250848 ats_case-0.6.9/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.9/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.9/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-06 07:58:10.942507 ats_case-0.6.9/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 07:58:11.262022 ats_case-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-06 07:57:40.000000 ats_case-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.688865 ats_case-0.7.0/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-06 09:09:23.687869 ats_case-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.304833 ats_case-0.7.0/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.7.0/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.514277 ats_case-0.7.0/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.7.0/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17454 2023-05-06 09:07:41.000000 ats_case-0.7.0/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.7.0/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.7.0/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.7.0/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.583092 ats_case-0.7.0/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.7.0/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.7.0/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.7.0/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.636949 ats_case-0.7.0/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.0/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.7.0/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.7.0/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.674847 ats_case-0.7.0/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.7.0/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.7.0/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-06 09:09:23.401576 ats_case-0.7.0/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-06 09:09:22.000000 ats_case-0.7.0/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-06 09:09:22.000000 ats_case-0.7.0/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 09:09:22.000000 ats_case-0.7.0/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-06 09:09:22.000000 ats_case-0.7.0/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 09:09:22.000000 ats_case-0.7.0/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 09:09:23.689863 ats_case-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-06 09:07:54.000000 ats_case-0.7.0/setup.py
```

### Comparing `ats_case-0.6.9/PKG-INFO` & `ats_case-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.6.9
+Version: 0.7.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.9/README.md` & `ats_case-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/case/command.py` & `ats_case-0.7.0/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     :param param: desc-测试步骤描述
     :return:
     """
     desc = param.get('desc')
 
     def decorate(callback):
         def fn(*args, **kwargs):
-            client().message(desc).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
+            client().message({'msg': desc}).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
             r = callback(*args, **kwargs)
             return r
 
         return fn
 
     return decorate
 
@@ -478,15 +478,15 @@
         self._message = None
         self._parameter = None
 
     def operation(self, command: str):
         self._operation = command
         return self
 
-    def message(self, msg: str):
+    def message(self, msg):
         self._message = msg
         return self
 
     def parameter(self, param=None):
         self._parameter = param
         return self
```

### Comparing `ats_case-0.6.9/ats_case/case/context.py` & `ats_case-0.7.0/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/case/executor.py` & `ats_case-0.7.0/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/case/translator.py` & `ats_case-0.7.0/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/common/error.py` & `ats_case-0.7.0/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/manage/core.py` & `ats_case-0.7.0/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/manage/start.py` & `ats_case-0.7.0/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case/template/testcase_v1.tmp` & `ats_case-0.7.0/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/ats_case.egg-info/PKG-INFO` & `ats_case-0.7.0/ats_case.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.6.9
+Version: 0.7.0
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.9/ats_case.egg-info/SOURCES.txt` & `ats_case-0.7.0/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.9/setup.py` & `ats_case-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.6.9",
+    version="0.7.0",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

