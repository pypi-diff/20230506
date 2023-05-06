# Comparing `tmp/pointclass-0.6.tar.gz` & `tmp/pointclass-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pointclass-0.6.tar", last modified: Sat May  6 15:05:06 2023, max compression
+gzip compressed data, was "pointclass-0.7.tar", last modified: Sat May  6 15:17:22 2023, max compression
```

## Comparing `pointclass-0.6.tar` & `pointclass-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.583535 pointclass-0.6/
--rw-rw-rw-   0        0        0      177 2023-05-06 15:05:06.581273 pointclass-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.6/licence.txt.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.536934 pointclass-0.6/pointclass/
--rw-rw-rw-   0        0        0      835 2023-05-06 15:03:57.000000 pointclass-0.6/pointclass/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 15:05:06.580275 pointclass-0.6/pointclass.egg-info/
--rw-rw-rw-   0        0        0      177 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 15:05:06.000000 pointclass-0.6/pointclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 15:05:06.583535 pointclass-0.6/setup.cfg
--rw-rw-rw-   0        0        0      247 2023-05-06 15:04:21.000000 pointclass-0.6/setup1.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.724060 pointclass-0.7/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:17:22.723063 pointclass-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-25 10:31:30.000000 pointclass-0.7/licence.txt.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.708809 pointclass-0.7/pointclass/
+-rw-rw-rw-   0        0        0      835 2023-05-06 15:17:06.000000 pointclass-0.7/pointclass/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 15:17:22.722067 pointclass-0.7/pointclass.egg-info/
+-rw-rw-rw-   0        0        0      177 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 15:17:22.000000 pointclass-0.7/pointclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 15:17:22.724060 pointclass-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      247 2023-05-06 15:17:16.000000 pointclass-0.7/setup1.py
```

### Comparing `pointclass-0.6/pointclass/__init__.py` & `pointclass-0.7/pointclass/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,8 +15,8 @@
     def __eq__(self,p):
          return(self.x==p.x,self.y==p.y)
     def __repro__():
         return "point(self.x,self.y)"
     def distance(p1,p2):
         return math.hypot(p2.x-p1.x,p2.y-p1.y)
     def lpp():
-        print("from pulp import*|model=LpProblem(sense=LpMaximize|x=LpVariable(name="x",lowBound=0)|y=LpVariable(name="y",lowBound=0)|model+=(4*x+6*y<=24)|model+=(5*x+75*y<=15)|odel+=150*x+75*y|model.solve()|model.objective.value()x.value())|y.value())")
+        print("from pulp import*|model=LpProblem(sense=LpMaximize)|x=LpVariable(name="x",lowBound=0)|y=LpVariable(name="y",lowBound=0)|model+=(4*x+6*y<=24)|model+=(5*x+75*y<=15)|odel+=150*x+75*y|model.solve()|model.objective.value()x.value())|y.value()")
```

