# Comparing `tmp/log2file-1.3.tar.gz` & `tmp/log2file-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log2file-1.3.tar", last modified: Mon Apr 18 06:45:40 2022, max compression
+gzip compressed data, was "dist/log2file-1.4.tar", last modified: Sat May  6 06:23:20 2023, max compression
```

## Comparing `log2file-1.3.tar` & `log2file-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-04-18 06:45:40.001966 log2file-1.3/
--rw-r--r--   0 david      (501) staff       (20)     1048 2022-03-25 06:00:28.000000 log2file-1.3/LICENSE
--rw-r--r--   0 david      (501) staff       (20)     1511 2022-04-18 06:45:40.002067 log2file-1.3/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)     1105 2022-03-25 05:40:28.000000 log2file-1.3/README.md
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-04-18 06:45:40.000313 log2file-1.3/log2file/
--rw-r--r--   0 david      (501) staff       (20)       22 2022-03-25 05:28:46.000000 log2file-1.3/log2file/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2029 2022-04-18 06:41:39.000000 log2file-1.3/log2file/logger.py
--rw-r--r--   0 david      (501) staff       (20)      484 2020-01-20 05:40:48.000000 log2file-1.3/log2file/singleton.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2022-04-18 06:45:40.001767 log2file-1.3/log2file.egg-info/
--rw-r--r--   0 david      (501) staff       (20)     1511 2022-04-18 06:45:39.000000 log2file-1.3/log2file.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      226 2022-04-18 06:45:39.000000 log2file-1.3/log2file.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2022-04-18 06:45:39.000000 log2file-1.3/log2file.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2022-04-18 06:45:39.000000 log2file-1.3/log2file.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       78 2022-04-18 06:45:40.002527 log2file-1.3/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      606 2022-04-18 06:43:28.000000 log2file-1.3/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-05-06 06:23:20.158614 log2file-1.4/
+-rw-r--r--   0 david      (501) staff       (20)     1048 2022-03-25 06:00:28.000000 log2file-1.4/LICENSE
+-rw-r--r--   0 david      (501) staff       (20)     1939 2023-05-06 06:23:20.158740 log2file-1.4/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)     1570 2023-05-06 06:17:40.000000 log2file-1.4/README.md
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-05-06 06:23:20.156555 log2file-1.4/log2file/
+-rw-r--r--   0 david      (501) staff       (20)       22 2022-03-25 05:28:46.000000 log2file-1.4/log2file/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2172 2023-05-06 06:15:43.000000 log2file-1.4/log2file/logger.py
+-rw-r--r--   0 david      (501) staff       (20)      466 2022-06-09 03:03:45.000000 log2file-1.4/log2file/singleton.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-05-06 06:23:20.158359 log2file-1.4/log2file.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)     1939 2023-05-06 06:23:20.000000 log2file-1.4/log2file.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      226 2023-05-06 06:23:20.000000 log2file-1.4/log2file.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-05-06 06:23:20.000000 log2file-1.4/log2file.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-05-06 06:23:20.000000 log2file-1.4/log2file.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       78 2023-05-06 06:23:20.159206 log2file-1.4/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      606 2023-05-06 06:18:49.000000 log2file-1.4/setup.py
```

### Comparing `log2file-1.3/LICENSE` & `log2file-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `log2file-1.3/PKG-INFO` & `log2file-1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: log2file
-Version: 1.3
-Summary: A python logging wrapper
-Home-page: https://github.com/dwSun/pylog2file
-Author: dwSun
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # log2file
 
 python 自带 logging 模块的一个封装
 自己的项目经常用，每次都配置一堆很麻烦，就自己封装了一个。
 
 # 安装
 
@@ -33,24 +18,37 @@
 import logging
 
 # from multiprocessing import Pool
 from multiprocessing.dummy import Pool
 import time
 import random
 
-log2file.init()
-trace = log2file.trace
+log2file.init(console=True, name="test")
+
+# for root logger, don't use this or you will get many many logs,and all other loggers will be shadowed by root logger
+# log2file.init(console=True)
+
+trace_test = log2file.trace(name="test")
+# this is the trace for root logger, don't use this if you have not init root logger
+trace_root = log2file.trace()
+
+
+for i in range(20):
+    log2file.init(console=True, name=str(i))
 
+for i in range(20):
+    log2file.init(console=True, name=str(i))
 
-@trace("test")
+
+@trace_test("test_test111")
 def s():
     time.sleep(0.1 + random.randint(0, 100) / 1000)
 
 
-@trace("debug")
+@trace_root("root_debug")
 def s2():
     time.sleep(0.1 + random.randint(0, 100) / 1000)
 
 
 def fun(t):
     log = logging.getLogger(name=str(t))
     for i in range(100):
@@ -59,19 +57,17 @@
         s2()
 
 
 p = Pool(10)
 p.map(fun, range(20))
 p.close()
 p.join()
-
 ```
+
 # License
 
 [MIT](https://github.com/pythonml/douyin_image/blob/master/LICENSE)
 
 
 [version-badge]:   https://img.shields.io/badge/version-0.1-brightgreen.svg
 [version-link]:    https://pypi.python.org/pypi/douyin_image/
 [license-badge]:   https://img.shields.io/github/license/pythonml/douyin_image.sv
-
-
```

### Comparing `log2file-1.3/setup.py` & `log2file-1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as inf:
     long_description = inf.read()
 
 setuptools.setup(
     name="log2file",
-    version="1.3",
+    version="1.4",
     author="dwSun",
     author_email="",
     description="A python logging wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dwSun/pylog2file",
     packages=setuptools.find_packages(),
```

