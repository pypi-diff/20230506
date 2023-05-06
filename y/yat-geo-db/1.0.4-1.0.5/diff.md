# Comparing `tmp/yat_geo_db-1.0.4.tar.gz` & `tmp/yat_geo_db-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yat_geo_db-1.0.4.tar", last modified: Tue Apr  4 12:16:04 2023, max compression
+gzip compressed data, was "yat_geo_db-1.0.5.tar", last modified: Sat May  6 01:30:35 2023, max compression
```

## Comparing `yat_geo_db-1.0.4.tar` & `yat_geo_db-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 12:16:04.346107 yat_geo_db-1.0.4/
--rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4880 2023-04-04 12:16:04.345110 yat_geo_db-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4214 2023-01-17 19:31:53.000000 yat_geo_db-1.0.4/README.md
--rw-rw-rw-   0        0        0      682 2023-04-04 12:14:55.000000 yat_geo_db-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-04 12:16:04.346107 yat_geo_db-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-04-04 12:15:00.000000 yat_geo_db-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 12:16:04.328106 yat_geo_db-1.0.4/yat_geo_db/
--rw-rw-rw-   0        0        0       60 2023-01-11 17:08:33.000000 yat_geo_db-1.0.4/yat_geo_db/__init__.py
--rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.0.4/yat_geo_db/fuzzy.py
--rw-rw-rw-   0        0        0    27434 2023-04-03 22:06:35.000000 yat_geo_db-1.0.4/yat_geo_db/geo_manager.py
--rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.0.4/yat_geo_db/geometry.py
--rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.0.4/yat_geo_db/settings.py
--rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.0.4/yat_geo_db/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 12:16:04.344107 yat_geo_db-1.0.4/yat_geo_db.egg-info/
--rw-rw-rw-   0        0        0     4880 2023-04-04 12:16:04.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-04-04 12:16:04.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 12:16:04.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-04 12:16:04.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-04 12:16:04.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-11 17:08:51.000000 yat_geo_db-1.0.4/yat_geo_db.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-06 01:30:35.770799 yat_geo_db-1.0.5/
+-rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4880 2023-05-06 01:30:35.769797 yat_geo_db-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4214 2023-01-17 19:31:53.000000 yat_geo_db-1.0.5/README.md
+-rw-rw-rw-   0        0        0      682 2023-05-06 01:29:29.000000 yat_geo_db-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 01:30:35.770799 yat_geo_db-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-05-06 01:29:28.000000 yat_geo_db-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:30:35.756246 yat_geo_db-1.0.5/yat_geo_db/
+-rw-rw-rw-   0        0        0       60 2023-05-06 01:29:28.000000 yat_geo_db-1.0.5/yat_geo_db/__init__.py
+-rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.0.5/yat_geo_db/fuzzy.py
+-rw-rw-rw-   0        0        0    27434 2023-04-03 22:06:35.000000 yat_geo_db-1.0.5/yat_geo_db/geo_manager.py
+-rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.0.5/yat_geo_db/geometry.py
+-rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.0.5/yat_geo_db/settings.py
+-rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.0.5/yat_geo_db/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 01:30:35.768792 yat_geo_db-1.0.5/yat_geo_db.egg-info/
+-rw-rw-rw-   0        0        0     4880 2023-05-06 01:30:35.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-05-06 01:30:35.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 01:30:35.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-06 01:30:35.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 01:30:35.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-01-11 17:08:51.000000 yat_geo_db-1.0.5/yat_geo_db.egg-info/zip-safe
```

### Comparing `yat_geo_db-1.0.4/LICENSE` & `yat_geo_db-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.4/PKG-INFO` & `yat_geo_db-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yat_geo_db
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
```

### Comparing `yat_geo_db-1.0.4/README.md` & `yat_geo_db-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.4/pyproject.toml` & `yat_geo_db-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yat_geo_db"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
   { name="Robert Goss", email="rgoss@yat.ai" },
   { name="Jarod Hart", email="jhart@yat.ai" },
 ]
 description = "A simple and effective Python wrapper around the Open Geo DB managed by YAT"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `yat_geo_db-1.0.4/setup.py` & `yat_geo_db-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 
 install_requires = ['requests', 'numpy', 'jellyfish', 'pytz']
 
 setup(
     name='yat_geo_db',
-    version='1.0.4',
+    version='1.0.5',
     author='YAT, LLC',
     author_email='rgoss@yat.ai, jhart@yat.ai',
     packages=['yat_geo_db'],
     license="MIT",
     url='https://github.com/yat-co/yat-geo-db',
     install_requires=install_requires,
     classifiers=[
```

### Comparing `yat_geo_db-1.0.4/yat_geo_db/fuzzy.py` & `yat_geo_db-1.0.5/yat_geo_db/fuzzy.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.4/yat_geo_db/geo_manager.py` & `yat_geo_db-1.0.5/yat_geo_db/geo_manager.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.4/yat_geo_db/geometry.py` & `yat_geo_db-1.0.5/yat_geo_db/geometry.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.4/yat_geo_db.egg-info/PKG-INFO` & `yat_geo_db-1.0.5/yat_geo_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yat-geo-db
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
```

