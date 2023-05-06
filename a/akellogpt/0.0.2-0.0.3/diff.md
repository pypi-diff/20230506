# Comparing `tmp/akellogpt-0.0.2.tar.gz` & `tmp/akellogpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akellogpt-0.0.2.tar", last modified: Sat May  6 01:10:21 2023, max compression
+gzip compressed data, was "akellogpt-0.0.3.tar", last modified: Sat May  6 02:27:53 2023, max compression
```

## Comparing `akellogpt-0.0.2.tar` & `akellogpt-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.207539 akellogpt-0.0.2/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1075 2023-05-05 23:21:08.000000 akellogpt-0.0.2/LICENSE
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 01:10:21.207406 akellogpt-0.0.2/PKG-INFO
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1603 2023-05-06 00:30:29.000000 akellogpt-0.0.2/README.md
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.204637 akellogpt-0.0.2/akellogpt/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/__init__.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.205615 akellogpt-0.0.2/akellogpt/common/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/common/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      693 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/common/api.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.206047 akellogpt-0.0.2/akellogpt/screening/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     3385 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/screening/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      412 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/screening/mental_health.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.206792 akellogpt-0.0.2/akellogpt/screening/yaml/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      883 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/screening/yaml/gad7.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1342 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/screening/yaml/phq9.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1972 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/screening/yaml/sbq-r.yaml
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       77 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/settings.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.207195 akellogpt-0.0.2/akellogpt/test/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.2/akellogpt/test/__init__.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      649 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/test/test_gad7.py
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      668 2023-05-06 00:30:29.000000 akellogpt-0.0.2/akellogpt/test/test_phq9.py
-drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 01:10:21.205386 akellogpt-0.0.2/akellogpt.egg-info/
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 01:10:21.000000 akellogpt-0.0.2/akellogpt.egg-info/PKG-INFO
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      545 2023-05-06 01:10:21.000000 akellogpt-0.0.2/akellogpt.egg-info/SOURCES.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)        1 2023-05-06 01:10:21.000000 akellogpt-0.0.2/akellogpt.egg-info/dependency_links.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       26 2023-05-06 01:10:21.000000 akellogpt-0.0.2/akellogpt.egg-info/requires.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       10 2023-05-06 01:10:21.000000 akellogpt-0.0.2/akellogpt.egg-info/top_level.txt
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)       38 2023-05-06 01:10:21.207575 akellogpt-0.0.2/setup.cfg
--rw-r--r--   0 vijayselvaraj   (501) staff       (20)      911 2023-05-06 01:09:21.000000 akellogpt-0.0.2/setup.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742904 akellogpt-0.0.3/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1075 2023-05-05 23:21:08.000000 akellogpt-0.0.3/LICENSE
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 02:27:53.742760 akellogpt-0.0.3/PKG-INFO
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1603 2023-05-06 00:30:29.000000 akellogpt-0.0.3/README.md
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.739843 akellogpt-0.0.3/akellogpt/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/__init__.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.740981 akellogpt-0.0.3/akellogpt/common/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/common/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      693 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/common/api.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.741504 akellogpt-0.0.3/akellogpt/screening/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     3383 2023-05-06 01:52:00.000000 akellogpt-0.0.3/akellogpt/screening/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      412 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/screening/mental_health.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742122 akellogpt-0.0.3/akellogpt/screening/yaml/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      883 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/gad7.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1342 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/phq9.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)     1972 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/screening/yaml/sbq-r.yaml
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       77 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/settings.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.742553 akellogpt-0.0.3/akellogpt/test/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        0 2023-05-05 23:21:08.000000 akellogpt-0.0.3/akellogpt/test/__init__.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      649 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/test/test_gad7.py
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      668 2023-05-06 00:30:29.000000 akellogpt-0.0.3/akellogpt/test/test_phq9.py
+drwxr-xr-x   0 vijayselvaraj   (501) staff       (20)        0 2023-05-06 02:27:53.740707 akellogpt-0.0.3/akellogpt.egg-info/
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      495 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/PKG-INFO
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      545 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)        1 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       26 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/requires.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       10 2023-05-06 02:27:53.000000 akellogpt-0.0.3/akellogpt.egg-info/top_level.txt
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)       38 2023-05-06 02:27:53.742945 akellogpt-0.0.3/setup.cfg
+-rw-r--r--   0 vijayselvaraj   (501) staff       (20)      911 2023-05-06 02:27:06.000000 akellogpt-0.0.3/setup.py
```

### Comparing `akellogpt-0.0.2/LICENSE` & `akellogpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/README.md` & `akellogpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/common/api.py` & `akellogpt-0.0.3/akellogpt/common/api.py`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/screening/__init__.py` & `akellogpt-0.0.3/akellogpt/screening/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         self.responses = []
 
     def add_option(self, name, value):
         """
         Add an option to the screening question
         """
 
-        option = ScreeningQuestion(name, value)
+        option = ScreeningOption(name, value)
         self.options.append(option)
 
     def add_response(self, response):
         """
         Add a response to the screening question
         """
```

### Comparing `akellogpt-0.0.2/akellogpt/screening/yaml/gad7.yaml` & `akellogpt-0.0.3/akellogpt/screening/yaml/gad7.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/screening/yaml/phq9.yaml` & `akellogpt-0.0.3/akellogpt/screening/yaml/phq9.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/screening/yaml/sbq-r.yaml` & `akellogpt-0.0.3/akellogpt/screening/yaml/sbq-r.yaml`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/test/test_gad7.py` & `akellogpt-0.0.3/akellogpt/test/test_gad7.py`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt/test/test_phq9.py` & `akellogpt-0.0.3/akellogpt/test/test_phq9.py`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/akellogpt.egg-info/SOURCES.txt` & `akellogpt-0.0.3/akellogpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akellogpt-0.0.2/setup.py` & `akellogpt-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'ChatGPT for healthcare applications'
 LONG_DESCRIPTION = 'Akello GPT helps ensure deterministic results for healthcare applications '
 
 setup(
     name="akellogpt",
     version=VERSION,
     description=DESCRIPTION,
```

