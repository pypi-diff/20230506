# Comparing `tmp/buildsys-dateversion-2023.5.1.23.tar.gz` & `tmp/buildsys-dateversion-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildsys-dateversion-2023.5.1.23.tar", last modified: Mon May  1 23:49:19 2023, max compression
+gzip compressed data, was "buildsys-dateversion-2023.5.6.tar", last modified: Sat May  6 03:17:48 2023, max compression
```

## Comparing `buildsys-dateversion-2023.5.1.23.tar` & `buildsys-dateversion-2023.5.6.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:49:19.019877 buildsys-dateversion-2023.5.1.23/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)    35149 2023-05-01 22:04:41.000000 buildsys-dateversion-2023.5.1.23/LICENSE
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       26 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5.1.23/MANIFEST.in
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       92 2023-05-01 23:49:19.019877 buildsys-dateversion-2023.5.1.23/PKG-INFO
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       72 2023-05-01 23:30:19.000000 buildsys-dateversion-2023.5.1.23/README.md
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      264 2023-05-01 23:28:43.000000 buildsys-dateversion-2023.5.1.23/pyproject.toml
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       38 2023-05-01 23:49:19.019877 buildsys-dateversion-2023.5.1.23/setup.cfg
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:49:19.017877 buildsys-dateversion-2023.5.1.23/src/
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:49:19.018877 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      187 2023-05-01 23:49:18.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/__init__.py
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:49:19.019877 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/__pycache__/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      351 2023-05-01 23:49:18.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)    12590 2023-05-01 23:49:18.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     9497 2023-05-01 23:47:29.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/_hooks.py
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-01 23:49:19.018877 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion.egg-info/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       92 2023-05-01 23:49:19.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion.egg-info/PKG-INFO
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      430 2023-05-01 23:49:19.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion.egg-info/SOURCES.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        1 2023-05-01 23:49:19.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion.egg-info/dependency_links.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       21 2023-05-01 23:49:19.000000 buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.203468 buildsys-dateversion-2023.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-06 03:17:47.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-06 03:17:44.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-05-06 03:17:44.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion/_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46455 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 03:17:48.000000 buildsys-dateversion-2023.5.6/src/buildsys_dateversion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 03:17:48.207468 buildsys-dateversion-2023.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 03:17:29.000000 buildsys-dateversion-2023.5.6/tests/test_sample_projects.py
```

### Comparing `buildsys-dateversion-2023.5.1.23/LICENSE` & `buildsys-dateversion-2023.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc` & `buildsys-dateversion-2023.5.6/src/buildsys_dateversion/__pycache__/_hooks.cpython-311.pyc`

 * *Files 21% similar despite different names*

#### Python bytecode

```diff
@@ -1,30 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0x914f5064 (Mon May  1 23:47:29 2023 UTC)
-files sz: 9497
+moddate:  0xc9c65564 (Sat May  6 03:17:29 2023 UTC)
+files sz: 12315
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
       016c035a04640064016c055a04640064026c066d065a060100640064036c
-      076d085a080100640064016c095a09020065016a0a000000000000000064
-      04a6010000ab0100000000000000005a0b020065006a0c00000000000000
-      006405a6010000ab010000000000000000724b650ba00d00000000000000
-      0000000000000000000000000065016a0e0000000000000000a6010000ab
-      0100000000000000000100650ba00f000000000000000000000000000000
-      0000000000020065016a100000000000000000020065006a0c0000000000
-      0000006405a6010000ab010000000000000000a6010000ab010000000000
-      000000a6010000ab0100000000000000000100020065026a110000000000
-      000000640665026a120000000000000000ac07a6020000ab020000000000
-      0000005a13640865146602640984045a1502004700640a8400640ba60200
-      00ab0200000000000000005a16640f640c84015a176410640d84015a1864
-      0f640e84015a1964015300
+      076d085a080100640064016c095a09640064016c0a5a0a020065016a0b00
+      000000000000006404a6010000ab0100000000000000005a0c020065006a
+      0d00000000000000006405a6010000ab010000000000000000724b650ca0
+      0e000000000000000000000000000000000000000065016a0f0000000000
+      000000a6010000ab0100000000000000000100650ca01000000000000000
+      00000000000000000000000000020065016a110000000000000000020065
+      006a0d00000000000000006405a6010000ab010000000000000000a60100
+      00ab010000000000000000a6010000ab0100000000000000000100020065
+      026a120000000000000000640665026a130000000000000000ac07a60200
+      00ab0200000000000000005a14640865156602640984045a160200470064
+      0a8400640ba6020000ab0200000000000000005a176412640c84015a1864
+      13640d84015a196412640e84015a1a6413640f84015a1b6413641084015a
+      1c6413641184015a1d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -63,98 +64,118 @@
                 64 POP_TOP
    
      8          66 LOAD_CONST               0 (0)
                 68 LOAD_CONST               1 (None)
                 70 IMPORT_NAME              9 (importlib)
                 72 STORE_NAME               9 (importlib)
    
-    10          74 PUSH_NULL
-                76 LOAD_NAME                1 (logging)
-                78 LOAD_ATTR               10 (getLogger)
-                88 LOAD_CONST               4 ('buildsys-dateversion')
-                90 PRECALL                  1
-                94 CALL                     1
-               104 STORE_NAME              11 (LOG)
-   
-    12         106 PUSH_NULL
-               108 LOAD_NAME                0 (os)
-               110 LOAD_ATTR               12 (getenv)
-               120 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
-               122 PRECALL                  1
-               126 CALL                     1
-               136 POP_JUMP_FORWARD_IF_FALSE    75 (to 288)
-   
-    13         138 LOAD_NAME               11 (LOG)
-               140 LOAD_METHOD             13 (setLevel)
-               162 LOAD_NAME                1 (logging)
-               164 LOAD_ATTR               14 (DEBUG)
-               174 PRECALL                  1
-               178 CALL                     1
-               188 POP_TOP
-   
-    14         190 LOAD_NAME               11 (LOG)
-               192 LOAD_METHOD             15 (addHandler)
-               214 PUSH_NULL
-               216 LOAD_NAME                1 (logging)
-               218 LOAD_ATTR               16 (FileHandler)
-               228 PUSH_NULL
-               230 LOAD_NAME                0 (os)
-               232 LOAD_ATTR               12 (getenv)
-               242 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
-               244 PRECALL                  1
-               248 CALL                     1
-               258 PRECALL                  1
-               262 CALL                     1
-               272 PRECALL                  1
-               276 CALL                     1
-               286 POP_TOP
-   
-    16     >>  288 PUSH_NULL
-               290 LOAD_NAME                2 (re)
-               292 LOAD_ATTR               17 (compile)
-               302 LOAD_CONST               6 ('^__version__ *=.*$')
-               304 LOAD_NAME                2 (re)
-               306 LOAD_ATTR               18 (MULTILINE)
-               316 KW_NAMES                 7
-               318 PRECALL                  2
-               322 CALL                     2
-               332 STORE_NAME              19 (VERSION_PATTERN)
-   
-    19         334 LOAD_CONST               8 ('version')
-               336 LOAD_NAME               20 (str)
-               338 BUILD_TUPLE              2
-               340 LOAD_CONST               9 (<code object normalized, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 19>)
-               342 MAKE_FUNCTION            4 (annotations)
-               344 STORE_NAME              21 (normalized)
-   
-    27         346 PUSH_NULL
-               348 LOAD_BUILD_CLASS
-               350 LOAD_CONST              10 (<code object DateVersion, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 27>)
-               352 MAKE_FUNCTION            0
-               354 LOAD_CONST              11 ('DateVersion')
-               356 PRECALL                  2
-               360 CALL                     2
-               370 STORE_NAME              22 (DateVersion)
-   
-   219         372 LOAD_CONST              15 ((None, None))
-               374 LOAD_CONST              12 (<code object build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 219>)
-               376 MAKE_FUNCTION            1 (defaults)
-               378 STORE_NAME              23 (build_wheel)
+     9          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               1 (None)
+                78 IMPORT_NAME             10 (sys)
+                80 STORE_NAME              10 (sys)
    
-   229         380 LOAD_CONST              16 ((None,))
-               382 LOAD_CONST              13 (<code object build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 229>)
+    11          82 PUSH_NULL
+                84 LOAD_NAME                1 (logging)
+                86 LOAD_ATTR               11 (getLogger)
+                96 LOAD_CONST               4 ('buildsys-dateversion')
+                98 PRECALL                  1
+               102 CALL                     1
+               112 STORE_NAME              12 (LOG)
+   
+    13         114 PUSH_NULL
+               116 LOAD_NAME                0 (os)
+               118 LOAD_ATTR               13 (getenv)
+               128 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
+               130 PRECALL                  1
+               134 CALL                     1
+               144 POP_JUMP_FORWARD_IF_FALSE    75 (to 296)
+   
+    14         146 LOAD_NAME               12 (LOG)
+               148 LOAD_METHOD             14 (setLevel)
+               170 LOAD_NAME                1 (logging)
+               172 LOAD_ATTR               15 (DEBUG)
+               182 PRECALL                  1
+               186 CALL                     1
+               196 POP_TOP
+   
+    15         198 LOAD_NAME               12 (LOG)
+               200 LOAD_METHOD             16 (addHandler)
+               222 PUSH_NULL
+               224 LOAD_NAME                1 (logging)
+               226 LOAD_ATTR               17 (FileHandler)
+               236 PUSH_NULL
+               238 LOAD_NAME                0 (os)
+               240 LOAD_ATTR               13 (getenv)
+               250 LOAD_CONST               5 ('BUILDSYS_DATEVERSION_DEBUG')
+               252 PRECALL                  1
+               256 CALL                     1
+               266 PRECALL                  1
+               270 CALL                     1
+               280 PRECALL                  1
+               284 CALL                     1
+               294 POP_TOP
+   
+    17     >>  296 PUSH_NULL
+               298 LOAD_NAME                2 (re)
+               300 LOAD_ATTR               18 (compile)
+               310 LOAD_CONST               6 ('^__version__ *=.*$')
+               312 LOAD_NAME                2 (re)
+               314 LOAD_ATTR               19 (MULTILINE)
+               324 KW_NAMES                 7
+               326 PRECALL                  2
+               330 CALL                     2
+               340 STORE_NAME              20 (VERSION_PATTERN)
+   
+    20         342 LOAD_CONST               8 ('version')
+               344 LOAD_NAME               21 (str)
+               346 BUILD_TUPLE              2
+               348 LOAD_CONST               9 (<code object normalized, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 20>)
+               350 MAKE_FUNCTION            4 (annotations)
+               352 STORE_NAME              22 (normalized)
+   
+    28         354 PUSH_NULL
+               356 LOAD_BUILD_CLASS
+               358 LOAD_CONST              10 (<code object DateVersion, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 28>)
+               360 MAKE_FUNCTION            0
+               362 LOAD_CONST              11 ('DateVersion')
+               364 PRECALL                  2
+               368 CALL                     2
+               378 STORE_NAME              23 (DateVersion)
+   
+   279         380 LOAD_CONST              18 ((None, None))
+               382 LOAD_CONST              12 (<code object build_wheel, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 279>)
                384 MAKE_FUNCTION            1 (defaults)
-               386 STORE_NAME              24 (build_sdist)
+               386 STORE_NAME              24 (build_wheel)
    
-   249         388 LOAD_CONST              15 ((None, None))
-               390 LOAD_CONST              14 (<code object build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 249>)
+   293         388 LOAD_CONST              19 ((None,))
+               390 LOAD_CONST              13 (<code object build_sdist, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 293>)
                392 MAKE_FUNCTION            1 (defaults)
-               394 STORE_NAME              25 (build_editable)
-               396 LOAD_CONST               1 (None)
-               398 RETURN_VALUE
+               394 STORE_NAME              25 (build_sdist)
+   
+   315         396 LOAD_CONST              18 ((None, None))
+               398 LOAD_CONST              14 (<code object build_editable, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 315>)
+               400 MAKE_FUNCTION            1 (defaults)
+               402 STORE_NAME              26 (build_editable)
+   
+   327         404 LOAD_CONST              19 ((None,))
+               406 LOAD_CONST              15 (<code object get_requires_for_build_wheel, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 327>)
+               408 MAKE_FUNCTION            1 (defaults)
+               410 STORE_NAME              27 (get_requires_for_build_wheel)
+   
+   333         412 LOAD_CONST              19 ((None,))
+               414 LOAD_CONST              16 (<code object get_requires_for_build_sdist, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 333>)
+               416 MAKE_FUNCTION            1 (defaults)
+               418 STORE_NAME              28 (get_requires_for_build_sdist)
+   
+   340         420 LOAD_CONST              19 ((None,))
+               422 LOAD_CONST              17 (<code object get_requires_for_build_editable, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 340>)
+               424 MAKE_FUNCTION            1 (defaults)
+               426 STORE_NAME              29 (get_requires_for_build_editable)
+               428 LOAD_CONST               1 (None)
+               430 RETURN_VALUE
    consts
       0
       None
       ('datetime',)
       ('contextmanager',)
       'buildsys-dateversion'
       'BUILDSYS_DATEVERSION_DEBUG'
@@ -167,19 +188,19 @@
          stacksize : 6
          flags     : 3
          code
             0x97006401a0000000000000000000000000000000000000000000640284
             007c00a00100000000000000000000000000000000000000006401a60100
             00ab0100000000000000004400a6000000ab000000000000000000a60100
             00ab0100000000000000005300
-          19           0 RESUME                   0
+          20           0 RESUME                   0
          
-          24           2 LOAD_CONST               1 ('.')
+          25           2 LOAD_CONST               1 ('.')
                        4 LOAD_METHOD              0 (join)
-                      26 LOAD_CONST               2 (<code object <listcomp>, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 24>)
+                      26 LOAD_CONST               2 (<code object <listcomp>, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 25>)
                       28 MAKE_FUNCTION            0
                       30 LOAD_FAST                0 (version)
                       32 LOAD_METHOD              1 (split)
                       54 LOAD_CONST               1 ('.')
                       56 PRECALL                  1
                       60 CALL                     1
                       70 GET_ITER
@@ -196,15 +217,15 @@
                nlocals   : 2
                stacksize : 7
                flags     : 19
                code
                   0x970067007c005d1e7d0174010000000000000000000074030000000000
                   00000000007c01a6010000ab010000000000000000a6010000ab01000000
                   000000000091028c1f5300
-                24           0 RESUME                   0
+                25           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                30 (to 68)
                              8 STORE_FAST               1 (x)
                             10 LOAD_GLOBAL              1 (NULL + str)
                             22 LOAD_GLOBAL              3 (NULL + int)
                             34 LOAD_FAST                1 (x)
@@ -216,260 +237,532 @@
                             66 JUMP_BACKWARD           31 (to 6)
                        >>   68 RETURN_VALUE
                consts
                names      ('str', 'int')
                varnames   ('.0', 'x')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '<listcomp>'
