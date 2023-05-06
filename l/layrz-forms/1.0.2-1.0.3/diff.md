# Comparing `tmp/layrz-forms-1.0.2.tar.gz` & `tmp/layrz-forms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz-forms-1.0.2.tar", last modified: Sat May  6 00:31:11 2023, max compression
+gzip compressed data, was "layrz-forms-1.0.3.tar", last modified: Sat May  6 01:18:04 2023, max compression
```

## Comparing `layrz-forms-1.0.2.tar` & `layrz-forms-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.415672 layrz-forms-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:31:11.414672 layrz-forms-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.410672 layrz-forms-1.0.2/layrz/
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.410672 layrz-forms-1.0.2/layrz/forms/
--rw-rw-rw-   0 root         (0) root         (0)     4290 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.412672 layrz-forms-1.0.2/layrz/forms/fields/
--rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/base.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/boolean.py
--rw-rw-rw-   0 root         (0) root         (0)     2585 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/char.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/email.py
--rw-rw-rw-   0 root         (0) root         (0)     1185 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/id.py
--rw-rw-rw-   0 root         (0) root         (0)     1659 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/layrz/forms/fields/number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 00:31:11.414672 layrz-forms-1.0.2/layrz_forms.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 00:31:11.000000 layrz-forms-1.0.2/layrz_forms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 00:31:11.415672 layrz-forms-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 00:31:01.000000 layrz-forms-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.543738 layrz-forms-1.0.3/layrz/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.543738 layrz-forms-1.0.3/layrz/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     5524 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.546738 layrz-forms-1.0.3/layrz/forms/fields/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/char.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/id.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/layrz/forms/fields/number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 01:18:04.547738 layrz-forms-1.0.3/layrz_forms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-06 01:18:04.000000 layrz-forms-1.0.3/layrz_forms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 01:18:04.548739 layrz-forms-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-06 01:17:54.000000 layrz-forms-1.0.3/setup.py
```

### Comparing `layrz-forms-1.0.2/LICENSE` & `layrz-forms-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.2/PKG-INFO` & `layrz-forms-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.2
+Version: 1.0.3
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.2/README.md` & `layrz-forms-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `layrz-forms-1.0.2/layrz/forms/__init__.py` & `layrz-forms-1.0.3/layrz/forms/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,114 +3,128 @@
 from .fields.boolean import BooleanField
 from .fields.char import CharField
 from .fields.email import EmailField
 from .fields.id import IdField
 from .fields.json import JsonField
 from .fields.number import NumberField
 import inspect
-from multiprocessing import Pool, Manager
-from functools import partial
 
 
 class Form:
   """
   Form class
   ---
   Notes:
     - Any member that starts with `_` will be ignored.
   """
 
   _obj = {}
   _errors = {}
-  _cleaned_data = {}
   _clean_functions = []
   _attributes = {}
+  _nested_attrs = {}
+  _sub_forms_attrs = {}
 
   def __init__(self, obj=dict):
     """ Constructor """
-    self._errors = {}
     self._obj = obj
+    self.calculate_members()
+
+  @property
+  def _reserverd_words(self):
+    """ Reserved words """
+    return ('add_errors', 'change_obj', 'clean', 'errors', 'is_valid', 'set_obj', 'calculate_members', 'cleaned_data')
+
+  @property
+  def cleaned_data(self):
+    """ Returns the cleaned data """
+    return self._obj
+
+  def calculate_members(self):
+    """ Calculate members """
+    self._errors = {}
     self._clean_functions = []
     self._attributes = {}
+    self._nested_attrs = {}
+    self._sub_forms_attrs = {}
 
     for item in inspect.getmembers(self):
       if item[0] in self._reserverd_words:
         continue
       if item[0].startswith('_'):
         continue
       elif item[0].startswith('clean'):
         self._clean_functions.append(item[0])
       elif isinstance(item[1], Field):
         self._attributes[item[0]] = item[1]
+      elif isinstance(item[1], list):
+        self._nested_attrs[item[0]] = item[1]
+      elif isinstance(item[1], Form):
+        self._sub_forms_attrs[item[0]] = item[1]
+      else:
+        print('Unknown field', item[0])
 
-  @property
-  def _reserverd_words(self):
-    """ Reserved words """
-    return ('add_errors', 'change_obj', 'clean', 'errors', 'is_valid')
-
-  @property
-  def cleaned_data(self):
-    """ Returns the cleaned data """
-    return self._cleaned_data
+  def set_obj(self, obj):
+    """ Set the object """
+    self._obj = obj
 
   def is_valid(self):
     """ Returns if the form is valid """
-    manager = Manager()
-    errors = manager.dict()
-    cleaned_data = manager.dict()
-
-    func = partial(self._validate_field, errors=errors, cleaned_data=cleaned_data)
-    with Pool() as pool:
-      pool.map(func, self._attributes.items())
+    self._errors = {}
 
-    self._cleaned_data = dict(cleaned_data)
-    self._errors = dict(errors)
+    for field in self._attributes.items():
+      self._validate_field(field=field)
+
+    for field, form in self._sub_forms_attrs.items():
+      self._validate_sub_form(field=field, form=form, data=self._obj.get(field, {}))
+
+    for field, form in self._nested_attrs.items():
+      self._validate_sub_form_as_list(field=field, form=form[0])
 
     for func in self._clean_functions:
       self._clean(clean_func=func)
 
   def errors(self):
     """ Returns the list of errors """
     return self._errors
 
-  def _validate_field(self, field, errors, cleaned_data):
+  def _validate_field(self, field):
     """ Validate field """
     if isinstance(field[1], Field):
       func = getattr(field[1], 'validate')
       if callable(func):
         # Validate if the validate function has the correct parameters
         params = [p for p, _ in inspect.signature(func).parameters.items()]
+        valid_params = ['key', 'value', 'errors']
 
-        if len(params) != 4:
-          raise Exception(f'{type(field[1])} validate method has no the correct parameters')
+        if len(params) != len(valid_params):
+          raise Exception(f'{type(field[1])} validate method has no the correct parameters')  #pylint: disable=W0719
 
-        valid_params = ['key', 'value', 'errors', 'cleaned_data']
         is_valid = False
         for param in params:
           if param in valid_params:
             is_valid = True
             continue
           is_valid = False
           break
 
         if not is_valid:
-          raise Exception(
-            f"{field[0]} of type {type(field[1]).__name__} validate method has no the correct " +\
-            f"parameters. Expected parameters: {', '.join(valid_params)}. " +\
-            f"Actual parameters: {', '.join(params)}"
+          raise Exception(   #pylint: disable=W0719
+            f'{field[0]} of type {type(field[1]).__name__} validate method has no the correct ' +\
+            f'parameters. Expected parameters: {", ".join(valid_params)}. ' +\
+            f'Actual parameters: {", ".join(params)}'
           )
 
         field[1].validate(
           key=field[0],
           value=self._obj.get(field[0], None),
-          errors=errors,
-          cleaned_data=cleaned_data,
+          errors=self._errors,
         )
       else:
-        raise Exception(f'{type(field[1])} has no validate method')
+        raise Exception(f'{type(field[1])} has no validate method')  #pylint: disable=W0719
 
   def _clean(self, clean_func):
     """ Clean function """
     func = getattr(self, clean_func)
     if callable(func):
       func()
 
@@ -123,15 +137,15 @@
         Key of the field
       code: str
         Code of the error
       extra_args: dict
         Extra arguments to add to the error
     """
     if key == '' or code == '':
-      raise
+      raise Exception('key and code are required')  #pylint: disable=W0719
     camel_key = self._convert_to_camel(key=key)
 
     if camel_key not in self._errors:
       self._errors[camel_key] = []
 
     new_error = {'code': code}
     if extra_args and isinstance(extra_args, dict):
@@ -144,14 +158,33 @@
   def _convert_to_camel(self, key):
     """
     Convert the key to camel case
     """
     init, *temp = key.split('_')
 
     field = ''.join([init, *map(str.title, temp)])
-    field_items = field.split(".")
+    field_items = field.split('.')
 
     field_final = []
     for item in field_items:
       field_final.append(''.join([item[0].lower(), item[1:]]))
 
     return '.'.join(field_final)
+
+  def _validate_sub_form(self, field, form, data):
+    """ Validate sub form """
+    form.set_obj(data)
+    form.calculate_members()
+    if not form.is_valid():
+      for key, errors in form.errors().items():
+        for error in errors:
+          code = error['code']
+          del error['code']
+          self.add_errors(key=f'{field}.{key}', code=code, extra_args=error)
+
+  def _validate_sub_form_as_list(self, field, form):
+    """ Validate sub form for list """
+    list_obj = self._obj.get(field, [])
+
+    if isinstance(list_obj, (list, tuple)):
+      for i, obj in enumerate(list_obj):
+        self._validate_sub_form(field=f'{field}.{i}', form=form, data=obj)
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/base.py` & `layrz-forms-1.0.3/layrz/forms/fields/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,30 +3,26 @@
 
 class Field:
   """ Field abstract class """
 
   def __init__(self, required=False):
     self.required = required
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """ Validate is the field is blank or None if is required
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    cleaned_data[key] = value
-
     if self.required:
       if value is None:
         self._append_error(key=key, errors=errors, to_add={'code': 'required'})
 
   def _convert_to_camel(self, key):
     """
     Convert the key to camel case
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/boolean.py` & `layrz-forms-1.0.3/layrz/forms/fields/id.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-""" Boolean field """
+""" ID field """
 from .base import Field
 
 
-class BooleanField(Field):
+class IdField(Field):
   """
   IdField class for validation
   ---
   Attributes
     required: bool
       Indicates if the field is required or not
   """
 
   def __init__(self, required=False):
-    super(BooleanField, self).__init__(required=required)
+    super(IdField, self).__init__(required=required)
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """
     Validate the field with the following rules:
-    - Should be a bool
+    - Should be a number or a string that can be converted to a number
+    - The number should be greater than 0
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    super(BooleanField, self).validate(key=key, value=value, errors=errors, cleaned_data=cleaned_data)
+    super(IdField, self).validate(key=key, value=value, errors=errors)
 
-    if not isinstance(value, bool):
+    if not isinstance(value, (int, str)):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
+    else:
+      if isinstance(value, str):
+        value = int(value)
+      if value <= 0:
+        self._append_error(
+          key=key,
+          errors=errors,
+          to_add={'code': 'invalid'},
+        )
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/char.py` & `layrz-forms-1.0.3/layrz/forms/fields/char.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,34 +29,32 @@
   ):
     super(CharField, self).__init__(required=required)
     self.max_length = max_length
     self.min_length = min_length
     self.empty = empty
     self.choices = choices
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """
     Validate the field with the following rules:
     - Should not be empty if required
     - Should be one of the choices indicated if choices is not None
     - Should be less than max_length if max_length is not None
     - Should be greater than min_length if min_length is not None
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    super(CharField, self).validate(key=key, value=value, errors=errors, cleaned_data=cleaned_data)
+    super(CharField, self).validate(key=key, value=value, errors=errors)
 
     if value is not None:
       if not self.empty:
         if len(value) == 0:
           self._append_error(
             key=key,
             errors=errors,
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/email.py` & `layrz-forms-1.0.3/layrz/forms/fields/email.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,31 +22,29 @@
     empty=False,
     regex=r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-z]{2,63}$',
   ):
     super(EmailField, self).__init__(required=required)
     self.empty = empty
     self.regex = regex
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """
     Validate the field with the following rules:
     - Should be a valid email, the validation will compile the regex
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    super(EmailField, self).validate(key=key, value=value, errors=errors, cleaned_data=cleaned_data)
+    super(EmailField, self).validate(key=key, value=value, errors=errors)
 
     if isinstance(value, str):
       if not self.empty:
         if value == '' or value is None:
           self._append_error(
             key=key,
             errors=errors,
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/json.py` & `layrz-forms-1.0.3/layrz/forms/fields/json.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,34 +21,32 @@
     empty=False,
     datatype=dict,
   ):
     super(JsonField, self).__init__(required=required)
     self.empty = empty
     self.datatype = datatype
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """
     Validate the field with the following rules:
     - Should be a dict or list (Depending of the datatype)
     - If `empty` is False, the field should not be empty
       * For `dict`, should have at least 1 key
       * For `list`, should have at least 1 item
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    super(JsonField, self).validate(key=key, value=value, errors=errors, cleaned_data=cleaned_data)
+    super(JsonField, self).validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, self.datatype):
       self._append_error(
         key=key,
         errors=errors,
         to_add={'code': 'invalid'},
       )
```

