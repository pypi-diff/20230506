# Comparing `tmp/trackplot-0.2.3.tar.gz` & `tmp/trackplot-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.3.tar", last modified: Fri May  5 05:00:06 2023, max compression
+gzip compressed data, was "trackplot-0.2.4.tar", last modified: Sat May  6 03:27:34 2023, max compression
```

## Comparing `trackplot-0.2.3.tar` & `trackplot-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.853056 trackplot-0.2.3/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.3/LICENSE
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-05 05:00:06.852759 trackplot-0.2.3/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.3/Pipfile
--rw-r--r--   0 zhangyiming   (501) staff       (20)    95508 2023-05-05 02:05:45.000000 trackplot-0.2.3/Pipfile.lock
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6521 2023-05-05 03:12:18.000000 trackplot-0.2.3/README.md
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1135 2023-05-04 09:50:39.000000 trackplot-0.2.3/pyproject.toml
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-05-05 05:00:06.853149 trackplot-0.2.3/setup.cfg
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-05-05 04:58:29.000000 trackplot-0.2.3/setup.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.836518 trackplot-0.2.3/trackplot/
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/__init__.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.840298 trackplot-0.2.3/trackplot/anno/
--rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/AxLabel.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/anno/theme.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.844079 trackplot-0.2.3/trackplot/base/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/CoordinateMap.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.3/trackplot/base/GenomicLoci.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Protein.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8274 2023-05-05 03:48:03.000000 trackplot-0.2.3/trackplot/base/ReadDepth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.3/trackplot/base/Readder.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Stroke.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/Transcript.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/base/pyUniprot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-05-05 04:58:29.000000 trackplot-0.2.3/trackplot/cli.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.845806 trackplot-0.2.3/trackplot/conf/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/DomainSetting.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/config.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/conf/drawing.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.852406 trackplot-0.2.3/trackplot/file/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.3/trackplot/file/ATAC.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.3/trackplot/file/Bam.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/BedGraph.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Bigwig.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Depth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Fasta.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.3/trackplot/file/File.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.3/trackplot/file/Motif.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.3/trackplot/file/ReadSegments.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.3/trackplot/file/Reference.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/file/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    45287 2023-02-25 16:01:18.000000 trackplot-0.2.3/trackplot/plot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.3/trackplot/plot_func.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.3/trackplot/plot_tests.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-05 05:00:06.839065 trackplot-0.2.3/trackplot.egg-info/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/entry_points.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-05 01:34:01.000000 trackplot-0.2.3/trackplot.egg-info/not-zip-safe
--rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/requires.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-05-05 05:00:06.000000 trackplot-0.2.3/trackplot.egg-info/top_level.txt
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.908008 trackplot-0.2.4/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.4/LICENSE
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-06 03:27:34.907755 trackplot-0.2.4/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.4/Pipfile
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    95508 2023-05-05 02:05:45.000000 trackplot-0.2.4/Pipfile.lock
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6521 2023-05-05 03:12:18.000000 trackplot-0.2.4/README.md
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1135 2023-05-04 09:50:39.000000 trackplot-0.2.4/pyproject.toml
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-05-06 03:27:34.908095 trackplot-0.2.4/setup.cfg
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-05-06 02:51:20.000000 trackplot-0.2.4/setup.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.895828 trackplot-0.2.4/trackplot/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/__init__.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.899471 trackplot-0.2.4/trackplot/anno/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/AxLabel.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/anno/theme.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.902943 trackplot-0.2.4/trackplot/base/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/CoordinateMap.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.4/trackplot/base/GenomicLoci.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Protein.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8662 2023-05-06 03:18:03.000000 trackplot-0.2.4/trackplot/base/ReadDepth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.4/trackplot/base/Readder.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Stroke.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/Transcript.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/base/pyUniprot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-05-06 02:51:20.000000 trackplot-0.2.4/trackplot/cli.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.903998 trackplot-0.2.4/trackplot/conf/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/DomainSetting.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/config.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/conf/drawing.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.907448 trackplot-0.2.4/trackplot/file/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.4/trackplot/file/ATAC.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.4/trackplot/file/Bam.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/BedGraph.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Bigwig.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Depth.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Fasta.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.4/trackplot/file/File.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/Junction.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.4/trackplot/file/Motif.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.4/trackplot/file/ReadSegments.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.4/trackplot/file/Reference.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/file/__init__.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.4/trackplot/plot.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.4/trackplot/plot_func.py
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.4/trackplot/plot_tests.py
+drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-05-06 03:27:34.898085 trackplot-0.2.4/trackplot.egg-info/
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     6707 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/entry_points.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/not-zip-safe
+-rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/requires.txt
+-rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-05-06 03:27:34.000000 trackplot-0.2.4/trackplot.egg-info/top_level.txt
```

### Comparing `trackplot-0.2.3/LICENSE` & `trackplot-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/PKG-INFO` & `trackplot-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
```

### Comparing `trackplot-0.2.3/Pipfile.lock` & `trackplot-0.2.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/README.md` & `trackplot-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/pyproject.toml` & `trackplot-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/setup.py` & `trackplot-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from configparser import ConfigParser
 from setuptools import setup, find_packages
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def locate_packages():
     __dir__ = os.path.dirname(os.path.abspath(__file__))
     pipfile = os.path.join(__dir__, "Pipfile")
