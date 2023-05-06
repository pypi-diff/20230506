# Comparing `tmp/pyaipersonality-0.0.6.tar.gz` & `tmp/pyaipersonality-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-0.0.6.tar", last modified: Sat May  6 19:06:07 2023, max compression
+gzip compressed data, was "pyaipersonality-0.0.7.tar", last modified: Sat May  6 19:11:06 2023, max compression
```

## Comparing `pyaipersonality-0.0.6.tar` & `pyaipersonality-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.280325 pyaipersonality-0.0.6/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     9224 2023-05-06 19:06:07.279325 pyaipersonality-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8731 2023-05-06 19:04:54.000000 pyaipersonality-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.254323 pyaipersonality-0.0.6/pyaipersonality/
--rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.6/pyaipersonality/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.278323 pyaipersonality-0.0.6/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0     9224 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 19:06:07.281324 pyaipersonality-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-06 19:04:50.000000 pyaipersonality-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:11:06.256893 pyaipersonality-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     9224 2023-05-06 19:11:06.256893 pyaipersonality-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8731 2023-05-06 19:04:54.000000 pyaipersonality-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 19:11:06.240321 pyaipersonality-0.0.7/pyaipersonality/
+-rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.7/pyaipersonality/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:11:06.255430 pyaipersonality-0.0.7/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0     9224 2023-05-06 19:11:06.000000 pyaipersonality-0.0.7/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-06 19:11:06.000000 pyaipersonality-0.0.7/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:11:06.000000 pyaipersonality-0.0.7/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-06 19:11:06.000000 pyaipersonality-0.0.7/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:11:06.000000 pyaipersonality-0.0.7/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:11:06.256893 pyaipersonality-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-06 19:11:00.000000 pyaipersonality-0.0.7/setup.py
```

### Comparing `pyaipersonality-0.0.6/LICENSE` & `pyaipersonality-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.6/PKG-INFO` & `pyaipersonality-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyaipersonality-0.0.6/README.md` & `pyaipersonality-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.6/pyaipersonality/__init__.py` & `pyaipersonality-0.0.7/pyaipersonality/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.6/pyaipersonality.egg-info/PKG-INFO` & `pyaipersonality-0.0.7/pyaipersonality.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyaipersonality-0.0.6/setup.py` & `pyaipersonality-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="0.0.6",
+    version="0.0.7",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
```

