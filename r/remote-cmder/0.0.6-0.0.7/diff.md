# Comparing `tmp/remote-cmder-0.0.6.tar.gz` & `tmp/remote-cmder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-cmder-0.0.6.tar", last modified: Tue Mar 28 12:11:21 2023, max compression
+gzip compressed data, was "remote-cmder-0.0.7.tar", last modified: Sat May  6 09:15:29 2023, max compression
```

## Comparing `remote-cmder-0.0.6.tar` & `remote-cmder-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:11:21.798240 remote-cmder-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-28 12:11:21.798240 remote-cmder-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:11:21.794240 remote-cmder-0.0.6/remote_cmder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:11:21.798240 remote-cmder-0.0.6/remote_cmder/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/modules/cmder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/modules/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:11:21.798240 remote-cmder-0.0.6/remote_cmder/settings/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/settings/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/remote_cmder/settings/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:11:21.794240 remote-cmder-0.0.6/remote_cmder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-03-28 12:11:21.000000 remote-cmder-0.0.6/remote_cmder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-28 12:11:21.000000 remote-cmder-0.0.6/remote_cmder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:11:21.000000 remote-cmder-0.0.6/remote_cmder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-28 12:11:21.000000 remote-cmder-0.0.6/remote_cmder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 12:11:21.000000 remote-cmder-0.0.6/remote_cmder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:11:21.798240 remote-cmder-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-28 12:10:49.000000 remote-cmder-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/remote_cmder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/remote_cmder/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/core/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/remote_cmder/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/modules/cmder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/modules/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/remote_cmder/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/settings/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/remote_cmder/settings/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/remote_cmder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-06 09:15:28.000000 remote-cmder-0.0.7/remote_cmder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-06 09:15:28.000000 remote-cmder-0.0.7/remote_cmder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 09:15:28.000000 remote-cmder-0.0.7/remote_cmder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 09:15:28.000000 remote-cmder-0.0.7/remote_cmder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 09:15:28.000000 remote-cmder-0.0.7/remote_cmder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 09:15:29.030381 remote-cmder-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-06 09:14:55.000000 remote-cmder-0.0.7/setup.py
```

### Comparing `remote-cmder-0.0.6/LICENSE` & `remote-cmder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/PKG-INFO` & `remote-cmder-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-cmder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Remote cmder
 Home-page: https://github.com/zondatw/remote_cmder
 Author: Zonda Yang
 Author-email: u226699@gmail.com
 License: MIT
 Keywords: remote cmder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `remote-cmder-0.0.6/README.md` & `remote-cmder-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/pyproject.toml` & `remote-cmder-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/remote_cmder/cli.py` & `remote-cmder-0.0.7/remote_cmder/cli.py`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/remote_cmder/modules/cmder.py` & `remote-cmder-0.0.7/remote_cmder/modules/cmder.py`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/remote_cmder/modules/server.py` & `remote-cmder-0.0.7/remote_cmder/modules/server.py`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/remote_cmder/settings/logger.py` & `remote-cmder-0.0.7/remote_cmder/settings/logger.py`

 * *Files identical despite different names*

### Comparing `remote-cmder-0.0.6/remote_cmder.egg-info/PKG-INFO` & `remote-cmder-0.0.7/remote_cmder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remote-cmder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Remote cmder
 Home-page: https://github.com/zondatw/remote_cmder
 Author: Zonda Yang
 Author-email: u226699@gmail.com
 License: MIT
 Keywords: remote cmder
 Classifier: Programming Language :: Python :: 3
```

### Comparing `remote-cmder-0.0.6/setup.py` & `remote-cmder-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 requirements = []
 with open("requirements.txt", "r") as fh:
     for line in fh:
         requirements.append(line.strip())
 
 setuptools.setup(
     name="remote-cmder",
-    version="0.0.6",
+    version="0.0.7",
     author="Zonda Yang",
     author_email="u226699@gmail.com",
     description="Remote cmder",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zondatw/remote_cmder",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     keywords="remote cmder",
-    packages=["remote_cmder", "remote_cmder.modules", "remote_cmder.settings"],
+    packages=["remote_cmder", "remote_cmder.modules", "remote_cmder.settings", "remote_cmder.core"],
     python_requires=">=3.7",
     entry_points={
         "console_scripts": [
             "remote-cmder=remote_cmder.cli:main",
         ],
     },
     install_requires=requirements,
```

