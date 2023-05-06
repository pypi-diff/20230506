# Comparing `tmp/jixn_utils-0.0.1.tar.gz` & `tmp/jixn_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jixn_utils-0.0.1.tar", last modified: Sat May  6 06:47:23 2023, max compression
+gzip compressed data, was "jixn_utils-0.0.2.tar", last modified: Sat May  6 06:55:53 2023, max compression
```

## Comparing `jixn_utils-0.0.1.tar` & `jixn_utils-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 06:47:23.553396 jixn_utils-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 jixn_utils-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-05-06 06:47:23.553396 jixn_utils-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-05-06 06:27:28.000000 jixn_utils-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 06:47:23.540961 jixn_utils-0.0.1/jixn_util/
--rw-rw-rw-   0        0        0     2452 2023-04-20 03:16:10.000000 jixn_utils-0.0.1/jixn_util/GetConfig.py
--rw-rw-rw-   0        0        0     3607 2023-03-10 07:58:55.000000 jixn_utils-0.0.1/jixn_util/JudgeFile.py
--rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 jixn_utils-0.0.1/jixn_util/__init__.py
--rw-rw-rw-   0        0        0     8397 2023-05-06 06:22:15.000000 jixn_utils-0.0.1/jixn_util/dbmysql.py
--rw-rw-rw-   0        0        0     3201 2023-03-21 07:10:32.000000 jixn_utils-0.0.1/jixn_util/gen_guid.py
--rw-rw-rw-   0        0        0     9259 2023-04-20 03:16:10.000000 jixn_utils-0.0.1/jixn_util/jixn_parser.py
--rw-rw-rw-   0        0        0    91465 2023-04-20 03:16:10.000000 jixn_utils-0.0.1/jixn_util/jixn_parser_嵌套类型.py
--rw-rw-rw-   0        0        0    37882 2023-04-20 03:16:10.000000 jixn_utils-0.0.1/jixn_util/jixn_utils.py
--rw-rw-rw-   0        0        0     2716 2023-04-20 03:16:10.000000 jixn_utils-0.0.1/jixn_util/sendnews.py
-drwxrwxrwx   0        0        0        0 2023-05-06 06:47:23.553396 jixn_utils-0.0.1/jixn_utils.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-06 06:47:23.000000 jixn_utils-0.0.1/jixn_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-05-06 06:47:23.000000 jixn_utils-0.0.1/jixn_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 06:47:23.000000 jixn_utils-0.0.1/jixn_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 06:47:23.000000 jixn_utils-0.0.1/jixn_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 06:47:23.553396 jixn_utils-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1136 2023-05-06 06:47:18.000000 jixn_utils-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.271077 jixn_utils-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-06 06:29:33.000000 jixn_utils-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-05-06 06:55:53.270079 jixn_utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       26 2023-05-06 06:27:28.000000 jixn_utils-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.264078 jixn_utils-0.0.2/jixn_utils/
+-rw-rw-rw-   0        0        0     2452 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/GetConfig.py
+-rw-rw-rw-   0        0        0     3607 2023-03-10 07:58:55.000000 jixn_utils-0.0.2/jixn_utils/JudgeFile.py
+-rw-rw-rw-   0        0        0        0 2023-05-06 06:24:35.000000 jixn_utils-0.0.2/jixn_utils/__init__.py
+-rw-rw-rw-   0        0        0     8397 2023-05-06 06:22:15.000000 jixn_utils-0.0.2/jixn_utils/dbmysql.py
+-rw-rw-rw-   0        0        0     3201 2023-03-21 07:10:32.000000 jixn_utils-0.0.2/jixn_utils/gen_guid.py
+-rw-rw-rw-   0        0        0     9259 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_parser.py
+-rw-rw-rw-   0        0        0    91465 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_parser_嵌套类型.py
+-rw-rw-rw-   0        0        0    37882 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/jixn_utils.py
+-rw-rw-rw-   0        0        0     2716 2023-04-20 03:16:10.000000 jixn_utils-0.0.2/jixn_utils/sendnews.py
+drwxrwxrwx   0        0        0        0 2023-05-06 06:55:53.268077 jixn_utils-0.0.2/jixn_utils.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 06:55:53.000000 jixn_utils-0.0.2/jixn_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 06:55:53.271077 jixn_utils-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1136 2023-05-06 06:55:46.000000 jixn_utils-0.0.2/setup.py
```

### Comparing `jixn_utils-0.0.1/LICENSE.txt` & `jixn_utils-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/GetConfig.py` & `jixn_utils-0.0.2/jixn_utils/GetConfig.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/JudgeFile.py` & `jixn_utils-0.0.2/jixn_utils/JudgeFile.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/dbmysql.py` & `jixn_utils-0.0.2/jixn_utils/dbmysql.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/gen_guid.py` & `jixn_utils-0.0.2/jixn_utils/gen_guid.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/jixn_parser.py` & `jixn_utils-0.0.2/jixn_utils/jixn_parser.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/jixn_parser_嵌套类型.py` & `jixn_utils-0.0.2/jixn_utils/jixn_parser_嵌套类型.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/jixn_utils.py` & `jixn_utils-0.0.2/jixn_utils/jixn_utils.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/jixn_util/sendnews.py` & `jixn_utils-0.0.2/jixn_utils/sendnews.py`

 * *Files identical despite different names*

### Comparing `jixn_utils-0.0.1/setup.py` & `jixn_utils-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jixn_utils",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.1",  # 包版本号，便于维护版本
+    version="0.0.2",  # 包版本号，便于维护版本
     author="jixn",  # 作者，可以写自己的姓名
     author_email="jixn@example.com",  # 作者联系方式，可写自己的邮箱地址
     description="一个工具包啊这",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

