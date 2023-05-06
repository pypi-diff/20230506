# Comparing `tmp/superscreen-0.8.1.tar.gz` & `tmp/superscreen-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superscreen-0.8.1.tar", last modified: Mon Apr  3 20:50:51 2023, max compression
+gzip compressed data, was "superscreen-0.8.2.tar", last modified: Sat May  6 18:47:15 2023, max compression
```

## Comparing `superscreen-0.8.1.tar` & `superscreen-0.8.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.141297 superscreen-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-03 20:50:41.000000 superscreen-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-03 20:50:51.141297 superscreen-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-03 20:50:41.000000 superscreen-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:50:51.141297 superscreen-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-04-03 20:50:42.000000 superscreen-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.133297 superscreen-0.8.1/superscreen/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.137297 superscreen-0.8.1/superscreen/device/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26205 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/device/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    46147 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/device/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/device/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/fem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    41663 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.137297 superscreen-0.8.1/superscreen/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/sources/current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/sources/dipole.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/sources/vortex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.141297 superscreen-0.8.1/superscreen/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    18608 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/units.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38166 2023-04-03 20:50:42.000000 superscreen-0.8.1/superscreen/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:50:51.137297 superscreen-0.8.1/superscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-03 20:50:51.000000 superscreen-0.8.1/superscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-03 20:50:51.000000 superscreen-0.8.1/superscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:50:51.000000 superscreen-0.8.1/superscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-03 20:50:51.000000 superscreen-0.8.1/superscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 20:50:51.000000 superscreen-0.8.1/superscreen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-06 18:47:03.000000 superscreen-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 18:47:15.049204 superscreen-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-06 18:47:03.000000 superscreen-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:47:15.049204 superscreen-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-06 18:47:03.000000 superscreen-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.045204 superscreen-0.8.2/superscreen/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26205 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46147 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11042 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/device/transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15052 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/fem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21535 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48459 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/dipole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/sources/vortex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.049204 superscreen-0.8.2/superscreen/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7810 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38166 2023-05-06 18:47:03.000000 superscreen-0.8.2/superscreen/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:47:15.045204 superscreen-0.8.2/superscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 18:47:14.000000 superscreen-0.8.2/superscreen.egg-info/top_level.txt
```

### Comparing `superscreen-0.8.1/LICENSE` & `superscreen-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/PKG-INFO` & `superscreen-0.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.8.1
+Version: 0.8.2
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
@@ -18,17 +18,18 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: jax
 License-File: LICENSE
 
 
 # SuperScreen
```

### Comparing `superscreen-0.8.1/README.md` & `superscreen-0.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 Click the badge below and navigate to `docs/notebooks/` to try `SuperScreen` interactively online via [Binder](https://mybinder.org/):
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/loganbvh/superscreen/HEAD)
 
 ## Install `SuperScreen`
 
