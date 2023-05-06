# Comparing `tmp/roberto-2.0.3.tar.gz` & `tmp/roberto-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roberto-2.0.3.tar", last modified: Mon Jun 13 09:01:10 2022, max compression
+gzip compressed data, was "roberto-2.0.4.tar", last modified: Sat May  6 17:17:40 2023, max compression
```

## Comparing `roberto-2.0.3.tar` & `roberto-2.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:10.649933 roberto-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-06-13 09:01:07.000000 roberto-2.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-13 09:01:07.000000 roberto-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-06-13 09:01:10.649933 roberto-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5178 2022-06-13 09:01:07.000000 roberto-2.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:10.649933 roberto-2.0.3/roberto/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-06-13 09:00:50.000000 roberto-2.0.3/roberto/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    14026 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/default_config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/program.py
--rw-r--r--   0 runner    (1001) docker     (121)    10100 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4795 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:10.649933 roberto-2.0.3/roberto/test/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/test/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     9536 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9812 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/testenvs.py
--rw-r--r--   0 runner    (1001) docker     (121)    15439 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     7112 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/venv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-13 09:01:07.000000 roberto-2.0.3/roberto/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-13 09:01:10.649933 roberto-2.0.3/roberto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5884 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-13 09:01:10.000000 roberto-2.0.3/roberto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-13 09:01:10.649933 roberto-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2593 2022-06-13 09:01:07.000000 roberto-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:40.961856 roberto-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-06 17:17:39.000000 roberto-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 17:17:39.000000 roberto-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-06 17:17:40.961856 roberto-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-06 17:17:39.000000 roberto-2.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:40.961856 roberto-2.0.4/roberto/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-06 17:17:28.000000 roberto-2.0.4/roberto/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/default_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:40.961856 roberto-2.0.4/roberto/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/test/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/testenvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-06 17:17:39.000000 roberto-2.0.4/roberto/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:17:40.961856 roberto-2.0.4/roberto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-06 17:17:40.000000 roberto-2.0.4/roberto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:17:40.961856 roberto-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2620 2023-05-06 17:17:39.000000 roberto-2.0.4/setup.py
```

### Comparing `roberto-2.0.3/LICENSE.txt` & `roberto-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/PKG-INFO` & `roberto-2.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: roberto
-Version: 2.0.3
+Version: 2.0.4
 Summary: Collection of configurable development workflows
 Home-page: https://github.com/theochem/roberto
 Author: HORTON-ChemTools Dev Team
 Author-email: horton.chemtools@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://travis-ci.com/theochem/roberto.svg?branch=master
     :target: https://travis-ci.com/theochem/roberto
 .. image:: https://anaconda.org/theochem/roberto/badges/version.svg
     :target: https://anaconda.org/theochem/roberto
 .. image:: https://codecov.io/gh/theochem/roberto/branch/master/graph/badge.svg
@@ -65,15 +66,15 @@
 the remaining tasks. These remaining tasks (4-10) are configurable and can be
 changed to work for Python and/or CMake projects.
 
 
 Installation
 ============
 
-Python 3 (>=3.6) must be installed. Other dependencies will be pulled in with
+Python 3 (>=3.7) must be installed. Other dependencies will be pulled in with
 the instructions below.
 
 Roberto can be installed with conda:
 
 .. code-block:: bash
 
     conda install theochem::roberto
```

### Comparing `roberto-2.0.3/README.rst` & `roberto-2.0.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 the remaining tasks. These remaining tasks (4-10) are configurable and can be
 changed to work for Python and/or CMake projects.
 
 
 Installation
 ============
 
-Python 3 (>=3.6) must be installed. Other dependencies will be pulled in with
+Python 3 (>=3.7) must be installed. Other dependencies will be pulled in with
 the instructions below.
 
 Roberto can be installed with conda:
 
 .. code-block:: bash
 
     conda install theochem::roberto
```

### Comparing `roberto-2.0.3/roberto/__init__.py` & `roberto-2.0.4/roberto/__init__.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/__main__.py` & `roberto-2.0.4/roberto/__main__.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/config.py` & `roberto-2.0.4/roberto/config.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/default_config.yaml` & `roberto-2.0.4/roberto/default_config.yaml`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/program.py` & `roberto-2.0.4/roberto/program.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/requirements.py` & `roberto-2.0.4/roberto/requirements.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/tasks.py` & `roberto-2.0.4/roberto/tasks.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/test/__init__.py` & `roberto-2.0.4/roberto/test/__init__.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/test/test_requirements.py` & `roberto-2.0.4/roberto/test/test_requirements.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import os
 
 from ..requirements import compute_req_hash
 
 
 def test_req_hash(tmpdir):
-    tmpdir = str(tmpdir)  # for python-3.5 compatibility
     req_items = set(["conda-build", "anaconda-client", "conda-verify"])
     # Use a fake but safe recipe dir
     fn_foo = os.path.join(tmpdir, "foo")
     with open(fn_foo, "w") as f:
         f.write("bar")
     req_fns = set([fn_foo])
     hash1 = compute_req_hash(req_items, req_fns)
```