### Comparing `layrz-forms-1.0.2/layrz/forms/fields/number.py` & `layrz-forms-1.0.3/layrz/forms/fields/number.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,31 +25,29 @@
     max_value=None,
   ):
     super(NumberField, self).__init__(required=required)
     self.datatype = datatype
     self.min_value = min_value
     self.max_value = max_value
 
-  def validate(self, key, value, errors, cleaned_data):
+  def validate(self, key, value, errors):
     """
     Validate the field with the following rules:
     - Should be a int or float (Depending of the datatype)
     ---
     Arguments
       key: str
         Key of the field
       value: any
         Value to validate
       errors: dict
         Dict of errors
-      cleaned_data: dict
-        Dict of cleaned data
     """
 
-    super(NumberField, self).validate(key=key, value=value, errors=errors, cleaned_data=cleaned_data)
+    super(NumberField, self).validate(key=key, value=value, errors=errors)
 
     if not isinstance(value, self.datatype):
       self._append_error(key=key, errors=errors, to_add={'code': 'invalid'})
     else:
       try:
         if self.min_value is not None:
           if self.datatype(value) < self.datatype(self.min_value):
```

### Comparing `layrz-forms-1.0.2/layrz_forms.egg-info/PKG-INFO` & `layrz-forms-1.0.3/layrz_forms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-forms
-Version: 1.0.2
+Version: 1.0.3
 Summary: Layrz forms and tools for Python
 Author: Golden M
 Author-email: software@goldenmcorp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `layrz-forms-1.0.2/setup.py` & `layrz-forms-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """ Setup """
 import setuptools
 
 
 def long_description():
   """ Return long description """
-  with open("README.md", "r", encoding='utf-8') as fh:
+  with open('README.md', 'r', encoding='utf-8') as fh:
     return fh.read()
 
 
 setuptools.setup(
   name="layrz-forms",
-  version="1.0.2",
+  version="1.0.3",
   author="Golden M",
   author_email="software@goldenmcorp.com",
   description="Layrz forms and tools for Python",
   long_description=long_description(),
   long_description_content_type="text/markdown",
   packages=setuptools.find_packages(),
   classifiers=[
```

