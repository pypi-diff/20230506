# Comparing `tmp/crawler_commons-0.0.2.tar.gz` & `tmp/crawler_commons-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crawler_commons-0.0.2.tar", last modified: Wed May  3 17:15:53 2023, max compression
+gzip compressed data, was "crawler_commons-0.0.3.tar", last modified: Sat May  6 07:39:55 2023, max compression
```

## Comparing `crawler_commons-0.0.2.tar` & `crawler_commons-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawlutils/
--rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.2/crawlutils/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.2/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.2/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      552 2023-05-03 17:15:51.000000 crawler_commons-0.0.2/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      419 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      205 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       11 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/crawler_commons.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-03 17:15:53.000000 crawler_commons-0.0.2/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.330787 crawler_commons-0.0.3/
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 crawler_commons-0.0.3/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:39:55.330556 crawler_commons-0.0.3/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)       27 2023-03-17 05:41:21.000000 crawler_commons-0.0.3/README.md
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.329080 crawler_commons-0.0.3/crawapi/
+-rw-r--r--   0 nezah      (501) staff       (20)     2460 2023-05-06 07:35:34.000000 crawler_commons-0.0.3/crawapi/__init__.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.329941 crawler_commons-0.0.3/crawler_commons.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      399 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      250 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       19 2023-05-06 07:39:55.000000 crawler_commons-0.0.3/crawler_commons.egg-info/top_level.txt
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-05-06 07:39:55.330312 crawler_commons-0.0.3/crawlutils/
+-rw-r--r--   0 nezah      (501) staff       (20)     2535 2023-05-03 17:15:32.000000 crawler_commons-0.0.3/crawlutils/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1556 2023-05-06 07:27:29.000000 crawler_commons-0.0.3/crawlutils/text_utils.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-05-06 07:39:55.330846 crawler_commons-0.0.3/setup.cfg
+-rw-r--r--   0 nezah      (501) staff       (20)      569 2023-05-06 07:37:36.000000 crawler_commons-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `crawler_commons-0.0.2/crawlutils/__init__.py` & `crawler_commons-0.0.3/crawlutils/__init__.py`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.2/LICENSE` & `crawler_commons-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crawler_commons-0.0.2/setup.py` & `crawler_commons-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 
 setuptools.setup(
     name="crawler_commons",
-    version="0.0.2",
+    version="0.0.3",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="crawler commons",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/crawler_commons",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         # 패키지에 대한 태그
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
 )
```

