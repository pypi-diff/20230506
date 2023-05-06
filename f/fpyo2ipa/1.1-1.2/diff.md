# Comparing `tmp/fpyo2ipa-1.1.tar.gz` & `tmp/fpyo2ipa-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpyo2ipa-1.1.tar", last modified: Fri May  5 18:30:43 2023, max compression
+gzip compressed data, was "fpyo2ipa-1.2.tar", last modified: Sat May  6 09:34:17 2023, max compression
```

## Comparing `fpyo2ipa-1.1.tar` & `fpyo2ipa-1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.347428 fpyo2ipa-1.1/
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-05-05 13:41:18.000000 fpyo2ipa-1.1/LICENSE
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)       83 2023-05-05 17:56:02.000000 fpyo2ipa-1.1/MANIFEST.in
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-05 18:30:43.347298 fpyo2ipa-1.1/PKG-INFO
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:19:31.000000 fpyo2ipa-1.1/README.md
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.344795 fpyo2ipa-1.1/fpyo2ipa/
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.346044 fpyo2ipa-1.1/fpyo2ipa/Tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:29.000000 fpyo2ipa-1.1/fpyo2ipa/Tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      124 2023-05-05 13:35:04.000000 fpyo2ipa-1.1/fpyo2ipa/Tools/check_system.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      137 2023-05-05 13:33:33.000000 fpyo2ipa-1.1/fpyo2ipa/Tools/check_venv.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1240 2023-05-05 18:19:29.000000 fpyo2ipa-1.1/fpyo2ipa/Tools/unzip_assets.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:02.000000 fpyo2ipa-1.1/fpyo2ipa/__init__.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.346319 fpyo2ipa-1.1/fpyo2ipa/assets/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:13.000000 fpyo2ipa-1.1/fpyo2ipa/assets/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)   478515 2023-05-05 18:20:02.000000 fpyo2ipa-1.1/fpyo2ipa/assets/pyo2ipadist.zip
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.347084 fpyo2ipa-1.1/fpyo2ipa/beeware_tools/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:20.000000 fpyo2ipa-1.1/fpyo2ipa/beeware_tools/__init__.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     2427 2023-05-05 18:21:36.000000 fpyo2ipa-1.1/fpyo2ipa/beeware_tools/edit_beeware_project.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)     1906 2023-05-05 18:27:44.000000 fpyo2ipa-1.1/fpyo2ipa/beeware_tools/the_app_py.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-05-05 14:43:41.000000 fpyo2ipa-1.1/fpyo2ipa/beeware_tools/the_localhost_py.py
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      593 2023-05-05 17:19:11.000000 fpyo2ipa-1.1/fpyo2ipa/build.py
-drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 18:30:43.345554 fpyo2ipa-1.1/fpyo2ipa.egg-info/
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-05 18:30:43.000000 fpyo2ipa-1.1/fpyo2ipa.egg-info/PKG-INFO
--rw-r--r--   0 yousifaladwani   (501) staff       (20)      591 2023-05-05 18:30:43.000000 fpyo2ipa-1.1/fpyo2ipa.egg-info/SOURCES.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-05 18:30:43.000000 fpyo2ipa-1.1/fpyo2ipa.egg-info/dependency_links.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       10 2023-05-05 18:30:43.000000 fpyo2ipa-1.1/fpyo2ipa.egg-info/requires.txt
--rw-r--r--   0 yousifaladwani   (501) staff       (20)        9 2023-05-05 18:30:43.000000 fpyo2ipa-1.1/fpyo2ipa.egg-info/top_level.txt
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-05 17:49:16.000000 fpyo2ipa-1.1/pyproject.toml
--rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-05 18:30:43.347473 fpyo2ipa-1.1/setup.cfg
--rw-rw-r--   0 yousifaladwani   (501) staff       (20)      611 2023-05-05 18:30:34.000000 fpyo2ipa-1.1/setup.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.097716 fpyo2ipa-1.2/
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)     1071 2023-05-05 13:41:18.000000 fpyo2ipa-1.2/LICENSE
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)       83 2023-05-05 17:56:02.000000 fpyo2ipa-1.2/MANIFEST.in
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-06 09:34:17.097558 fpyo2ipa-1.2/PKG-INFO
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:19:31.000000 fpyo2ipa-1.2/README.md
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.093869 fpyo2ipa-1.2/fpyo2ipa/
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.095151 fpyo2ipa-1.2/fpyo2ipa/Tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:29.000000 fpyo2ipa-1.2/fpyo2ipa/Tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      124 2023-05-05 13:35:04.000000 fpyo2ipa-1.2/fpyo2ipa/Tools/check_system.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      137 2023-05-05 13:33:33.000000 fpyo2ipa-1.2/fpyo2ipa/Tools/check_venv.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1240 2023-05-05 18:19:29.000000 fpyo2ipa-1.2/fpyo2ipa/Tools/unzip_assets.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:02.000000 fpyo2ipa-1.2/fpyo2ipa/__init__.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.095446 fpyo2ipa-1.2/fpyo2ipa/assets/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:13.000000 fpyo2ipa-1.2/fpyo2ipa/assets/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)   478515 2023-05-05 18:20:02.000000 fpyo2ipa-1.2/fpyo2ipa/assets/pyo2ipadist.zip
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.097128 fpyo2ipa-1.2/fpyo2ipa/beeware_tools/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        0 2023-05-05 17:43:20.000000 fpyo2ipa-1.2/fpyo2ipa/beeware_tools/__init__.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     2427 2023-05-05 18:21:36.000000 fpyo2ipa-1.2/fpyo2ipa/beeware_tools/edit_beeware_project.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)     1906 2023-05-05 18:27:44.000000 fpyo2ipa-1.2/fpyo2ipa/beeware_tools/the_app_py.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      977 2023-05-05 14:43:41.000000 fpyo2ipa-1.2/fpyo2ipa/beeware_tools/the_localhost_py.py
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      593 2023-05-05 17:19:11.000000 fpyo2ipa-1.2/fpyo2ipa/build.py
+drwxr-xr-x   0 yousifaladwani   (501) staff       (20)        0 2023-05-06 09:34:17.094579 fpyo2ipa-1.2/fpyo2ipa.egg-info/
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      352 2023-05-06 09:34:17.000000 fpyo2ipa-1.2/fpyo2ipa.egg-info/PKG-INFO
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)      591 2023-05-06 09:34:17.000000 fpyo2ipa-1.2/fpyo2ipa.egg-info/SOURCES.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        1 2023-05-06 09:34:17.000000 fpyo2ipa-1.2/fpyo2ipa.egg-info/dependency_links.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       18 2023-05-06 09:34:17.000000 fpyo2ipa-1.2/fpyo2ipa.egg-info/requires.txt
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)        9 2023-05-06 09:34:17.000000 fpyo2ipa-1.2/fpyo2ipa.egg-info/top_level.txt
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      103 2023-05-05 17:49:16.000000 fpyo2ipa-1.2/pyproject.toml
+-rw-r--r--   0 yousifaladwani   (501) staff       (20)       38 2023-05-06 09:34:17.097758 fpyo2ipa-1.2/setup.cfg
+-rw-rw-r--   0 yousifaladwani   (501) staff       (20)      619 2023-05-06 09:33:29.000000 fpyo2ipa-1.2/setup.py
```

### Comparing `fpyo2ipa-1.1/LICENSE` & `fpyo2ipa-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/Tools/unzip_assets.py` & `fpyo2ipa-1.2/fpyo2ipa/Tools/unzip_assets.py`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/assets/pyo2ipadist.zip` & `fpyo2ipa-1.2/fpyo2ipa/assets/pyo2ipadist.zip`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/beeware_tools/edit_beeware_project.py` & `fpyo2ipa-1.2/fpyo2ipa/beeware_tools/edit_beeware_project.py`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/beeware_tools/the_app_py.py` & `fpyo2ipa-1.2/fpyo2ipa/beeware_tools/the_app_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/beeware_tools/the_localhost_py.py` & `fpyo2ipa-1.2/fpyo2ipa/beeware_tools/the_localhost_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa/build.py` & `fpyo2ipa-1.2/fpyo2ipa/build.py`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/fpyo2ipa.egg-info/SOURCES.txt` & `fpyo2ipa-1.2/fpyo2ipa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpyo2ipa-1.1/setup.py` & `fpyo2ipa-1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fpyo2ipa',
-    version='1.1',
+    version='1.2',
     author='SKbarbon',
     description='A package tool that allow you to built a python iOS apps with flet UI.',
     long_description="https://github.com/SKbarbon/fpyo2ipa",
     url='https://github.com/SKbarbon/fpyo2ipa',
-    install_requires=["briefcase"],
+    install_requires=["briefcase==0.3.14"],
     include_package_data=True,
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: MacOS :: MacOS X",
     ],
     include_dirs=["assets"],
```

