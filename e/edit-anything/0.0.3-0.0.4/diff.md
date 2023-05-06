# Comparing `tmp/edit-anything-0.0.3.tar.gz` & `tmp/edit-anything-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edit-anything-0.0.3.tar", last modified: Sat May  6 08:08:28 2023, max compression
+gzip compressed data, was "edit-anything-0.0.4.tar", last modified: Sat May  6 08:38:04 2023, max compression
```

## Comparing `edit-anything-0.0.3.tar` & `edit-anything-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.900666 edit-anything-0.0.3/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       52 2023-05-06 07:50:25.000000 edit-anything-0.0.3/MANIFEST.in
--rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 08:08:28.900153 edit-anything-0.0.3/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      361 2023-05-06 07:50:25.000000 edit-anything-0.0.3/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.881940 edit-anything-0.0.3/edit_anything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      681 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1683 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       55 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:52:47.000000 edit-anything-0.0.3/edit_anything.egg-info/not-zip-safe
--rw-r--r--   0 alvin-pc   (501) staff       (20)      129 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       10 2023-05-06 08:08:28.000000 edit-anything-0.0.3/edit_anything.egg-info/top_level.txt
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.882830 edit-anything-0.0.3/fastmodel/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.883169 edit-anything-0.0.3/fastmodel/backend/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.883612 edit-anything-0.0.3/fastmodel/backend/constant/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/constant/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      160 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/constant/biz_constants.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.883983 edit-anything-0.0.3/fastmodel/backend/domain/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/domain/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.885029 edit-anything-0.0.3/fastmodel/backend/domain/dto/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/domain/dto/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      174 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/domain/dto/req_classes.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      124 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/domain/dto/rsp_classes.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.885690 edit-anything-0.0.3/fastmodel/backend/exception/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/exception/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1221 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/exception/exceptions.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.886458 edit-anything-0.0.3/fastmodel/backend/inference/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/inference/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1160 2023-05-06 08:06:54.000000 edit-anything-0.0.3/fastmodel/backend/inference/inference.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.887365 edit-anything-0.0.3/fastmodel/backend/process/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/process/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/process/cv_process.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.889346 edit-anything-0.0.3/fastmodel/backend/util/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/util/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/util/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2066 2023-05-06 08:06:54.000000 edit-anything-0.0.3/fastmodel/backend/util/img_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1197 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/backend/util/str_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.889901 edit-anything-0.0.3/fastmodel/frontend/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.890298 edit-anything-0.0.3/fastmodel/frontend/edit-anything/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.877401 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.891526 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/css/
--rw-r--r--   0 alvin-pc   (501) staff       (20)    50507 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
--rw-r--r--   0 alvin-pc   (501) staff       (20)   101568 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.893052 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/img/
--rw-r--r--   0 alvin-pc   (501) staff       (20)    10462 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/img/favicon.ico
--rw-r--r--   0 alvin-pc   (501) staff       (20)   163424 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      697 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/index.html
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.898547 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/
--rw-r--r--   0 alvin-pc   (501) staff       (20)   834928 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/764.d32bc368.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2272 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)    49531 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)    39046 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/main.7d537378.js
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2226 2023-05-06 07:50:25.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.877780 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.878007 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/img/
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.899155 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/img/in/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:07:53.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/img/in/a.txt
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:08:28.899567 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/img/out/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-06 08:07:53.000000 edit-anything-0.0.3/fastmodel/frontend/edit-anything/tmp/img/out/a.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2689 2023-05-06 08:06:54.000000 edit-anything-0.0.3/fastmodel/main.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-06 08:08:28.900840 edit-anything-0.0.3/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1104 2023-05-06 08:08:27.000000 edit-anything-0.0.3/setup.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       52 2023-05-06 07:21:01.000000 edit-anything-0.0.4/MANIFEST.in
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      661 2023-05-06 08:38:04.557640 edit-anything-0.0.4/PKG-INFO
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      361 2023-05-06 07:21:01.000000 edit-anything-0.0.4/README.md
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/edit_anything.egg-info/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      661 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/PKG-INFO
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1683 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       54 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/entry_points.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 08:34:08.000000 edit-anything-0.0.4/edit_anything.egg-info/not-zip-safe
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      129 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/requires.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       10 2023-05-06 08:38:04.000000 edit-anything-0.0.4/edit_anything.egg-info/top_level.txt
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/__init__.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/__init__.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/constant/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/constant/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      160 2023-05-06 07:42:14.000000 edit-anything-0.0.4/fastmodel/backend/constant/biz_constants.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/domain/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/__init__.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/domain/dto/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      174 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/req_classes.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      124 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/domain/dto/rsp_classes.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/exception/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        1 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/exception/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1221 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/exception/exceptions.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/inference/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/inference/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1160 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/backend/inference/inference.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/process/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/process/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       65 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/process/cv_process.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/backend/util/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/__init__.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     3118 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/file.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2066 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/backend/util/img_util.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1197 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/backend/util/str_util.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/__init__.py
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    50507 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/801e8f75.css
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   101568 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/db720fc8.css
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    10462 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/favicon.ico
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   163424 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)      697 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/index.html
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)   834928 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2272 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    49531 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)    39046 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/main.7d537378.js
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     2226 2023-05-06 07:21:01.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.553640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/in/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/in/a.txt
+drwxr-xr-x   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:38:04.557640 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/out/
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)        0 2023-05-06 08:12:38.000000 edit-anything-0.0.4/fastmodel/frontend/edit-anything/tmp/img/out/a.txt
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     3425 2023-05-06 08:33:23.000000 edit-anything-0.0.4/fastmodel/main.py
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)       38 2023-05-06 08:38:04.557640 edit-anything-0.0.4/setup.cfg
+-rw-r--r--   0 PJLAB\xujun (409470380) PJLAB\domain^users (409469441)     1104 2023-05-06 08:36:52.000000 edit-anything-0.0.4/setup.py
```

### Comparing `edit-anything-0.0.3/PKG-INFO` & `edit-anything-0.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edit-anything
-Version: 0.0.3
+Version: 0.0.4
 Summary: EditAnything
 Home-page: https://github.com/xxx/xxxx
 Author: wfbi
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: EditAnything
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 
 # Install EditAnything In Local
 
 ```shell
 bash run.sh
@@ -34,9 +33,7 @@
 # 客户端安装
 pip install editanything -U
 # 启动服务
 editanything
 # 客户端访问
 http://{ip:9911}
 ```
