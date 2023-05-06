# Comparing `tmp/LogAssist-1.0.6.tar.gz` & `tmp/LogAssist-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.6.tar", last modified: Sat May  6 03:08:48 2023, max compression
+gzip compressed data, was "LogAssist-1.0.7.tar", last modified: Sat May  6 04:39:56 2023, max compression
```

## Comparing `LogAssist-1.0.6.tar` & `LogAssist-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.334051 LogAssist-1.0.6/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.321787 LogAssist-1.0.6/LogAssist/
--rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.6/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     6990 2023-05-06 03:07:24.000000 LogAssist-1.0.6/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-06 03:08:48.330517 LogAssist-1.0.6/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2441 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-06 03:08:48.000000 LogAssist-1.0.6/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-06 03:08:47.000000 LogAssist-1.0.6/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2441 2023-05-06 03:08:48.332546 LogAssist-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1756 2023-05-06 02:59:35.000000 LogAssist-1.0.6/README.md
--rw-rw-rw-   0        0        0      709 2023-05-06 03:08:32.000000 LogAssist-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 03:08:48.335057 LogAssist-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-06 03:08:39.000000 LogAssist-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:39:56.719015 LogAssist-1.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-06 04:39:56.692005 LogAssist-1.0.7/LogAssist/
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.7/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     6966 2023-05-06 04:36:35.000000 LogAssist-1.0.7/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-06 04:39:56.712013 LogAssist-1.0.7/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0      792 2023-05-06 04:39:56.000000 LogAssist-1.0.7/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-06 04:39:56.000000 LogAssist-1.0.7/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 04:39:56.000000 LogAssist-1.0.7/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-06 04:39:56.000000 LogAssist-1.0.7/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      792 2023-05-06 04:39:56.718009 LogAssist-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1756 2023-05-06 02:59:35.000000 LogAssist-1.0.7/README.md
+-rw-rw-rw-   0        0        0      685 2023-05-06 04:39:13.000000 LogAssist-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 04:39:56.719015 LogAssist-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      848 2023-05-06 04:39:07.000000 LogAssist-1.0.7/setup.py
```

### Comparing `LogAssist-1.0.6/LICENSE` & `LogAssist-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.6/README.md` & `LogAssist-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.6/pyproject.toml` & `LogAssist-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "LogAssist"
-version = "1.0.6"
-authors = [
-  { name="horrible", email="shinjpn1@gmail.com" },
-]
-description = "A simple and customizable logging library for Python."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-keywords=['LogAssist', 'Log Assist', 'logassist', 'log assist',  'Logger',  'logger']
-
-
-[project.urls]
-"Homepage" = "https://github.com/horrible-gh/Logger"
-"Bug Tracker" = "https://github.com/horrible-gh/Logger/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "LogAssist"
+version = "1.0.7"
+authors = [
+  { name="horrible", email="shinjpn1@gmail.com" },
+]
+description = "A simple and customizable logging library for Python."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+keywords=['LogAssist', 'Log Assist', 'logassist', 'log assist',  'Logger',  'logger']
+
+
+[project.urls]
+"Homepage" = "https://github.com/horrible-gh/Logger"
+"Bug Tracker" = "https://github.com/horrible-gh/Logger/issues"
```

### Comparing `LogAssist-1.0.6/setup.py` & `LogAssist-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-
-setup(
-    name='LogAssist',
-    version='1.0.6',
-    description='LogAssist package',
-    author='horrible-gh',
-    author_email='shinjpn1@gmail.com',
-    url='https://github.com/horrible-gh/LogAssist.git',
-    packages=find_packages(),
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    python_requires='>=3.6',
-    install_requires=[
-    ],
-)
+from setuptools import setup, find_packages
+
+setup(
+    name='LogAssist',
+    version='1.0.7',
+    description='LogAssist package',
+    author='horrible-gh',
+    author_email='shinjpn1@gmail.com',
+    url='https://github.com/horrible-gh/LogAssist.git',
+    packages=find_packages(),
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    python_requires='>=3.6',
+    install_requires=[
+    ],
+)
```

