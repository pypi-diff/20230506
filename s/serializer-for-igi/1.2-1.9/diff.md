# Comparing `tmp/serializer_for_igi-1.2.tar.gz` & `tmp/serializer_for_igi-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_for_igi-1.2.tar", last modified: Fri May  5 20:57:20 2023, max compression
+gzip compressed data, was "serializer_for_igi-1.9.tar", last modified: Fri May  5 23:23:12 2023, max compression
```

## Comparing `serializer_for_igi-1.2.tar` & `serializer_for_igi-1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.131338 serializer_for_igi-1.2/
--rw-rw-r--   0 denis     (1000) denis     (1000)      378 2023-05-05 20:57:20.131338 serializer_for_igi-1.2/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)        2 2023-05-05 20:54:13.000000 serializer_for_igi-1.2/README.md
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.107338 serializer_for_igi-1.2/serializer_for_igi.egg-info/
--rw-rw-r--   0 denis     (1000) denis     (1000)      378 2023-05-05 20:57:20.000000 serializer_for_igi-1.2/serializer_for_igi.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1000) denis     (1000)      491 2023-05-05 20:57:20.000000 serializer_for_igi-1.2/serializer_for_igi.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-05 20:57:20.000000 serializer_for_igi-1.2/serializer_for_igi.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1000) denis     (1000)       73 2023-05-05 20:57:20.000000 serializer_for_igi-1.2/serializer_for_igi.egg-info/top_level.txt
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.107338 serializer_for_igi-1.2/serializers/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 17:29:30.000000 serializer_for_igi-1.2/serializers/__init__.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.111338 serializer_for_igi-1.2/serializers/dict_serializer/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:04:44.000000 serializer_for_igi-1.2/serializers/dict_serializer/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)    12987 2023-05-05 20:29:37.000000 serializer_for_igi-1.2/serializers/dict_serializer/functions.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      265 2023-05-05 17:28:54.000000 serializer_for_igi-1.2/serializers/factory_serializer.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.115338 serializer_for_igi-1.2/serializers/json/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:04:34.000000 serializer_for_igi-1.2/serializers/json/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      588 2023-05-05 16:16:48.000000 serializer_for_igi-1.2/serializers/json/json.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     1863 2023-04-13 21:01:46.000000 serializer_for_igi-1.2/serializers/json/parse_json.py
-drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 20:57:20.127338 serializer_for_igi-1.2/serializers/xml/
--rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:06:37.000000 serializer_for_igi-1.2/serializers/xml/__init__.py
--rw-rw-r--   0 denis     (1000) denis     (1000)      827 2023-05-05 16:34:02.000000 serializer_for_igi-1.2/serializers/xml/xml.py
--rw-rw-r--   0 denis     (1000) denis     (1000)     3322 2023-05-05 16:31:30.000000 serializer_for_igi-1.2/serializers/xml/xml_parser.py
--rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-05 20:57:20.131338 serializer_for_igi-1.2/setup.cfg
--rw-rw-r--   0 denis     (1000) denis     (1000)      596 2023-05-05 18:00:33.000000 serializer_for_igi-1.2/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.394171 serializer_for_igi-1.9/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      423 2023-05-05 23:23:12.394171 serializer_for_igi-1.9/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)        2 2023-05-05 20:54:13.000000 serializer_for_igi-1.9/README.md
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.378171 serializer_for_igi-1.9/serializer_for_igi.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      423 2023-05-05 23:23:11.000000 serializer_for_igi-1.9/serializer_for_igi.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)      491 2023-05-05 23:23:12.000000 serializer_for_igi-1.9/serializer_for_igi.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-05-05 23:23:11.000000 serializer_for_igi-1.9/serializer_for_igi.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       73 2023-05-05 23:23:12.000000 serializer_for_igi-1.9/serializer_for_igi.egg-info/top_level.txt
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.378171 serializer_for_igi-1.9/serializers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 17:29:30.000000 serializer_for_igi-1.9/serializers/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.382171 serializer_for_igi-1.9/serializers/dict_serializer/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:04:44.000000 serializer_for_igi-1.9/serializers/dict_serializer/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    11426 2023-05-05 23:17:02.000000 serializer_for_igi-1.9/serializers/dict_serializer/functions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      265 2023-05-05 17:28:54.000000 serializer_for_igi-1.9/serializers/factory_serializer.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.390171 serializer_for_igi-1.9/serializers/json/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:04:34.000000 serializer_for_igi-1.9/serializers/json/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      754 2023-05-05 22:50:10.000000 serializer_for_igi-1.9/serializers/json/json.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2275 2023-05-05 22:49:47.000000 serializer_for_igi-1.9/serializers/json/parse_json.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-05-05 23:23:12.394171 serializer_for_igi-1.9/serializers/xml/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-05 16:06:37.000000 serializer_for_igi-1.9/serializers/xml/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      687 2023-05-05 23:15:14.000000 serializer_for_igi-1.9/serializers/xml/xml.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3322 2023-05-05 16:31:30.000000 serializer_for_igi-1.9/serializers/xml/xml_parser.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-05-05 23:23:12.394171 serializer_for_igi-1.9/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)      596 2023-05-05 23:19:01.000000 serializer_for_igi-1.9/setup.py
```

### Comparing `serializer_for_igi-1.2/serializers/dict_serializer/functions.py` & `serializer_for_igi-1.9/serializers/dict_serializer/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         obj = serealize_func(obj)
     elif (inspect.iscode(obj)):
         obj = serealize_code(obj)
     elif (inspect.isclass(obj)):
         obj = ser_class_old(obj)
     elif (inspect.ismethoddescriptor(obj) or inspect.isbuiltin(obj)):
         obj = serealize_instance(obj)
