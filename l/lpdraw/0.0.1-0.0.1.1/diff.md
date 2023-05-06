# Comparing `tmp/lpdraw-0.0.1.tar.gz` & `tmp/lpdraw-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpdraw-0.0.1.tar", last modified: Fri Apr 21 14:50:23 2023, max compression
+gzip compressed data, was "lpdraw-0.0.1.1.tar", last modified: Sat May  6 13:54:23 2023, max compression
```

## Comparing `lpdraw-0.0.1.tar` & `lpdraw-0.0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:50:23.159580 lpdraw-0.0.1/
--rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-20 19:31:35.000000 lpdraw-0.0.1/LICENSE
--rw-r--r--   0 ubaid      (501) staff       (20)     5780 2023-04-21 14:50:23.159432 lpdraw-0.0.1/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)     5337 2023-04-21 14:29:53.000000 lpdraw-0.0.1/README.md
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:50:23.158395 lpdraw-0.0.1/lpdraw/
--rw-r--r--   0 ubaid      (501) staff       (20)       71 2023-04-20 19:07:34.000000 lpdraw-0.0.1/lpdraw/__init__.py
--rw-r--r--   0 ubaid      (501) staff       (20)     2301 2023-04-21 14:48:27.000000 lpdraw-0.0.1/lpdraw/draw.py
-drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-04-21 14:50:23.159180 lpdraw-0.0.1/lpdraw.egg-info/
--rw-r--r--   0 ubaid      (501) staff       (20)     5780 2023-04-21 14:50:23.000000 lpdraw-0.0.1/lpdraw.egg-info/PKG-INFO
--rw-r--r--   0 ubaid      (501) staff       (20)      209 2023-04-21 14:50:23.000000 lpdraw-0.0.1/lpdraw.egg-info/SOURCES.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-04-21 14:50:23.000000 lpdraw-0.0.1/lpdraw.egg-info/dependency_links.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        8 2023-04-21 14:50:23.000000 lpdraw-0.0.1/lpdraw.egg-info/requires.txt
--rw-r--r--   0 ubaid      (501) staff       (20)        7 2023-04-21 14:50:23.000000 lpdraw-0.0.1/lpdraw.egg-info/top_level.txt
--rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-04-21 14:50:23.159622 lpdraw-0.0.1/setup.cfg
--rw-r--r--   0 ubaid      (501) staff       (20)     1915 2023-04-21 14:48:32.000000 lpdraw-0.0.1/setup.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:54:23.489764 lpdraw-0.0.1.1/
+-rw-r--r--   0 ubaid      (501) staff       (20)     1072 2023-04-20 19:31:35.000000 lpdraw-0.0.1.1/LICENSE
+-rw-r--r--   0 ubaid      (501) staff       (20)     5782 2023-05-06 13:54:23.489644 lpdraw-0.0.1.1/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)     5337 2023-05-06 13:52:09.000000 lpdraw-0.0.1.1/README.md
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:54:23.488857 lpdraw-0.0.1.1/lpdraw/
+-rw-r--r--   0 ubaid      (501) staff       (20)       71 2023-05-06 13:47:15.000000 lpdraw-0.0.1.1/lpdraw/__init__.py
+-rw-r--r--   0 ubaid      (501) staff       (20)     2354 2023-05-06 13:52:28.000000 lpdraw-0.0.1.1/lpdraw/draw.py
+drwxr-xr-x   0 ubaid      (501) staff       (20)        0 2023-05-06 13:54:23.489478 lpdraw-0.0.1.1/lpdraw.egg-info/
+-rw-r--r--   0 ubaid      (501) staff       (20)     5782 2023-05-06 13:54:23.000000 lpdraw-0.0.1.1/lpdraw.egg-info/PKG-INFO
+-rw-r--r--   0 ubaid      (501) staff       (20)      209 2023-05-06 13:54:23.000000 lpdraw-0.0.1.1/lpdraw.egg-info/SOURCES.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        1 2023-05-06 13:54:23.000000 lpdraw-0.0.1.1/lpdraw.egg-info/dependency_links.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       18 2023-05-06 13:54:23.000000 lpdraw-0.0.1.1/lpdraw.egg-info/requires.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)        7 2023-05-06 13:54:23.000000 lpdraw-0.0.1.1/lpdraw.egg-info/top_level.txt
+-rw-r--r--   0 ubaid      (501) staff       (20)       38 2023-05-06 13:54:23.489804 lpdraw-0.0.1.1/setup.cfg
+-rw-r--r--   0 ubaid      (501) staff       (20)     1927 2023-05-06 13:52:28.000000 lpdraw-0.0.1.1/setup.py
```

### Comparing `lpdraw-0.0.1/LICENSE` & `lpdraw-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lpdraw-0.0.1/PKG-INFO` & `lpdraw-0.0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpdraw
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A simple python drawing package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 This package can display the output on terminal as well as visually appealing grayscale image.
 
 ## Usage
 
 **Example:**
 ```python
 from lpdraw import Line, Circle, Clear, DisplayTerminal
-from lptypes import i32, Const
+from lpython import i32, Const
 
 from numpy import empty, int32
 
 def main():
     Width: Const[i32] = 100 # x-axis limits [0, 99]
     Height: Const[i32] = 40 # y-axis limits [0, 39]
     Screen: i32[Height, Width] = empty((Height, Width), dtype=int32)
```

