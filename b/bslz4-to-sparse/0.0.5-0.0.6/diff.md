# Comparing `tmp/bslz4_to_sparse-0.0.5.tar.gz` & `tmp/bslz4_to_sparse-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bslz4_to_sparse-0.0.5.tar", last modified: Mon Mar 27 14:18:35 2023, max compression
+gzip compressed data, was "bslz4_to_sparse-0.0.6.tar", last modified: Sat May  6 11:59:19 2023, max compression
```

## Comparing `bslz4_to_sparse-0.0.5.tar` & `bslz4_to_sparse-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.963108 bslz4_to_sparse-0.0.5/
--rw-r--r--   0 wright    (2427) id11      (1611)     1067 2023-03-06 21:46:52.000000 bslz4_to_sparse-0.0.5/LICENSE
--rw-r--r--   0 wright    (2427) id11      (1611)      142 2023-03-13 13:21:39.000000 bslz4_to_sparse-0.0.5/MANIFEST.in
--rw-r--r--   0 wright    (2427) id11      (1611)      610 2023-03-27 14:18:35.954121 bslz4_to_sparse-0.0.5/PKG-INFO
--rw-r--r--   0 wright    (2427) id11      (1611)      226 2023-03-07 11:25:12.000000 bslz4_to_sparse-0.0.5/README.md
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.664115 bslz4_to_sparse-0.0.5/bitshuffle/
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.801110 bslz4_to_sparse-0.0.5/bitshuffle/src/
--rw-r--r--   0 wright    (2427) id11      (1611)    65340 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_core.c
--rw-r--r--   0 wright    (2427) id11      (1611)     4533 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_core.h
--rw-r--r--   0 wright    (2427) id11      (1611)     2233 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_internals.h
--rw-r--r--   0 wright    (2427) id11      (1611)     2483 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.5/bitshuffle/src/iochain.c
--rw-r--r--   0 wright    (2427) id11      (1611)     2616 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.5/bitshuffle/src/iochain.h
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.863108 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/
--rw-r--r--   0 wright    (2427) id11      (1611)      610 2023-03-27 14:18:35.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/PKG-INFO
--rw-r--r--   0 wright    (2427) id11      (1611)      529 2023-03-27 14:18:35.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/SOURCES.txt
--rw-r--r--   0 wright    (2427) id11      (1611)        1 2023-03-27 14:18:35.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/dependency_links.txt
--rw-r--r--   0 wright    (2427) id11      (1611)       11 2023-03-27 14:18:35.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/requires.txt
--rw-r--r--   0 wright    (2427) id11      (1611)       16 2023-03-27 14:18:35.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparse.egg-info/top_level.txt
--rw-r--r--   0 wright    (2427) id11      (1611)    27339 2023-03-26 08:06:13.000000 bslz4_to_sparse-0.0.5/bslz4_to_sparsemodule.c
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.666138 bslz4_to_sparse-0.0.5/lz4/
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.889148 bslz4_to_sparse-0.0.5/lz4/lib/
--rw-r--r--   0 wright    (2427) id11      (1611)   114204 2023-03-12 06:07:55.000000 bslz4_to_sparse-0.0.5/lz4/lib/lz4.c
--rw-r--r--   0 wright    (2427) id11      (1611)    44421 2023-03-12 06:07:57.000000 bslz4_to_sparse-0.0.5/lz4/lib/lz4.h
--rw-r--r--   0 wright    (2427) id11      (1611)      118 2023-03-07 07:34:45.000000 bslz4_to_sparse-0.0.5/pyproject.toml
--rw-r--r--   0 wright    (2427) id11      (1611)       38 2023-03-27 14:18:35.964103 bslz4_to_sparse-0.0.5/setup.cfg
--rw-r--r--   0 wright    (2427) id11      (1611)     2737 2023-03-26 08:02:47.000000 bslz4_to_sparse-0.0.5/setup.py
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.928112 bslz4_to_sparse-0.0.5/src/
--rw-r--r--   0 wright    (2427) id11      (1611)     3513 2023-03-26 08:51:55.000000 bslz4_to_sparse-0.0.5/src/__init__.py
--rw-r--r--   0 wright    (2427) id11      (1611)     1337 2023-03-17 13:49:45.000000 bslz4_to_sparse-0.0.5/src/bslz4_to_sparse.c
--rw-r--r--   0 wright    (2427) id11      (1611)     1548 2023-03-17 13:49:47.000000 bslz4_to_sparse-0.0.5/src/bslz4_to_sparse.pyf
-drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-03-27 14:18:35.941130 bslz4_to_sparse-0.0.5/test/
--rw-r--r--   0 wright    (2427) id11      (1611)     4249 2023-03-27 14:17:12.000000 bslz4_to_sparse-0.0.5/test/test1.py
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.399632 bslz4_to_sparse-0.0.6/
+-rw-r--r--   0 wright    (2427) id11      (1611)     1067 2023-03-06 21:46:52.000000 bslz4_to_sparse-0.0.6/LICENSE
+-rw-r--r--   0 wright    (2427) id11      (1611)      142 2023-03-13 13:21:39.000000 bslz4_to_sparse-0.0.6/MANIFEST.in
+-rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-06 11:59:19.397646 bslz4_to_sparse-0.0.6/PKG-INFO
+-rw-r--r--   0 wright    (2427) id11      (1611)      226 2023-03-07 11:25:12.000000 bslz4_to_sparse-0.0.6/README.md
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.257643 bslz4_to_sparse-0.0.6/bitshuffle/
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.324650 bslz4_to_sparse-0.0.6/bitshuffle/src/
+-rw-r--r--   0 wright    (2427) id11      (1611)    65340 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     4533 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.h
+-rw-r--r--   0 wright    (2427) id11      (1611)     2233 2023-03-12 06:15:25.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_internals.h
+-rw-r--r--   0 wright    (2427) id11      (1611)     2483 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     2616 2023-03-06 21:36:40.000000 bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.h
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.349668 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/
+-rw-r--r--   0 wright    (2427) id11      (1611)      464 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/PKG-INFO
+-rw-r--r--   0 wright    (2427) id11      (1611)      737 2023-05-06 11:59:19.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/SOURCES.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)        1 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/dependency_links.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)       11 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/requires.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)       16 2023-05-06 11:59:18.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparse.egg-info/top_level.txt
+-rw-r--r--   0 wright    (2427) id11      (1611)    28422 2023-04-21 14:28:51.000000 bslz4_to_sparse-0.0.6/bslz4_to_sparsemodule.c
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.261647 bslz4_to_sparse-0.0.6/lz4/
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.362660 bslz4_to_sparse-0.0.6/lz4/lib/
+-rw-r--r--   0 wright    (2427) id11      (1611)   114204 2023-03-12 06:07:55.000000 bslz4_to_sparse-0.0.6/lz4/lib/lz4.c
+-rw-r--r--   0 wright    (2427) id11      (1611)    44421 2023-03-12 06:07:57.000000 bslz4_to_sparse-0.0.6/lz4/lib/lz4.h
+-rw-r--r--   0 wright    (2427) id11      (1611)      118 2023-03-07 07:34:45.000000 bslz4_to_sparse-0.0.6/pyproject.toml
+-rw-r--r--   0 wright    (2427) id11      (1611)       38 2023-05-06 11:59:19.400632 bslz4_to_sparse-0.0.6/setup.cfg
+-rw-r--r--   0 wright    (2427) id11      (1611)     2780 2023-05-06 11:57:53.000000 bslz4_to_sparse-0.0.6/setup.py
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.385629 bslz4_to_sparse-0.0.6/src/
+-rw-r--r--   0 wright    (2427) id11      (1611)     3390 2023-05-06 11:58:03.000000 bslz4_to_sparse-0.0.6/src/__init__.py
+-rw-r--r--   0 wright    (2427) id11      (1611)     3842 2023-03-17 14:19:19.000000 bslz4_to_sparse-0.0.6/src/bshuf.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     1337 2023-03-17 13:49:45.000000 bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.c
+-rw-r--r--   0 wright    (2427) id11      (1611)     1548 2023-03-17 13:49:47.000000 bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.pyf
+drwxr-xr-x   0 wright    (2427) id11      (1611)        0 2023-05-06 11:59:19.391650 bslz4_to_sparse-0.0.6/test/
+-rw-r--r--   0 wright    (2427) id11      (1611)     4249 2023-03-27 14:17:12.000000 bslz4_to_sparse-0.0.6/test/test1.py
```

### Comparing `bslz4_to_sparse-0.0.5/LICENSE` & `bslz4_to_sparse-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_core.c` & `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_core.h` & `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_core.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bitshuffle/src/bitshuffle_internals.h` & `bslz4_to_sparse-0.0.6/bitshuffle/src/bitshuffle_internals.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bitshuffle/src/iochain.c` & `bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bitshuffle/src/iochain.h` & `bslz4_to_sparse-0.0.6/bitshuffle/src/iochain.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/bslz4_to_sparsemodule.c` & `bslz4_to_sparse-0.0.6/bslz4_to_sparsemodule.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /* File: bslz4_to_sparsemodule.c
  * This file is auto-generated with f2py (version:2).
  * f2py is a Fortran to Python Interface Generator (FPIG), Second Edition,
  * written by Pearu Peterson <pearu@cens.ioc.ee>.
- * Generation date: Sun Mar 26 08:06:13 2023
+ * Generation date: Fri Apr 21 14:28:50 2023
  * Do not edit this file directly unless you know what you are doing!!!
  */
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
@@ -235,35 +235,39 @@
   static char *capi_kwlist[] = {"cmp","msk","out","outP","thresh",NULL};
 
 /*routdebugenter*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_clock();
 #endif
   if (!PyArg_ParseTupleAndKeywords(capi_args,capi_keywds,\
-    "OOOOO:bslz4_to_sparse.bslz4_uint8_t",\
+    "OOOOO|:bslz4_to_sparse.bslz4_uint8_t",\
     capi_kwlist,&cmp_capi,&msk_capi,&out_capi,&outP_capi,&thresh_capi))
     return NULL;
 /*frompyobj*/
   /* Processing variable cmp */
   ;
   capi_cmp_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_cmp_tmp = array_from_pyobj(NPY_UBYTE,cmp_Dims,cmp_Rank,capi_cmp_intent,cmp_capi);
   if (capi_cmp_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     cmp = (unsigned_char *)(PyArray_DATA(capi_cmp_tmp));
 
   /* Processing variable msk */
   ;
   capi_msk_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_msk_tmp = array_from_pyobj(NPY_UBYTE,msk_Dims,msk_Rank,capi_msk_intent,msk_capi);
   if (capi_msk_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     msk = (unsigned_char *)(PyArray_DATA(capi_msk_tmp));
 
   /* Processing variable thresh */
     f2py_success = int_from_pyobj(&thresh,thresh_capi,"bslz4_to_sparse.bslz4_uint8_t() 5th argument (thresh) can't be converted to int");
   if (f2py_success) {
   /* Processing variable cmpN */
@@ -273,26 +277,30 @@
   NIJ = len(msk);
   CHECKSCALAR(len(msk)>=NIJ,"len(msk)>=NIJ","hidden NIJ","bslz4_uint8_t:NIJ=%d",NIJ) {
   /* Processing variable out */
   out_Dims[0]=NIJ;
   capi_out_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_out_tmp = array_from_pyobj(NPY_UBYTE,out_Dims,out_Rank,capi_out_intent,out_capi);
   if (capi_out_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     out = (unsigned_char *)(PyArray_DATA(capi_out_tmp));
 
   /* Processing variable outP */
   outP_Dims[0]=NIJ;
   capi_outP_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_outP_tmp = array_from_pyobj(NPY_UINT,outP_Dims,outP_Rank,capi_outP_intent,outP_capi);
   if (capi_outP_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint8_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     outP = (unsigned *)(PyArray_DATA(capi_outP_tmp));
 
 /*end of frompyobj*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_call_clock();
 #endif
@@ -404,35 +412,39 @@
   static char *capi_kwlist[] = {"cmp","msk","out","outP","thresh",NULL};
 
 /*routdebugenter*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_clock();
 #endif
   if (!PyArg_ParseTupleAndKeywords(capi_args,capi_keywds,\
-    "OOOOO:bslz4_to_sparse.bslz4_uint16_t",\
+    "OOOOO|:bslz4_to_sparse.bslz4_uint16_t",\
     capi_kwlist,&cmp_capi,&msk_capi,&out_capi,&outP_capi,&thresh_capi))
     return NULL;
 /*frompyobj*/
   /* Processing variable cmp */
   ;
   capi_cmp_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_cmp_tmp = array_from_pyobj(NPY_UBYTE,cmp_Dims,cmp_Rank,capi_cmp_intent,cmp_capi);
   if (capi_cmp_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     cmp = (unsigned_char *)(PyArray_DATA(capi_cmp_tmp));
 
   /* Processing variable msk */
   ;
   capi_msk_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_msk_tmp = array_from_pyobj(NPY_UBYTE,msk_Dims,msk_Rank,capi_msk_intent,msk_capi);
   if (capi_msk_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     msk = (unsigned_char *)(PyArray_DATA(capi_msk_tmp));
 
   /* Processing variable thresh */
     f2py_success = int_from_pyobj(&thresh,thresh_capi,"bslz4_to_sparse.bslz4_uint16_t() 5th argument (thresh) can't be converted to int");
   if (f2py_success) {
   /* Processing variable cmpN */
@@ -442,26 +454,30 @@
   NIJ = len(msk);
   CHECKSCALAR(len(msk)>=NIJ,"len(msk)>=NIJ","hidden NIJ","bslz4_uint16_t:NIJ=%d",NIJ) {
   /* Processing variable out */
   out_Dims[0]=NIJ;
   capi_out_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_out_tmp = array_from_pyobj(NPY_USHORT,out_Dims,out_Rank,capi_out_intent,out_capi);
   if (capi_out_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     out = (unsigned_short *)(PyArray_DATA(capi_out_tmp));
 
   /* Processing variable outP */
   outP_Dims[0]=NIJ;
   capi_outP_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_outP_tmp = array_from_pyobj(NPY_UINT,outP_Dims,outP_Rank,capi_outP_intent,outP_capi);
   if (capi_outP_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint16_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     outP = (unsigned *)(PyArray_DATA(capi_outP_tmp));
 
 /*end of frompyobj*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_call_clock();
 #endif
@@ -573,35 +589,39 @@
   static char *capi_kwlist[] = {"cmp","msk","out","outP","thresh",NULL};
 
 /*routdebugenter*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_clock();
 #endif
   if (!PyArg_ParseTupleAndKeywords(capi_args,capi_keywds,\
-    "OOOOO:bslz4_to_sparse.bslz4_uint32_t",\
+    "OOOOO|:bslz4_to_sparse.bslz4_uint32_t",\
     capi_kwlist,&cmp_capi,&msk_capi,&out_capi,&outP_capi,&thresh_capi))
     return NULL;
 /*frompyobj*/
   /* Processing variable cmp */
   ;
   capi_cmp_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_cmp_tmp = array_from_pyobj(NPY_UBYTE,cmp_Dims,cmp_Rank,capi_cmp_intent,cmp_capi);
   if (capi_cmp_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 1st argument `cmp' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     cmp = (unsigned_char *)(PyArray_DATA(capi_cmp_tmp));
 
   /* Processing variable msk */
   ;
   capi_msk_intent |= F2PY_INTENT_IN|F2PY_INTENT_C;
   capi_msk_tmp = array_from_pyobj(NPY_UBYTE,msk_Dims,msk_Rank,capi_msk_intent,msk_capi);
   if (capi_msk_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 2nd argument `msk' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     msk = (unsigned_char *)(PyArray_DATA(capi_msk_tmp));
 
   /* Processing variable thresh */
     f2py_success = int_from_pyobj(&thresh,thresh_capi,"bslz4_to_sparse.bslz4_uint32_t() 5th argument (thresh) can't be converted to int");
   if (f2py_success) {
   /* Processing variable cmpN */
@@ -611,26 +631,30 @@
   NIJ = len(msk);
   CHECKSCALAR(len(msk)>=NIJ,"len(msk)>=NIJ","hidden NIJ","bslz4_uint32_t:NIJ=%d",NIJ) {
   /* Processing variable out */
   out_Dims[0]=NIJ;
   capi_out_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_out_tmp = array_from_pyobj(NPY_UINT,out_Dims,out_Rank,capi_out_intent,out_capi);
   if (capi_out_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 3rd argument `out' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     out = (unsigned *)(PyArray_DATA(capi_out_tmp));
 
   /* Processing variable outP */
   outP_Dims[0]=NIJ;
   capi_outP_intent |= F2PY_INTENT_INOUT|F2PY_INTENT_C;
   capi_outP_tmp = array_from_pyobj(NPY_UINT,outP_Dims,outP_Rank,capi_outP_intent,outP_capi);
   if (capi_outP_tmp == NULL) {
-    if (!PyErr_Occurred())
-      PyErr_SetString(bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    PyObject *exc, *val, *tb;
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_SetString(exc ? exc : bslz4_to_sparse_error,"failed in converting 4th argument `outP' of bslz4_to_sparse.bslz4_uint32_t to C/Fortran array" );
+    npy_PyErr_ChainExceptionsCause(exc, val, tb);
   } else {
     outP = (unsigned *)(PyArray_DATA(capi_outP_tmp));
 
 /*end of frompyobj*/
 #ifdef F2PY_REPORT_ATEXIT
 f2py_start_call_clock();
 #endif
@@ -712,62 +736,53 @@
 };
 
 static PyMethodDef f2py_module_methods[] = {
 
   {NULL,NULL}
 };
 
-#if PY_VERSION_HEX >= 0x03000000
 static struct PyModuleDef moduledef = {
   PyModuleDef_HEAD_INIT,
   "bslz4_to_sparse",
   NULL,
   -1,
   f2py_module_methods,
   NULL,
   NULL,
   NULL,
   NULL
 };
-#endif
 
-#if PY_VERSION_HEX >= 0x03000000
-#define RETVAL m
 PyMODINIT_FUNC PyInit_bslz4_to_sparse(void) {
-#else
-#define RETVAL
-PyMODINIT_FUNC initbslz4_to_sparse(void) {
-#endif
   int i;
   PyObject *m,*d, *s, *tmp;
-#if PY_VERSION_HEX >= 0x03000000
   m = bslz4_to_sparse_module = PyModule_Create(&moduledef);
-#else
-  m = bslz4_to_sparse_module = Py_InitModule("bslz4_to_sparse", f2py_module_methods);
-#endif
-  Py_TYPE(&PyFortran_Type) = &PyType_Type;
+  Py_SET_TYPE(&PyFortran_Type, &PyType_Type);
   import_array();
   if (PyErr_Occurred())
-    {PyErr_SetString(PyExc_ImportError, "can't initialize module bslz4_to_sparse (failed to import numpy)"); return RETVAL;}
+    {PyErr_SetString(PyExc_ImportError, "can't initialize module bslz4_to_sparse (failed to import numpy)"); return m;}
   d = PyModule_GetDict(m);
   s = PyString_FromString("$Revision: $");
   PyDict_SetItemString(d, "__version__", s);
-#if PY_VERSION_HEX >= 0x03000000
+  Py_DECREF(s);
   s = PyUnicode_FromString(
-#else
-  s = PyString_FromString(
-#endif
     "This module 'bslz4_to_sparse' is auto-generated with f2py (version:2).\nFunctions:\n"
 "  bslz4_uint8_t = bslz4_uint8_t(cmp,msk,out,outP,thresh)\n"
 "  bslz4_uint16_t = bslz4_uint16_t(cmp,msk,out,outP,thresh)\n"
 "  bslz4_uint32_t = bslz4_uint32_t(cmp,msk,out,outP,thresh)\n"
 ".");
   PyDict_SetItemString(d, "__doc__", s);
-  bslz4_to_sparse_error = PyErr_NewException ("bslz4_to_sparse.error", NULL, NULL);
   Py_DECREF(s);
+  bslz4_to_sparse_error = PyErr_NewException ("bslz4_to_sparse.error", NULL, NULL);
+  /*
+   * Store the error object inside the dict, so that it could get deallocated.
+   * (in practice, this is a module, so it likely will not and cannot.)
+   */
+  PyDict_SetItemString(d, "_bslz4_to_sparse_error", bslz4_to_sparse_error);
+  Py_DECREF(bslz4_to_sparse_error);
   for(i=0;f2py_routine_defs[i].name!=NULL;i++) {
     tmp = PyFortranObject_NewAsAttr(&f2py_routine_defs[i]);
     PyDict_SetItemString(d, f2py_routine_defs[i].name, tmp);
     Py_DECREF(tmp);
   }
 
 
@@ -778,13 +793,12 @@
 /*eof initcommonhooks*/
 
 
 #ifdef F2PY_REPORT_ATEXIT
   if (! PyErr_Occurred())
     on_exit(f2py_report_on_exit,(void*)"bslz4_to_sparse");
 #endif
-
-  return RETVAL;
+  return m;
 }
 #ifdef __cplusplus
 }
 #endif
```

### Comparing `bslz4_to_sparse-0.0.5/lz4/lib/lz4.c` & `bslz4_to_sparse-0.0.6/lz4/lib/lz4.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/lz4/lib/lz4.h` & `bslz4_to_sparse-0.0.6/lz4/lib/lz4.h`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/setup.py` & `bslz4_to_sparse-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
             if line.find('avx2')>=0:
                 flags.append('-mavx2')
                 break
 
 ext = Extension( "bslz4_to_sparse",
                  sources = ["src/bslz4_to_sparse.pyf",
                             "src/bslz4_to_sparse.c",
+                            "src/bshuf.c",
                             "lz4/lib/lz4.c",
                             "bitshuffle/src/bitshuffle_core.c",
                             "bitshuffle/src/iochain.c",  ],
                  include_dirs  = [ numpy.get_include(),
                                    numpy.f2py.get_include(), ],
                  extra_compile_args = flags + [ '-O3',
                                     '-DF2PY_REPORT_ON_ARRAY_COPY=1',
@@ -62,12 +63,12 @@
        ext_package = 'bslz4_to_sparse',
        ext_modules = [ext, ],
        cmdclass = { 'build_ext' : build_ext_subclass },
        install_requires = ["numpy", "h5py"],
        author = 'Jon Wright',
        author_email = 'wright@esrf.fr',
        url = "http://github.com/jonwright/bslz4_to_sparse",
-       version = '0.0.5',
+       version = '0.0.6',
        license = 'MIT',
        long_description = readme,
        long_description_content_type='text/markdown',
 )
```

### Comparing `bslz4_to_sparse-0.0.5/src/__init__.py` & `bslz4_to_sparse-0.0.6/src/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 
 import numpy as np
 import ctypes
 from .bslz4_to_sparse import bslz4_uint32_t, bslz4_uint16_t, bslz4_uint8_t
 
-version = '0.0.5'
+version = '0.0.6'
 
 # We cast away the 'read-only' nature of python bytes.
 # Not needed for the latest numpy.
 buffer_from_memory = ctypes.pythonapi.PyMemoryView_FromMemory
 buffer_from_memory.restype = ctypes.py_object
 buffer_from_memory.argtypes = (ctypes.c_void_p, ctypes.c_int, ctypes.c_int)
 
+def npbuf( buf ):
+    if isinstance( buf, np.ndarray ):
+        return buf
+    else:
+        return np.frombuffer( buffer_from_memory( buf, len(buf), 0x200), np.uint8 )
+
+
 class chunk2sparse:
     
     def __init__(self, mask, dtype = np.uint16):
         self.nfast = mask.shape[1]
         self.mask = mask.ravel()
         self.indices = np.empty(mask.size, np.uint32)
         self.values = np.empty(mask.size, dtype)
         self.fun = (None, 
                     bslz4_uint8_t, 
                     bslz4_uint16_t, 
                     None, 
                     bslz4_uint32_t)[ dtype.itemsize ]
         
     def __call__(self, buffer, cut):
-        npixels = self.fun(  np.frombuffer( 
-            buffer_from_memory( buffer, len(buffer), 0x200), np.uint8 ),
-            self.mask, self.values, self.indices, cut)
+        npixels = self.fun( npbuf(buffer),
+                self.mask, self.values, self.indices, cut)
         return npixels, (self.values, self.indices)
     
     def coo(self, buffer, cut):
         """Computes i,j indices and MAKES COPIES"""
         npixels, _ = self.__call__(buffer, cut)
         row = np.empty( npixels, np.uint16 )
         col = np.empty( npixels, np.uint16 )
@@ -65,23 +71,20 @@
     # todo : h5py malloc free version coming? see https://github.com/h5py/h5py/pull/2232
     filtinfo, buffer = ds.id.read_direct_chunk( (num, 0, 0) )
     #
     # h5py returns a bytes object that is read only. Older versions of numpy insist
     # to make a copy. We work around that using ctypes to set a writeable flag.
     #                                                      PyBUF_WRITE 0x200
     if ds.dtype == np.uint16:
-        npixels = bslz4_uint16_t(  np.frombuffer( 
-            buffer_from_memory( buffer, len(buffer), 0x200), np.uint8 ),
+        npixels = bslz4_uint16_t( npbuf(buffer),
             mask, values, indices, cut)
     elif ds.dtype == np.uint32:
-        npixels = bslz4_uint32_t(np.frombuffer( 
-            buffer_from_memory( buffer, len(buffer), 0x200), np.uint8 ),
+        npixels = bslz4_uint32_t( npbuf(buffer),
             mask, values, indices, cut)
     elif ds.dtype == np.uint8:
-        npixels = bslz4_uint8_t(  np.frombuffer( 
-            buffer_from_memory( buffer, len(buffer), 0x200), np.uint8 ),
+        npixels = bslz4_uint8_t( npbuf(buffer),
             mask, values, indices, cut)
     else:
         raise Exception("no decoder for your type")
     if npixels < 0:
         raise Exception("Error decoding: %d"%(npixels))
     return npixels, (values, indices)
```

### Comparing `bslz4_to_sparse-0.0.5/src/bslz4_to_sparse.c` & `bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.c`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/src/bslz4_to_sparse.pyf` & `bslz4_to_sparse-0.0.6/src/bslz4_to_sparse.pyf`

 * *Files identical despite different names*

### Comparing `bslz4_to_sparse-0.0.5/test/test1.py` & `bslz4_to_sparse-0.0.6/test/test1.py`

 * *Files identical despite different names*

