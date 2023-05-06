# Comparing `tmp/kubernetes-square-1.3.0.tar.gz` & `tmp/kubernetes-square-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes-square-1.3.0.tar", max compression
+gzip compressed data, was "kubernetes-square-1.3.2.tar", max compression
```

## Comparing `kubernetes-square-1.3.0.tar` & `kubernetes-square-1.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes-square-1.3.0/LICENSE
--rw-r--r--   0        0        0      816 2023-04-07 04:24:51.071471 kubernetes-square-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3531 2021-09-06 17:16:58.000000 kubernetes-square-1.3.0/resources/defaultconfig.yaml
--rw-r--r--   0        0        0     1382 2023-04-07 04:24:51.071471 kubernetes-square-1.3.0/square/__init__.py
--rw-r--r--   0        0        0      203 2021-09-06 17:16:58.000000 kubernetes-square-1.3.0/square/__main__.py
--rw-r--r--   0        0        0     5095 2023-03-16 06:14:23.918379 kubernetes-square-1.3.0/square/cfgfile.py
--rw-r--r--   0        0        0     1851 2021-09-06 17:16:58.000000 kubernetes-square-1.3.0/square/dotdict.py
--rw-r--r--   0        0        0     6867 2023-03-22 01:24:34.210365 kubernetes-square-1.3.0/square/dtypes.py
--rw-r--r--   0        0        0    33744 2023-03-22 01:24:34.210365 kubernetes-square-1.3.0/square/k8s.py
--rw-r--r--   0        0        0    14924 2023-03-16 06:14:23.918379 kubernetes-square-1.3.0/square/main.py
--rw-r--r--   0        0        0    39403 2023-03-16 06:14:23.918379 kubernetes-square-1.3.0/square/manio.py
--rw-r--r--   0        0        0    29840 2023-03-16 06:14:23.918379 kubernetes-square-1.3.0/square/square.py
--rw-r--r--   0        0        0      901 2023-04-07 05:06:46.609230 kubernetes-square-1.3.0/setup.py
--rw-r--r--   0        0        0      610 2023-04-07 05:06:46.609397 kubernetes-square-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes-square-1.3.2/LICENSE
+-rw-r--r--   0        0        0      757 2023-05-06 09:05:28.381602 kubernetes-square-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3531 2021-09-06 17:16:58.000000 kubernetes-square-1.3.2/resources/defaultconfig.yaml
+-rw-r--r--   0        0        0     1382 2023-05-06 09:05:28.381602 kubernetes-square-1.3.2/square/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes-square-1.3.2/square/__main__.py
+-rw-r--r--   0        0        0     5095 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/cfgfile.py
+-rw-r--r--   0        0        0     1851 2021-09-06 17:16:58.000000 kubernetes-square-1.3.2/square/dotdict.py
+-rw-r--r--   0        0        0     6867 2023-03-22 01:24:34.210365 kubernetes-square-1.3.2/square/dtypes.py
+-rw-r--r--   0        0        0    33744 2023-03-22 01:24:34.210365 kubernetes-square-1.3.2/square/k8s.py
+-rw-r--r--   0        0        0    14924 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/main.py
+-rw-r--r--   0        0        0    39403 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/manio.py
+-rw-r--r--   0        0        0    29840 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/square.py
+-rw-r--r--   0        0        0      800 2023-05-06 09:08:47.845837 kubernetes-square-1.3.2/setup.py
+-rw-r--r--   0        0        0      485 2023-05-06 09:08:47.846128 kubernetes-square-1.3.2/PKG-INFO
```

### Comparing `kubernetes-square-1.3.0/LICENSE` & `kubernetes-square-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/pyproject.toml` & `kubernetes-square-1.3.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [tool.poetry]
 name = "kubernetes-square"
-version = "1.3.0"
+version = "1.3.2"
 description = ""
 authors = ["Oliver Nagy <olitheolix@gmail.com>"]
 packages = [
     { include = "square" },
 ]
 include = ["resources/defaultconfig.yaml"]
 
 
 [tool.poetry.dependencies]
