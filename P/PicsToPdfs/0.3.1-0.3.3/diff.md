# Comparing `tmp/PicsToPdfs-0.3.1.tar.gz` & `tmp/PicsToPdfs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.3.1.tar", last modified: Sat May  6 03:27:43 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.3.tar", last modified: Sat May  6 03:48:31 2023, max compression
```

## Comparing `PicsToPdfs-0.3.1.tar` & `PicsToPdfs-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.977662 PicsToPdfs-0.3.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      481 2023-05-06 03:27:43.977662 PicsToPdfs-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.967663 PicsToPdfs-0.3.1/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.974666 PicsToPdfs-0.3.1/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.976708 PicsToPdfs-0.3.1/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.1/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:27:43.972662 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      481 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 03:27:43.000000 PicsToPdfs-0.3.1/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.1/README.md
--rw-rw-rw-   0        0        0      135 2023-05-06 03:27:43.978662 PicsToPdfs-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-05-06 03:27:26.000000 PicsToPdfs-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.236891 PicsToPdfs-0.3.3/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      387 2023-05-06 03:48:31.236891 PicsToPdfs-0.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.222896 PicsToPdfs-0.3.3/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.231889 PicsToPdfs-0.3.3/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/Function/__init__.py
+-rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:35.000000 PicsToPdfs-0.3.3/PicsToPdfs/Function/imgToPdf.pyd
+-rw-rw-rw-   0        0        0   110592 2023-05-05 07:05:23.000000 PicsToPdfs-0.3.3/PicsToPdfs/PicToPdf.pyd
+drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.235891 PicsToPdfs-0.3.3/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    79360 2023-04-28 06:28:53.000000 PicsToPdfs-0.3.3/PicsToPdfs/Ui/PicToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.3/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 03:48:31.229891 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 03:48:31.000000 PicsToPdfs-0.3.3/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.3/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-06 03:48:31.237889 PicsToPdfs-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      959 2023-05-06 03:41:29.000000 PicsToPdfs-0.3.3/setup.py
```

### Comparing `PicsToPdfs-0.3.1/LICENSE.txt` & `PicsToPdfs-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.3.1/setup.py` & `PicsToPdfs-0.3.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
-PATCH = 1
+PATCH = 3
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "PicsToPdfs",
-	version = VERSION,
-    author ="wangweidong",
-    author_email = "17891967090@163.com",
-    description='PDF撕裂者单个功能',
+    version=VERSION,
+    author="wangweidong",
+    author_email="17891967090@163.com",
+    description='图片转PDF',
     long_description_content_type="text/markdown",
-	url = 'https://mail.163.com/js6/main.jsp?sid=PAlGWIYldfIQjfQTFYllFVEyKXidwtNk&df=mail163_letter#module=welcome.WelcomeModule%7C%7B%7D',
-	long_description = open('README.md',encoding="utf-8").read(),
+    url='https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
+    long_description=open('README.md', encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
-	packages = find_packages(),
- 	# license = 'Apache',
-   	classifiers = [
-       'Programming Language :: Python',
+    packages=find_packages(),
+    # license = '',
+    classifiers=[
+        'Programming Language :: Python',
 
     ],
-    #包含的类型
-    package_data={'': ['*.csv', '*.txt','.toml', "*.pyd",'*.exe', '*.db']}, #这个很重要
-    include_package_data=True #也选上
+    # 包含的类型
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db']},  # 这个很重要
+    include_package_data=True  # 也选上
 
 )
```

