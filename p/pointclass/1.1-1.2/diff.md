# Comparing `tmp/pointclass-1.1.tar.gz` & `tmp/pointclass-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-1.1.tar", last modified: Sat May  6 16:21:50 2023, max compression
+gzip compressed data, was "pointclass-1.2.tar", last modified: Sat May  6 16:29:22 2023, max compression
```

## Comparing `pointclass-1.1.tar` & `pointclass-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:21:50.678412 pointclass-1.1/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:21:50.672556 pointclass-1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-1.1/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 16:21:50.641509 pointclass-1.1/pointclass/
--rw-rw-rw-   0        0        0     1041 2023-05-06 16:21:29.000000 pointclass-1.1/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:21:50.671580 pointclass-1.1/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:21:50.000000 pointclass-1.1/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-06 16:21:50.000000 pointclass-1.1/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:21:50.000000 pointclass-1.1/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 16:21:50.000000 pointclass-1.1/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 16:21:50.679612 pointclass-1.1/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-05-06 16:21:35.000000 pointclass-1.1/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.370464 pointclass-1.2/
+-rw-rw-rw-   0        0        0      177 2023-05-06 16:29:22.370464 pointclass-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-1.2/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.347040 pointclass-1.2/pointclass/
+-rw-rw-rw-   0        0        0     1045 2023-05-06 16:29:07.000000 pointclass-1.2/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:29:22.368515 pointclass-1.2/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 16:29:22.000000 pointclass-1.2/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:29:22.370464 pointclass-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 16:27:31.000000 pointclass-1.2/setup1.py
```

### Comparing `pointclass-1.1/pointclass/__init__.py` & `pointclass-1.2/pointclass/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,22 @@
+def copy():
+        print("from pulp import*")
+        print("model=LpProblem(sense=LpMaximize)")
+        print("x=LpVariable(name='x',lowBound=0)")
+        print("y=LpVariable(name='y',lowBound=0)")
+        print("model+=(4*x+6*y<=24)")
+        print("model+=(5*x+75*y<=15)")
+        print("model+=150*x+75*y")
+        print("model.solve()")
+        print("model.objective.value()")
+        print("x.value()") 
+        print("y.value()")
+        print("copy")
 import math
+
 class point:
     def __init__(self,x=0,y=0):
         self.x=x
         self.y=y
     def show(self):
         return self.x
         return self.y
@@ -14,20 +28,8 @@
         return(self.x * p.x,self.y * p.y)
     def __eq__(self,p):
          return(self.x==p.x,self.y==p.y)
     def __repro__():
         return "point(self.x,self.y)"
     def distance(p1,p2):
         return math.hypot(p2.x-p1.x,p2.y-p1.y)
-    def copy():
-        print("from pulp import*")
-        print("model=LpProblem(sense=LpMaximize)")
-        print("x=LpVariable(name='x',lowBound=0)")
-        print("y=LpVariable(name='y',lowBound=0)")
-        print("model+=(4*x+6*y<=24)")
-        print("model+=(5*x+75*y<=15)")
-        print("model+=150*x+75*y")
-        print("model.solve()")
-        print("model.objective.value()")
-        print("x.value()") 
-        print("y.value()")
-        print("copy")
+
```