-colorama = "^0.4.1"
-google = "^2.0"
-google-api-python-client = "^1.7"
-jsonpatch = "^1.24"
-python = "^3.10"
-pyyaml = "^5.1"
-requests = "^2.22"
-colorlog = "^4.0"
-pydantic = "^1.8"
-backoff = "^1.10.0"
+backoff = "*"
+colorama = "*"
+colorlog = "*"
+google = "*"
+google-api-python-client = "*"
+jsonpatch = "*"
+pydantic = ">=1.8"
+python = ">=3.10"
+pyyaml = "*"
+requests = "*"
 
 [tool.poetry.dev-dependencies]
-bumpversion = "^0.5.3"
-flake8 = "^3.7"
-flake8-isort = "^2.7"
-ipython = "^8.10"
-isort = "^4.3"
-pytest = "^7.2"
-pytest-cov = "^2.7"
-pytest-dotenv = "^0.4.0"
-pytest-flake8 = "^1.0"
-requests-mock = "^1.7"
-sh = "^1.12"
+bumpversion = "*"
+flake8 = "*"
+flake8-isort = "*"
+ipython = ">=8.10"
+isort = "*"
+pytest = ">=7.2"
+pytest-cov = "*"
+pytest-dotenv = "*"
+pytest-flake8 = "*"
+requests-mock = "*"
+sh = "*"
 
 [tool.poetry.scripts]
 square = 'square.main:main'
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kubernetes-square-1.3.0/resources/defaultconfig.yaml` & `kubernetes-square-1.3.2/resources/defaultconfig.yaml`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/__init__.py` & `kubernetes-square-1.3.2/square/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import sys
 
 from . import square
 from .cfgfile import load
 
-__version__ = '1.3.0'
+__version__ = '1.3.2'
 
 
 # ---------------------------------------------------------------------------
 # Global Runtime Constants
 # ---------------------------------------------------------------------------
 # Determine the base folder. This is usually the folder of this very file, but
 # will be different if we run inside a bundle produced by PyInstaller.
```

### Comparing `kubernetes-square-1.3.0/square/cfgfile.py` & `kubernetes-square-1.3.2/square/cfgfile.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/dotdict.py` & `kubernetes-square-1.3.2/square/dotdict.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/dtypes.py` & `kubernetes-square-1.3.2/square/dtypes.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/k8s.py` & `kubernetes-square-1.3.2/square/k8s.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/main.py` & `kubernetes-square-1.3.2/square/main.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/manio.py` & `kubernetes-square-1.3.2/square/manio.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/square/square.py` & `kubernetes-square-1.3.2/square/square.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.0/setup.py` & `kubernetes-square-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 packages = \
 ['square']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['backoff>=1.10.0,<2.0.0',
- 'colorama>=0.4.1,<0.5.0',
- 'colorlog>=4.0,<5.0',
- 'google-api-python-client>=1.7,<2.0',
- 'google>=2.0,<3.0',
- 'jsonpatch>=1.24,<2.0',
- 'pydantic>=1.8,<2.0',
- 'pyyaml>=5.1,<6.0',
- 'requests>=2.22,<3.0']
+['backoff',
+ 'colorama',
+ 'colorlog',
+ 'google',
+ 'google-api-python-client',
+ 'jsonpatch',
+ 'pydantic>=1.8',
+ 'pyyaml',
+ 'requests']
 
 entry_points = \
 {'console_scripts': ['square = square.main:main']}
 
 setup_kwargs = {
     'name': 'kubernetes-square',
-    'version': '1.3.0',
+    'version': '1.3.2',
     'description': '',
     'long_description': None,
     'author': 'Oliver Nagy',
     'author_email': 'olitheolix@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
+    'python_requires': '>=3.10',
 }
 
 
 setup(**setup_kwargs)
```