-               firstlineno 24
+               firstlineno 25
                lnotab 0x
          names      ('join', 'split')
          varnames   ('version',)
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'normalized'
-         firstlineno 19
+         firstlineno 20
          lnotab 0x0205
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
-            0x970065005a0164005a026412640284015a036504640365056602640484
-            04a6000000ab0000000000000000005a06640365056602640584045a0765
-            0464036505660264068404a6000000ab0000000000000000005a08650464
-            078400a6000000ab0000000000000000005a096504640365056602640884
-            04a6000000ab0000000000000000005a0a650464036505660264098404a6
-            000000ab0000000000000000005a0b6504640365056602640a8404a60000
-            00ab0000000000000000005a0c640365056602640b84045a0d640c650564
-            03650e6604640d84045a0f6510640e8400a6000000ab0000000000000000
-            005a11640f84005a12641084005a13641184005a1464015300
-          27           0 RESUME                   0
+            0x970065005a0164005a026419640284015a036504640365056602640484
+            04a6000000ab0000000000000000005a06650464036505660264058404a6
+            000000ab0000000000000000005a07650464036505660264068404a60000
+            00ab0000000000000000005a08650464036509660264078404a6000000ab
+            0000000000000000005a0a640365096602640884045a0b65046403650966
+            0264098404a6000000ab0000000000000000005a0c650464036509660264
+            0a8404a6000000ab0000000000000000005a0d6504640b8400a6000000ab
+            0000000000000000005a0e6504640365096602640c8404a6000000ab0000
+            000000000000005a0f6504640365096602640d8404a6000000ab00000000
+            00000000005a106504640365096602640e8404a6000000ab000000000000
+            0000005a11640365096602640f84045a1264106509640365136604641184
+            045a14651564128400a6000000ab0000000000000000005a16641384005a
+            17641484005a18641584005a19641684005a1a641784005a1b641884005a
+            1c64015300
+          28           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DateVersion')
                        8 STORE_NAME               2 (__qualname__)
          
-          28          10 LOAD_CONST              18 ((None,))
-                      12 LOAD_CONST               2 (<code object __init__, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 28>)
+          29          10 LOAD_CONST              25 ((None,))
+                      12 LOAD_CONST               2 (<code object __init__, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 29>)
                       14 MAKE_FUNCTION            1 (defaults)
                       16 STORE_NAME               3 (__init__)
          
-          33          18 LOAD_NAME                4 (property)
+          36          18 LOAD_NAME                4 (property)
          
-          34          20 LOAD_CONST               3 ('return')
-                      22 LOAD_NAME                5 (str)
+          37          20 LOAD_CONST               3 ('return')
+                      22 LOAD_NAME                5 (dict)
                       24 BUILD_TUPLE              2
-                      26 LOAD_CONST               4 (<code object marker, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 33>)
+                      26 LOAD_CONST               4 (<code object pyproject_toml, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 36>)
                       28 MAKE_FUNCTION            4 (annotations)
          
-          33          30 PRECALL                  0
+          36          30 PRECALL                  0
                       34 CALL                     0
          
-          34          44 STORE_NAME               6 (marker)
+          37          44 STORE_NAME               6 (pyproject_toml)
+         
+          53          46 LOAD_NAME                4 (property)
+         
+          54          48 LOAD_CONST               3 ('return')
+                      50 LOAD_NAME                5 (dict)
+                      52 BUILD_TUPLE              2
+                      54 LOAD_CONST               5 (<code object project_config, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 53>)
+                      56 MAKE_FUNCTION            4 (annotations)
+         
+          53          58 PRECALL                  0
+                      62 CALL                     0
+         
+          54          72 STORE_NAME               7 (project_config)
+         
+          57          74 LOAD_NAME                4 (property)
+         
+          58          76 LOAD_CONST               3 ('return')
+                      78 LOAD_NAME                5 (dict)
+                      80 BUILD_TUPLE              2
+                      82 LOAD_CONST               6 (<code object tool_config, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 57>)
+                      84 MAKE_FUNCTION            4 (annotations)
+         
+          57          86 PRECALL                  0
+                      90 CALL                     0
+         
+          58         100 STORE_NAME               8 (tool_config)
+         
+          66         102 LOAD_NAME                4 (property)
+         
+          67         104 LOAD_CONST               3 ('return')
+                     106 LOAD_NAME                9 (str)
+                     108 BUILD_TUPLE              2
+                     110 LOAD_CONST               7 (<code object marker, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 66>)
+                     112 MAKE_FUNCTION            4 (annotations)
+         
+          66         114 PRECALL                  0
+                     118 CALL                     0
+         
+          67         128 STORE_NAME              10 (marker)
+         
+          73         130 LOAD_CONST               3 ('return')
+                     132 LOAD_NAME                9 (str)
+                     134 BUILD_TUPLE              2
+                     136 LOAD_CONST               8 (<code object _find_version_path, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 73>)
+                     138 MAKE_FUNCTION            4 (annotations)
+                     140 STORE_NAME              11 (_find_version_path)
+         
+          90         142 LOAD_NAME                4 (property)
+         
+          91         144 LOAD_CONST               3 ('return')
+                     146 LOAD_NAME                9 (str)
+                     148 BUILD_TUPLE              2
+                     150 LOAD_CONST               9 (<code object version_path, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 90>)
+                     152 MAKE_FUNCTION            4 (annotations)
          
-          40          46 LOAD_CONST               3 ('return')
-                      48 LOAD_NAME                5 (str)
-                      50 BUILD_TUPLE              2
-                      52 LOAD_CONST               5 (<code object _find_version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 40>)
-                      54 MAKE_FUNCTION            4 (annotations)
-                      56 STORE_NAME               7 (_find_version_path)
+          90         154 PRECALL                  0
+                     158 CALL                     0
          
-          57          58 LOAD_NAME                4 (property)
+          91         168 STORE_NAME              12 (version_path)
          
-          58          60 LOAD_CONST               3 ('return')
-                      62 LOAD_NAME                5 (str)
-                      64 BUILD_TUPLE              2
-                      66 LOAD_CONST               6 (<code object version_path, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 57>)
-                      68 MAKE_FUNCTION            4 (annotations)
+          96         170 LOAD_NAME                4 (property)
          
-          57          70 PRECALL                  0
-                      74 CALL                     0
+          97         172 LOAD_CONST               3 ('return')
+                     174 LOAD_NAME                9 (str)
+                     176 BUILD_TUPLE              2
+                     178 LOAD_CONST              10 (<code object build_backend_name, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 96>)
+                     180 MAKE_FUNCTION            4 (annotations)
          
-          58          84 STORE_NAME               8 (version_path)
+          96         182 PRECALL                  0
+                     186 CALL                     0
          
-          63          86 LOAD_NAME                4 (property)
+          97         196 STORE_NAME              13 (build_backend_name)
          
-          64          88 LOAD_CONST               7 (<code object build_backend, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 63>)
-                      90 MAKE_FUNCTION            0
+         102         198 LOAD_NAME                4 (property)
          
-          63          92 PRECALL                  0
-                      96 CALL                     0
+         103         200 LOAD_CONST              11 (<code object build_backend, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 102>)
+                     202 MAKE_FUNCTION            0
          
-          64         106 STORE_NAME               9 (build_backend)
+         102         204 PRECALL                  0
+                     208 CALL                     0
          
-          84         108 LOAD_NAME                4 (property)
+         103         218 STORE_NAME              14 (build_backend)
          
-          85         110 LOAD_CONST               3 ('return')
-                     112 LOAD_NAME                5 (str)
-                     114 BUILD_TUPLE              2
-                     116 LOAD_CONST               8 (<code object index_url, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 84>)
-                     118 MAKE_FUNCTION            4 (annotations)
+         120         220 LOAD_NAME                4 (property)
          
-          84         120 PRECALL                  0
-                     124 CALL                     0
+         121         222 LOAD_CONST               3 ('return')
+                     224 LOAD_NAME                9 (str)
+                     226 BUILD_TUPLE              2
+                     228 LOAD_CONST              12 (<code object index_url, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 120>)
+                     230 MAKE_FUNCTION            4 (annotations)
          
-          85         134 STORE_NAME              10 (index_url)
+         120         232 PRECALL                  0
+                     236 CALL                     0
          
-          94         136 LOAD_NAME                4 (property)
+         121         246 STORE_NAME              15 (index_url)
          
-          95         138 LOAD_CONST               3 ('return')
-                     140 LOAD_NAME                5 (str)
-                     142 BUILD_TUPLE              2
-                     144 LOAD_CONST               9 (<code object distribution_name, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 94>)
-                     146 MAKE_FUNCTION            4 (annotations)
+         131         248 LOAD_NAME                4 (property)
          
-          94         148 PRECALL                  0
-                     152 CALL                     0
+         132         250 LOAD_CONST               3 ('return')
+                     252 LOAD_NAME                9 (str)
+                     254 BUILD_TUPLE              2
+                     256 LOAD_CONST              13 (<code object distribution_name, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 131>)
+                     258 MAKE_FUNCTION            4 (annotations)
          
-          95         162 STORE_NAME              11 (distribution_name)
+         131         260 PRECALL                  0
+                     264 CALL                     0
          
-         115         164 LOAD_NAME                4 (property)
+         132         274 STORE_NAME              16 (distribution_name)
          
-         116         166 LOAD_CONST               3 ('return')
-                     168 LOAD_NAME                5 (str)
-                     170 BUILD_TUPLE              2
-                     172 LOAD_CONST              10 (<code object version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 115>)
-                     174 MAKE_FUNCTION            4 (annotations)
+         135         276 LOAD_NAME                4 (property)
          
-         115         176 PRECALL                  0
-                     180 CALL                     0
+         136         278 LOAD_CONST               3 ('return')
+                     280 LOAD_NAME                9 (str)
+                     282 BUILD_TUPLE              2
+                     284 LOAD_CONST              14 (<code object version, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 135>)
+                     286 MAKE_FUNCTION            4 (annotations)
          
-         116         190 STORE_NAME              12 (version)
+         135         288 PRECALL                  0
+                     292 CALL                     0
          
-         123         192 LOAD_CONST               3 ('return')
-                     194 LOAD_NAME                5 (str)
-                     196 BUILD_TUPLE              2
-                     198 LOAD_CONST              11 (<code object _get_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 123>)
-                     200 MAKE_FUNCTION            4 (annotations)
-                     202 STORE_NAME              13 (_get_version)
+         136         302 STORE_NAME              17 (version)
          
-         144         204 LOAD_CONST              12 ('candidate_version')
-                     206 LOAD_NAME                5 (str)
-                     208 LOAD_CONST               3 ('return')
-                     210 LOAD_NAME               14 (bool)
-                     212 BUILD_TUPLE              4
-                     214 LOAD_CONST              13 (<code object version_in_repository, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 144>)
-                     216 MAKE_FUNCTION            4 (annotations)
-                     218 STORE_NAME              15 (version_in_repository)
+         143         304 LOAD_CONST               3 ('return')
+                     306 LOAD_NAME                9 (str)
+                     308 BUILD_TUPLE              2
+                     310 LOAD_CONST              15 (<code object _get_version, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 143>)
+                     312 MAKE_FUNCTION            4 (annotations)
+                     314 STORE_NAME              18 (_get_version)
          
-         169         220 LOAD_NAME               16 (contextmanager)
+         164         316 LOAD_CONST              16 ('candidate_version')
+                     318 LOAD_NAME                9 (str)
+                     320 LOAD_CONST               3 ('return')
+                     322 LOAD_NAME               19 (bool)
+                     324 BUILD_TUPLE              4
+                     326 LOAD_CONST              17 (<code object version_in_repository, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 164>)
+                     328 MAKE_FUNCTION            4 (annotations)
+                     330 STORE_NAME              20 (version_in_repository)
          
-         170         222 LOAD_CONST              14 (<code object patched_version, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 169>)
-                     224 MAKE_FUNCTION            0
+         189         332 LOAD_NAME               21 (contextmanager)
          
-         169         226 PRECALL                  0
-                     230 CALL                     0
+         190         334 LOAD_CONST              18 (<code object patched_version, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 189>)
+                     336 MAKE_FUNCTION            0
          
-         170         240 STORE_NAME              17 (patched_version)
+         189         338 PRECALL                  0
+                     342 CALL                     0
          
-         195         242 LOAD_CONST              15 (<code object delegate_build_wheel, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 195>)
-                     244 MAKE_FUNCTION            0
-                     246 STORE_NAME              18 (delegate_build_wheel)
+         190         352 STORE_NAME              22 (patched_version)
          
-         204         248 LOAD_CONST              16 (<code object delegate_build_sdist, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 204>)
-                     250 MAKE_FUNCTION            0
-                     252 STORE_NAME              19 (delegate_build_sdist)
+         215         354 LOAD_CONST              19 (<code object delegate_build_wheel, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 215>)
+                     356 MAKE_FUNCTION            0
+                     358 STORE_NAME              23 (delegate_build_wheel)
          
