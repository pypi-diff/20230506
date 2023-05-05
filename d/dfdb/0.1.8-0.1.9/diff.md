# Comparing `tmp/dfdb-0.1.8.tar.gz` & `tmp/dfdb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfdb-0.1.8.tar", last modified: Tue Apr 25 05:46:04 2023, max compression
+gzip compressed data, was "dfdb-0.1.9.tar", last modified: Fri May  5 22:24:54 2023, max compression
```

## Comparing `dfdb-0.1.8.tar` & `dfdb-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 05:46:04.408804 dfdb-0.1.8/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2023-03-25 18:57:15.000000 dfdb-0.1.8/LICENSE
--rw-r--r--   0 hoyinchau   (501) staff       (20)       28 2023-03-30 21:11:25.000000 dfdb-0.1.8/MANIFEST.in
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-04-25 05:46:04.408653 dfdb-0.1.8/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-03-25 18:57:15.000000 dfdb-0.1.8/README.md
--rw-r--r--   0 hoyinchau   (501) staff       (20)      831 2023-04-25 04:48:09.000000 dfdb-0.1.8/pyproject.toml
--rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-04-25 05:46:04.408845 dfdb-0.1.8/setup.cfg
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 05:46:04.405540 dfdb-0.1.8/src/
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 05:46:04.407635 dfdb-0.1.8/src/dfdb/
--rw-r--r--   0 hoyinchau   (501) staff       (20)      243 2023-04-16 02:48:50.000000 dfdb-0.1.8/src/dfdb/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2533 2023-04-25 05:41:09.000000 dfdb-0.1.8/src/dfdb/abc.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2337 2023-04-23 19:21:24.000000 dfdb-0.1.8/src/dfdb/alter.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      272 2023-04-25 04:15:30.000000 dfdb-0.1.8/src/dfdb/config.toml
--rw-r--r--   0 hoyinchau   (501) staff       (20)     8504 2023-04-25 05:32:20.000000 dfdb-0.1.8/src/dfdb/database.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    57214 2023-04-25 05:37:33.000000 dfdb-0.1.8/src/dfdb/dataframe.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1430 2023-04-25 05:30:55.000000 dfdb-0.1.8/src/dfdb/defs.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3300 2023-04-25 05:44:50.000000 dfdb-0.1.8/src/dfdb/parsing.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     6093 2023-04-25 05:37:59.000000 dfdb-0.1.8/src/dfdb/triggers.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7621 2023-04-25 05:20:20.000000 dfdb-0.1.8/src/dfdb/types.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 05:46:04.408318 dfdb-0.1.8/src/dfdb.egg-info/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1766 2023-04-25 05:46:04.000000 dfdb-0.1.8/src/dfdb.egg-info/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)      421 2023-04-25 05:46:04.000000 dfdb-0.1.8/src/dfdb.egg-info/SOURCES.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-04-25 05:46:04.000000 dfdb-0.1.8/src/dfdb.egg-info/dependency_links.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       75 2023-04-25 05:46:04.000000 dfdb-0.1.8/src/dfdb.egg-info/requires.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        5 2023-04-25 05:46:04.000000 dfdb-0.1.8/src/dfdb.egg-info/top_level.txt
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-04-25 05:46:04.408452 dfdb-0.1.8/test/
--rw-r--r--   0 hoyinchau   (501) staff       (20)    26676 2023-04-25 05:38:33.000000 dfdb-0.1.8/test/test_dataframe.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-05-05 22:24:54.363101 dfdb-0.1.9/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2023-03-25 18:57:15.000000 dfdb-0.1.9/LICENSE
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       28 2023-03-30 21:11:25.000000 dfdb-0.1.9/MANIFEST.in
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2757 2023-05-05 22:24:54.362829 dfdb-0.1.9/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1051 2023-04-25 22:45:17.000000 dfdb-0.1.9/README.md
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      831 2023-05-05 22:23:01.000000 dfdb-0.1.9/pyproject.toml
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-05-05 22:24:54.363160 dfdb-0.1.9/setup.cfg
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-05-05 22:24:53.832300 dfdb-0.1.9/src/
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-05-05 22:24:54.361068 dfdb-0.1.9/src/dfdb/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      243 2023-04-16 02:48:50.000000 dfdb-0.1.9/src/dfdb/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2533 2023-04-25 05:41:09.000000 dfdb-0.1.9/src/dfdb/abc.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2337 2023-04-23 19:21:24.000000 dfdb-0.1.9/src/dfdb/alter.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      272 2023-04-25 04:15:30.000000 dfdb-0.1.9/src/dfdb/config.toml
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     8504 2023-04-25 05:32:20.000000 dfdb-0.1.9/src/dfdb/database.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    58091 2023-05-05 22:22:03.000000 dfdb-0.1.9/src/dfdb/dataframe.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1430 2023-04-25 05:30:55.000000 dfdb-0.1.9/src/dfdb/defs.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3300 2023-04-25 05:44:50.000000 dfdb-0.1.9/src/dfdb/parsing.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6093 2023-04-25 05:37:59.000000 dfdb-0.1.9/src/dfdb/triggers.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7621 2023-04-25 05:20:20.000000 dfdb-0.1.9/src/dfdb/types.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-05-05 22:24:54.362247 dfdb-0.1.9/src/dfdb.egg-info/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2757 2023-05-05 22:24:53.000000 dfdb-0.1.9/src/dfdb.egg-info/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      421 2023-05-05 22:24:53.000000 dfdb-0.1.9/src/dfdb.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-05-05 22:24:53.000000 dfdb-0.1.9/src/dfdb.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       75 2023-05-05 22:24:53.000000 dfdb-0.1.9/src/dfdb.egg-info/requires.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        5 2023-05-05 22:24:53.000000 dfdb-0.1.9/src/dfdb.egg-info/top_level.txt
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-05-05 22:24:54.362428 dfdb-0.1.9/test/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    26676 2023-04-25 05:38:33.000000 dfdb-0.1.9/test/test_dataframe.py
```

### Comparing `dfdb-0.1.8/LICENSE` & `dfdb-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/pyproject.toml` & `dfdb-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dfdb"
-version = "0.1.8"
+version = "0.1.9"
 description = "Pandas-like interface for manipulating SQL databases."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     'numpy',