### Comparing `roberto-2.0.3/roberto/test/test_utils.py` & `roberto-2.0.4/roberto/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/testenvs.py` & `roberto-2.0.4/roberto/testenvs.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/tools.py` & `roberto-2.0.4/roberto/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
     def execute(self, ctx, package, fmtkwargs):
         """Execute the tool for a given package."""
         if ctx.absolute:
             on_merge_branch = True
         else:
             result = ctx.run(f'git diff {ctx.git.merge_branch}..HEAD --stat', hide='out')
-            on_merge_branch = (result.stdout.strip() == "")
+            on_merge_branch = result.stdout.strip() == ""
         if on_merge_branch:
             self._run_commands(ctx, package, fmtkwargs, self.commands_master)
         else:
             self._run_commands(ctx, package, fmtkwargs, self.commands_feature)
 
 
 class LintStatic(Lint):
```

### Comparing `roberto-2.0.3/roberto/utils.py` & `roberto-2.0.4/roberto/utils.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto/version.py` & `roberto-2.0.4/roberto/version.py`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/roberto.egg-info/PKG-INFO` & `roberto-2.0.4/roberto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: roberto
-Version: 2.0.3
+Version: 2.0.4
 Summary: Collection of configurable development workflows
 Home-page: https://github.com/theochem/roberto
 Author: HORTON-ChemTools Dev Team
 Author-email: horton.chemtools@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
 License-File: LICENSE.txt
 
 .. image:: https://travis-ci.com/theochem/roberto.svg?branch=master
     :target: https://travis-ci.com/theochem/roberto
 .. image:: https://anaconda.org/theochem/roberto/badges/version.svg
     :target: https://anaconda.org/theochem/roberto
 .. image:: https://codecov.io/gh/theochem/roberto/branch/master/graph/badge.svg
@@ -65,15 +66,15 @@
 the remaining tasks. These remaining tasks (4-10) are configurable and can be
 changed to work for Python and/or CMake projects.
 
 
 Installation
 ============
 
-Python 3 (>=3.6) must be installed. Other dependencies will be pulled in with
+Python 3 (>=3.7) must be installed. Other dependencies will be pulled in with
 the instructions below.
 
 Roberto can be installed with conda:
 
 .. code-block:: bash
 
     conda install theochem::roberto
```

### Comparing `roberto-2.0.3/roberto.egg-info/SOURCES.txt` & `roberto-2.0.4/roberto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roberto-2.0.3/setup.py` & `roberto-2.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,56 +28,53 @@
     ./setup.py install --user
 """
 
 import os
 
 from setuptools import setup
 
-
-NAME = 'roberto'
+NAME = "roberto"
 
 
 def get_version_info():
     """Read __version__ and DEV_CLASSIFIER from version.py, using exec, not import."""
-    with open(os.path.join(NAME, 'version.py'), 'r') as f:
+    with open(os.path.join(NAME, "version.py"), "r") as f:
         myglobals = {"__name__": f"{NAME}.version"}
         exec(f.read(), myglobals)  # pylint: disable=exec-used
-    return myglobals['__version__'], myglobals['DEV_CLASSIFIER']
+    return myglobals["__version__"], myglobals["DEV_CLASSIFIER"]
 
 
 def load_readme():
     """Load README for display on PyPI."""
-    with open('README.rst') as f:
+    with open("README.rst") as f:
         return f.read()
 
 
 VERSION, DEV_CLASSIFIER = get_version_info()
 
 
 setup(
     name=NAME,
     version=VERSION,
     package_dir={NAME: NAME},
-    packages=[NAME, NAME + '.test'],
-    description='Collection of configurable development workflows',
+    packages=[NAME, NAME + ".test"],
+    description="Collection of configurable development workflows",
     long_description=load_readme(),
-    author='HORTON-ChemTools Dev Team',
-    author_email='horton.chemtools@gmail.com',
-    url='https://github.com/theochem/roberto',
+    author="HORTON-ChemTools Dev Team",
+    author_email="horton.chemtools@gmail.com",
+    url="https://github.com/theochem/roberto",
     include_package_data=True,
-    install_requires=[
-        'invoke', 'pyyaml', 'importlib_resources; python_version < "3.7"'],
-    python_requires='>=3.6',
-    entry_points={
-        'console_scripts': ['rob = roberto.__main__:main']
-    },
+    install_requires=["invoke", "pyyaml", 'importlib_resources; python_version < "3.7"'],
+    python_requires=">=3.7",
+    entry_points={"console_scripts": ["rob = roberto.__main__:main"]},
     classifiers=[
         DEV_CLASSIFIER,
-        'Environment :: Console',
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Operating System :: POSIX :: Linux',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Environment :: Console",
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Operating System :: POSIX :: Linux",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