-
-
```

### Comparing `edit-anything-0.0.3/edit_anything.egg-info/PKG-INFO` & `edit-anything-0.0.4/edit_anything.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edit-anything
-Version: 0.0.3
+Version: 0.0.4
 Summary: EditAnything
 Home-page: https://github.com/xxx/xxxx
 Author: wfbi
 Author-email: myname@example.com
 License: Apache License 2.0
 Keywords: EditAnything
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 
 # Install EditAnything In Local
 
 ```shell
 bash run.sh
@@ -34,9 +33,7 @@
 # 客户端安装
 pip install editanything -U
 # 启动服务
 editanything
 # 客户端访问
 http://{ip:9911}
 ```
-
-
```

### Comparing `edit-anything-0.0.3/edit_anything.egg-info/SOURCES.txt` & `edit-anything-0.0.4/edit_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/backend/exception/exceptions.py` & `edit-anything-0.0.4/fastmodel/backend/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/backend/inference/inference.py` & `edit-anything-0.0.4/fastmodel/backend/inference/inference.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/backend/util/file.py` & `edit-anything-0.0.4/fastmodel/backend/util/file.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/backend/util/img_util.py` & `edit-anything-0.0.4/fastmodel/backend/util/img_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/backend/util/str_util.py` & `edit-anything-0.0.4/fastmodel/backend/util/str_util.py`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/css/801e8f75.css` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/801e8f75.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/css/db720fc8.css` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/css/db720fc8.css`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/img/favicon.ico` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/assets/img/low-salary.de80db91.jpg`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/index.html` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/index.html`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/764.d32bc368.js` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/764.d32bc368.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/antd.a691f5d1.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/main.7d537378.js` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/main.7d537378.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js` & `edit-anything-0.0.4/fastmodel/frontend/edit-anything/js/runtime~main.0144593e.js`

 * *Files identical despite different names*

### Comparing `edit-anything-0.0.3/setup.py` & `edit-anything-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     for dirpath, dirnames, filenames in os.walk(base_dir):
         for filename in filenames:
             file_list.append(os.path.join(dirpath, filename))
     return file_list
 
 setup(
     name='edit-anything',
-    version='0.0.3',
+    version='0.0.4',
     description='EditAnything',
     long_description=utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='wfbi',
     author_email='myname@example.com',
     keywords='EditAnything',
     url='https://github.com/xxx/xxxx',
```

