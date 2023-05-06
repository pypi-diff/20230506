# Comparing `tmp/edit-anything-0.0.1.tar.gz` & `tmp/edit-anything-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edit-anything-0.0.1.tar", last modified: Sat May  6 07:52:47 2023, max compression
+gzip compressed data, was "edit-anything-0.0.2.tar", last modified: Sat May  6 08:00:59 2023, max compression
```

## Comparing `edit-anything-0.0.1.tar` & `edit-anything-0.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.064477 edit-anything-0.0.1/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       52 2023-05-06 07:50:25.000000 edit-anything-0.0.1/MANIFEST.in
--rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 07:52:47.063976 edit-anything-0.0.1/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      361 2023-05-06 07:50:25.000000 edit-anything-0.0.1/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.042242 edit-anything-0.0.1/edit_anything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1582 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       55 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/not-zip-safe
--rw-r--r--   0 alvin-pc   (501) staff       (20)      129 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       10 2023-05-06 07:52:47.000000 edit-anything-0.0.1/edit_anything.egg-info/top_level.txt
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.042735 edit-anything-0.0.1/fastmodel/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.043016 edit-anything-0.0.1/fastmodel/backend/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.043593 edit-anything-0.0.1/fastmodel/backend/constant/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/constant/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      160 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/constant/biz_constants.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.044071 edit-anything-0.0.1/fastmodel/backend/domain/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/domain/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.045394 edit-anything-0.0.1/fastmodel/backend/domain/dto/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/domain/dto/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      174 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/domain/dto/req_classes.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      124 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/domain/dto/rsp_classes.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.046523 edit-anything-0.0.1/fastmodel/backend/exception/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/exception/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1221 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/exception/exceptions.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.047377 edit-anything-0.0.1/fastmodel/backend/inference/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/inference/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1137 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/inference/inference.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.048328 edit-anything-0.0.1/fastmodel/backend/process/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/process/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/process/cv_process.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.050532 edit-anything-0.0.1/fastmodel/backend/util/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/util/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/util/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2043 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/util/img_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1197 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/backend/util/str_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.051076 edit-anything-0.0.1/fastmodel/frontend/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.051447 edit-anything-0.0.1/fastmodel/frontend/edit-anything/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.039266 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.053195 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/css/
--rw-r--r--   0 alvin-pc   (501) staff       (20)    50507 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
--rw-r--r--   0 alvin-pc   (501) staff       (20)   101568 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.056527 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/img/
--rw-r--r--   0 alvin-pc   (501) staff       (20)    10462 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/img/favicon.ico
--rw-r--r--   0 alvin-pc   (501) staff       (20)   163424 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      697 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/index.html
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:52:47.063218 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/
--rw-r--r--   0 alvin-pc   (501) staff       (20)   834928 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/764.d32bc368.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2272 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)    49531 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)    39046 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/main.7d537378.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2226 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2686 2023-05-06 07:50:25.000000 edit-anything-0.0.1/fastmodel/main.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-06 07:52:47.064648 edit-anything-0.0.1/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1104 2023-05-06 07:52:36.000000 edit-anything-0.0.1/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.671977 edit-anything-0.0.2/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       52 2023-05-06 07:50:25.000000 edit-anything-0.0.2/MANIFEST.in
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 08:00:59.671543 edit-anything-0.0.2/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      361 2023-05-06 07:50:25.000000 edit-anything-0.0.2/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.647187 edit-anything-0.0.2/edit_anything.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1582 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       55 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:52:47.000000 edit-anything-0.0.2/edit_anything.egg-info/not-zip-safe
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      129 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       10 2023-05-06 08:00:59.000000 edit-anything-0.0.2/edit_anything.egg-info/top_level.txt
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.647812 edit-anything-0.0.2/fastmodel/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.648425 edit-anything-0.0.2/fastmodel/backend/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.648865 edit-anything-0.0.2/fastmodel/backend/constant/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/constant/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      160 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/constant/biz_constants.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.650768 edit-anything-0.0.2/fastmodel/backend/domain/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/domain/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.652212 edit-anything-0.0.2/fastmodel/backend/domain/dto/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/domain/dto/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      174 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/domain/dto/req_classes.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      124 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/domain/dto/rsp_classes.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.653239 edit-anything-0.0.2/fastmodel/backend/exception/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/exception/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1221 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/exception/exceptions.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.654080 edit-anything-0.0.2/fastmodel/backend/inference/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/inference/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1137 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/inference/inference.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.654859 edit-anything-0.0.2/fastmodel/backend/process/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/process/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/process/cv_process.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.657436 edit-anything-0.0.2/fastmodel/backend/util/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/util/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/util/file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2043 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/util/img_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1197 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/backend/util/str_util.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.658159 edit-anything-0.0.2/fastmodel/frontend/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.658410 edit-anything-0.0.2/fastmodel/frontend/edit-anything/
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.642949 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.659631 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/css/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)    50507 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
+-rw-r--r--   0 alvin-pc   (501) staff       (20)   101568 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.661334 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/img/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)    10462 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/img/favicon.ico
+-rw-r--r--   0 alvin-pc   (501) staff       (20)   163424 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      697 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/index.html
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:00:59.670484 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)   834928 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/764.d32bc368.js
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2272 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)    49531 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
+-rw-r--r--   0 alvin-pc   (501) staff       (20)    39046 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/main.7d537378.js
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2226 2023-05-06 07:50:25.000000 edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2666 2023-05-06 08:00:22.000000 edit-anything-0.0.2/fastmodel/main.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-06 08:00:59.672153 edit-anything-0.0.2/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1104 2023-05-06 08:00:53.000000 edit-anything-0.0.2/setup.py
```

### Comparing `edit-anything-0.0.1/PKG-INFO` & `edit-anything-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edit-anything
-Version: 0.0.1
+Version: 0.0.2
 Summary: EditAnything
 Home-page: https://github.com/xxx/xxxx
 Author: wfbi
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: EditAnything
 Platform: UNKNOWN