-         209         254 LOAD_CONST              17 (<code object delegate_build_editable, file "/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 209>)
-                     256 MAKE_FUNCTION            0
-                     258 STORE_NAME              20 (delegate_build_editable)
-                     260 LOAD_CONST               1 (None)
-                     262 RETURN_VALUE
+         224         360 LOAD_CONST              20 (<code object delegate_build_sdist, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 224>)
+                     362 MAKE_FUNCTION            0
+                     364 STORE_NAME              24 (delegate_build_sdist)
+         
+         229         366 LOAD_CONST              21 (<code object delegate_build_editable, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 229>)
+                     368 MAKE_FUNCTION            0
+                     370 STORE_NAME              25 (delegate_build_editable)
+         
+         238         372 LOAD_CONST              22 (<code object get_requires_for_build_editable, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 238>)
+                     374 MAKE_FUNCTION            0
+                     376 STORE_NAME              26 (get_requires_for_build_editable)
+         
+         241         378 LOAD_CONST              23 (<code object get_requires_for_build_sdist, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 241>)
+                     380 MAKE_FUNCTION            0
+                     382 STORE_NAME              27 (get_requires_for_build_sdist)
+         
+         268         384 LOAD_CONST              24 (<code object get_requires_for_build_wheel, file "/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py", line 268>)
+                     386 MAKE_FUNCTION            0
+                     388 STORE_NAME              28 (get_requires_for_build_wheel)
+                     390 LOAD_CONST               1 (None)
+                     392 RETURN_VALUE
          consts
             'DateVersion'
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c0170016900a00000000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c005f010000000000000000740500
                   0000000000000000006a030000000000000000a6000000ab000000000000
-                  0000007c005f020000000000000000740800000000000000000000a00500
-                  0000000000000000000000000000000000000064017c006a020000000000
-                  000000a6020000ab020000000000000000010064005300
-                28           0 RESUME                   0
+                  0000007c005f02000000000000000064007c005f04000000000000000064
+                  007c005f050000000000000000740c00000000000000000000a007000000
+                  000000000000000000000000000000000064017c006a0200000000000000
+                  00a6020000ab020000000000000000010064005300
+                29           0 RESUME                   0
                
-                29           2 LOAD_FAST                1 (config_settings)
+                30           2 LOAD_FAST                1 (config_settings)
                              4 JUMP_IF_TRUE_OR_POP      1 (to 8)
                              6 BUILD_MAP                0
                        >>    8 LOAD_METHOD              0 (copy)
                             30 PRECALL                  0
                             34 CALL                     0
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (config_settings)
                
-                30          56 LOAD_GLOBAL              5 (NULL + datetime)
+                31          56 LOAD_GLOBAL              5 (NULL + datetime)
                             68 LOAD_ATTR                3 (utcnow)
                             78 PRECALL                  0
                             82 CALL                     0
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               2 (datetime)
                
-                31         104 LOAD_GLOBAL              8 (LOG)
-                           116 LOAD_METHOD              5 (debug)
-                           138 LOAD_CONST               1 ('operating with datetime = %s')
-                           140 LOAD_FAST                0 (self)
-                           142 LOAD_ATTR                2 (datetime)
-                           152 PRECALL                  2
-                           156 CALL                     2
-                           166 POP_TOP
-                           168 LOAD_CONST               0 (None)
-                           170 RETURN_VALUE
+                32         104 LOAD_CONST               0 (None)
+                           106 LOAD_FAST                0 (self)
+                           108 STORE_ATTR               4 (_pyproject_toml)
+               
+                33         118 LOAD_CONST               0 (None)
+                           120 LOAD_FAST                0 (self)
+                           122 STORE_ATTR               5 (_tool_config)
+               
+                34         132 LOAD_GLOBAL             12 (LOG)
+                           144 LOAD_METHOD              7 (debug)
+                           166 LOAD_CONST               1 ('operating with datetime = %s')
+                           168 LOAD_FAST                0 (self)
+                           170 LOAD_ATTR                2 (datetime)
+                           180 PRECALL                  2
+                           184 CALL                     2
+                           194 POP_TOP
+                           196 LOAD_CONST               0 (None)
+                           198 RETURN_VALUE
                consts
                   None
                   'operating with datetime = %s'
-               names      ('copy', 'config_settings', 'datetime', 'utcnow', 'LOG', 'debug')
+               names      ('copy', 'config_settings', 'datetime', 'utcnow', '_pyproject_toml', '_tool_config', 'LOG', 'debug')
                varnames   ('self', 'config_settings')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '__init__'
-               firstlineno 28
-               lnotab 0x020136013001
+               firstlineno 29
+               lnotab 0x0201360130010e010e01
             'return'
             code
                argcount  : 1
+               nlocals   : 4
+               stacksize : 6
+               flags     : 3
+               code
+                  0x97007c006a00000000000000000080787402000000000000000000006a
+                  02000000000000000064016b05000000007205640264006c037d016e0464
+                  0264006c047d01740b0000000000000000000064036404a6020000ab0200
+                  0000000000000035007d027c01a006000000000000000000000000000000
+                  00000000007c02a6010000ab0100000000000000007d03640064006400a6
+                  020000ab02000000000000000001006e0b23003100730477027803590077
+                  010100590001000100740e00000000000000000000a00800000000000000
+                  0000000000000000000000000064057c03a6020000ab0200000000000000
+                  0001007c037c005f0000000000000000007c006a00000000000000000053
+                  00
+                36           0 RESUME                   0
+               
+                38           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_pyproject_toml)
+                            14 POP_JUMP_FORWARD_IF_NOT_NONE   120 (to 256)
+               
+                39          16 LOAD_GLOBAL              2 (sys)
+                            28 LOAD_ATTR                2 (version_info)
+                            38 LOAD_CONST               1 ((3, 11))
+                            40 COMPARE_OP               5 (>=)
+                            46 POP_JUMP_FORWARD_IF_FALSE     5 (to 58)
+               
+                40          48 LOAD_CONST               2 (0)
+                            50 LOAD_CONST               0 (None)
+                            52 IMPORT_NAME              3 (tomllib)
+                            54 STORE_FAST               1 (tomllib)
+                            56 JUMP_FORWARD             4 (to 66)
+               
+                42     >>   58 LOAD_CONST               2 (0)
+                            60 LOAD_CONST               0 (None)
+                            62 IMPORT_NAME              4 (tomli)
+                            64 STORE_FAST               1 (tomllib)
+               
+                44     >>   66 LOAD_GLOBAL             11 (NULL + open)
+                            78 LOAD_CONST               3 ('pyproject.toml')
+                            80 LOAD_CONST               4 ('rb')
+                            82 PRECALL                  2
+                            86 CALL                     2
+                            96 BEFORE_WITH
+                            98 STORE_FAST               2 (f)
+               
+                45         100 LOAD_FAST                1 (tomllib)
+                           102 LOAD_METHOD              6 (load)
+                           124 LOAD_FAST                2 (f)
+                           126 PRECALL                  1
+                           130 CALL                     1
+                           140 STORE_FAST               3 (data)
+               
+                44         142 LOAD_CONST               0 (None)
+                           144 LOAD_CONST               0 (None)
+                           146 LOAD_CONST               0 (None)
+                           148 PRECALL                  2
+                           152 CALL                     2
+                           162 POP_TOP
+                           164 JUMP_FORWARD            11 (to 188)
+                       >>  166 PUSH_EXC_INFO
+                           168 WITH_EXCEPT_START
+                           170 POP_JUMP_FORWARD_IF_TRUE     4 (to 180)
+                           172 RERAISE                  2
+                       >>  174 COPY                     3
+                           176 POP_EXCEPT
+                           178 RERAISE                  1
+                       >>  180 POP_TOP
+                           182 POP_EXCEPT
+                           184 POP_TOP
+                           186 POP_TOP
+               
+                47     >>  188 LOAD_GLOBAL             14 (LOG)
+                           200 LOAD_METHOD              8 (debug)
+                           222 LOAD_CONST               5 ('Loaded project metadata: %s')
+                           224 LOAD_FAST                3 (data)
+                           226 PRECALL                  2
+                           230 CALL                     2
+                           240 POP_TOP
+               
+                49         242 LOAD_FAST                3 (data)
+                           244 LOAD_FAST                0 (self)
+                           246 STORE_ATTR               0 (_pyproject_toml)
+               
+                51     >>  256 LOAD_FAST                0 (self)
+                           258 LOAD_ATTR                0 (_pyproject_toml)
+                           268 RETURN_VALUE
+               ExceptionTable:
+                 98 to 140 -> 166 [1] lasti
+                 166 to 172 -> 174 [3] lasti
+                 180 to 180 -> 174 [3] lasti
+               consts
+                  None
+                  (3, 11)
+                  0
+                  'pyproject.toml'
+                  'rb'
+                  'Loaded project metadata: %s'
+               names      ('_pyproject_toml', 'sys', 'version_info', 'tomllib', 'tomli', 'open', 'load', 'LOG', 'debug')
+               varnames   ('self', 'tomllib', 'f', 'data')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'pyproject_toml'
+               firstlineno 36
+               lnotab 0x02020e0120010a02080222012aff2e0336020e02
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code 0x97007c006a0000000000000000006401190000000000000000005300
+                53           0 RESUME                   0
+               
+                55           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (pyproject_toml)
+                            14 LOAD_CONST               1 ('project')
+                            16 BINARY_SUBSCR
+                            26 RETURN_VALUE
+               consts
+                  None
+                  'project'
+               names      ('pyproject_toml',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'project_config'
+               firstlineno 53
+               lnotab 0x0202
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a00000000000000000080547c006a010000000000000000a0
+                  0200000000000000000000000000000000000000006401a6010000ab0100
+                  0000000000000070016900a0020000000000000000000000000000000000
+                  0000006402a6010000ab010000000000000000700169007c005f00000000
+                  00000000007c006a000000000000000000a0030000000000000000000000
+                  000000000000000000a6000000ab0000000000000000007c005f00000000
+                  00000000007c006a0000000000000000005300
+                57           0 RESUME                   0
+               
+                59           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (_tool_config)
+                            14 POP_JUMP_FORWARD_IF_NOT_NONE    84 (to 184)
+               
+                60          16 LOAD_FAST                0 (self)
+                            18 LOAD_ATTR                1 (pyproject_toml)
+                            28 LOAD_METHOD              2 (get)
+                            50 LOAD_CONST               1 ('tool')
+                            52 PRECALL                  1
+                            56 CALL                     1
+                            66 JUMP_IF_TRUE_OR_POP      1 (to 70)
+                            68 BUILD_MAP                0
+                       >>   70 LOAD_METHOD              2 (get)
+               
+                61          92 LOAD_CONST               2 ('buildsys-dateversion')
+               
+                60          94 PRECALL                  1
+                            98 CALL                     1
+                           108 JUMP_IF_TRUE_OR_POP      1 (to 112)
+               
+                62         110 BUILD_MAP                0
+               
+                60     >>  112 LOAD_FAST                0 (self)
+                           114 STORE_ATTR               0 (_tool_config)
+               
+                63         124 LOAD_FAST                0 (self)
+                           126 LOAD_ATTR                0 (_tool_config)
+                           136 LOAD_METHOD              3 (copy)
+                           158 PRECALL                  0
+                           162 CALL                     0
+                           172 LOAD_FAST                0 (self)
+                           174 STORE_ATTR               0 (_tool_config)
+               
+                64     >>  184 LOAD_FAST                0 (self)
+                           186 LOAD_ATTR                0 (_tool_config)
+                           196 RETURN_VALUE
+               consts
+                  None
+                  'tool'
+                  'buildsys-dateversion'
+               names      ('_tool_config', 'pyproject_toml', 'get', 'copy')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'tool_config'
+               firstlineno 57
+               lnotab 0x02020e014c0102ff100202fe0c033c01
+            code
+               argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000700164025300
-                33           0 RESUME                   0
+                66           0 RESUME                   0
                
-                36           2 LOAD_FAST                0 (self)
-                             4 LOAD_ATTR                0 (config_settings)
+                69           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (tool_config)
                             14 LOAD_METHOD              1 (get)
-                            36 LOAD_CONST               1 ('dateversion-version-marker')
+                            36 LOAD_CONST               1 ('version-marker')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 JUMP_IF_TRUE_OR_POP      1 (to 56)
                
-                37          54 LOAD_CONST               2 ('generated by buildsys-dateversion')
+                70          54 LOAD_CONST               2 ('generated by buildsys-dateversion')
                
-                35     >>   56 RETURN_VALUE
+                68     >>   56 RETURN_VALUE
                consts
                   None
-                  'dateversion-version-marker'
+                  'version-marker'
                   'generated by buildsys-dateversion'
-               names      ('config_settings', 'get')
+               names      ('tool_config', 'get')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'marker'
-               firstlineno 33
+               firstlineno 66
                lnotab 0x0203340102fe
             code
                argcount  : 1
                nlocals   : 6
                stacksize : 7
                flags     : 3
                code
@@ -484,504 +777,421 @@
                   000000000000000000000000000000000000007413000000000000000000
                   007c05a6010000ab010000000000000000a00a0000000000000000000000
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   000000000000007221740a00000000000000000000a00b00000000000000
                   0000000000000000000000000064047c05a6020000ab0200000000000000
                   0001007c05630201006302010053008cae8cb77419000000000000000000
                   006405a6010000ab0100000000000000008201
-                40           0 RESUME                   0
+                73           0 RESUME                   0
                
-                41           2 LOAD_GLOBAL              1 (NULL + os)
+                74           2 LOAD_GLOBAL              1 (NULL + os)
                             14 LOAD_ATTR                1 (walk)
                             24 LOAD_CONST               1 ('.')
                             26 PRECALL                  1
                             30 CALL                     1
                             40 GET_ITER
                        >>   42 FOR_ITER               182 (to 408)
                             44 UNPACK_SEQUENCE          3
                             48 STORE_FAST               1 (dirpath)
                             50 STORE_FAST               2 (_)
                             52 STORE_FAST               3 (files)
                
-                42          54 LOAD_FAST                3 (files)
+                75          54 LOAD_FAST                3 (files)
                             56 GET_ITER
                        >>   58 FOR_ITER               173 (to 406)
                             60 STORE_FAST               4 (file)
                
-                43          62 LOAD_FAST                4 (file)
+                76          62 LOAD_FAST                4 (file)
                             64 LOAD_METHOD              2 (endswith)
                             86 LOAD_CONST               2 ('.py')
                             88 PRECALL                  1
                             92 CALL                     1
                            102 POP_JUMP_FORWARD_IF_TRUE     1 (to 106)
                
-                44         104 JUMP_BACKWARD           24 (to 58)
+                77         104 JUMP_BACKWARD           24 (to 58)
                
-                46     >>  106 LOAD_GLOBAL              0 (os)
+                79     >>  106 LOAD_GLOBAL              0 (os)
                            118 LOAD_ATTR                3 (path)
                            128 LOAD_METHOD              4 (join)
                            150 LOAD_FAST                1 (dirpath)
                            152 LOAD_FAST                4 (file)
                            154 PRECALL                  2
                            158 CALL                     2
                            168 STORE_FAST               5 (path)
                
-                47         170 LOAD_GLOBAL             10 (LOG)
+                80         170 LOAD_GLOBAL             10 (LOG)
                            182 LOAD_METHOD              6 (debug)
                            204 LOAD_CONST               3 ('Checking file %s')
                            206 LOAD_FAST                5 (path)
                            208 PRECALL                  2
                            212 CALL                     2
                            222 POP_TOP
                
-                48         224 LOAD_GLOBAL             14 (VERSION_PATTERN)
+                81         224 LOAD_GLOBAL             14 (VERSION_PATTERN)
                            236 LOAD_METHOD              8 (search)
                            258 LOAD_GLOBAL             19 (NULL + open)
                            270 LOAD_FAST                5 (path)
                            272 PRECALL                  1
                            276 CALL                     1
                            286 LOAD_METHOD             10 (read)
                            308 PRECALL                  0
                            312 CALL                     0
                            322 PRECALL                  1
                            326 CALL                     1
                            336 POP_JUMP_FORWARD_IF_FALSE    33 (to 404)
                
-                49         338 LOAD_GLOBAL             10 (LOG)
+                82         338 LOAD_GLOBAL             10 (LOG)
                            350 LOAD_METHOD             11 (info)
                            372 LOAD_CONST               4 ('detected __version__ in %s')
                            374 LOAD_FAST                5 (path)
                            376 PRECALL                  2
                            380 CALL                     2
                            390 POP_TOP
                
-                50         392 LOAD_FAST                5 (path)
+                83         392 LOAD_FAST                5 (path)
                            394 SWAP                     2
                            396 POP_TOP
                            398 SWAP                     2
                            400 POP_TOP
                            402 RETURN_VALUE
                
-                48     >>  404 JUMP_BACKWARD          174 (to 58)
+                81     >>  404 JUMP_BACKWARD          174 (to 58)
                
-                42     >>  406 JUMP_BACKWARD          183 (to 42)
+                75     >>  406 JUMP_BACKWARD          183 (to 42)
                
-                53     >>  408 LOAD_GLOBAL             25 (NULL + RuntimeError)
+                86     >>  408 LOAD_GLOBAL             25 (NULL + RuntimeError)
                
-                54         420 LOAD_CONST               5 ('Could not locate a file in the source tree defining `__version__`')
+                87         420 LOAD_CONST               5 ('Could not locate a file in the source tree defining `__version__`')
                
-                53         422 PRECALL                  1
+                86         422 PRECALL                  1
                            426 CALL                     1
                            436 RAISE_VARARGS            1
                consts
                   None
                   '.'
                   '.py'
                   'Checking file %s'
                   'detected __version__ in %s'
                   'Could not locate a file in the source tree defining `__version__`'
                names      ('os', 'walk', 'endswith', 'path', 'join', 'LOG', 'debug', 'VERSION_PATTERN', 'search', 'open', 'read', 'info', 'RuntimeError')
                varnames   ('self', 'dirpath', '_', 'files', 'file', 'path')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '_find_version_path'
-               firstlineno 40
+               firstlineno 73
                lnotab 0x0201340108012a01020240013601720136010cfe02fa020b0c0102ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x970064017c006a0000000000000000007601721c7c00a0010000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   006a00000000000000000064013c0000007c006a00000000000000000064
                   01190000000000000000005300
-                57           0 RESUME                   0
+                90           0 RESUME                   0
                
-                59           2 LOAD_CONST               1 ('dateversion-version-path')
+                92           2 LOAD_CONST               1 ('version-path')
                              4 LOAD_FAST                0 (self)
-                             6 LOAD_ATTR                0 (config_settings)
+                             6 LOAD_ATTR                0 (tool_config)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE    28 (to 76)
                
-                60          20 LOAD_FAST                0 (self)
+                93          20 LOAD_FAST                0 (self)
                             22 LOAD_METHOD              1 (_find_version_path)
                             44 PRECALL                  0
                             48 CALL                     0
                             58 LOAD_FAST                0 (self)
-                            60 LOAD_ATTR                0 (config_settings)
-                            70 LOAD_CONST               1 ('dateversion-version-path')
+                            60 LOAD_ATTR                0 (tool_config)
+                            70 LOAD_CONST               1 ('version-path')
                             72 STORE_SUBSCR
                
-                61     >>   76 LOAD_FAST                0 (self)
-                            78 LOAD_ATTR                0 (config_settings)
-                            88 LOAD_CONST               1 ('dateversion-version-path')
+                94     >>   76 LOAD_FAST                0 (self)
+                            78 LOAD_ATTR                0 (tool_config)
+                            88 LOAD_CONST               1 ('version-path')
                             90 BINARY_SUBSCR
                            100 RETURN_VALUE
                consts
                   None
-                  'dateversion-version-path'
-               names      ('config_settings', '_find_version_path')
+                  'version-path'
+               names      ('tool_config', '_find_version_path')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version_path'
-               firstlineno 57
+               firstlineno 90
                lnotab 0x020212013801
             code
                argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c006a000000000000000000a00100000000000000000000000000
+                  000000000000006401a6010000ab010000000000000000700164025300
+                96           0 RESUME                   0
+               
+                99           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (tool_config)
+                            14 LOAD_METHOD              1 (get)
+                            36 LOAD_CONST               1 ('build-backend')
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 JUMP_IF_TRUE_OR_POP      1 (to 56)
+                            54 LOAD_CONST               2 ('setuptools.build_meta:__legacy__')
+               
+                98     >>   56 RETURN_VALUE
+               consts
+                  None
+                  'build-backend'
+                  'setuptools.build_meta:__legacy__'
+               names      ('tool_config', 'get')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'build_backend_name'
+               firstlineno 96
+               lnotab 0x020336ff
+            code
+               argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
-                  0x970064017c006a0000000000000000007601729c7c006a000000000000
-                  000000a00100000000000000000000000000000000000000006402a60100
-                  00ab010000000000000000700164037d017c01a002000000000000000000
-                  00000000000000000000006404a6010000ab0100000000000000007d0274
-                  07000000000000000000006a0400000000000000007c0264051900000000
-                  0000000000a6010000ab0100000000000000007d037c037d04740b000000
-                  000000000000007c02a6010000ab01000000000000000064066b02000000
-                  007216740d000000000000000000007c037c026407190000000000000000
-                  00a6020000ab0200000000000000007d04740e00000000000000000000a0
-                  08000000000000000000000000000000000000000064087c017c04a60300
-                  00ab03000000000000000001007c047c006a00000000000000000064013c
-                  0000007c006a0000000000000000006401190000000000000000005300
-                63           0 RESUME                   0
+                  0x970064017c006a000000000000000000760172877c006a010000000000
+                  0000007d017c01a002000000000000000000000000000000000000000064
+                  02a6010000ab0100000000000000007d027407000000000000000000006a
+                  0400000000000000007c02640319000000000000000000a6010000ab0100
+                  000000000000007d037c037d04740b000000000000000000007c02a60100
+                  00ab01000000000000000064046b02000000007216740d00000000000000
+                  0000007c037c02640519000000000000000000a6020000ab020000000000
+                  0000007d04740e00000000000000000000a0080000000000000000000000
+                  00000000000000000064067c017c04a6030000ab03000000000000000001
+                  007c047c006a00000000000000000064013c0000007c006a000000000000
+                  0000006401190000000000000000005300
+               102           0 RESUME                   0
                
-                65           2 LOAD_CONST               1 ('dateversion-build-backend-object')
+               104           2 LOAD_CONST               1 ('dateversion-build-backend-object')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
-                            18 POP_JUMP_FORWARD_IF_FALSE   156 (to 332)
+                            18 POP_JUMP_FORWARD_IF_FALSE   135 (to 290)
                
-                67          20 LOAD_FAST                0 (self)
-                            22 LOAD_ATTR                0 (config_settings)
-                            32 LOAD_METHOD              1 (get)
-                            54 LOAD_CONST               2 ('dateversion-build-backend')
-                            56 PRECALL                  1
-                            60 CALL                     1
-                            70 JUMP_IF_TRUE_OR_POP      1 (to 74)
-               
-                68          72 LOAD_CONST               3 ('setuptools.build_meta:__legacy__')
-               
-                66     >>   74 STORE_FAST               1 (backend_name)
-               
-                71          76 LOAD_FAST                1 (backend_name)
-                            78 LOAD_METHOD              2 (split)
-                           100 LOAD_CONST               4 (':')
-                           102 PRECALL                  1
-                           106 CALL                     1
-                           116 STORE_FAST               2 (components)
-               
-                72         118 LOAD_GLOBAL              7 (NULL + importlib)
-                           130 LOAD_ATTR                4 (import_module)
-                           140 LOAD_FAST                2 (components)
-                           142 LOAD_CONST               5 (0)
-                           144 BINARY_SUBSCR
-                           154 PRECALL                  1
-                           158 CALL                     1
-                           168 STORE_FAST               3 (module)
-               
-                73         170 LOAD_FAST                3 (module)
-                           172 STORE_FAST               4 (backend)
-               
-                75         174 LOAD_GLOBAL             11 (NULL + len)
-                           186 LOAD_FAST                2 (components)
-                           188 PRECALL                  1
-                           192 CALL                     1
-                           202 LOAD_CONST               6 (2)
-                           204 COMPARE_OP               2 (==)
-                           210 POP_JUMP_FORWARD_IF_FALSE    22 (to 256)
-               
-                76         212 LOAD_GLOBAL             13 (NULL + getattr)
-                           224 LOAD_FAST                3 (module)
-                           226 LOAD_FAST                2 (components)
-                           228 LOAD_CONST               7 (1)
-                           230 BINARY_SUBSCR
-                           240 PRECALL                  2
-                           244 CALL                     2
-                           254 STORE_FAST               4 (backend)
-               
-                78     >>  256 LOAD_GLOBAL             14 (LOG)
-                           268 LOAD_METHOD              8 (debug)
-                           290 LOAD_CONST               8 ('using build backend %s (%s)')
-                           292 LOAD_FAST                1 (backend_name)
-                           294 LOAD_FAST                4 (backend)
-                           296 PRECALL                  3
-                           300 CALL                     3
-                           310 POP_TOP
-               
-                80         312 LOAD_FAST                4 (backend)
-                           314 LOAD_FAST                0 (self)
-                           316 LOAD_ATTR                0 (config_settings)
-                           326 LOAD_CONST               1 ('dateversion-build-backend-object')
-                           328 STORE_SUBSCR
-               
-                82     >>  332 LOAD_FAST                0 (self)
-                           334 LOAD_ATTR                0 (config_settings)
-                           344 LOAD_CONST               1 ('dateversion-build-backend-object')
-                           346 BINARY_SUBSCR
-                           356 RETURN_VALUE
+               105          20 LOAD_FAST                0 (self)
+                            22 LOAD_ATTR                1 (build_backend_name)
+                            32 STORE_FAST               1 (backend_name)
+               
+               107          34 LOAD_FAST                1 (backend_name)
+                            36 LOAD_METHOD              2 (split)
+                            58 LOAD_CONST               2 (':')
+                            60 PRECALL                  1
+                            64 CALL                     1
+                            74 STORE_FAST               2 (components)
+               
+               108          76 LOAD_GLOBAL              7 (NULL + importlib)
+                            88 LOAD_ATTR                4 (import_module)
+                            98 LOAD_FAST                2 (components)
+                           100 LOAD_CONST               3 (0)
+                           102 BINARY_SUBSCR
+                           112 PRECALL                  1
+                           116 CALL                     1
+                           126 STORE_FAST               3 (module)
+               
+               109         128 LOAD_FAST                3 (module)
+                           130 STORE_FAST               4 (backend)
+               
+               111         132 LOAD_GLOBAL             11 (NULL + len)
+                           144 LOAD_FAST                2 (components)
+                           146 PRECALL                  1
+                           150 CALL                     1
+                           160 LOAD_CONST               4 (2)
+                           162 COMPARE_OP               2 (==)
+                           168 POP_JUMP_FORWARD_IF_FALSE    22 (to 214)
+               
+               112         170 LOAD_GLOBAL             13 (NULL + getattr)
+                           182 LOAD_FAST                3 (module)
+                           184 LOAD_FAST                2 (components)
+                           186 LOAD_CONST               5 (1)
+                           188 BINARY_SUBSCR
+                           198 PRECALL                  2
+                           202 CALL                     2
+                           212 STORE_FAST               4 (backend)
+               
+               114     >>  214 LOAD_GLOBAL             14 (LOG)
+                           226 LOAD_METHOD              8 (debug)
+                           248 LOAD_CONST               6 ('using build backend %s (%s)')
+                           250 LOAD_FAST                1 (backend_name)
+                           252 LOAD_FAST                4 (backend)
+                           254 PRECALL                  3
+                           258 CALL                     3
+                           268 POP_TOP
+               
+               116         270 LOAD_FAST                4 (backend)
+                           272 LOAD_FAST                0 (self)
+                           274 LOAD_ATTR                0 (config_settings)
+                           284 LOAD_CONST               1 ('dateversion-build-backend-object')
+                           286 STORE_SUBSCR
+               
+               118     >>  290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                0 (config_settings)
+                           302 LOAD_CONST               1 ('dateversion-build-backend-object')
+                           304 BINARY_SUBSCR
+                           314 RETURN_VALUE
                consts
                   None
                   'dateversion-build-backend-object'
-                  'dateversion-build-backend'
-                  'setuptools.build_meta:__legacy__'
                   ':'
                   0
                   2
                   1
                   'using build backend %s (%s)'
-               names      ('config_settings', 'get', 'split', 'importlib', 'import_module', 'len', 'getattr', 'LOG', 'debug')
+               names      ('config_settings', 'build_backend_name', 'split', 'importlib', 'import_module', 'len', 'getattr', 'LOG', 'debug')
                varnames   ('self', 'backend_name', 'components', 'module', 'backend')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'build_backend'
-               firstlineno 63
-               lnotab 0x02021202340102fe02052a013401040226012c0238021402
+               firstlineno 102
+               lnotab 0x020212010e022a013401040226012c0238021402
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000700164027d017c
                   01a00200000000000000000000000000000000000000006403a6010000ab
                   010000000000000000721f7c01640064048502190000000000000000007d
                   017c01a00200000000000000000000000000000000000000006403a60100
                   00ab010000000000000000b01f7c015300
-                84           0 RESUME                   0
+               120           0 RESUME                   0
                
-                87           2 LOAD_FAST                0 (self)
+               124           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (config_settings)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_CONST               1 ('dateversion-index-url')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 JUMP_IF_TRUE_OR_POP      1 (to 56)
                
-                88          54 LOAD_CONST               2 ('https://pypi.org/simple')
+               125          54 LOAD_CONST               2 ('https://pypi.org/simple')
                
-                86     >>   56 STORE_FAST               1 (out)
+               122     >>   56 STORE_FAST               1 (out)
                
-                90          58 LOAD_FAST                1 (out)
+               127          58 LOAD_FAST                1 (out)
                             60 LOAD_METHOD              2 (endswith)
                             82 LOAD_CONST               3 ('/')
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_JUMP_FORWARD_IF_FALSE    31 (to 162)
                
-                91     >>  100 LOAD_FAST                1 (out)
+               128     >>  100 LOAD_FAST                1 (out)
                            102 LOAD_CONST               0 (None)
                            104 LOAD_CONST               4 (-1)
                            106 BUILD_SLICE              2
                            108 BINARY_SUBSCR
                            118 STORE_FAST               1 (out)
                
-                90         120 LOAD_FAST                1 (out)
+               127         120 LOAD_FAST                1 (out)
                            122 LOAD_METHOD              2 (endswith)
                            144 LOAD_CONST               3 ('/')
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_JUMP_BACKWARD_IF_TRUE    31 (to 100)
                
-                92     >>  162 LOAD_FAST                1 (out)
+               129     >>  162 LOAD_FAST                1 (out)
                            164 RETURN_VALUE
                consts
                   None
                   'dateversion-index-url'
                   'https://pypi.org/simple'
                   '/'
                   -1
                names      ('config_settings', 'get', 'endswith')
                varnames   ('self', 'out')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'index_url'
-               firstlineno 84
-               lnotab 0x0203340102fe02042a0114ff2a02
+               firstlineno 120
+               lnotab 0x0204340102fd02052a0114ff2a02
             code
                argcount  : 1
-               nlocals   : 4
-               stacksize : 6
+               nlocals   : 1
+               stacksize : 2
                flags     : 3
-               code
-                  0x970064017c006a0000000000000000007601727f0900640264006c017d
-                  016e0b23000100640264006c027d0159006e037803590077017407000000
-                  0000000000000064036404a6020000ab02000000000000000035007d027c
-                  01a00400000000000000000000000000000000000000007c02a6010000ab
-                  0100000000000000007d03640064006400a6020000ab0200000000000000
-                  0001006e0b23003100730477027803590077010100590001000100740a00
-                  000000000000000000a00600000000000000000000000000000000000000
-                  0064057c03a6020000ab02000000000000000001007c0364061900000000
-                  00000000006407190000000000000000007c006a00000000000000000064
-                  013c0000007c006a00000000000000000064011900000000000000000053
-                  00
-                94           0 RESUME                   0
-               
-                96           2 LOAD_CONST               1 ('dateversion-distribution-name')
-                             4 LOAD_FAST                0 (self)
-                             6 LOAD_ATTR                0 (config_settings)
-                            16 CONTAINS_OP              1
-                            18 POP_JUMP_FORWARD_IF_FALSE   127 (to 274)
+               code 0x97007c006a0000000000000000006401190000000000000000005300
+               131           0 RESUME                   0
                
-                97          20 NOP
-               
-                98          22 LOAD_CONST               2 (0)
-                            24 LOAD_CONST               0 (None)
-                            26 IMPORT_NAME              1 (tomllib)
-                            28 STORE_FAST               1 (tomllib)
-                            30 JUMP_FORWARD            11 (to 54)
-                       >>   32 PUSH_EXC_INFO
-               
-                99          34 POP_TOP
-               
-               101          36 LOAD_CONST               2 (0)
-                            38 LOAD_CONST               0 (None)
-                            40 IMPORT_NAME              2 (tomli)
-                            42 STORE_FAST               1 (tomllib)
-                            44 POP_EXCEPT
-                            46 JUMP_FORWARD             3 (to 54)
-                       >>   48 COPY                     3
-                            50 POP_EXCEPT
-                            52 RERAISE                  1
-               
-               103     >>   54 LOAD_GLOBAL              7 (NULL + open)
-                            66 LOAD_CONST               3 ('pyproject.toml')
-                            68 LOAD_CONST               4 ('rb')
-                            70 PRECALL                  2
-                            74 CALL                     2
-                            84 BEFORE_WITH
-                            86 STORE_FAST               2 (f)
-               
-               104          88 LOAD_FAST                1 (tomllib)
-                            90 LOAD_METHOD              4 (load)
-                           112 LOAD_FAST                2 (f)
-                           114 PRECALL                  1
-                           118 CALL                     1
-                           128 STORE_FAST               3 (data)
-               
-               103         130 LOAD_CONST               0 (None)
-                           132 LOAD_CONST               0 (None)
-                           134 LOAD_CONST               0 (None)
-                           136 PRECALL                  2
-                           140 CALL                     2
-                           150 POP_TOP
-                           152 JUMP_FORWARD            11 (to 176)
-                       >>  154 PUSH_EXC_INFO
-                           156 WITH_EXCEPT_START
-                           158 POP_JUMP_FORWARD_IF_TRUE     4 (to 168)
-                           160 RERAISE                  2
-                       >>  162 COPY                     3
-                           164 POP_EXCEPT
-                           166 RERAISE                  1
-                       >>  168 POP_TOP
-                           170 POP_EXCEPT
-                           172 POP_TOP
-                           174 POP_TOP
-               
-               106     >>  176 LOAD_GLOBAL             10 (LOG)
-                           188 LOAD_METHOD              6 (info)
-                           210 LOAD_CONST               5 ('Loaded project metadata: %s')
-                           212 LOAD_FAST                3 (data)
-                           214 PRECALL                  2
-                           218 CALL                     2
-                           228 POP_TOP
-               
-               109         230 LOAD_FAST                3 (data)
-                           232 LOAD_CONST               6 ('project')
-                           234 BINARY_SUBSCR
-               
-               110         244 LOAD_CONST               7 ('name')
-               
-               109         246 BINARY_SUBSCR
-                           256 LOAD_FAST                0 (self)
-                           258 LOAD_ATTR                0 (config_settings)
-                           268 LOAD_CONST               1 ('dateversion-distribution-name')
-                           270 STORE_SUBSCR
-               
-               113     >>  274 LOAD_FAST                0 (self)
-                           276 LOAD_ATTR                0 (config_settings)
-                           286 LOAD_CONST               1 ('dateversion-distribution-name')
-                           288 BINARY_SUBSCR
-                           298 RETURN_VALUE
-               ExceptionTable:
-                 22 to 28 -> 32 [0]
-                 32 to 42 -> 48 [1] lasti
-                 86 to 128 -> 154 [1] lasti
-                 154 to 160 -> 162 [3] lasti
-                 168 to 168 -> 162 [3] lasti
+               133           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (project_config)
+                            14 LOAD_CONST               1 ('name')
+                            16 BINARY_SUBSCR
+                            26 RETURN_VALUE
                consts
                   None
-                  'dateversion-distribution-name'
-                  0
-                  'pyproject.toml'
-                  'rb'
-                  'Loaded project metadata: %s'
-                  'project'
                   'name'
-               names      ('config_settings', 'tomllib', 'tomli', 'open', 'load', 'LOG', 'info')
-               varnames   ('self', 'tomllib', 'f', 'data')
+               names      ('project_config',)
+               varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'distribution_name'
-               firstlineno 94
-               lnotab 0x0202120102010c010202120222012aff2e0336030e0102ff1c04
+               firstlineno 131
+               lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x970064017c006a0000000000000000007601721c7c00a0010000000000
                   000000000000000000000000000000a6000000ab0000000000000000007c
                   006a00000000000000000064013c0000007c006a00000000000000000064
                   01190000000000000000005300
-               115           0 RESUME                   0
+               135           0 RESUME                   0
                
-               117           2 LOAD_CONST               1 ('dateversion-distribution-version')
+               137           2 LOAD_CONST               1 ('dateversion-distribution-version')
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (config_settings)
                             16 CONTAINS_OP              1
                             18 POP_JUMP_FORWARD_IF_FALSE    28 (to 76)
                
-               120          20 LOAD_FAST                0 (self)
+               140          20 LOAD_FAST                0 (self)
                             22 LOAD_METHOD              1 (_get_version)
                             44 PRECALL                  0
                             48 CALL                     0
                
-               118          58 LOAD_FAST                0 (self)
+               138          58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                0 (config_settings)
                
-               119          70 LOAD_CONST               1 ('dateversion-distribution-version')
+               139          70 LOAD_CONST               1 ('dateversion-distribution-version')
                
-               118          72 STORE_SUBSCR
+               138          72 STORE_SUBSCR
                
-               121     >>   76 LOAD_FAST                0 (self)
+               141     >>   76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                0 (config_settings)
                             88 LOAD_CONST               1 ('dateversion-distribution-version')
                             90 BINARY_SUBSCR
                            100 RETURN_VALUE
                consts
                   None
                   'dateversion-distribution-version'
                names      ('config_settings', '_get_version')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version'
-               firstlineno 115
+               firstlineno 135
                lnotab 0x0202120326fe0c0102ff0403
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
@@ -991,65 +1201,65 @@
                   00000000007d037c00a00300000000000000000000000000000000000000
                   007c03a6010000ab01000000000000000073047c03630201005300740800
                   000000000000000000a00500000000000000000000000000000000000000
                   0064027c006a0600000000000000007c03a6030000ab0300000000000000
                   0001008c647401000000000000000000007403000000000000000000006a
                   0200000000000000006403a6010000ab010000000000000000a6010000ab
                   0100000000000000005300
-               123           0 RESUME                   0
+               143           0 RESUME                   0
                
-               124           2 BUILD_LIST               0
+               144           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (('%Y.%m', '%Y.%m.%d', '%Y.%m.%d.%H', '%Y.%m.%d.%H.%M'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               1 (formats)
                
-               131          10 LOAD_FAST                1 (formats)
+               151          10 LOAD_FAST                1 (formats)
                             12 GET_ITER
                        >>   14 FOR_ITER                99 (to 214)
                             16 STORE_FAST               2 (format)
                
-               132          18 LOAD_GLOBAL              1 (NULL + normalized)
+               152          18 LOAD_GLOBAL              1 (NULL + normalized)
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                1 (datetime)
                             42 LOAD_METHOD              2 (strftime)
                             64 LOAD_FAST                2 (format)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 PRECALL                  1
                             84 CALL                     1
                             94 STORE_FAST               3 (candidate)
                
-               133          96 LOAD_FAST                0 (self)
+               153          96 LOAD_FAST                0 (self)
                             98 LOAD_METHOD              3 (version_in_repository)
                            120 LOAD_FAST                3 (candidate)
                            122 PRECALL                  1
                            126 CALL                     1
                            136 POP_JUMP_FORWARD_IF_TRUE     4 (to 146)
                
-               134         138 LOAD_FAST                3 (candidate)
+               154         138 LOAD_FAST                3 (candidate)
                            140 SWAP                     2
                            142 POP_TOP
                            144 RETURN_VALUE
                
-               135     >>  146 LOAD_GLOBAL              8 (LOG)
+               155     >>  146 LOAD_GLOBAL              8 (LOG)
                            158 LOAD_METHOD              5 (info)
                
-               136         180 LOAD_CONST               2 ('%s-%s is already released, trying next...')
+               156         180 LOAD_CONST               2 ('%s-%s is already released, trying next...')
                
-               137         182 LOAD_FAST                0 (self)
+               157         182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                6 (distribution_name)
                
-               138         194 LOAD_FAST                3 (candidate)
+               158         194 LOAD_FAST                3 (candidate)
                
-               135         196 PRECALL                  3
+               155         196 PRECALL                  3
                            200 CALL                     3
                            210 POP_TOP
                            212 JUMP_BACKWARD          100 (to 14)
                
-               142     >>  214 LOAD_GLOBAL              1 (NULL + normalized)
+               162     >>  214 LOAD_GLOBAL              1 (NULL + normalized)
                            226 LOAD_GLOBAL              3 (NULL + datetime)
                            238 LOAD_ATTR                2 (strftime)
                            248 LOAD_CONST               3 ('%Y.%m.%d.%H.%M.%S')
                            250 PRECALL                  1
                            254 CALL                     1
                            264 PRECALL                  1
                            268 CALL                     1
@@ -1059,17 +1269,17 @@
                   ('%Y.%m', '%Y.%m.%d', '%Y.%m.%d.%H', '%Y.%m.%d.%H.%M')
                   '%s-%s is already released, trying next...'
                   '%Y.%m.%d.%H.%M.%S'
                names      ('normalized', 'datetime', 'strftime', 'version_in_repository', 'LOG', 'info', 'distribution_name')
                varnames   ('self', 'formats', 'format', 'candidate')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       '_get_version'
-               firstlineno 123
+               firstlineno 143
                lnotab 0x0201080708014e012a010801220102010c0102fd1207
             'candidate_version'
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 6
                flags     : 3
@@ -1091,84 +1301,84 @@
                   00000000007c0476006302640064006400a6020000ab0200000000000000
                   000100530023003100730477027803590077010100590001000100640053
                   002300740e000000000000000000006a0e00000000000000006a0f000000
                   0000000000240072257d057c05a010000000000000000000000000000000
                   0000000000a6000000ab00000000000000000064056b0200000000720659
                   0064007d057e05640653007c05820164007d057e05770177007803590077
                   01
-               144           0 RESUME                   0
+               164           0 RESUME                   0
                
-               145           2 LOAD_GLOBAL              0 (os)
+               165           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (join)
                             46 LOAD_FAST                0 (self)
                             48 LOAD_ATTR                3 (index_url)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                4 (distribution_name)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 STORE_FAST               2 (repo_url)
                
-               147          86 LOAD_GLOBAL             10 (LOG)
+               167          86 LOAD_GLOBAL             10 (LOG)
                             98 LOAD_METHOD              6 (info)
                            120 LOAD_CONST               1 ('looking for %s in %s ...')
                            122 LOAD_FAST                1 (candidate_version)
                            124 LOAD_FAST                2 (repo_url)
                            126 PRECALL                  3
                            130 CALL                     3
                            140 POP_TOP
                
-               150         142 NOP
+               170         142 NOP
                
-               151         144 LOAD_GLOBAL             14 (urllib)
+               171         144 LOAD_GLOBAL             14 (urllib)
                            156 LOAD_ATTR                8 (request)
                            166 LOAD_METHOD              9 (urlopen)
                            188 LOAD_FAST                2 (repo_url)
                            190 PRECALL                  1
                            194 CALL                     1
                            204 BEFORE_WITH
                            206 STORE_FAST               3 (response)
                
-               152         208 LOAD_GLOBAL             10 (LOG)
+               172         208 LOAD_GLOBAL             10 (LOG)
                            220 LOAD_METHOD             10 (debug)
                            242 LOAD_CONST               2 ('Response status: %s')
                            244 LOAD_FAST                3 (response)
                            246 LOAD_ATTR               11 (status)
                            256 PRECALL                  2
                            260 CALL                     2
                            270 POP_TOP
                
-               154         272 LOAD_FAST                3 (response)
+               174         272 LOAD_FAST                3 (response)
                            274 LOAD_METHOD             12 (read)
                            296 PRECALL                  0
                            300 CALL                     0
                            310 STORE_FAST               4 (body)
                
-               155         312 LOAD_GLOBAL             10 (LOG)
+               175         312 LOAD_GLOBAL             10 (LOG)
                            324 LOAD_METHOD             10 (debug)
                            346 LOAD_CONST               3 ('Response body: %s')
                            348 LOAD_FAST                4 (body)
                            350 PRECALL                  2
                            354 CALL                     2
                            364 POP_TOP
                
-               159         366 LOAD_FAST                0 (self)
+               179         366 LOAD_FAST                0 (self)
                            368 LOAD_ATTR                4 (distribution_name)
                            378 FORMAT_VALUE             0
                            380 LOAD_CONST               4 ('-')
                            382 LOAD_FAST                1 (candidate_version)
                            384 FORMAT_VALUE             0
                            386 BUILD_STRING             3
                            388 LOAD_METHOD             13 (encode)
                            410 PRECALL                  0
                            414 CALL                     0
                            424 LOAD_FAST                4 (body)
                            426 CONTAINS_OP              0
                
-               151         428 SWAP                     2
+               171         428 SWAP                     2
                            430 LOAD_CONST               0 (None)
                            432 LOAD_CONST               0 (None)
                            434 LOAD_CONST               0 (None)
                            436 PRECALL                  2
                            440 CALL                     2
                            450 POP_TOP
                            452 RETURN_VALUE
@@ -1183,44 +1393,44 @@
                            470 POP_EXCEPT
                            472 POP_TOP
                            474 POP_TOP
                            476 LOAD_CONST               0 (None)
                            478 RETURN_VALUE
                        >>  480 PUSH_EXC_INFO
                
-               161         482 LOAD_GLOBAL             14 (urllib)
+               181         482 LOAD_GLOBAL             14 (urllib)
                            494 LOAD_ATTR               14 (error)
                            504 LOAD_ATTR               15 (HTTPError)
                            514 CHECK_EXC_MATCH
                            516 POP_JUMP_FORWARD_IF_FALSE    37 (to 592)
                            518 STORE_FAST               5 (error)
                
-               162         520 LOAD_FAST                5 (error)
+               182         520 LOAD_FAST                5 (error)
                            522 LOAD_METHOD             16 (getcode)
                            544 PRECALL                  0
                            548 CALL                     0
                            558 LOAD_CONST               5 (404)
                            560 COMPARE_OP               2 (==)
                            566 POP_JUMP_FORWARD_IF_FALSE     6 (to 580)
                
-               166         568 POP_EXCEPT
+               186         568 POP_EXCEPT
                            570 LOAD_CONST               0 (None)
                            572 STORE_FAST               5 (error)
                            574 DELETE_FAST              5 (error)
                            576 LOAD_CONST               6 (False)
                            578 RETURN_VALUE
                
-               167     >>  580 LOAD_FAST                5 (error)
+               187     >>  580 LOAD_FAST                5 (error)
                            582 RAISE_VARARGS            1
                        >>  584 LOAD_CONST               0 (None)
                            586 STORE_FAST               5 (error)
                            588 DELETE_FAST              5 (error)
                            590 RERAISE                  1
                
-               161     >>  592 RERAISE                  0
+               181     >>  592 RERAISE                  0
                        >>  594 COPY                     3
                            596 POP_EXCEPT
                            598 RERAISE                  1
                ExceptionTable:
                  144 to 204 -> 480 [0]
                  206 to 426 -> 454 [1] lasti
                  428 to 450 -> 480 [0]
@@ -1240,17 +1450,17 @@
                   '-'
                   404
                   False
                names      ('os', 'path', 'join', 'index_url', 'distribution_name', 'LOG', 'info', 'urllib', 'request', 'urlopen', 'debug', 'status', 'read', 'encode', 'error', 'HTTPError', 'getcode')
                varnames   ('self', 'candidate_version', 'repo_url', 'response', 'body', 'error')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'version_in_repository'
-               firstlineno 144
+               firstlineno 164
                lnotab 0x020154023803020140014002280136043ef8360a260130040c010cfa
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 35
                code
@@ -1268,124 +1478,124 @@
                   2a7401000000000000000000007c006a0100000000000000006403a60200
                   00ab020000000000000000a0080000000000000000000000000000000000
                   0000007c01a6010000ab0100000000000000000100640053006400530023
                   007c027c016b030000000072297401000000000000000000007c006a0100
                   000000000000006403a6020000ab020000000000000000a0080000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   00010077007700780359007701
-               169           0 RETURN_GENERATOR
+               189           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
                
-               171           6 LOAD_GLOBAL              1 (NULL + open)
+               191           6 LOAD_GLOBAL              1 (NULL + open)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (version_path)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 LOAD_METHOD              2 (read)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 STORE_FAST               1 (old_version_content)
                
-               172          82 LOAD_FAST                1 (old_version_content)
+               192          82 LOAD_FAST                1 (old_version_content)
                             84 STORE_FAST               2 (new_version_content)
                
-               179          86 LOAD_FAST                0 (self)
+               199          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                3 (marker)
                             98 LOAD_FAST                1 (old_version_content)
                            100 CONTAINS_OP              1
                            102 POP_JUMP_FORWARD_IF_FALSE    56 (to 216)
                
-               180         104 LOAD_GLOBAL              8 (VERSION_PATTERN)
+               200         104 LOAD_GLOBAL              8 (VERSION_PATTERN)
                            116 LOAD_METHOD              5 (sub)
                
-               181         138 LOAD_CONST               1 ('__version__ = ')
+               201         138 LOAD_CONST               1 ('__version__ = ')
                            140 LOAD_GLOBAL             13 (NULL + repr)
                            152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                7 (version)
                            164 PRECALL                  1
                            168 CALL                     1
                            178 FORMAT_VALUE             0
                            180 LOAD_CONST               2 ('  # ')
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                3 (marker)
                            194 FORMAT_VALUE             0
                            196 BUILD_STRING             4
                
-               182         198 LOAD_FAST                1 (old_version_content)
+               202         198 LOAD_FAST                1 (old_version_content)
                
-               180         200 PRECALL                  2
+               200         200 PRECALL                  2
                            204 CALL                     2
                            214 STORE_FAST               2 (new_version_content)
                
-               184     >>  216 NOP
+               204     >>  216 NOP
                
-               187         218 LOAD_FAST                2 (new_version_content)
+               207         218 LOAD_FAST                2 (new_version_content)
                            220 LOAD_FAST                1 (old_version_content)
                            222 COMPARE_OP               3 (!=)
                            228 POP_JUMP_FORWARD_IF_FALSE    40 (to 310)
                
-               188         230 LOAD_GLOBAL              1 (NULL + open)
+               208         230 LOAD_GLOBAL              1 (NULL + open)
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                1 (version_path)
                            254 LOAD_CONST               3 ('w')
                            256 PRECALL                  2
                            260 CALL                     2
                            270 LOAD_METHOD              8 (write)
                            292 LOAD_FAST                2 (new_version_content)
                            294 PRECALL                  1
                            298 CALL                     1
                            308 POP_TOP
                
-               189     >>  310 LOAD_CONST               0 (None)
+               209     >>  310 LOAD_CONST               0 (None)
                            312 YIELD_VALUE
                            314 RESUME                   1
                            316 POP_TOP
                
-               191         318 LOAD_FAST                2 (new_version_content)
+               211         318 LOAD_FAST                2 (new_version_content)
                            320 LOAD_FAST                1 (old_version_content)
                            322 COMPARE_OP               3 (!=)
                            328 POP_JUMP_FORWARD_IF_FALSE    42 (to 414)
                
-               193         330 LOAD_GLOBAL              1 (NULL + open)
+               213         330 LOAD_GLOBAL              1 (NULL + open)
                            342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                1 (version_path)
                            354 LOAD_CONST               3 ('w')
                            356 PRECALL                  2
                            360 CALL                     2
                            370 LOAD_METHOD              8 (write)
                            392 LOAD_FAST                1 (old_version_content)
                            394 PRECALL                  1
                            398 CALL                     1
                            408 POP_TOP
                            410 LOAD_CONST               0 (None)
                            412 RETURN_VALUE
                
-               191     >>  414 LOAD_CONST               0 (None)
+               211     >>  414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                            420 LOAD_FAST                2 (new_version_content)
                            422 LOAD_FAST                1 (old_version_content)
                            424 COMPARE_OP               3 (!=)
                            430 POP_JUMP_FORWARD_IF_FALSE    41 (to 514)
                
-               193         432 LOAD_GLOBAL              1 (NULL + open)
+               213         432 LOAD_GLOBAL              1 (NULL + open)
                            444 LOAD_FAST                0 (self)
                            446 LOAD_ATTR                1 (version_path)
                            456 LOAD_CONST               3 ('w')
                            458 PRECALL                  2
                            462 CALL                     2
                            472 LOAD_METHOD              8 (write)
                            494 LOAD_FAST                1 (old_version_content)
                            496 PRECALL                  1
                            500 CALL                     1
                            510 POP_TOP
                            512 RERAISE                  0
                
-               191     >>  514 RERAISE                  0
+               211     >>  514 RERAISE                  0
                        >>  516 COPY                     3
                            518 POP_EXCEPT
                            520 RERAISE                  1
                ExceptionTable:
                  218 to 316 -> 418 [0]
                  418 to 514 -> 516 [1] lasti
                consts
@@ -1393,365 +1603,705 @@
                   '__version__ = '
                   '  # '
                   'w'
                names      ('open', 'version_path', 'read', 'marker', 'VERSION_PATTERN', 'sub', 'repr', 'version', 'write')
                varnames   ('self', 'old_version_content', 'new_version_content')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'patched_version'
-               firstlineno 169
+               firstlineno 189
                lnotab
                   0x06024c010407120122013c0102fe100402030c01500108020c0254fe12
                   0252fe
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000053
                   00
-               195           0 RESUME                   0
+               215           0 RESUME                   0
                
-               198           2 LOAD_FAST                0 (self)
+               218           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_wheel)
                
-               199          36 LOAD_FAST                1 (wheel_directory)
+               219          36 LOAD_FAST                1 (wheel_directory)
                
-               200          38 LOAD_FAST                2 (config_settings)
+               220          38 LOAD_FAST                2 (config_settings)
                
-               201          40 LOAD_FAST                3 (metadata_directory)
+               221          40 LOAD_FAST                3 (metadata_directory)
                
-               198          42 KW_NAMES                 1
+               218          42 KW_NAMES                 1
                             44 PRECALL                  3
                             48 CALL                     3
                             58 RETURN_VALUE
                consts
                   None
                   ('config_settings', 'metadata_directory')
                names      ('build_backend', 'build_wheel')
                varnames   ('self', 'wheel_directory', 'config_settings', 'metadata_directory')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_wheel'
-               firstlineno 195
+               firstlineno 215
                lnotab 0x020322010201020102fd
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c02ac01a6020000ab0200000000000000005300
-               204           0 RESUME                   0
+               224           0 RESUME                   0
                
-               205           2 LOAD_FAST                0 (self)
+               225           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_sdist)
                
-               206          36 LOAD_FAST                1 (sdist_directory)
+               226          36 LOAD_FAST                1 (sdist_directory)
                             38 LOAD_FAST                2 (config_settings)
                
-               205          40 KW_NAMES                 1
+               225          40 KW_NAMES                 1
                             42 PRECALL                  2
                             46 CALL                     2
                             56 RETURN_VALUE
                consts
                   None
                   ('sdist_directory', 'config_settings')
                names      ('build_backend', 'build_sdist')
                varnames   ('self', 'sdist_directory', 'config_settings')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_sdist'
-               firstlineno 204
+               firstlineno 224
                lnotab 0x0201220104ff
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c017c027c03ac01a6030000ab03000000000000000053
                   00
-               209           0 RESUME                   0
+               229           0 RESUME                   0
                
-               212           2 LOAD_FAST                0 (self)
+               232           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (build_backend)
                             14 LOAD_METHOD              1 (build_editable)
                
-               213          36 LOAD_FAST                1 (wheel_directory)
+               233          36 LOAD_FAST                1 (wheel_directory)
                
-               214          38 LOAD_FAST                2 (config_settings)
+               234          38 LOAD_FAST                2 (config_settings)
                
-               215          40 LOAD_FAST                3 (metadata_directory)
+               235          40 LOAD_FAST                3 (metadata_directory)
                
-               212          42 KW_NAMES                 1
+               232          42 KW_NAMES                 1
                             44 PRECALL                  3
                             48 CALL                     3
                             58 RETURN_VALUE
                consts
                   None
                   ('config_settings', 'metadata_directory')
                names      ('build_backend', 'build_editable')
                varnames   ('self', 'wheel_directory', 'config_settings', 'metadata_directory')
                freevars   ()
                cellvars   ()
-               filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
                name       'delegate_build_editable'
-               firstlineno 209
+               firstlineno 229
                lnotab 0x020322010201020102fd
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 2
+               flags     : 3
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000a60000
+                  00ab0000000000000000005300
+               238           0 RESUME                   0
+               
+               239           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (get_requires_for_build_wheel)
+                            26 PRECALL                  0
+                            30 CALL                     0
+                            40 RETURN_VALUE
+               consts
+                  None
+               names      ('get_requires_for_build_wheel',)
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'get_requires_for_build_editable'
+               firstlineno 238
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 4
+               flags     : 3
+               code
+                  0x970067007d017400000000000000000000006a01000000000000000064
+                  016b0000000000731a7c006a020000000000000000a00300000000000000
+                  000000000000000000000000006402a6010000ab01000000000000000072
+                  157c01a00400000000000000000000000000000000000000006403a60100
+                  00ab01000000000000000001007400000000000000000000006a01000000
+                  000000000064016b000000000072157c01a0040000000000000000000000
+                  0000000000000000006404a6010000ab0100000000000000000100740a00
+                  000000000000000000a00600000000000000000000000000000000000000
+                  0064057c01a6020000ab02000000000000000001007c015300
+               241           0 RESUME                   0
+               
+               242           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (out)
+               
+               255           6 LOAD_GLOBAL              0 (sys)
+                            18 LOAD_ATTR                1 (version_info)
+                            28 LOAD_CONST               1 ((3, 11))
+                            30 COMPARE_OP               0 (<)
+                            36 POP_JUMP_FORWARD_IF_TRUE    26 (to 90)
+                            38 LOAD_FAST                0 (self)
+                            40 LOAD_ATTR                2 (build_backend_name)
+                            50 LOAD_METHOD              3 (startswith)
+               
+               256          72 LOAD_CONST               2 ('setuptools.')
+               
+               255          74 PRECALL                  1
+                            78 CALL                     1
+                            88 POP_JUMP_FORWARD_IF_FALSE    21 (to 132)
+               
+               259     >>   90 LOAD_FAST                1 (out)
+                            92 LOAD_METHOD              4 (append)
+                           114 LOAD_CONST               3 ('setuptools>=40.8.0')
+                           116 PRECALL                  1
+                           120 CALL                     1
+                           130 POP_TOP
+               
+               261     >>  132 LOAD_GLOBAL              0 (sys)
+                           144 LOAD_ATTR                1 (version_info)
+                           154 LOAD_CONST               1 ((3, 11))
+                           156 COMPARE_OP               0 (<)
+                           162 POP_JUMP_FORWARD_IF_FALSE    21 (to 206)
+               
+               262         164 LOAD_FAST                1 (out)
+                           166 LOAD_METHOD              4 (append)
+                           188 LOAD_CONST               4 ('tomli>=2.0.1')
+                           190 PRECALL                  1
+                           194 CALL                     1
+                           204 POP_TOP
+               
+               264     >>  206 LOAD_GLOBAL             10 (LOG)
+                           218 LOAD_METHOD              6 (info)
+                           240 LOAD_CONST               5 ('sdist requires: %s')
+                           242 LOAD_FAST                1 (out)
+                           244 PRECALL                  2
+                           248 CALL                     2
+                           258 POP_TOP
+               
+               266         260 LOAD_FAST                1 (out)
+                           262 RETURN_VALUE
+               consts
+                  None
+                  (3, 11)
+                  'setuptools.'
+                  'setuptools>=40.8.0'
+                  'tomli>=2.0.1'
+                  'sdist requires: %s'
+               names      ('sys', 'version_info', 'build_backend_name', 'startswith', 'append', 'LOG', 'info')
+               varnames   ('self', 'out')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'get_requires_for_build_sdist'
+               firstlineno 241
+               lnotab 0x0201040d420102ff10042a0220012a023602
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c00a0000000000000000000000000000000000000000000a60000
+                  00ab0000000000000000007d017402000000000000000000006a02000000
+                  000000000064016b0000000000731a7c006a030000000000000000a00400
+                  000000000000000000000000000000000000006402a6010000ab01000000
+                  000000000072157c01a00500000000000000000000000000000000000000
+                  006403a6010000ab01000000000000000001007c015300
+               268           0 RESUME                   0
+               
+               269           2 LOAD_FAST                0 (self)
+                             4 LOAD_METHOD              0 (get_requires_for_build_sdist)
+                            26 PRECALL                  0
+                            30 CALL                     0
+                            40 STORE_FAST               1 (out)
+               
+               271          42 LOAD_GLOBAL              2 (sys)
+                            54 LOAD_ATTR                2 (version_info)
+                            64 LOAD_CONST               1 ((3, 11))
+                            66 COMPARE_OP               0 (<)
+                            72 POP_JUMP_FORWARD_IF_TRUE    26 (to 126)
+                            74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                3 (build_backend_name)
+                            86 LOAD_METHOD              4 (startswith)
+               
+               272         108 LOAD_CONST               2 ('setuptools.')
+               
+               271         110 PRECALL                  1
+                           114 CALL                     1
+                           124 POP_JUMP_FORWARD_IF_FALSE    21 (to 168)
+               
+               275     >>  126 LOAD_FAST                1 (out)
+                           128 LOAD_METHOD              5 (append)
+                           150 LOAD_CONST               3 ('wheel')
+                           152 PRECALL                  1
+                           156 CALL                     1
+                           166 POP_TOP
+               
+               276     >>  168 LOAD_FAST                1 (out)
+                           170 RETURN_VALUE
+               consts
+                  None
+                  (3, 11)
+                  'setuptools.'
+                  'wheel'
+               names      ('get_requires_for_build_sdist', 'sys', 'version_info', 'build_backend_name', 'startswith', 'append')
+               varnames   ('self', 'out')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+               name       'get_requires_for_build_wheel'
+               firstlineno 268
+               lnotab 0x02012802420102ff10042a01
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'str', 'marker', '_find_version_path', 'version_path', 'build_backend', 'index_url', 'distribution_name', 'version', '_get_version', 'bool', 'version_in_repository', 'contextmanager', 'patched_version', 'delegate_build_wheel', 'delegate_build_sdist', 'delegate_build_editable')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'dict', 'pyproject_toml', 'project_config', 'tool_config', 'str', 'marker', '_find_version_path', 'version_path', 'build_backend_name', 'build_backend', 'index_url', 'distribution_name', 'version', '_get_version', 'bool', 'version_in_repository', 'contextmanager', 'patched_version', 'delegate_build_wheel', 'delegate_build_sdist', 'delegate_build_editable', 'get_requires_for_build_editable', 'get_requires_for_build_sdist', 'get_requires_for_build_wheel')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'DateVersion'
-         firstlineno 27
+         firstlineno 28
          lnotab
