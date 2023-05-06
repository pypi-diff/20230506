# Comparing `tmp/ats_case-0.6.8.tar.gz` & `tmp/ats_case-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.6.8.tar", last modified: Fri May  5 06:11:49 2023, max compression
+gzip compressed data, was "ats_case-0.6.9.tar", last modified: Sat May  6 07:58:11 2023, max compression
```

## Comparing `ats_case-0.6.8.tar` & `ats_case-0.6.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.671155 ats_case-0.6.8/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.8/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-05 06:11:49.668676 ats_case-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.269760 ats_case-0.6.8/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.8/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.490541 ats_case-0.6.8/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.8/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17450 2023-05-04 06:36:02.000000 ats_case-0.6.8/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.8/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.6.8/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.6.8/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.560392 ats_case-0.6.8/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.8/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.8/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.6.8/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.623403 ats_case-0.6.8/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.8/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.6.8/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.6.8/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.658377 ats_case-0.6.8/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.8/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.8/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-05 06:11:49.368236 ats_case-0.6.8/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-05 06:11:48.000000 ats_case-0.6.8/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-05 06:11:48.000000 ats_case-0.6.8/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:11:48.000000 ats_case-0.6.8/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-05 06:11:48.000000 ats_case-0.6.8/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 06:11:48.000000 ats_case-0.6.8/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 06:11:49.671155 ats_case-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-05 06:10:30.000000 ats_case-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.262022 ats_case-0.6.9/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.6.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-06 07:58:11.260028 ats_case-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:10.840645 ats_case-0.6.9/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.6.9/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.065626 ats_case-0.6.9/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.6.9/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17450 2023-05-04 06:36:02.000000 ats_case-0.6.9/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9976 2023-04-23 06:01:24.000000 ats_case-0.6.9/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.6.9/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5548 2023-05-04 06:36:02.000000 ats_case-0.6.9/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.140737 ats_case-0.6.9/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.6.9/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.6.9/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.6.9/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.209888 ats_case-0.6.9/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.9/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.6.9/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.6.9/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:11.250848 ats_case-0.6.9/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.6.9/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.6.9/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-06 07:58:10.942507 ats_case-0.6.9/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 07:58:10.000000 ats_case-0.6.9/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 07:58:11.262022 ats_case-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-06 07:57:40.000000 ats_case-0.6.9/setup.py
```

### Comparing `ats_case-0.6.8/PKG-INFO` & `ats_case-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.6.8
+Version: 0.6.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.8/README.md` & `ats_case-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/case/command.py` & `ats_case-0.6.9/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/case/context.py` & `ats_case-0.6.9/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/case/executor.py` & `ats_case-0.6.9/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/case/translator.py` & `ats_case-0.6.9/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/common/error.py` & `ats_case-0.6.9/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/manage/core.py` & `ats_case-0.6.9/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/manage/start.py` & `ats_case-0.6.9/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case/template/testcase_v1.tmp` & `ats_case-0.6.9/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/ats_case.egg-info/PKG-INFO` & `ats_case-0.6.9/ats_case.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.6.8
+Version: 0.6.9
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.6.8/ats_case.egg-info/SOURCES.txt` & `ats_case-0.6.9/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.6.8/setup.py` & `ats_case-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.6.8",
+    version="0.6.9",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

