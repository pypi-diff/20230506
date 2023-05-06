# Comparing `tmp/layrz-forms-1.0.1.tar.gz` & `tmp/layrz-forms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.1.tar", last modified: Sat May  6 00:28:37 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.2.tar", last modified: Sat May  6 00:31:11 2023, max compression
```

## Comparing `layrz-forms-1.0.1.tar` & `layrz-forms-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:28:37.974220 layrz-forms-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:28:37.973220 layrz-forms-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:28:37.969219 layrz-forms-1.0.1/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:28:37.969219 layrz-forms-1.0.1/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:28:37.972220 layrz-forms-1.0.1/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2631 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:28:37.973220 layrz-forms-1.0.1/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:28:37.000000 layrz-forms-1.0.1/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 00:28:37.000000 layrz-forms-1.0.1/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 00:28:37.000000 layrz-forms-1.0.1/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 00:28:37.000000 layrz-forms-1.0.1/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 00:28:37.974220 layrz-forms-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 00:28:28.000000 layrz-forms-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.415672 layrz-forms-1.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:31:11.414672 layrz-forms-1.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.410672 layrz-forms-1.0.2/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.410672 layrz-forms-1.0.2/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.412672 layrz-forms-1.0.2/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.414672 layrz-forms-1.0.2/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 00:31:11.415672 layrz-forms-1.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/setup.py
```

### Comparing `layrz-forms-1.0.1/LICENSE` & `layrz-forms-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/PKG-INFO` & `layrz-forms-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.1/README.md` & `layrz-forms-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/__init__.py` & `layrz-forms-1.0.2/layrz/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/base.py` & `layrz-forms-1.0.2/layrz/forms/fields/base.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.2/layrz/forms/fields/boolean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Boolean field """
 from .base import Field
-from layrz.converters import convert_to_camel
 
 
 class BooleanField(Field):
   """
   IdField class for validation
   ---
   Attributes
```

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/char.py` & `layrz-forms-1.0.2/layrz/forms/fields/char.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Email field """
 from .base import Field
-from layrz.converters import convert_to_camel
 
 
 class CharField(Field):
   """
   CharField class for validation
   ---
   Attributes
```

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/email.py` & `layrz-forms-1.0.2/layrz/forms/fields/email.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/id.py` & `layrz-forms-1.0.2/layrz/forms/fields/id.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/json.py` & `layrz-forms-1.0.2/layrz/forms/fields/json.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz/forms/fields/number.py` & `layrz-forms-1.0.2/layrz/forms/fields/number.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.1/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.2/layrz_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.1
+Version: 1.0.2
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.1/setup.py` & `layrz-forms-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   """ Return long description """
   with open("README.md", "r", encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.1",
+  version="1.0.2",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