-            0x0a01080502010aff0e0102060c1102010aff0e010205020104ff0e0102
-            1402010aff0e01020902010aff0e01021402010aff0e0102070c15101902
-            0104ff0e01021906090605
+            0x0a01080702010aff0e01021002010aff0e01020302010aff0e01020802
+            010aff0e0102060c1102010aff0e01020502010aff0e010205020104ff0e
+            01021102010aff0e01020a02010aff0e01020302010aff0e0102070c1510
+            19020104ff0e0102190609060506090603061b
       'DateVersion'
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
-            0x97007401000000000000000000007c01ac01a6010000ab010000000000
-            0000007d037c03a0010000000000000000000000000000000000000000a6
-            000000ab000000000000000000350001007c03a002000000000000000000
-            00000000000000000000007c007c017c02ac02a6030000ab030000000000
-            0000006302640064006400a6020000ab0200000000000000000100530023
-            00310073047702780359007701010059000100010064005300
-         219           0 RESUME                   0
-         
-         220           2 LOAD_GLOBAL              1 (NULL + DateVersion)
-                      14 LOAD_FAST                1 (config_settings)
-                      16 KW_NAMES                 1
-                      18 PRECALL                  1
-                      22 CALL                     1
-                      32 STORE_FAST               3 (helper)
-         
-         221          34 LOAD_FAST                3 (helper)
-                      36 LOAD_METHOD              1 (patched_version)
-                      58 PRECALL                  0
-                      62 CALL                     0
-                      72 BEFORE_WITH
-                      74 POP_TOP
-         
-         222          76 LOAD_FAST                3 (helper)
-                      78 LOAD_METHOD              2 (delegate_build_wheel)
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c007c017c02a6040000ab04000000000000000001
+            007405000000000000000000007c01ac02a6010000ab0100000000000000
+            007d037c03a0030000000000000000000000000000000000000000a60000
+            00ab000000000000000000350001007c03a0040000000000000000000000
+            0000000000000000007c007c017c02ac03a6030000ab0300000000000000
+            006302640064006400a6020000ab02000000000000000001005300230031
+            0073047702780359007701010059000100010064005300
+         279           0 RESUME                   0
          