-`SuperScreen` requires `python >=3.7, <3.10`. We recommend installing `SuperScreen` in a fresh [`conda` environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). For more details, see the [documentation](https://superscreen.readthedocs.io/en/latest/).
+`SuperScreen` requires `python >=3.7, <3.11`. We recommend installing `SuperScreen` in a fresh [`conda` environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html). For more details, see the [documentation](https://superscreen.readthedocs.io/en/latest/).
 
 ### Install via `pip`
 
 From [PyPI](https://pypi.org/project/superscreen/), the Python Package Index:
 
 ```bash
 pip install superscreen
```

### Comparing `superscreen-0.8.1/setup.py` & `superscreen-0.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 LONG_DESCRIPTION = __doc__
 
 NAME = "superscreen"
 AUTHOR = "Logan Bishop-Van Horn"
 AUTHOR_EMAIL = "logan.bvh@gmail.com"
 URL = "https://github.com/loganbvh/superscreen"
 LICENSE = "MIT"
-PYTHON_VERSION = ">=3.7, <3.10"
+PYTHON_VERSION = ">=3.7, <3.11"
 
 INSTALL_REQUIRES = [
     "dill",
     "ipython",
     "joblib",
     "jupyter",
     "matplotlib",
@@ -73,14 +73,15 @@
 Operating System :: POSIX
 Operating System :: Unix
 Operating System :: Microsoft :: Windows
 Programming Language :: Python
 Programming Language :: Python :: 3.7
 Programming Language :: Python :: 3.8
 Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
 Topic :: Scientific/Engineering
 Topic :: Scientific/Engineering :: Physics
 """
 
 CLASSIFIERS = [line for line in CLASSIFIERS.splitlines() if line]
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "superconductor meissner screening"
```

### Comparing `superscreen-0.8.1/superscreen/__init__.py` & `superscreen-0.8.2/superscreen/__init__.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/about.py` & `superscreen-0.8.2/superscreen/about.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/device/components.py` & `superscreen-0.8.2/superscreen/device/components.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/device/device.py` & `superscreen-0.8.2/superscreen/device/device.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/device/mesh.py` & `superscreen-0.8.2/superscreen/device/mesh.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/device/transport.py` & `superscreen-0.8.2/superscreen/device/transport.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/fem.py` & `superscreen-0.8.2/superscreen/fem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import warnings
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import scipy.linalg as la
 import scipy.sparse as sp
 from matplotlib.path import Path
-from scipy.spatial.distance import cdist
 
 
 def in_polygon(
     poly_points: np.ndarray,
     query_points: np.ndarray,
     radius: float = 0,
 ) -> Union[bool, np.ndarray]:
@@ -413,32 +412,7 @@
             / (la.norm(vec1, axis=1) * la.norm(vec2, axis=1))
         )
         weights /= weights.sum()
         assert (weights > 0).all()
         gx[i, :] = np.einsum("i, ij -> j", weights, Gx[t, :])
         gy[i, :] = np.einsum("i, ij -> j", weights, Gy[t, :])
     return sp.csr_matrix(gx), sp.csr_matrix(gy)
-
-
-def cdist_batched(
-    XA: np.ndarray, XB: np.ndarray, *, batch_size: int = 0, **kwargs
-) -> np.ndarray:
-    """A batched version of scipy.spatial.distance.cdist.
-
-    The batching is performed over the second input array, XB. See the docs
-    for scipy.spatial.distance.cdist for keyword argument options.
-
-    Args:
-        XA: An mA by n array of mA original observations in an n-dimensional space.
-        XB: An mB by n array of mB original observations in an n-dimensional space.
-        batch_size: The maximum size of each batch of XB values.
-            Setting batch_size <= 0 results in no batching.
-
-    Returns:
-        An mA by mB distance matrix.
-    """
-    if "out" in kwargs:
-        raise ValueError("cdist_batched does not support the 'out' keyword argument.")
-    if batch_size <= 0:
-        return cdist(XA, XB, **kwargs)
-    batches = np.array_split(XB, range(batch_size, XB.shape[0], batch_size))
-    return np.concatenate([cdist(XA, batch) for batch in batches], axis=1)
```

### Comparing `superscreen-0.8.1/superscreen/fluxoid.py` & `superscreen-0.8.2/superscreen/fluxoid.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/geometry.py` & `superscreen-0.8.2/superscreen/geometry.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/io.py` & `superscreen-0.8.2/superscreen/io.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/parallel.py` & `superscreen-0.8.2/superscreen/parallel.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/parameter.py` & `superscreen-0.8.2/superscreen/parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/solution.py` & `superscreen-0.8.2/superscreen/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple, Union
 
 import dill
 import matplotlib.pyplot as plt
 import numpy as np
 import pint
 from scipy import interpolate
+from scipy.spatial.distance import cdist
 
 from .about import version_dict
 from .device import Device, Polygon
-from .fem import cdist_batched, in_polygon
+from .fem import in_polygon
 from .parameter import Constant
 from .sources.current import biot_savart_2d
 
 logger = logging.getLogger(__name__)
 
 
 class Vortex(NamedTuple):
@@ -733,15 +734,14 @@
         self,
         positions: np.ndarray,
         *,
         zs: Optional[Union[float, np.ndarray]] = None,
         units: Optional[str] = None,
         with_units: bool = True,
         return_sum: bool = True,
-        batch_size: int = 0,
     ) -> Union[np.ndarray, Dict[str, np.ndarray]]:
         """Calculates the vector potential due to currents in the device at any
         point(s) in space. Note that this only considers the vector potential
         due to currents in the device, so only represents the total vector potential
         in cases where the applied field is zero (e.g. models with only vortices and/or
         circulating currents).
 
@@ -763,16 +763,14 @@
                 the fields are calculated in a plane parallel to the x-y plane.
                 If zs is any array, then it must be same length as positions.
             units: Units to which to convert the vector potential.
             with_units: Whether to return the vector potential as a ``pint.Quantity``
                 with units attached.
             return_sum: Whether to return the sum of the potential from all layers in
                 the device, or a dict of ``{layer_name: potential_from_layer}``.
-            batch_size: The maximum size of each batch of positions.
-                See :func:`superscreen.fem.cdist_batched`.
 
         Returns:
             An np.ndarray if return_sum is True, otherwise a dict of
             ``{layer_name: potential_from_layer}``. If with_units is True, then the
             array(s) will contain pint.Quantities. ``potential_from_layer`` will have
             shape ``(m, 3)``.
         """
@@ -797,17 +795,15 @@
             # constant zs
             zs = zs * np.ones(positions.shape[0], dtype=dtype)
         if not isinstance(zs, np.ndarray):
             raise ValueError(f"Expected zs to be an ndarray, but got {type(zs)}.")
         if zs.ndim == 1:
             # We need zs to be shape (m, 1)
             zs = zs[:, np.newaxis]
-        rho2 = cdist_batched(
-            positions, points, batch_size=batch_size, metric="sqeuclidean"
-        ).astype(dtype, copy=False)
+        rho2 = cdist(positions, points, metric="sqeuclidean").astype(dtype, copy=False)
         # Compute the vector potential at the specified positions
         # from the currents in each layer
         vector_potentials = {}
         for name, layer in device.layers.items():
             dz = zs - layer.z0
             if np.any(dz == 0):
                 raise ValueError(
```

### Comparing `superscreen-0.8.1/superscreen/solve.py` & `superscreen-0.8.2/superscreen/solve.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/sources/constant.py` & `superscreen-0.8.2/superscreen/sources/constant.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/sources/current.py` & `superscreen-0.8.2/superscreen/sources/current.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/sources/dipole.py` & `superscreen-0.8.2/superscreen/sources/dipole.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/sources/vortex.py` & `superscreen-0.8.2/superscreen/sources/vortex.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_device.py` & `superscreen-0.8.2/superscreen/test/test_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     smaller = sc.geometry.circle(radius - 0.01)
     bigger = sc.geometry.circle(radius + 0.01)
     assert polygon.on_boundary(smaller, radius=0.1).all()
     assert polygon.on_boundary(bigger, radius=0.1).all()
     assert not polygon.on_boundary(smaller, radius=0.001).any()
     assert not polygon.on_boundary(bigger, radius=0.001).any()
-    assert polygon.on_boundary(smaller, index=True).dtype is np.dtype(int)
+    assert issubclass(polygon.on_boundary(smaller, index=True).dtype.type, np.integer)
 
 
 def test_polygon_join():
     square1 = sc.Polygon(points=sc.geometry.box(1))
     square2 = sc.Polygon(points=sc.geometry.translate(sc.geometry.box(1), 0.5, 0.5))
     square3 = sc.geometry.box(1, center=(-0.25, 0.25))
     name = "name"
```

### Comparing `superscreen-0.8.1/superscreen/test/test_io.py` & `superscreen-0.8.2/superscreen/test/test_io.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_parallel.py` & `superscreen-0.8.2/superscreen/test/test_parallel.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_parameter.py` & `superscreen-0.8.2/superscreen/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_solution.py` & `superscreen-0.8.2/superscreen/test/test_solution.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_solve.py` & `superscreen-0.8.2/superscreen/test/test_solve.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_sources.py` & `superscreen-0.8.2/superscreen/test/test_sources.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_transport.py` & `superscreen-0.8.2/superscreen/test/test_transport.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/test/test_visualization.py` & `superscreen-0.8.2/superscreen/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen/visualization.py` & `superscreen-0.8.2/superscreen/visualization.py`

 * *Files identical despite different names*

### Comparing `superscreen-0.8.1/superscreen.egg-info/PKG-INFO` & `superscreen-0.8.2/superscreen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superscreen
-Version: 0.8.1
+Version: 0.8.2
 Summary: SuperScreen: simulate Meissner screening in 2D superconducting devices.
 Home-page: https://github.com/loganbvh/superscreen
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor meissner screening
 Platform: Linux
@@ -18,17 +18,18 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.7, <3.11
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: jax
 License-File: LICENSE
 
 
 # SuperScreen
```

### Comparing `superscreen-0.8.1/superscreen.egg-info/SOURCES.txt` & `superscreen-0.8.2/superscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

