# Comparing `tmp/layrz-forms-1.0.3.tar.gz` & `tmp/layrz-forms-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.3.tar", last modified: Sat May  6 01:18:04 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.4.tar", last modified: Sat May  6 01:24:57 2023, max compression
```

## Comparing `layrz-forms-1.0.3.tar` & `layrz-forms-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.543738 layrz-forms-1.0.3/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.543738 layrz-forms-1.0.3/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     5524 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.546738 layrz-forms-1.0.3/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.547738 layrz-forms-1.0.3/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.633822 layrz-forms-1.0.4/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.634822 layrz-forms-1.0.4/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     5559 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.636822 layrz-forms-1.0.4/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:24:57.638823 layrz-forms-1.0.4/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 01:24:57.000000 layrz-forms-1.0.4/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 01:24:57.639823 layrz-forms-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 01:24:47.000000 layrz-forms-1.0.4/setup.py
```

### Comparing `layrz-forms-1.0.3/LICENSE` & `layrz-forms-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/PKG-INFO` & `layrz-forms-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.3
+Version: 1.0.4
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.3/README.md` & `layrz-forms-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/__init__.py` & `layrz-forms-1.0.4/layrz/forms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
     for field, form in self._nested_attrs.items():
       self._validate_sub_form_as_list(field=field, form=form[0])
 
     for func in self._clean_functions:
       self._clean(clean_func=func)
 
+    return len(self._errors) == 0
+
   def errors(self):
     """ Returns the list of errors """
     return self._errors
 
   def _validate_field(self, field):
     """ Validate field """
     if isinstance(field[1], Field):
```

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/base.py` & `layrz-forms-1.0.4/layrz/forms/fields/base.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.4/layrz/forms/fields/boolean.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/char.py` & `layrz-forms-1.0.4/layrz/forms/fields/char.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/email.py` & `layrz-forms-1.0.4/layrz/forms/fields/email.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/id.py` & `layrz-forms-1.0.4/layrz/forms/fields/id.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/json.py` & `layrz-forms-1.0.4/layrz/forms/fields/json.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz/forms/fields/number.py` & `layrz-forms-1.0.4/layrz/forms/fields/number.py`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.3/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.4/layrz_forms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.3
+Version: 1.0.4
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.3/setup.py` & `layrz-forms-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   """ Return long description """
   with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.3",
+  version="1.0.4",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