-         223         100 LOAD_FAST                0 (wheel_directory)
+         280           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
          
-         224         102 LOAD_FAST                1 (config_settings)
-         
-         225         104 LOAD_FAST                2 (metadata_directory)
-         
-         222         106 KW_NAMES                 2
-                     108 PRECALL                  3
-                     112 CALL                     3
-         
-         221         122 SWAP                     2
-                     124 LOAD_CONST               0 (None)
-                     126 LOAD_CONST               0 (None)
-                     128 LOAD_CONST               0 (None)
-                     130 PRECALL                  2
-                     134 CALL                     2
-                     144 POP_TOP
-                     146 RETURN_VALUE
-                 >>  148 PUSH_EXC_INFO
-                     150 WITH_EXCEPT_START
-                     152 POP_JUMP_FORWARD_IF_TRUE     4 (to 162)
-                     154 RERAISE                  2
-                 >>  156 COPY                     3
-                     158 POP_EXCEPT
-                     160 RERAISE                  1
-                 >>  162 POP_TOP
-                     164 POP_EXCEPT
-                     166 POP_TOP
-                     168 POP_TOP
-                     170 LOAD_CONST               0 (None)
-                     172 RETURN_VALUE
+         281          36 LOAD_CONST               1 ('build_wheel %s %s %s')
+                      38 LOAD_FAST                0 (wheel_directory)
+                      40 LOAD_FAST                1 (config_settings)
+                      42 LOAD_FAST                2 (metadata_directory)
+         
+         280          44 PRECALL                  4
+                      48 CALL                     4
+                      58 POP_TOP
+         
+         284          60 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      72 LOAD_FAST                1 (config_settings)
+                      74 KW_NAMES                 2
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 STORE_FAST               3 (helper)
+         
+         285          92 LOAD_FAST                3 (helper)
+                      94 LOAD_METHOD              3 (patched_version)
+                     116 PRECALL                  0
+                     120 CALL                     0
+                     130 BEFORE_WITH
+                     132 POP_TOP
+         
+         286         134 LOAD_FAST                3 (helper)
+                     136 LOAD_METHOD              4 (delegate_build_wheel)
+         
+         287         158 LOAD_FAST                0 (wheel_directory)
+         
+         288         160 LOAD_FAST                1 (config_settings)
+         
+         289         162 LOAD_FAST                2 (metadata_directory)
+         
+         286         164 KW_NAMES                 3
+                     166 PRECALL                  3
+                     170 CALL                     3
+         
+         285         180 SWAP                     2
+                     182 LOAD_CONST               0 (None)
+                     184 LOAD_CONST               0 (None)
+                     186 LOAD_CONST               0 (None)
+                     188 PRECALL                  2
+                     192 CALL                     2
+                     202 POP_TOP
+                     204 RETURN_VALUE
+                 >>  206 PUSH_EXC_INFO
+                     208 WITH_EXCEPT_START
+                     210 POP_JUMP_FORWARD_IF_TRUE     4 (to 220)
+                     212 RERAISE                  2
+                 >>  214 COPY                     3
+                     216 POP_EXCEPT
+                     218 RERAISE                  1
+                 >>  220 POP_TOP
+                     222 POP_EXCEPT
+                     224 POP_TOP
+                     226 POP_TOP
+                     228 LOAD_CONST               0 (None)
+                     230 RETURN_VALUE
          ExceptionTable:
