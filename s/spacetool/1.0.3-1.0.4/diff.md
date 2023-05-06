# Comparing `tmp/spacetool-1.0.3.tar.gz` & `tmp/spacetool-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetool-1.0.3.tar", last modified: Sat May  6 03:09:19 2023, max compression
+gzip compressed data, was "spacetool-1.0.4.tar", last modified: Sat May  6 03:23:06 2023, max compression
```

## Comparing `spacetool-1.0.3.tar` & `spacetool-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.615988 spacetool-1.0.3/
--rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.3/LICENSE
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:09:19.615868 spacetool-1.0.3/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.3/README.md
--rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-06 03:09:19.616029 spacetool-1.0.3/setup.cfg
--rw-r--r--   0 leo        (501) staff       (20)     2519 2023-05-06 03:09:09.000000 spacetool-1.0.3/setup.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.614715 spacetool-1.0.3/spacetool/
--rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.3/spacetool/__init__.py
--rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.3/spacetool/__version__.py
--rw-r--r--   0 leo        (501) staff       (20)    52059 2023-05-06 03:07:37.000000 spacetool-1.0.3/spacetool/main_tool.py
-drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:09:19.615661 spacetool-1.0.3/spacetool.egg-info/
--rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/PKG-INFO
--rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/SOURCES.txt
--rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/dependency_links.txt
--rw-r--r--   0 leo        (501) staff       (20)       60 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/requires.txt
--rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-06 03:09:19.000000 spacetool-1.0.3/spacetool.egg-info/top_level.txt
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:23:06.622924 spacetool-1.0.4/
+-rw-r--r--   0 leo        (501) staff       (20)     1068 2022-11-03 01:53:28.000000 spacetool-1.0.4/LICENSE
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:23:06.622811 spacetool-1.0.4/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      135 2023-04-10 02:45:30.000000 spacetool-1.0.4/README.md
+-rw-r--r--   0 leo        (501) staff       (20)       38 2023-05-06 03:23:06.622967 spacetool-1.0.4/setup.cfg
+-rw-r--r--   0 leo        (501) staff       (20)     2483 2023-05-06 03:23:03.000000 spacetool-1.0.4/setup.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:23:06.621621 spacetool-1.0.4/spacetool/
+-rw-r--r--   0 leo        (501) staff       (20)        0 2022-11-03 01:53:28.000000 spacetool-1.0.4/spacetool/__init__.py
+-rw-r--r--   0 leo        (501) staff       (20)        7 2022-11-08 03:02:34.000000 spacetool-1.0.4/spacetool/__version__.py
+-rw-r--r--   0 leo        (501) staff       (20)    52059 2023-05-06 03:07:37.000000 spacetool-1.0.4/spacetool/main_tool.py
+drwxr-xr-x   0 leo        (501) staff       (20)        0 2023-05-06 03:23:06.622644 spacetool-1.0.4/spacetool.egg-info/
+-rw-r--r--   0 leo        (501) staff       (20)      432 2023-05-06 03:23:06.000000 spacetool-1.0.4/spacetool.egg-info/PKG-INFO
+-rw-r--r--   0 leo        (501) staff       (20)      260 2023-05-06 03:23:06.000000 spacetool-1.0.4/spacetool.egg-info/SOURCES.txt
+-rw-r--r--   0 leo        (501) staff       (20)        1 2023-05-06 03:23:06.000000 spacetool-1.0.4/spacetool.egg-info/dependency_links.txt
+-rw-r--r--   0 leo        (501) staff       (20)       27 2023-05-06 03:23:06.000000 spacetool-1.0.4/spacetool.egg-info/requires.txt
+-rw-r--r--   0 leo        (501) staff       (20)       10 2023-05-06 03:23:06.000000 spacetool-1.0.4/spacetool.egg-info/top_level.txt
```

### Comparing `spacetool-1.0.3/LICENSE` & `spacetool-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacetool-1.0.3/setup.py` & `spacetool-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from setuptools import find_packages
 
 
 from setuptools import setup, find_packages
 
 setup(
     name="spacetool",
-    version="1.0.3",
+    version="1.0.4",
     description='space.top的数据管理工具',
     author="Leo Ni",
     author_email="nij6173@gmail.com",
     url='http://space.top/',
     packages=find_packages(),
-    install_requires=["requests", "cos-python-sdk-v5==1.9.23", "qcloud-python-sts==3.1.3"],
+    install_requires=["requests", "cos-python-sdk-v5"],
     python_requires=">=3.6,<3.11",
     keywords=['data', "spacedata"],
     license='MIT',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `spacetool-1.0.3/spacetool/main_tool.py` & `spacetool-1.0.4/spacetool/main_tool.py`

 * *Files identical despite different names*