```

### Comparing `trackplot-0.2.3/trackplot/anno/theme.py` & `trackplot-0.2.4/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/CoordinateMap.py` & `trackplot-0.2.4/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/GenomicLoci.py` & `trackplot-0.2.4/trackplot/base/GenomicLoci.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/Junction.py` & `trackplot-0.2.4/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/Protein.py` & `trackplot-0.2.4/trackplot/base/Protein.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/ReadDepth.py` & `trackplot-0.2.4/trackplot/base/ReadDepth.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     u"""
     Migrated from SplicePlot ReadDepth class
 
     add a parent class to handle all the position comparison
     """
 
     __slots__ = [
-        "junction_dict_plus", "junction_dict_minus",
+        "_junction_dict_plus_", "_junction_dict_minus_",
         "_minus_", "_plus_", "_number_of_merged_",
         "strand_aware", "site_plus", "site_minus",
     ]
 
     def __init__(self,
                  wiggle: np.array,
                  site_plus: Optional[np.array] = None,
@@ -44,51 +44,63 @@
         :param strand_aware: strand specific depth
         :param junction_dict_plus: these splice junction from plus strand
         :param junction_dict_minus: these splice junction from minus strand
         """
         self._plus_ = wiggle
         self.strand_aware = strand_aware
         self._minus_ = abs(minus) if minus is not None else minus
-        self.junction_dict_plus = junction_dict_plus
-        self.junction_dict_minus = junction_dict_minus
+        self._junction_dict_plus_ = junction_dict_plus
+        self._junction_dict_minus_ = junction_dict_minus
         self.site_plus = site_plus
         self.site_minus = site_minus * -1 if site_minus is not None else site_minus
 
         self._number_of_merged_ = 1
 
     @property
     def plus(self) -> Optional[np.array]:
-        if self._plus_ is not None and self._number_of_merged_ > 0:
+        if not self._transformed_or_normalized_ and self._plus_ is not None and self._number_of_merged_ > 0:
             return self._plus_ / self._number_of_merged_
         return self._plus_
 
     @property
     def minus(self) -> Optional[np.array]:
-        if self._minus_ is not None and self._number_of_merged_ > 0:
+        if not self._transformed_or_normalized_ and self._minus_ is not None and self._number_of_merged_ > 0:
             return self._minus_ / self._number_of_merged_
         return self._minus_
 
     @property
     def wiggle(self) -> np.array:
         if (self._plus_ is None or not self._plus_.any()) and self._minus_ is not None:
             return self.minus
 
         if self._plus_ is not None and self._minus_ is not None:
             return self.plus + self.minus
 
         return self.plus
 
     @property
+    def junctions_plus(self) -> dict:
+        if self._number_of_merged_ > 1:
+            return {k: v / self._number_of_merged_ for k, v in self._junction_dict_plus_.items()}
+        return self._junction_dict_plus_
+
+    @property
+    def junctions_minus(self) -> dict:
+        if self._number_of_merged_ > 1:
+            return {k: v / self._number_of_merged_ for k, v in self._junction_dict_minus_.items()}
+        return self._junction_dict_minus_
+
+    @property
     def junctions_dict(self) -> dict:
         res = {}
-        if self.junction_dict_plus:
-            res.update(self.junction_dict_plus)
+        if self._junction_dict_plus_:
+            res.update(self.junctions_plus)
 
-        if self.junction_dict_minus:
-            res.update(self.junction_dict_minus)
+        if self._junction_dict_minus_:
+            res.update(self.junctions_minus)
         return res
 
     @property
     def max(self) -> float:
         return max(self.wiggle, default=0)
 
     def __add__(self, other):
@@ -101,18 +113,18 @@
             A new ReadDepth object containing the sum of the two original ReadDepth objects
         """
 
         if self.wiggle is not None and other.wiggle is not None:
             if len(self.wiggle) == len(other.wiggle):
                 junc_plus, junc_minus = {}, {}
 
-                for i in [self.junction_dict_plus, other.junction_dict_plus]:
+                for i in [self._junction_dict_plus_, other._junction_dict_plus_]:
                     if i:
                         junc_plus.update(i)
-                for i in [self.junction_dict_minus, other.junction_dict_minus]:
+                for i in [self._junction_dict_minus_, other._junction_dict_minus_]:
                     if i:
                         junc_minus.update(i)
 
                 minus = None
                 if self._minus_ is not None and other._minus_ is not None:
                     minus = self._minus_ + other._minus_
                 elif self._minus_ is None and other._minus_ is not None:
@@ -147,66 +159,69 @@
 
     def add_customized_junctions(self, other):
         u"""
         Add customized junctions to plot
         :param other:
         :return:
         """
-        junc_plus, junc_minus = {}, {}
 
-        for key, value in other.junctions_dict.items():
-            if key in self.junctions_dict.keys():
-                if key.strand == "+":
-                    self.junction_dict_plus[key] = value + other.junctions_dict[key]
-                else:
-                    self.junction_dict_minus[key] = value + other.junctions_dict[key]
-            else:
-                if key.strand == "+":
-                    self.junction_dict_plus[key] = other.junctions_dict[key]
-                else:
-                    self.junction_dict_minus[key] = other.junctions_dict[key]
+        for k, v in other._junction_dict_plus_:
+            self._junction_dict_plus_[k] = v + self._junction_dict_plus_.get(k, 0)
+
+        for k, v in other._junction_dict_minus_:
+            self._junction_dict_minus_[k] = v + self._junction_dict_minus_.get(k, 0)
 
         return self.junctions_dict
 
     def transform(self, log_trans: str):
         funcs = {"10": np.log10, "2": np.log2, "zscore": zscore, "e": np.log}
 
         if log_trans in funcs.keys():
-            if self.plus is not None:
-                self.plus = funcs[log_trans](self.plus + 1)
+            if self._plus_ is not None:
+                self._plus_ = funcs[log_trans](self._plus_ + 1)
 
             if self.minus is not None:
-                self.minus = funcs[log_trans](self.minus + 1)
+                self._minus_ = funcs[log_trans](self._minus_ + 1)
 
     def normalize(self, size_factor: float, format_: str = "normal", read_length: float = 0):
         u"""
         Convert reads counts to cpm, fpkm or just scale with scale_factor
 
-        Inspired by `rpkm_per_region` from [MISO](https://github.com/yarden/MISO/blob/b71402188000465e3430736a11ea118fd5639a4a/misopy/sam_rpkm.py#L51)
+        Inspired by `rpkm_per_region` from
+        [MISO](https://github.com/yarden/MISO/blob/b71402188000465e3430736a11ea118fd5639a4a/misopy/sam_rpkm.py#L51)
         """
 
         if format_ == "rpkm" and read_length > 0:
             # for rpkm the size_factor is total reads
-            self.plus = np.divide(self.plus,
-                                  np.multiply((np.sum(self.plus != 0) - read_length + 1) / 1e3, size_factor / 1e6))
-            if self.minus is not None:
-                self.minus = np.divide(self.minus,
-                                       np.multiply((np.sum(self.minus != 0) - read_length + 1) / 1e3,
-                                                   size_factor / 1e6))
+            self._plus_ = np.divide(
+                self._plus_,
+                np.multiply(
+                    (np.sum(self._plus_ != 0) - read_length + 1) / 1e3,
+                    size_factor / 1e6
+                )
+            )
+            if self._minus_ is not None:
+                self._minus_ = np.divide(
+                    self._minus_,
+                    np.multiply(
+                        (np.sum(self._minus_ != 0) - read_length + 1) / 1e3,
+                        size_factor / 1e6
+                    )
+                )
             elif format_ == "cpm" and read_length > 0:
                 # for cpm the size_factor is total reads
-                self.plus = np.divide(self.plus, np.divide(size_factor, 1e6))
-                if self.minus is not None:
-                    self.minus = np.divide(self.minus, np.divide(size_factor, 1e6))
+                self._plus_ = np.divide(self._plus_, np.divide(size_factor, 1e6))
+                if self._minus_ is not None:
+                    self._minus_ = np.divide(self._minus_, np.divide(size_factor, 1e6))
         elif format_ == "cpm" and read_length > 0:
             # for cpm the size_factor is total reads
-            self.plus = np.divide(self.plus, np.divide(size_factor, 1e6))
-            if self.minus is not None:
-                self.minus = np.divide(self.minus, np.divide(size_factor, 1e6))
+            self._plus_ = np.divide(self._plus_, np.divide(size_factor, 1e6))
+            if self._minus_ is not None:
+                self._minus_ = np.divide(self._minus_, np.divide(size_factor, 1e6))
         elif size_factor is not None and size_factor > 0 and format_ == "atac":
-            self.plus = np.divide(self.plus, size_factor)  # * 100
-            if self.minus is not None:
-                self.minus = np.divide(self.minus, size_factor)
+            self._plus_ = np.divide(self._plus_, size_factor)  # * 100
+            if self._minus_ is not None:
+                self._minus_ = np.divide(self._minus_, size_factor)
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `trackplot-0.2.3/trackplot/base/Readder.py` & `trackplot-0.2.4/trackplot/base/Readder.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/Stroke.py` & `trackplot-0.2.4/trackplot/base/Stroke.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/Transcript.py` & `trackplot-0.2.4/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/base/pyUniprot.py` & `trackplot-0.2.4/trackplot/base/pyUniprot.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/cli.py` & `trackplot-0.2.4/trackplot/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
 from trackplot.plot import Plot
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def decode_region(region: str):
     regions = region.split(":")
```

### Comparing `trackplot-0.2.3/trackplot/conf/DomainSetting.py` & `trackplot-0.2.4/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/conf/config.py` & `trackplot-0.2.4/trackplot/conf/config.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/conf/drawing.py` & `trackplot-0.2.4/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/ATAC.py` & `trackplot-0.2.4/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Bam.py` & `trackplot-0.2.4/trackplot/file/Bam.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/BedGraph.py` & `trackplot-0.2.4/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Bigwig.py` & `trackplot-0.2.4/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Depth.py` & `trackplot-0.2.4/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Fasta.py` & `trackplot-0.2.4/trackplot/file/Fasta.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/File.py` & `trackplot-0.2.4/trackplot/file/File.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.4/trackplot/file/HiCMatrixTrack.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Junction.py` & `trackplot-0.2.4/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Motif.py` & `trackplot-0.2.4/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/ReadSegments.py` & `trackplot-0.2.4/trackplot/file/ReadSegments.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/file/Reference.py` & `trackplot-0.2.4/trackplot/file/Reference.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/plot.py` & `trackplot-0.2.4/trackplot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,17 @@
                 obj.load(region=region, *args, **kwargs)
         else:
             with Pool(n_jobs) as p:
                 kwargs_ = deepcopy(kwargs)
                 kwargs_["region"] = region
                 self.obj = p.map(__load__, [[o, args, kwargs_] for o in self.obj])
 
+        for obj in self.obj:
+            obj.transform()
+
         if self.type == "density":
             if len(self.obj) > 1:
                 data = self.obj[0].data
                 for obj in self.obj[1:]:
                     data += obj.data
 
                 for obj in self.obj:
@@ -1042,20 +1045,20 @@
                 self.plots = p.map(__load__, cmds)
 
         # count the plots size
         for p in self.plots:
             if n_jobs <= 1:
                 p.load(self.region, junctions=self.junctions.get(p.obj[0].label, {}), *args, **kwargs)
 
-            for obj in p.obj:
-                if isinstance(obj, ReadSegment):
-                    continue
-                if isinstance(obj, HiCTrack):
-                    continue
-                obj.transform()
+            # for obj in p.obj:
+            #     if isinstance(obj, ReadSegment):
+            #         continue
+            #     if isinstance(obj, HiCTrack):
+            #         continue
+            #     obj.transform()
 
             plots_n_rows += p.len(reference_scale)
             if p.type in ["heatmap", "hic"]:
                 plots_n_cols = 2
 
             if p.is_single_cell:
                 height_ratio.append(sc_height_ratio.get(p.type, 1))
```

### Comparing `trackplot-0.2.3/trackplot/plot_func.py` & `trackplot-0.2.4/trackplot/plot_func.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot/plot_tests.py` & `trackplot-0.2.4/trackplot/plot_tests.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.3/trackplot.egg-info/PKG-INFO` & `trackplot-0.2.4/trackplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trackplot
-Version: 0.2.3
+Version: 0.2.4
 Home-page: https://github.com/ygidtu/trackplot
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # trackplot
```

### Comparing `trackplot-0.2.3/trackplot.egg-info/SOURCES.txt` & `trackplot-0.2.4/trackplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