### Comparing `lpdraw-0.0.1/README.md` & `lpdraw-0.0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This package can display the output on terminal as well as visually appealing grayscale image.
 
 ## Usage
 
 **Example:**
 ```python
 from lpdraw import Line, Circle, Clear, DisplayTerminal
-from lptypes import i32, Const
+from lpython import i32, Const
 
 from numpy import empty, int32
 
 def main():
     Width: Const[i32] = 100 # x-axis limits [0, 99]
     Height: Const[i32] = 40 # y-axis limits [0, 39]
     Screen: i32[Height, Width] = empty((Height, Width), dtype=int32)
```

### Comparing `lpdraw-0.0.1/lpdraw/draw.py` & `lpdraw-0.0.1.1/lpdraw/draw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from lptypes import i32, f64, TypeVar
+from lpython import i32, f64, TypeVar
+import numpy
 
 H = TypeVar("H")
 W = TypeVar("W")
 
 def Pixel(H: i32, W: i32, Screen: i32[H, W], x: i32, y: i32) -> None:
     if x >= 0 and y >= 0 and x < W and y < H:
-        Screen[i32(int(H - 1 - y)), i32(int(x))] = 255
+        Screen[H - 1 - y, x] = 255
 
 def Clear(H: i32, W: i32, Screen: i32[H, W]):
     i: i32
     j: i32
     for i in range(H):
         for j in range(W):
             Screen[i, j] = 0
@@ -48,41 +49,48 @@
     for i in range(H):
         for j in range(W):
             print(Screen[i, j])
 
 def Line(H: i32, W: i32, Screen: i32[H, W], x1: i32, y1: i32, x2: i32, y2: i32) -> None:
     dx: i32 = abs(x2 - x1)
     dy: i32 = abs(y2 - y1)
+
     sx: i32
     sy: i32
 
-    if x1 > x2:
-        sx = -1
-    else:
+    if x1 < x2:
         sx = 1
-    if y1 > y2:
-        sy = -1
     else:
+        sx = -1
+
+    if y1 < y2:
         sy = 1
+    else:
+        sy = -1
 
     err: i32 = dx - dy
 
     while x1 != x2 or y1 != y2:
         Pixel(H, W, Screen, x1, y1)
         e2: i32 = 2 * err
+
         if e2 > -dy:
             err -= dy
             x1 += sx
+
+        if x1 == x2 and y1 == y2:
+            Pixel(H, W, Screen, x1, y1)
+            break
+
         if e2 < dx:
             err += dx
             y1 += sy
-    Pixel(H, W, Screen, x2, y2)
 
 def Circle(H: i32, W: i32, Screen: i32[H, W], x: i32, y: i32, r: f64) -> None:
-    x0: i32 = i32(int(r))
+    x0: i32 = i32(r)
     y0: i32 = 0
     err: i32 = 0
 
     while x0 >= y0:
         Pixel(H, W, Screen, x + x0, y + y0)
         Pixel(H, W, Screen, x - x0, y + y0)
         Pixel(H, W, Screen, x + x0, y - y0)
```

### Comparing `lpdraw-0.0.1/lpdraw.egg-info/PKG-INFO` & `lpdraw-0.0.1.1/lpdraw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpdraw
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: A simple python drawing package
 Home-page: https://github.com/Shaikh-Ubaid/lpython_packages
 Author: Ubaid Shaikh
 Author-email: shaikhubaid769@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 This package can display the output on terminal as well as visually appealing grayscale image.
 
 ## Usage
 
 **Example:**
 ```python
 from lpdraw import Line, Circle, Clear, DisplayTerminal
-from lptypes import i32, Const
+from lpython import i32, Const
 
 from numpy import empty, int32
 
 def main():
     Width: Const[i32] = 100 # x-axis limits [0, 99]
     Height: Const[i32] = 40 # y-axis limits [0, 39]
     Screen: i32[Height, Width] = empty((Height, Width), dtype=int32)
```

### Comparing `lpdraw-0.0.1/setup.py` & `lpdraw-0.0.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # The setup.py file is used as the build script for setuptools. Setuptools is a
 # package that allows you to easily build and distribute Python distributions.
 
 import setuptools
 
 # Define required packages. Alternatively, these could be defined in a separate
 # file and read in here.
-REQUIRED_PACKAGES=["lptypes"]
+REQUIRED_PACKAGES=["lpython_emulation"]
 
-VERSION="0.0.1"
+VERSION="0.0.1.1"
 
 # Read in the project description. We define this in the README file.
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lpdraw",                                              # name of project
```