-           74 to 120 -> 148 [1] lasti
-           148 to 154 -> 156 [3] lasti
-           162 to 162 -> 156 [3] lasti
+           132 to 178 -> 206 [1] lasti
+           206 to 212 -> 214 [3] lasti
+           220 to 220 -> 214 [3] lasti
          consts
             None
+            'build_wheel %s %s %s'
             ('config_settings',)
             ('config_settings', 'metadata_directory')
-         names      ('DateVersion', 'patched_version', 'delegate_build_wheel')
+         names      ('LOG', 'debug', 'DateVersion', 'patched_version', 'delegate_build_wheel')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'helper')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_wheel'
-         firstlineno 219
-         lnotab 0x020120012a0118010201020102fd10ff
+         firstlineno 279
+         lnotab 0x0201220108ff100420012a0118010201020102fd10ff
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
-            0x97007401000000000000000000007c01ac01a6010000ab010000000000
-            0000007d027c02a0010000000000000000000000000000000000000000a6
-            000000ab000000000000000000350001007c02a002000000000000000000
-            00000000000000000000007c007c01a6020000ab02000000000000000063
-            02640064006400a6020000ab020000000000000000010053002300310073
-            047702780359007701010059000100010064005300
-         229           0 RESUME                   0
-         
-         230           2 LOAD_GLOBAL              1 (NULL + DateVersion)
-                      14 LOAD_FAST                1 (config_settings)
-                      16 KW_NAMES                 1
-                      18 PRECALL                  1
-                      22 CALL                     1
-                      32 STORE_FAST               2 (helper)
-         
-         231          34 LOAD_FAST                2 (helper)
-                      36 LOAD_METHOD              1 (patched_version)
-                      58 PRECALL                  0
-                      62 CALL                     0
-                      72 BEFORE_WITH
-                      74 POP_TOP
-         
-         232          76 LOAD_FAST                2 (helper)
-                      78 LOAD_METHOD              2 (delegate_build_sdist)
-                     100 LOAD_FAST                0 (sdist_directory)
-                     102 LOAD_FAST                1 (config_settings)
-                     104 PRECALL                  2
-                     108 CALL                     2
-         
-         231         118 SWAP                     2
-                     120 LOAD_CONST               0 (None)
-                     122 LOAD_CONST               0 (None)
-                     124 LOAD_CONST               0 (None)
-                     126 PRECALL                  2
-                     130 CALL                     2
-                     140 POP_TOP
-                     142 RETURN_VALUE
-                 >>  144 PUSH_EXC_INFO
-                     146 WITH_EXCEPT_START
-                     148 POP_JUMP_FORWARD_IF_TRUE     4 (to 158)
-                     150 RERAISE                  2
-                 >>  152 COPY                     3
-                     154 POP_EXCEPT
-                     156 RERAISE                  1
-                 >>  158 POP_TOP
-                     160 POP_EXCEPT
-                     162 POP_TOP
-                     164 POP_TOP
-                     166 LOAD_CONST               0 (None)
-                     168 RETURN_VALUE
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c007c01a6030000ab030000000000000000010074
+            05000000000000000000007c01ac02a6010000ab0100000000000000007d
+            027c02a0030000000000000000000000000000000000000000a6000000ab
+            000000000000000000350001007c02a00400000000000000000000000000
+            000000000000007c007c01a6020000ab0200000000000000006302640064
+            006400a6020000ab02000000000000000001005300230031007304770278
+            0359007701010059000100010064005300
+         293           0 RESUME                   0
+         
+         294           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
+                      36 LOAD_CONST               1 ('build_sdist %s %s')
+                      38 LOAD_FAST                0 (sdist_directory)
+                      40 LOAD_FAST                1 (config_settings)
+                      42 PRECALL                  3
+                      46 CALL                     3
+                      56 POP_TOP
+         
+         296          58 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      70 LOAD_FAST                1 (config_settings)
+                      72 KW_NAMES                 2
+                      74 PRECALL                  1
+                      78 CALL                     1
+                      88 STORE_FAST               2 (helper)
+         
+         297          90 LOAD_FAST                2 (helper)
+                      92 LOAD_METHOD              3 (patched_version)
+                     114 PRECALL                  0
+                     118 CALL                     0
+                     128 BEFORE_WITH
+                     130 POP_TOP
+         
+         298         132 LOAD_FAST                2 (helper)
+                     134 LOAD_METHOD              4 (delegate_build_sdist)
+                     156 LOAD_FAST                0 (sdist_directory)
+                     158 LOAD_FAST                1 (config_settings)
+                     160 PRECALL                  2
+                     164 CALL                     2
+         
+         297         174 SWAP                     2
+                     176 LOAD_CONST               0 (None)
+                     178 LOAD_CONST               0 (None)
+                     180 LOAD_CONST               0 (None)
+                     182 PRECALL                  2
+                     186 CALL                     2
+                     196 POP_TOP
+                     198 RETURN_VALUE
+                 >>  200 PUSH_EXC_INFO
+                     202 WITH_EXCEPT_START
+                     204 POP_JUMP_FORWARD_IF_TRUE     4 (to 214)
+                     206 RERAISE                  2
+                 >>  208 COPY                     3
+                     210 POP_EXCEPT
+                     212 RERAISE                  1
+                 >>  214 POP_TOP
+                     216 POP_EXCEPT
+                     218 POP_TOP
+                     220 POP_TOP
+                     222 LOAD_CONST               0 (None)
+                     224 RETURN_VALUE
          ExceptionTable:
