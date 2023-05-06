# Comparing `tmp/buildsys-dateversion-2023.5.6.tar.gz` & `tmp/buildsys-dateversion-2023.5.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildsys-dateversion-2023.5.6.tar", last modified: Sat May  6 03:17:48 2023, max compression
+gzip compressed data, was "buildsys-dateversion-2023.5.6.3.tar", last modified: Sat May  6 03:30:50 2023, max compression
```

## Comparing `buildsys-dateversion-2023.5.6.tar` & `buildsys-dateversion-2023.5.6.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.203468 buildsys-dateversion-2023.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 03:17:47.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-06 03:17:44.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-06 03:17:44.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/tests/test_sample_projects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46507 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-06 03:30:49.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-06 03:30:47.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-06 03:30:47.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46507 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 03:30:50.000000 buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:30:50.134740 buildsys-dateversion-2023.5.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 03:30:38.000000 buildsys-dateversion-2023.5.6.3/tests/test_sample_projects.py
```

### Comparing `buildsys-dateversion-2023.5.6/LICENSE` & `buildsys-dateversion-2023.5.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6/PKG-INFO` & `buildsys-dateversion-2023.5.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildsys-dateversion
-Version: 2023.5.6
+Version: 2023.5.6.3
 Summary: Easy date-based versioning for Python projects
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,15 +684,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # buildsys-dateversion
 
 Easy date-based versioning for Python projects.
 