-    elif inspect.ismemberdescriptor(obj):
+    elif inspect.ismemberdescriptor(obj):  
         obj = serealize_instance(obj)
     elif inspect.isgetsetdescriptor(obj):
         obj = serealize_instance(obj)
     elif isinstance(obj, type(type.__dict__)):
         obj = serealize_instance(obj)
     elif inspect.ismodule(obj):
         return serealize_module(obj)
@@ -161,15 +161,14 @@
     result['value'] = serealize(value)
     
     return result
     '''
     
     
 def serealize_object(obj):
-    print(type(obj))
     
     serealized = dict()
     serealized['type'] = 'object'
     serealized['value'] = serealize({'__object_type__': type(obj), '__fields__': obj.__dict__})
     
     #for key, value in inspect.getmembers(obj):
     #    if not key.startwith('__') and not inspect.isfunction(value):
@@ -303,110 +302,15 @@
         
     return res
 
 def deseralize_module(obj):
     return __import__(obj['value'])
             
 
-class A:
-    def __init__(self):
-        pass
-    
-    def func(self, a):
-        print(a**a)
-        
-    class F:
-        def __init__(self):
-            pass
-        
-        def func_2(self, g):
-            print(g**g)
-        
-
-        
-class B(A):
-    def __init__(self):
-        pass
-    
-    def func_1(self, b):
-        print(b**b)
-        
-tmp = deseralize(serealize(B))
-print(type(tmp))
-a = tmp()
-a.func(2)
-b = a.F()
-b.func_2(5)
-
-print(tmp.__bases__)
-
-def rec(n):
-    if (n == 1):
-        return 1
-    return n + rec(n-1)
-
-tmp = serealize(rec)
-tmp = deseralize(tmp)
-
-print(tmp(23))
-
-def my_shiny_new_decorator(function_to_decorate):
-    def the_wrapper_around_the_original_function():
-        function_to_decorate()
-
-    return the_wrapper_around_the_original_function
-
-
-def stand_alone_function():
-    print("Я простая одинокая функция, ты ведь не посмеешь меня изменять?")
-
-
-stand_alone_function_decorated = my_shiny_new_decorator(stand_alone_function)
-
-print(stand_alone_function_decorated())
-
-print(type(stand_alone_function_decorated))
-
-tmp = deseralize(serealize(my_shiny_new_decorator))
-
-print(type(tmp))
-
-
-
-x = lambda a : a + 10
-
-tmp = deseralize(serealize(x))
-
-print(tmp(10))
-
-def g(b):
-    return b+5
-
-def f(arr):
-    return sorted(arr)
-
-print(f([0.5, 0.6]))
-
-tmp = serealize(f)
-tmp = deseralize(tmp)
-
-print(1)
-
-print(tmp([0.5, 0.6]), type(tmp), 'qwe')
-
-class A:
-    a = 123
-    
-    def __init__(self):
-        pass
-
-a = A()
-tmp = deseralize(serealize(a))
 
-print(tmp.a)
 
 
 '''
 def ser_class(obj):
     res = {'type':'class', '__name__':obj.__name__}
     
     for attr in inspect.getmembers(obj):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `serializer_for_igi-1.2/serializers/json/parse_json.py` & `serializer_for_igi-1.9/serializers/json/parse_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 def parse_json(obj):
+    if (obj == '[]') :
+        return {}
+    
     if (obj[0] in ['{', '[']):
         res = dict()
         bracket_num = 0
         res_list = list()
         is_list = (obj[0] == '[')
         obj = obj[1:-1]
         tmp_str = ''
@@ -44,8 +47,10 @@
     
     if is_list:
         return res_list
     else:
         return res
     
     
-print(parse_json("{'type': 'dict', 'value': [[{'type': 'int', 'value': 1}, {'type': 'int', 'value': 1}], [{'type': 'int', 'value': 2}, {'type': 'int', 'value': 2}], [{'type': 'int', 'value': 3}, {'type': 'int', 'value': 3}], [{'type': 'int', 'value': 4}, {'type': 'tuple', 'value': [{'type': 'int', 'value': 5}, {'type': 'int', 'value': 6}, {'type': 'int', 'value': 7}]}]]}"))
+print(parse_json("{'type': 'list', 'value': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}, {'type': 'int', 'value': 3}, {'type': 'tuple', 'value': [{'type': 'int', 'value': 4}, {'type': 'int', 'value': 5}, {'type': 'dict', 'value': [[{'type': 'int', 'value': 6}, {'type': 'str', 'value': '6'}], [{'type': 'int', 'value': 7}, {'type': 'int', 'value': 789}]]}]}]}"))
+
+print("{'type': 'list', 'value': [{'type': 'int', 'value': 1}, {'type': 'int', 'value': 2}, {'type': 'int', 'value': 3}, {'type': 'tuple', 'value': [{'type': 'int', 'value': 4}, {'type': 'int', 'value': 5}, {'type': 'dict', 'value': [[{'type': 'int', 'value': 6}, {'type': 'str', 'value': '6'}], [{'type': 'int', 'value': 7}, {'type': 'int', 'value': 789}]]}]}]}")
```

### Comparing `serializer_for_igi-1.2/serializers/xml/xml_parser.py` & `serializer_for_igi-1.9/serializers/xml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `serializer_for_igi-1.2/setup.py` & `serializer_for_igi-1.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="serializer_for_igi",
-    version="1.02",
+    version="1.09",
     description="library for python serialization as lab",
     url="https://github.com/SeMsei/pythn_igi/tree/lab3/Lab_3",
     author="Denis Fomichevskiy",
     author_email="fomichevsjiy@gmail.com",
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.10",
```

