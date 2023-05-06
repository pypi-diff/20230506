# Comparing `tmp/pointclass-0.9.tar.gz` & `tmp/pointclass-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.9.tar", last modified: Sat May  6 16:08:19 2023, max compression
+gzip compressed data, was "pointclass-1.0.tar", last modified: Sat May  6 16:17:32 2023, max compression
```

## Comparing `pointclass-0.9.tar` & `pointclass-1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 16:08:19.058225 pointclass-0.9/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:08:19.057246 pointclass-0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.9/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 16:08:19.040422 pointclass-0.9/pointclass/
--rw-rw-rw-   0        0        0     1006 2023-05-06 16:07:48.000000 pointclass-0.9/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 16:08:19.056271 pointclass-0.9/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-05-06 16:08:18.000000 pointclass-0.9/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-06 16:08:18.000000 pointclass-0.9/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 16:08:18.000000 pointclass-0.9/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 16:08:18.000000 pointclass-0.9/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 16:08:19.058225 pointclass-0.9/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-05-06 16:07:55.000000 pointclass-0.9/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:17:32.033402 pointclass-1.0/
+-rw-rw-rw-   0        0        0      177 2023-05-06 16:17:32.033402 pointclass-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-1.0/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 16:17:32.015836 pointclass-1.0/pointclass/
+-rw-rw-rw-   0        0        0     1040 2023-05-06 16:17:00.000000 pointclass-1.0/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:17:32.032426 pointclass-1.0/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 16:17:31.000000 pointclass-1.0/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 16:17:31.000000 pointclass-1.0/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:17:31.000000 pointclass-1.0/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 16:17:31.000000 pointclass-1.0/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:17:32.034379 pointclass-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 16:17:11.000000 pointclass-1.0/setup1.py
```

### Comparing `pointclass-0.9/pointclass/__init__.py` & `pointclass-1.0/pointclass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,19 @@
     def __eq__(self,p):
          return(self.x==p.x,self.y==p.y)
     def __repro__():
         return "point(self.x,self.y)"
     def distance(p1,p2):
         return math.hypot(p2.x-p1.x,p2.y-p1.y)
     def lpp():
-       print("from pulp import*")
-       print("model=LpProblem(sense=LpMaximize)")
-       print("x=LpVariable(name='x',lowBound=0)")
-       print("y=LpVariable(name='y',lowBound=0)")
-       print("model+=(4*x+6*y<=24)")
-       print("model+=(5*x+75*y<=15)")
-       print("model+=150*x+75*y")
-       print("model.solve()")
-       print("model.objective.value()")
-       print("x.value()") 
-       print("y.value()")
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
```

