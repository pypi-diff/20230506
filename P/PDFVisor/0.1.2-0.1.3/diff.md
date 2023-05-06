# Comparing `tmp/PDFVisor-0.1.2.tar.gz` & `tmp/PDFVisor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PDFVisor-0.1.2.tar", last modified: Sat May  6 14:00:49 2023, max compression
+gzip compressed data, was "PDFVisor-0.1.3.tar", last modified: Sat May  6 16:04:00 2023, max compression
```

## Comparing `PDFVisor-0.1.2.tar` & `PDFVisor-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:49.917055 PDFVisor-0.1.2/
--rw-rw-rw-   0        0        0      888 2023-03-30 11:59:20.000000 PDFVisor-0.1.2/LICENSE.rst
--rw-rw-rw-   0        0        0       60 2023-05-05 14:14:13.000000 PDFVisor-0.1.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:49.834372 PDFVisor-0.1.2/PDFVisor.egg-info/
--rw-rw-rw-   0        0        0     1478 2023-05-06 14:00:49.000000 PDFVisor-0.1.2/PDFVisor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-05-06 14:00:49.000000 PDFVisor-0.1.2/PDFVisor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 14:00:49.000000 PDFVisor-0.1.2/PDFVisor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-06 14:00:49.000000 PDFVisor-0.1.2/PDFVisor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 14:00:49.000000 PDFVisor-0.1.2/PDFVisor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1478 2023-05-06 14:00:49.917055 PDFVisor-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:40.000000 PDFVisor-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 14:00:49.928580 PDFVisor-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1815 2023-05-06 13:59:50.000000 PDFVisor-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:49.865616 PDFVisor-0.1.2/src/
--rw-rw-rw-   0        0        0     9817 2023-05-06 13:36:35.000000 PDFVisor-0.1.2/src/PDFViewr.py
--rw-rw-rw-   0        0        0        0 2023-04-07 17:56:52.000000 PDFVisor-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     4113 2023-04-14 20:56:10.000000 PDFVisor-0.1.2/src/funcsVisorPDF.py
-drwxrwxrwx   0        0        0        0 2023-05-06 14:00:49.917055 PDFVisor-0.1.2/src/img/
--rw-rw-rw-   0        0        0     5315 2023-04-21 15:35:44.000000 PDFVisor-0.1.2/src/img/avanceDeshabilitado.png
--rw-rw-rw-   0        0        0     4991 2023-04-21 14:52:58.000000 PDFVisor-0.1.2/src/img/avanceHighlight.png
--rw-rw-rw-   0        0        0     4385 2023-04-21 15:23:16.000000 PDFVisor-0.1.2/src/img/avanceHighlightPressed.png
--rw-rw-rw-   0        0        0     5250 2023-04-20 10:47:56.000000 PDFVisor-0.1.2/src/img/avanceNormal.png
--rw-rw-rw-   0        0        0     5231 2023-04-21 15:37:12.000000 PDFVisor-0.1.2/src/img/retroDeshabilitado.png
--rw-rw-rw-   0        0        0     4836 2023-04-21 15:27:38.000000 PDFVisor-0.1.2/src/img/retroHighlight.png
--rw-rw-rw-   0        0        0     4305 2023-04-21 15:24:26.000000 PDFVisor-0.1.2/src/img/retroHighlightPressed.png
--rw-rw-rw-   0        0        0     5947 2023-04-20 17:09:38.000000 PDFVisor-0.1.2/src/img/retroNormal.png
--rw-rw-rw-   0        0        0  1206884 2022-05-07 05:19:20.000000 PDFVisor-0.1.2/src/times.ttf
+drwxrwxrwx   0        0        0        0 2023-05-06 16:04:00.884785 PDFVisor-0.1.3/
+-rw-rw-rw-   0        0        0      888 2023-03-30 11:59:20.000000 PDFVisor-0.1.3/LICENSE.rst
+-rw-rw-rw-   0        0        0       52 2023-05-06 14:23:16.000000 PDFVisor-0.1.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-06 16:04:00.853503 PDFVisor-0.1.3/PDFVisor.egg-info/
+-rw-rw-rw-   0        0        0     1478 2023-05-06 16:04:00.000000 PDFVisor-0.1.3/PDFVisor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-05-06 16:04:00.000000 PDFVisor-0.1.3/PDFVisor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 16:04:00.000000 PDFVisor-0.1.3/PDFVisor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-06 16:04:00.000000 PDFVisor-0.1.3/PDFVisor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 16:04:00.000000 PDFVisor-0.1.3/PDFVisor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1478 2023-05-06 16:04:00.884785 PDFVisor-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1171 2023-03-29 11:56:40.000000 PDFVisor-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-06 16:04:00.884785 PDFVisor-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1779 2023-05-06 16:03:35.000000 PDFVisor-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 16:04:00.869153 PDFVisor-0.1.3/src/
+-rw-rw-rw-   0        0        0     9817 2023-05-06 14:10:16.000000 PDFVisor-0.1.3/src/PDFViewr.py
+-rw-rw-rw-   0        0        0        0 2023-04-07 17:56:52.000000 PDFVisor-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0     4113 2023-04-14 20:56:10.000000 PDFVisor-0.1.3/src/funcsVisorPDF.py
```

### Comparing `PDFVisor-0.1.2/LICENSE.rst` & `PDFVisor-0.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.2/PDFVisor.egg-info/PKG-INFO` & `PDFVisor-0.1.3/PDFVisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.2/PKG-INFO` & `PDFVisor-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PDFVisor
-Version: 0.1.2
+Version: 0.1.3
 Summary: Recurso para moverse por documentos PDF
 Author: Antonio San Román
 Author-email: asanro46@gmail.com
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
```

### Comparing `PDFVisor-0.1.2/README.md` & `PDFVisor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.2/setup.py` & `PDFVisor-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,26 +28,26 @@
       "numpy",
       "PyMuPDF",
       "opencv-contrib-python",
       ] 
 
 setup(
     name= "PDFVisor",
-    version= '0.1.2',
+    version= '0.1.3',
     description= 'Recurso para moverse por documentos PDF',
     long_description=  (HERE / "README.md").read_text(encoding='utf-8'),
     long_description_content_type= "text/markdown",
     author= 'Antonio San Román',
     author_email= 'asanro46@gmail.com',
     install_requires=INSTALL_REQUIRES,
     license= 'MIT',
     packages= ['PDFVisor'],
     package_dir= {'PDFVisor': 'src'},
     package_data = {
-        'PDFVisor': ['funcsVisorPDF.py', '*README.md', "LICENSE.rst", "MANIFEST.in"]
+        'PDFVisor': ['README.md', "LICENSE.rst"]
     },
     include_package_data=True,
     python_requires='>=3.4',
     cmdclass={
          'register': register,
          'upload': upload
          }
```

### Comparing `PDFVisor-0.1.2/src/PDFViewr.py` & `PDFVisor-0.1.3/src/PDFViewr.py`

 * *Files identical despite different names*

### Comparing `PDFVisor-0.1.2/src/funcsVisorPDF.py` & `PDFVisor-0.1.3/src/funcsVisorPDF.py`

 * *Files identical despite different names*