-           74 to 116 -> 144 [1] lasti
-           144 to 150 -> 152 [3] lasti
-           158 to 158 -> 152 [3] lasti
+           130 to 172 -> 200 [1] lasti
+           200 to 206 -> 208 [3] lasti
+           214 to 214 -> 208 [3] lasti
          consts
             None
+            'build_sdist %s %s'
             ('config_settings',)
-         names      ('DateVersion', 'patched_version', 'delegate_build_sdist')
+         names      ('LOG', 'debug', 'DateVersion', 'patched_version', 'delegate_build_sdist')
          varnames   ('sdist_directory', 'config_settings', 'helper')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_sdist'
-         firstlineno 229
-         lnotab 0x020120012a012aff
+         firstlineno 293
+         lnotab 0x0201380220012a012aff
       code
          argcount  : 3
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
-            0x97007401000000000000000000007c01ac01a6010000ab010000000000
-            0000007d037c03a0010000000000000000000000000000000000000000a6
-            000000ab000000000000000000350001007c03a002000000000000000000
-            00000000000000000000007c007c017c02a6030000ab0300000000000000
-            006302640064006400a6020000ab02000000000000000001005300230031
-            0073047702780359007701010059000100010064005300
-         249           0 RESUME                   0
-         
-         250           2 LOAD_GLOBAL              1 (NULL + DateVersion)
-                      14 LOAD_FAST                1 (config_settings)
-                      16 KW_NAMES                 1
-                      18 PRECALL                  1
-                      22 CALL                     1
-                      32 STORE_FAST               3 (helper)
-         
-         252          34 LOAD_FAST                3 (helper)
-                      36 LOAD_METHOD              1 (patched_version)
-                      58 PRECALL                  0
-                      62 CALL                     0
-                      72 BEFORE_WITH
-                      74 POP_TOP
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c007c017c02a6040000ab04000000000000000001
+            007405000000000000000000007c01ac02a6010000ab0100000000000000
+            007d037c03a0030000000000000000000000000000000000000000a60000
+            00ab000000000000000000350001007c03a0040000000000000000000000
+            0000000000000000007c007c017c02a6030000ab03000000000000000063
+            02640064006400a6020000ab020000000000000000010053002300310073
+            047702780359007701010059000100010064005300
+         315           0 RESUME                   0
          
-         253          76 LOAD_FAST                3 (helper)
-                      78 LOAD_METHOD              2 (delegate_build_editable)
+         316           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
          
-         254         100 LOAD_FAST                0 (wheel_directory)
-                     102 LOAD_FAST                1 (config_settings)
-                     104 LOAD_FAST                2 (metadata_directory)
-         
-         253         106 PRECALL                  3
-                     110 CALL                     3
-         
-         252         120 SWAP                     2
-                     122 LOAD_CONST               0 (None)
-                     124 LOAD_CONST               0 (None)
-                     126 LOAD_CONST               0 (None)
-                     128 PRECALL                  2
-                     132 CALL                     2
-                     142 POP_TOP
-                     144 RETURN_VALUE
-                 >>  146 PUSH_EXC_INFO
-                     148 WITH_EXCEPT_START
-                     150 POP_JUMP_FORWARD_IF_TRUE     4 (to 160)
-                     152 RERAISE                  2
-                 >>  154 COPY                     3
-                     156 POP_EXCEPT
-                     158 RERAISE                  1
-                 >>  160 POP_TOP
-                     162 POP_EXCEPT
-                     164 POP_TOP
-                     166 POP_TOP
-                     168 LOAD_CONST               0 (None)
-                     170 RETURN_VALUE
+         317          36 LOAD_CONST               1 ('build_editable %s %s %s')
+                      38 LOAD_FAST                0 (wheel_directory)
+                      40 LOAD_FAST                1 (config_settings)
+                      42 LOAD_FAST                2 (metadata_directory)
+         
+         316          44 PRECALL                  4
+                      48 CALL                     4
+                      58 POP_TOP
+         
+         319          60 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      72 LOAD_FAST                1 (config_settings)
+                      74 KW_NAMES                 2
+                      76 PRECALL                  1
+                      80 CALL                     1
+                      90 STORE_FAST               3 (helper)
+         
+         321          92 LOAD_FAST                3 (helper)
+                      94 LOAD_METHOD              3 (patched_version)
+                     116 PRECALL                  0
+                     120 CALL                     0
+                     130 BEFORE_WITH
+                     132 POP_TOP
+         
+         322         134 LOAD_FAST                3 (helper)
+                     136 LOAD_METHOD              4 (delegate_build_editable)
+         
+         323         158 LOAD_FAST                0 (wheel_directory)
+                     160 LOAD_FAST                1 (config_settings)
+                     162 LOAD_FAST                2 (metadata_directory)
+         
+         322         164 PRECALL                  3
+                     168 CALL                     3
+         
+         321         178 SWAP                     2
+                     180 LOAD_CONST               0 (None)
+                     182 LOAD_CONST               0 (None)
+                     184 LOAD_CONST               0 (None)
+                     186 PRECALL                  2
+                     190 CALL                     2
+                     200 POP_TOP
+                     202 RETURN_VALUE
+                 >>  204 PUSH_EXC_INFO
+                     206 WITH_EXCEPT_START
+                     208 POP_JUMP_FORWARD_IF_TRUE     4 (to 218)
+                     210 RERAISE                  2
+                 >>  212 COPY                     3
+                     214 POP_EXCEPT
+                     216 RERAISE                  1
+                 >>  218 POP_TOP
+                     220 POP_EXCEPT
+                     222 POP_TOP
+                     224 POP_TOP
+                     226 LOAD_CONST               0 (None)
+                     228 RETURN_VALUE
          ExceptionTable:
