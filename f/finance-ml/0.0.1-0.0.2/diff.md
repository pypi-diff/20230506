# Comparing `tmp/finance_ml-0.0.1.tar.gz` & `tmp/finance_ml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\finance_ml-0.0.1.tar", last modified: Sat May  6 18:41:27 2023, max compression
+gzip compressed data, was "dist\finance_ml-0.0.2.tar", last modified: Sat May  6 19:29:08 2023, max compression
```

## Comparing `finance_ml-0.0.1.tar` & `finance_ml-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:41:27.000000 finance_ml-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      556 2023-05-06 18:41:27.000000 finance_ml-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/
--rw-rw-rw-   0        0        0      556 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:41:27.000000 finance_ml-0.0.1/finance_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 18:41:27.000000 finance_ml-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-05-06 18:32:40.000000 finance_ml-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:41:27.000000 finance_ml-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 18:41:27.000000 finance_ml-0.0.1/src/finance_ml/
--rw-rw-rw-   0        0        0       53 2023-05-06 18:36:47.000000 finance_ml-0.0.1/src/finance_ml/__init__.py
--rw-rw-rw-   0        0        0       75 2023-05-06 18:23:10.000000 finance_ml-0.0.1/src/finance_ml/dataprep_ml.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-06 16:37:21.000000 finance_ml-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      603 2023-05-06 19:29:08.000000 finance_ml-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-06 16:43:18.000000 finance_ml-0.0.2/README.md
+-rw-rw-rw-   0        0        0      201 2023-05-06 16:37:21.000000 finance_ml-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:29:08.000000 finance_ml-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1128 2023-05-06 19:28:54.000000 finance_ml-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml/
+-rw-rw-rw-   0        0        0       39 2023-05-06 19:18:52.000000 finance_ml-0.0.2/src/finance_ml/__init__.py
+-rw-rw-rw-   0        0        0       75 2023-05-06 18:23:10.000000 finance_ml-0.0.2/src/finance_ml/dataprep_ml.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/
+-rw-rw-rw-   0        0        0      603 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 19:29:08.000000 finance_ml-0.0.2/src/finance_ml.egg-info/top_level.txt
```

### Comparing `finance_ml-0.0.1/PKG-INFO` & `finance_ml-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: finance_ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# Example Package
+
+Finance ml by masarac.
```

### Comparing `finance_ml-0.0.1/finance_ml.egg-info/PKG-INFO` & `finance_ml-0.0.2/src/finance_ml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: finance-ml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Application of Machine Learning in Finances
 Author: Fabio Maia
 Author-email: <fabio.masaracchia@gmail.com>
 Keywords: python,finance,mlops
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# Example Package
+
+Finance ml by masarac.
```

### Comparing `finance_ml-0.0.1/setup.py` & `finance_ml-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Application of Machine Learning in Finances'
 LONG_DESCRIPTION = 'A package that allows you to build pipelines and evaluate trading strategies, resulting in instructions to operate in the market.'
 
+
+with open("README.md", "r") as f:
+    long_description = f.read()
+
+
 # Setting up
 setup(
     name="finance_ml",
     version=VERSION,
     author="Fabio Maia",
     author_email="<fabio.masaracchia@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
-    packages=find_packages(),
+    long_description=long_description,
+    packages=find_packages(where='src'),
+    package_dir={'': 'src'},
     install_requires=['pandas', 'numpy', 'matplotlib'],
     keywords=['python', 'finance', 'mlops'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

