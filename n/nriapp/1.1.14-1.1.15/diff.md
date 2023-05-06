# Comparing `tmp/nriapp-1.1.14.tar.gz` & `tmp/nriapp-1.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.14.tar", last modified: Sat May  6 05:23:19 2023, max compression
+gzip compressed data, was "nriapp-1.1.15.tar", last modified: Sat May  6 05:26:31 2023, max compression
```

## Comparing `nriapp-1.1.14.tar` & `nriapp-1.1.15.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.297211 nriapp-1.1.14/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.14/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.14/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-05-06 05:23:19.297211 nriapp-1.1.14/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.14/README
--rw-rw-rw-   0        0        0      341 2023-05-06 05:20:19.000000 nriapp-1.1.14/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-06 05:23:19.297211 nriapp-1.1.14/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-05-06 05:20:34.000000 nriapp-1.1.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.266011 nriapp-1.1.14/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.281611 nriapp-1.1.14/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.14/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.281611 nriapp-1.1.14/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.14/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.14/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.281611 nriapp-1.1.14/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    17188 2023-05-05 05:36:38.000000 nriapp-1.1.14/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.14/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   101629 2023-04-30 17:20:44.000000 nriapp-1.1.14/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.297211 nriapp-1.1.14/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.14/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.14/src/nriapp/helper/visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-06 05:23:19.281611 nriapp-1.1.14/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-05-06 05:23:19.000000 nriapp-1.1.14/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-05-06 05:23:19.000000 nriapp-1.1.14/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 05:23:19.000000 nriapp-1.1.14/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-06 05:23:19.000000 nriapp-1.1.14/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 05:23:19.000000 nriapp-1.1.14/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    36761 2023-04-29 10:16:03.000000 nriapp-1.1.14/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.263397 nriapp-1.1.15/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.15/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.15/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-05-06 05:26:31.263397 nriapp-1.1.15/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.15/README
+-rw-rw-rw-   0        0        0      344 2023-05-06 05:25:35.000000 nriapp-1.1.15/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-06 05:26:31.263397 nriapp-1.1.15/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-05-06 05:25:51.000000 nriapp-1.1.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.122997 nriapp-1.1.15/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.185397 nriapp-1.1.15/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.15/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.200997 nriapp-1.1.15/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.15/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.15/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.232197 nriapp-1.1.15/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    17188 2023-05-05 05:36:38.000000 nriapp-1.1.15/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.15/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   101629 2023-04-30 17:20:44.000000 nriapp-1.1.15/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.263397 nriapp-1.1.15/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.15/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.15/src/nriapp/helper/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:26:31.169797 nriapp-1.1.15/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 05:26:30.000000 nriapp-1.1.15/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    36761 2023-04-29 10:16:03.000000 nriapp-1.1.15/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.14/LICENSE` & `nriapp-1.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/setup.py` & `nriapp-1.1.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.14',
+   version='1.1.15',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.14/src/nriapp/changelog.txt` & `nriapp-1.1.15/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.15/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.15/src/nriapp/core/dataexplorer.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.15/src/nriapp/core/msgraphapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.15/src/nriapp/core/mssentinelapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/multifactor.py` & `nriapp-1.1.15/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/core/vtquery.py` & `nriapp-1.1.15/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/helper/doc.py` & `nriapp-1.1.15/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/helper/login.py` & `nriapp-1.1.15/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/helper/pylog.py` & `nriapp-1.1.15/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/helper/requestheader.py` & `nriapp-1.1.15/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.15/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.14/src/nriapp/nriapp.py` & `nriapp-1.1.15/src/nriapp/nriapp.py`

 * *Files identical despite different names*