-    'pandas>=2.0.0',
+    'pandas>=1.5.3',
     'SQLAlchemy>=2.0.0',
     'hyclib>=0.1.13',
     'addict', # attribute access for options
     'beautifulsoup4', # prettifying output of df.to_html()
 ]
 
 [project.urls]
```

### Comparing `dfdb-0.1.8/src/dfdb/abc.py` & `dfdb-0.1.9/src/dfdb/abc.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/alter.py` & `dfdb-0.1.9/src/dfdb/alter.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/database.py` & `dfdb-0.1.9/src/dfdb/database.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/dataframe.py` & `dfdb-0.1.9/src/dfdb/dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -593,23 +593,51 @@
         return self[:,self.eval(condition, level=level + 1)]
     
     def append(self, obj, execute=True):
         if isinstance(obj, pd.DataFrame):
             obj = obj.to_dict('records')
         elif isinstance(obj, pd.Series):
             obj = obj.to_dict()
-                
-        sql = sa.insert(self.table).values(obj)
+            
+        sql = sa.insert(self.table).values(_clean_input(obj))
             
         if execute:
             with self.db.connect() as con:
                 con.execute(sql)
         else:
             return sql
+        
+
+def _clean_input(obj):
+    def clean_element(v):
+        if v is pd.NA:
+            return None
+        return v
+    
+    if isinstance(obj, tuple):
+        return tuple(clean_element(v) for v in obj)
+    
+    elif isinstance(obj, dict):
+        return {k: clean_element(v) for k, v in obj.items()}
+    
+    elif isinstance(obj, list):
+        new_obj = []
+        for v in obj:
+            if isinstance(v, tuple):
+                new_v = tuple(clean_element(vi) for vi in v)
+            elif isinstance(v, dict):
+                new_v = {ki: clean_element(vi) for ki, vi in v.items()}
+            else:
+                raise TypeError(f"each element of list must be a tuple or dict, but {type(v)=}.")
+            new_obj.append(new_v)
             
+        return new_obj
+    
+    else:
+        raise TypeError(f"obj must be a tuple, list, or dict, but {type(obj)=}.")
             
 class LocIndexer:
     def __init__(self, df):
         self.df = df
         
     def __getitem__(self, key):
         if key is Ellipsis:
```

### Comparing `dfdb-0.1.8/src/dfdb/defs.py` & `dfdb-0.1.9/src/dfdb/defs.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/parsing.py` & `dfdb-0.1.9/src/dfdb/parsing.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/triggers.py` & `dfdb-0.1.9/src/dfdb/triggers.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/src/dfdb/types.py` & `dfdb-0.1.9/src/dfdb/types.py`

 * *Files identical despite different names*

### Comparing `dfdb-0.1.8/test/test_dataframe.py` & `dfdb-0.1.9/test/test_dataframe.py`

 * *Files identical despite different names*