-           74 to 118 -> 146 [1] lasti
-           146 to 152 -> 154 [3] lasti
-           160 to 160 -> 154 [3] lasti
+           132 to 176 -> 204 [1] lasti
+           204 to 210 -> 212 [3] lasti
+           218 to 218 -> 212 [3] lasti
          consts
             None
+            'build_editable %s %s %s'
             ('config_settings',)
-         names      ('DateVersion', 'patched_version', 'delegate_build_editable')
+         names      ('LOG', 'debug', 'DateVersion', 'patched_version', 'delegate_build_editable')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'helper')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
          name       'build_editable'
-         firstlineno 249
-         lnotab 0x020120022a01180106ff0eff
+         firstlineno 315
+         lnotab 0x0201220108ff100320022a01180106ff0eff
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c00a6020000ab0200000000000000000100740500
+            0000000000000000007c00ac02a6010000ab0100000000000000007d017c
+            01a0030000000000000000000000000000000000000000a6000000ab0000
+            000000000000005300
+         327           0 RESUME                   0
+         
+         328           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
+                      36 LOAD_CONST               1 ('get_requires_for_build_wheel %s')
+                      38 LOAD_FAST                0 (config_settings)
+                      40 PRECALL                  2
+                      44 CALL                     2
+                      54 POP_TOP
+         
+         329          56 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      68 LOAD_FAST                0 (config_settings)
+                      70 KW_NAMES                 2
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 STORE_FAST               1 (helper)
+         
+         330          88 LOAD_FAST                1 (helper)
+                      90 LOAD_METHOD              3 (get_requires_for_build_wheel)
+                     112 PRECALL                  0
+                     116 CALL                     0
+                     126 RETURN_VALUE
+         consts
+            None
+            'get_requires_for_build_wheel %s'
+            ('config_settings',)
+         names      ('LOG', 'debug', 'DateVersion', 'get_requires_for_build_wheel')
+         varnames   ('config_settings', 'helper')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         name       'get_requires_for_build_wheel'
+         firstlineno 327
+         lnotab 0x020136012001
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c00a6020000ab0200000000000000000100740500
+            0000000000000000007c00ac02a6010000ab0100000000000000007d017c
+            01a0030000000000000000000000000000000000000000a6000000ab0000
+            000000000000005300
+         333           0 RESUME                   0
+         
+         334           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
+                      36 LOAD_CONST               1 ('get_requires_for_build_sdist %s')
+                      38 LOAD_FAST                0 (config_settings)
+                      40 PRECALL                  2
+                      44 CALL                     2
+                      54 POP_TOP
+         
+         336          56 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      68 LOAD_FAST                0 (config_settings)
+                      70 KW_NAMES                 2
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 STORE_FAST               1 (helper)
+         
+         337          88 LOAD_FAST                1 (helper)
+                      90 LOAD_METHOD              3 (get_requires_for_build_sdist)
+                     112 PRECALL                  0
+                     116 CALL                     0
+                     126 RETURN_VALUE
+         consts
+            None
+            'get_requires_for_build_sdist %s'
+            ('config_settings',)
+         names      ('LOG', 'debug', 'DateVersion', 'get_requires_for_build_sdist')
+         varnames   ('config_settings', 'helper')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         name       'get_requires_for_build_sdist'
+         firstlineno 333
+         lnotab 0x020136022001
+      code
+         argcount  : 1
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            0000000000000064017c00a6020000ab0200000000000000000100740500
+            0000000000000000007c00ac02a6010000ab0100000000000000007d017c
+            01a0030000000000000000000000000000000000000000a6000000ab0000
+            000000000000005300
+         340           0 RESUME                   0
+         
+         341           2 LOAD_GLOBAL              0 (LOG)
+                      14 LOAD_METHOD              1 (debug)
+                      36 LOAD_CONST               1 ('get_requires_for_build_editable %s')
+                      38 LOAD_FAST                0 (config_settings)
+                      40 PRECALL                  2
+                      44 CALL                     2
+                      54 POP_TOP
+         
+         342          56 LOAD_GLOBAL              5 (NULL + DateVersion)
+                      68 LOAD_FAST                0 (config_settings)
+                      70 KW_NAMES                 2
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 STORE_FAST               1 (helper)
+         
+         343          88 LOAD_FAST                1 (helper)
+                      90 LOAD_METHOD              3 (get_requires_for_build_editable)
+                     112 PRECALL                  0
+                     116 CALL                     0
+                     126 RETURN_VALUE
+         consts
+            None
+            'get_requires_for_build_editable %s'
+            ('config_settings',)
+         names      ('LOG', 'debug', 'DateVersion', 'get_requires_for_build_editable')
+         varnames   ('config_settings', 'helper')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+         name       'get_requires_for_build_editable'
+         firstlineno 340
+         lnotab 0x020136012001
       (None, None)
       (None,)
-   names      ('os', 'logging', 're', 'urllib.request', 'urllib', 'urllib.error', 'datetime', 'contextlib', 'contextmanager', 'importlib', 'getLogger', 'LOG', 'getenv', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'str', 'normalized', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable')
+   names      ('os', 'logging', 're', 'urllib.request', 'urllib', 'urllib.error', 'datetime', 'contextlib', 'contextmanager', 'importlib', 'sys', 'getLogger', 'LOG', 'getenv', 'setLevel', 'DEBUG', 'addHandler', 'FileHandler', 'compile', 'MULTILINE', 'VERSION_PATTERN', 'str', 'normalized', 'DateVersion', 'build_wheel', 'build_sdist', 'build_editable', 'get_requires_for_build_wheel', 'get_requires_for_build_sdist', 'get_requires_for_build_editable')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/rmcgover/src/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
+   filename   '/home/runner/work/buildsys-dateversion/buildsys-dateversion/src/buildsys_dateversion/_hooks.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010801080108010c010c01080220022001340162022e
-      030c081a7f0041080a0814
+      0x00ff0201080108010801080108010c010c010801080220022001340162
+      022e030c081a7f007c080e0816080c08060807
```

### Comparing `buildsys-dateversion-2023.5.1.23/src/buildsys_dateversion/_hooks.py` & `buildsys-dateversion-2023.5.6/src/buildsys_dateversion/_hooks.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import re
 import urllib.request
 import urllib.error
 from datetime import datetime
 from contextlib import contextmanager
 import importlib
+import sys
 
 LOG = logging.getLogger("buildsys-dateversion")
 
 if os.getenv("BUILDSYS_DATEVERSION_DEBUG"):
     LOG.setLevel(logging.DEBUG)
     LOG.addHandler(logging.FileHandler(os.getenv("BUILDSYS_DATEVERSION_DEBUG")))
 
@@ -24,20 +25,52 @@
     return ".".join([str(int(x)) for x in version.split(".")])
 
 
 class DateVersion:
     def __init__(self, config_settings=None):
         self.config_settings: dict = (config_settings or {}).copy()
         self.datetime = datetime.utcnow()
+        self._pyproject_toml = None
+        self._tool_config = None
         LOG.debug("operating with datetime = %s", self.datetime)
 
     @property
+    def pyproject_toml(self) -> dict:
+        if self._pyproject_toml is None:
+            if sys.version_info >= (3, 11):
+                import tomllib
+            else:
+                import tomli as tomllib
+
+            with open("pyproject.toml", "rb") as f:
+                data = tomllib.load(f)
+
+            LOG.debug("Loaded project metadata: %s", data)
+
+            self._pyproject_toml = data
+
+        return self._pyproject_toml
+
+    @property
+    def project_config(self) -> dict:
+        return self.pyproject_toml["project"]
+
+    @property
+    def tool_config(self) -> dict:
+        if self._tool_config is None:
+            self._tool_config = (self.pyproject_toml.get("tool") or {}).get(
+                "buildsys-dateversion"
+            ) or {}
+            self._tool_config = self._tool_config.copy()
+        return self._tool_config
+
+    @property
     def marker(self) -> str:
         return (
-            self.config_settings.get("dateversion-version-marker")
+            self.tool_config.get("version-marker")
             or "generated by buildsys-dateversion"
         )
 
     def _find_version_path(self) -> str:
         for dirpath, _, files in os.walk("."):
             for file in files:
                 if not file.endswith(".py"):
@@ -52,25 +85,28 @@
         # TODO: more helpful error string
         raise RuntimeError(
             "Could not locate a file in the source tree defining `__version__`"
         )
 
     @property
     def version_path(self) -> str:
-        if "dateversion-version-path" not in self.config_settings:
-            self.config_settings["dateversion-version-path"] = self._find_version_path()
-        return self.config_settings["dateversion-version-path"]
+        if "version-path" not in self.tool_config:
+            self.tool_config["version-path"] = self._find_version_path()
+        return self.tool_config["version-path"]
+
+    @property
+    def build_backend_name(self) -> str:
+        return (
+            self.tool_config.get("build-backend") or "setuptools.build_meta:__legacy__"
+        )
 
     @property
     def build_backend(self):
         if "dateversion-build-backend-object" not in self.config_settings:
-            backend_name = (
-                self.config_settings.get("dateversion-build-backend")
-                or "setuptools.build_meta:__legacy__"
-            )
+            backend_name = self.build_backend_name
 
             components = backend_name.split(":")
             module = importlib.import_module(components[0])
             backend = module
 
             if len(components) == 2:
                 backend = getattr(module, components[1])
@@ -80,41 +116,25 @@
             self.config_settings["dateversion-build-backend-object"] = backend
 
         return self.config_settings["dateversion-build-backend-object"]
 
     @property
     def index_url(self) -> str:
         out = (
+            # TODO: reuse pip or other standard env vars
             self.config_settings.get("dateversion-index-url")
             or "https://pypi.org/simple"
         )
         while out.endswith("/"):
             out = out[:-1]
         return out
 
     @property
     def distribution_name(self) -> str:
-        if "dateversion-distribution-name" not in self.config_settings:
-            try:
-                import tomllib
-            except:
-                # TODO: implement the hook to add this in requires
-                import tomli as tomllib
-
-            with open("pyproject.toml", "rb") as f:
-                data = tomllib.load(f)
-
-            LOG.info("Loaded project metadata: %s", data)
-
-            # TODO: nice error message if this fails
-            self.config_settings["dateversion-distribution-name"] = data["project"][
-                "name"
-            ]
-
-        return self.config_settings["dateversion-distribution-name"]
+        return self.project_config["name"]
 
     @property
     def version(self) -> str:
         if "dateversion-distribution-version" not in self.config_settings:
             self.config_settings[
                 "dateversion-distribution-version"
             ] = self._get_version()
@@ -211,26 +231,72 @@
     ):
         return self.build_backend.build_editable(
             wheel_directory,
             config_settings=config_settings,
             metadata_directory=metadata_directory,
         )
 
+    def get_requires_for_build_editable(self):
+        return self.get_requires_for_build_wheel()
+
+    def get_requires_for_build_sdist(self):
+        out = []
+
+        # Bootstrap problem on python < 3.11:
+        #
+        # There is no standard tomllib yet.
+        # We're about to ask for it to be installed.
+        #
+        # However, that hasn't happened yet, therefore we can't read pyproject.toml,
+        # therefore we can't know what the build backend name is & whether the
+        # setuptools default logic should be applied.
+        #
+        # To resolve this we're just going to assume that you might want setuptools.
+        # Don't like it? Upgrade to python 3.11.
+        if sys.version_info < (3, 11) or self.build_backend_name.startswith(
+            "setuptools."
+        ):
+            # apply the same default behavior as pip
+            out.append("setuptools>=40.8.0")
+
+        if sys.version_info < (3, 11):
+            out.append("tomli>=2.0.1")
+
+        LOG.info("sdist requires: %s", out)
+
+        return out
+
+    def get_requires_for_build_wheel(self):
+        out = self.get_requires_for_build_sdist()
+        # About the 3.11 check, see comment in get_requires_for_build_sdist
+        if sys.version_info < (3, 11) or self.build_backend_name.startswith(
+            "setuptools."
+        ):
+            # apply the same default behavior as pip
+            out.append("wheel")
+        return out
+
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
+    LOG.debug(
+        "build_wheel %s %s %s", wheel_directory, config_settings, metadata_directory
+    )
+
     helper = DateVersion(config_settings=config_settings)
     with helper.patched_version():
         return helper.delegate_build_wheel(
             wheel_directory,
             config_settings=config_settings,
             metadata_directory=metadata_directory,
         )
 
 
 def build_sdist(sdist_directory, config_settings=None):
+    LOG.debug("build_sdist %s %s", sdist_directory, config_settings)
+
     helper = DateVersion(config_settings=config_settings)
     with helper.patched_version():
         return helper.delegate_build_sdist(sdist_directory, config_settings)
 
 
 # FIXME: I only want to define build_editable here if the delegate backend
 # also defines that. But, how can I know which delegate is being used
@@ -243,19 +309,41 @@
 #   at hook execution time and not at import time. So we can't guarantee
 #   the working directory at this point, meaning we can't reliably locate
 #   pyproject.toml to look up settings there.
 #
 # We'll just define a build_editable always, and expect an error if
 # the delegate backend doesn't have it.
 def build_editable(wheel_directory, config_settings=None, metadata_directory=None):
+    LOG.debug(
+        "build_editable %s %s %s", wheel_directory, config_settings, metadata_directory
+    )
     helper = DateVersion(config_settings=config_settings)
     # Should there be version patching for editable mode or not??
     with helper.patched_version():
         return helper.delegate_build_editable(
             wheel_directory, config_settings, metadata_directory
         )
 
 
+def get_requires_for_build_wheel(config_settings=None):
+    LOG.debug("get_requires_for_build_wheel %s", config_settings)
+    helper = DateVersion(config_settings=config_settings)
+    return helper.get_requires_for_build_wheel()
+
+
+def get_requires_for_build_sdist(config_settings=None):
+    LOG.debug("get_requires_for_build_sdist %s", config_settings)
+
+    helper = DateVersion(config_settings=config_settings)
+    return helper.get_requires_for_build_sdist()
+
+
+def get_requires_for_build_editable(config_settings=None):
+    LOG.debug("get_requires_for_build_editable %s", config_settings)
+    helper = DateVersion(config_settings=config_settings)
+    return helper.get_requires_for_build_editable()
+
+
 # TODO: is it necessary to implement prepare_metadata_for_build_wheel
 # as well? Noting that PEP 517 says build_wheel must respect metadata
 # earlier prepared by prepare_metadata_for_build_wheel (if any), so in
 # that case, it'd be too late to patch the version.
```