-![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)
+[![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)](https://pypi.org/project/buildsys-dateversion/)
 
 <!--TOC-->
 
 - [buildsys-dateversion](#buildsys-dateversion)
   - [Overview](#overview)
   - [Usage](#usage)
     - [Prerequisites](#prerequisites)
```

### Comparing `buildsys-dateversion-2023.5.6/README.md` & `buildsys-dateversion-2023.5.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # buildsys-dateversion
 
 Easy date-based versioning for Python projects.
 
-![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)
+[![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)](https://pypi.org/project/buildsys-dateversion/)
 
 <!--TOC-->
 
 - [buildsys-dateversion](#buildsys-dateversion)
   - [Overview](#overview)
   - [Usage](#usage)
     - [Prerequisites](#prerequisites)
```

### Comparing `buildsys-dateversion-2023.5.6/pyproject.toml` & `buildsys-dateversion-2023.5.6.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,11 +11,14 @@
 [project.urls]
 homepage = "https://github.com/rohanpm/buildsys-dateversion"
 
 [tool.setuptools.dynamic]
 version = { attr = "buildsys_dateversion.__version__" }
 dependencies = { file = "requirements.in" }
 
+[tool.isort]
+profile = "black"
+
 [build-system]
 requires = []
 backend-path = ["src"]
 build-backend = "buildsys_dateversion"
```

### Comparing `buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc` & `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0xc9c65564 (Sat May  6 03:17:29 2023 UTC)
+moddate:  0xdec95564 (Sat May  6 03:30:38 2023 UTC)
 files sz: 388
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a056d
       065a06010064025a0767006403a2015a0864045300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (1)
-                 4 LOAD_CONST               1 (('build_sdist', 'build_wheel', 'build_editable', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel'))
+                 4 LOAD_CONST               1 (('build_editable', 'build_sdist', 'build_wheel', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel'))
                  6 IMPORT_NAME              0 (_hooks)
-                 8 IMPORT_FROM              1 (build_sdist)
-                10 STORE_NAME               1 (build_sdist)
-                12 IMPORT_FROM              2 (build_wheel)
-                14 STORE_NAME               2 (build_wheel)
-                16 IMPORT_FROM              3 (build_editable)
-                18 STORE_NAME               3 (build_editable)
+                 8 IMPORT_FROM              1 (build_editable)
+                10 STORE_NAME               1 (build_editable)
+                12 IMPORT_FROM              2 (build_sdist)
+                14 STORE_NAME               2 (build_sdist)
+                16 IMPORT_FROM              3 (build_wheel)
+                18 STORE_NAME               3 (build_wheel)
                 20 IMPORT_FROM              4 (get_requires_for_build_editable)
                 22 STORE_NAME               4 (get_requires_for_build_editable)
                 24 IMPORT_FROM              5 (get_requires_for_build_sdist)
                 26 STORE_NAME               5 (get_requires_for_build_sdist)
                 28 IMPORT_FROM              6 (get_requires_for_build_wheel)
                 30 STORE_NAME               6 (get_requires_for_build_wheel)
                 32 POP_TOP
@@ -35,19 +35,19 @@
                 40 LOAD_CONST               3 (('build_sdist', 'build_wheel', 'build_editable', 'get_requires_for_build_wheel', 'get_requires_for_build_sdist', 'get_requires_for_build_editable'))
                 42 LIST_EXTEND              1
                 44 STORE_NAME               8 (__all__)
                 46 LOAD_CONST               4 (None)
                 48 RETURN_VALUE
    consts
       1
-      ('build_sdist', 'build_wheel', 'build_editable', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel')
+      ('build_editable', 'build_sdist', 'build_wheel', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel')
       '0'
       ('build_sdist', 'build_wheel', 'build_editable', 'get_requires_for_build_wheel', 'get_requires_for_build_sdist', 'get_requires_for_build_editable')
       None
-   names      ('_hooks', 'build_sdist', 'build_wheel', 'build_editable', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel', '__version__', '__all__')
+   names      ('_hooks', 'build_editable', 'build_sdist', 'build_wheel', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel', '__version__', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/__init__.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020120090402
```

### Comparing `buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc` & `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,92 +1,92 @@
 magic:    0xa70d0d0a
-moddate:  0xc9c65564 (Sat May  6 03:17:29 2023 UTC)
+moddate:  0xdec95564 (Sat May  6 03:30:38 2023 UTC)
 files sz: 12315
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      016c035a04640064016c055a04640064026c066d065a060100640064036c
-      076d085a080100640064016c095a09640064016c0a5a0a020065016a0b00
-      000000000000006404a6010000ab0100000000000000005a0c020065006a
+      016c035a03640064016c045a04640064016c055a06640064016c075a0664
+      0064026c086d095a090100640064036c0a6d0a5a0a0100020065016a0b00
+      000000000000006404a6010000ab0100000000000000005a0c020065026a
       0d00000000000000006405a6010000ab010000000000000000724b650ca0
       0e000000000000000000000000000000000000000065016a0f0000000000
       000000a6010000ab0100000000000000000100650ca01000000000000000
       00000000000000000000000000020065016a110000000000000000020065
-      006a0d00000000000000006405a6010000ab010000000000000000a60100
+      026a0d00000000000000006405a6010000ab010000000000000000a60100
       00ab010000000000000000a6010000ab0100000000000000000100020065
-      026a120000000000000000640665026a130000000000000000ac07a60200
+      036a120000000000000000640665036a130000000000000000ac07a60200
       00ab0200000000000000005a14640865156602640984045a160200470064
       0a8400640ba6020000ab0200000000000000005a176412640c84015a1864
       13640d84015a196412640e84015a1a6413640f84015a1b6413641084015a
       1c6413641184015a1d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (os)
-                 8 STORE_NAME               0 (os)
+                 6 IMPORT_NAME              0 (importlib)
+                 8 STORE_NAME               0 (importlib)
    
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
                 14 IMPORT_NAME              1 (logging)
                 16 STORE_NAME               1 (logging)
    
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               1 (None)
-                22 IMPORT_NAME              2 (re)
-                24 STORE_NAME               2 (re)
+                22 IMPORT_NAME              2 (os)
+                24 STORE_NAME               2 (os)
    
      4          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               1 (None)
-                30 IMPORT_NAME              3 (urllib.request)
-                32 STORE_NAME               4 (urllib)
+                30 IMPORT_NAME              3 (re)
+                32 STORE_NAME               3 (re)
    
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               1 (None)
-                38 IMPORT_NAME              5 (urllib.error)
-                40 STORE_NAME               4 (urllib)
+                38 IMPORT_NAME              4 (sys)
+                40 STORE_NAME               4 (sys)
    
      6          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               2 (('datetime',))
-                46 IMPORT_NAME              6 (datetime)
-                48 IMPORT_FROM              6 (datetime)
-                50 STORE_NAME               6 (datetime)
-                52 POP_TOP
-   
-     7          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               3 (('contextmanager',))
-                58 IMPORT_NAME              7 (contextlib)
-                60 IMPORT_FROM              8 (contextmanager)
-                62 STORE_NAME               8 (contextmanager)
-                64 POP_TOP
-   
-     8          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               1 (None)
-                70 IMPORT_NAME              9 (importlib)
-                72 STORE_NAME               9 (importlib)
-   
-     9          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               1 (None)
-                78 IMPORT_NAME             10 (sys)
-                80 STORE_NAME              10 (sys)
+                44 LOAD_CONST               1 (None)
+                46 IMPORT_NAME              5 (urllib.error)
+                48 STORE_NAME               6 (urllib)
+   
+     7          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               1 (None)
+                54 IMPORT_NAME              7 (urllib.request)
+                56 STORE_NAME               6 (urllib)
+   
+     8          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               2 (('contextmanager',))
+                62 IMPORT_NAME              8 (contextlib)
+                64 IMPORT_FROM              9 (contextmanager)
+                66 STORE_NAME               9 (contextmanager)
+                68 POP_TOP
+   
+     9          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               3 (('datetime',))
+                74 IMPORT_NAME             10 (datetime)
+                76 IMPORT_FROM             10 (datetime)
+                78 STORE_NAME              10 (datetime)
+                80 POP_TOP
    
     11          82 PUSH_NULL
                 84 LOAD_NAME                1 (logging)
                 86 LOAD_ATTR               11 (getLogger)
                 96 LOAD_CONST               4 ('buildsys-dateversion')
                 98 PRECALL                  1
                102 CALL                     1
                112 STORE_NAME              12 (LOG)
    
     13         114 PUSH_NULL
-               116 LOAD_NAME                0 (os)
+               116 LOAD_NAME                2 (os)
                118 LOAD_ATTR               13 (getenv)
                128 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
                130 PRECALL                  1
                134 CALL                     1
                144 POP_JUMP_FORWARD_IF_FALSE    75 (to 296)
    
     14         146 LOAD_NAME               12 (LOG)
@@ -99,30 +99,30 @@
    
     15         198 LOAD_NAME               12 (LOG)
                200 LOAD_METHOD             16 (addHandler)
                222 PUSH_NULL
                224 LOAD_NAME                1 (logging)
                226 LOAD_ATTR               17 (FileHandler)
                236 PUSH_NULL
-               238 LOAD_NAME                0 (os)
+               238 LOAD_NAME                2 (os)
                240 LOAD_ATTR               13 (getenv)
                250 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
                252 PRECALL                  1
                256 CALL                     1
                266 PRECALL                  1
                270 CALL                     1
                280 PRECALL                  1
                284 CALL                     1
                294 POP_TOP
    
     17     >>  296 PUSH_NULL
-               298 LOAD_NAME                2 (re)
+               298 LOAD_NAME                3 (re)
                300 LOAD_ATTR               18 (compile)
                310 LOAD_CONST               6 ('^__version__ *=.*$')
-               312 LOAD_NAME                2 (re)
+               312 LOAD_NAME                3 (re)
                314 LOAD_ATTR               19 (MULTILINE)
                324 KW_NAMES                 7
                326 PRECALL                  2
                330 CALL                     2
                340 STORE_NAME              20 (VERSION_PATTERN)
    
     20         342 LOAD_CONST               8 ('version')
@@ -171,16 +171,16 @@
                424 MAKE_FUNCTION            1 (defaults)
                426 STORE_NAME              29 (get_requires_for_build_editable)
                428 LOAD_CONST               1 (None)
                430 RETURN_VALUE
    consts
       0
       None
-      ('datetime',)
       ('contextmanager',)
+      ('datetime',)
       'buildsys-dateversion'
       'BUILDSYS_DATEVERSION_DEBUG'
       '^__version__ *=.*$'
       ('flags',)
       'version'
       code
          argcount  : 1
@@ -2291,17 +2291,17 @@
          cellvars   ()
          filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'get_requires_for_build_editable'
          firstlineno 340
          lnotab 0x020136012001
       (None, None)
       (None,)
-   names      ('os', 'logging', 're', 'urllib.request', 'urllib', 'urllib.error', 'datetime', 'contextlib', 'contextmanager', 'importlib', 'sys', 'getLogger', 'LOG', 'getenv', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'str', 'normalized', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable', 'get_requires_for_build_wheel', 'get_requires_for_build_sdist', 'get_requires_for_build_editable')
+   names      ('importlib', 'logging', 'os', 're', 'sys', 'urllib.error', 'urllib', 'urllib.request', 'contextlib', 'contextmanager', 'datetime', 'getLogger', 'LOG', 'getenv', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'str', 'normalized', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable', 'get_requires_for_build_wheel', 'get_requires_for_build_sdist', 'get_requires_for_build_editable')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010801080108010c010c010801080220022001340162
+      0x00ff020108010801080108010801080108010c010c0220022001340162
       022e030c081a7f007c080e0816080c08060807
```

### Comparing `buildsys-dateversion-2023.5.6/src/buildsys_dateversion/_hooks.py` & `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion/_hooks.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import os
+import importlib
 import logging
+import os
 import re
-import urllib.request
+import sys
 import urllib.error
-from datetime import datetime
+import urllib.request
 from contextlib import contextmanager
-import importlib
-import sys
+from datetime import datetime
 
 LOG = logging.getLogger("buildsys-dateversion")
 
 if os.getenv("BUILDSYS_DATEVERSION_DEBUG"):
     LOG.setLevel(logging.DEBUG)
     LOG.addHandler(logging.FileHandler(os.getenv("BUILDSYS_DATEVERSION_DEBUG")))
```

### Comparing `buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/PKG-INFO` & `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildsys-dateversion
-Version: 2023.5.6
+Version: 2023.5.6.3
 Summary: Easy date-based versioning for Python projects
 Author-email: Rohan McGovern <rohan@mcgovern.id.au>
 Maintainer-email: Rohan McGovern <rohan@mcgovern.id.au>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -684,15 +684,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # buildsys-dateversion
 
 Easy date-based versioning for Python projects.
 
-![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)
+[![PyPI](https://img.shields.io/pypi/v/buildsys-dateversion)](https://pypi.org/project/buildsys-dateversion/)
 
 <!--TOC-->
 
 - [buildsys-dateversion](#buildsys-dateversion)
   - [Overview](#overview)
   - [Usage](#usage)
     - [Prerequisites](#prerequisites)
```

### Comparing `buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/SOURCES.txt` & `buildsys-dateversion-2023.5.6.3/src/buildsys_dateversion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.6/tests/test_sample_projects.py` & `buildsys-dateversion-2023.5.6.3/tests/test_sample_projects.py`

 * *Files identical despite different names*