```

### Comparing `edit-anything-0.0.1/edit_anything.egg-info/PKG-INFO` & `edit-anything-0.0.2/edit_anything.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edit-anything
-Version: 0.0.1
+Version: 0.0.2
 Summary: EditAnything
 Home-page: https://github.com/xxx/xxxx
 Author: wfbi
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: EditAnything
 Platform: UNKNOWN
```

### Comparing `edit-anything-0.0.1/edit_anything.egg-info/SOURCES.txt` & `edit-anything-0.0.2/edit_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/backend/exception/exceptions.py` & `edit-anything-0.0.2/fastmodel/backend/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/backend/inference/inference.py` & `edit-anything-0.0.2/fastmodel/backend/inference/inference.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/backend/util/file.py` & `edit-anything-0.0.2/fastmodel/backend/util/file.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/backend/util/img_util.py` & `edit-anything-0.0.2/fastmodel/backend/util/img_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/backend/util/str_util.py` & `edit-anything-0.0.2/fastmodel/backend/util/str_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/css/801e8f75.css` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/css/801e8f75.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/css/db720fc8.css` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/css/db720fc8.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/img/favicon.ico` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/index.html` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/index.html`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/764.d32bc368.js` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/764.d32bc368.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/main.7d537378.js` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/main.7d537378.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js` & `edit-anything-0.0.2/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.1/fastmodel/main.py` & `edit-anything-0.0.2/fastmodel/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 async def sd_inpaint(body: SdInpaintReqDto):
     image_base64 = body.image
     mask_base64 = body.mask
     image = img_base64_to_file(image_base64, generate_random_string(6))
     mask = img_base64_to_file(mask_base64, generate_random_string(6))
     prompt = body.prompt
     device = body.device
-    device = 'cuda'
 
     inpaint_img_path = inference_sd_inpaint(image, mask, prompt, device, generate_random_string(7))
 
 
     # todo base64 to image
 
     return {
```

### Comparing `edit-anything-0.0.1/setup.py` & `edit-anything-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for dirpath, dirnames, filenames in os.walk(base_dir):
         for filename in filenames:
             file_list.append(os.path.join(dirpath, filename))
     return file_list
 
 setup(
     name='edit-anything',
-    version='0.0.1',
+    version='0.0.2',
     description='EditAnything',
     long_description=utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='wfbi',
     author_email='myname@example.com',
     keywords='EditAnything',
     url='https://github.com/xxx/xxxx',
```

