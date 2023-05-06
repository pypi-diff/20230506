# Comparing `tmp/dumpulator-0.2.3.tar.gz` & `tmp/dumpulator-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumpulator-0.2.3.tar", last modified: Sat Apr  8 07:58:07 2023, max compression
+gzip compressed data, was "dumpulator-0.2.4.tar", last modified: Sat May  6 15:05:59 2023, max compression
```

## Comparing `dumpulator-0.2.3.tar` & `dumpulator-0.2.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.747960 dumpulator-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-04-08 07:58:07.000000 dumpulator-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-04-08 07:58:07.747960 dumpulator-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-08 07:58:07.000000 dumpulator-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-08 07:58:07.000000 dumpulator-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-08 07:58:07.747960 dumpulator-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-04-08 07:58:07.000000 dumpulator-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.739960 dumpulator-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.743960 dumpulator-0.2.3/src/dumpulator/
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19646 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/details.py
--rw-r--r--   0 runner    (1001) docker     (122)    75244 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/dumpulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/handles.py
--rw-r--r--   0 runner    (1001) docker     (122)    16474 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/memory.py
--rw-r--r--   0 runner    (1001) docker     (122)     5328 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)    21593 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/native.py
--rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/ntdevices.py
--rw-r--r--   0 runner    (1001) docker     (122)   123193 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/ntenums.py
--rw-r--r--   0 runner    (1001) docker     (122)    12534 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/ntprimitives.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/ntstructs.py
--rw-r--r--   0 runner    (1001) docker     (122)   235727 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator/ntsyscalls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.743960 dumpulator-0.2.3/src/dumpulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/dumpulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.743960 dumpulator-0.2.3/src/minidump/
--rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/__amain__.py
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     9689 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/aminidumpfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    11501 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/aminidumpreader.py
--rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/common_structs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/directory.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/header.py
--rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/minidumpfile.py
--rw-r--r--   0 runner    (1001) docker     (122)    11724 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/minidumpreader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/minidumpshell.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.747960 dumpulator-0.2.3/src/minidump/streams/
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/CommentStreamA.py
--rw-r--r--   0 runner    (1001) docker     (122)      627 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/CommentStreamW.py
--rw-r--r--   0 runner    (1001) docker     (122)    25274 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ContextStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    11428 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ExceptionStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/FunctionTableStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8898 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/HandleDataStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/HandleOperationListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/JavaScriptDataStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      549 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/LastReservedStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/Memory64ListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    12532 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/MemoryInfoListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/MemoryListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/MiscInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ModuleListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ProcessVmCountersStream.py
--rw-r--r--   0 runner    (1001) docker     (122)    14530 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/SystemInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       94 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/SystemMemoryInfoStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ThreadExListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6506 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ThreadInfoListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/ThreadListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/TokenStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/UnloadedModuleListStream.py
--rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.747960 dumpulator-0.2.3/src/minidump/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/createminidump.py
--rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/privileges.py
--rw-r--r--   0 runner    (1001) docker     (122)     7333 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/privileges_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.747960 dumpulator-0.2.3/src/minidump/utils/winapi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/winapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/winapi/defines.py
--rw-r--r--   0 runner    (1001) docker     (122)     6286 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/winapi/kernel32.py
--rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/winapi/psapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/utils/winapi/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/win_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     9188 2023-04-08 07:58:07.000000 dumpulator-0.2.3/src/minidump/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (122)     1359 2023-05-06 15:05:58.000000 dumpulator-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-05-06 15:05:59.511441 dumpulator-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-05-06 15:05:58.000000 dumpulator-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-05-06 15:05:58.000000 dumpulator-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-05-06 15:05:59.515442 dumpulator-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-06 15:05:58.000000 dumpulator-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.499441 dumpulator-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.503441 dumpulator-0.2.4/src/dumpulator/
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21634 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/details.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79009 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/dumpulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10865 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/handles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16598 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/memory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5442 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21591 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/native.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3924 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntdevices.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123193 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntenums.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13633 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntprimitives.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntstructs.py
+-rw-r--r--   0 runner    (1001) docker     (122)   235727 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/dumpulator/ntsyscalls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.503441 dumpulator-0.2.4/src/dumpulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10452 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-06 15:05:59.000000 dumpulator-0.2.4/src/dumpulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.507441 dumpulator-0.2.4/src/minidump/
+-rw-r--r--   0 runner    (1001) docker     (122)     3269 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__amain__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9689 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/aminidumpfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11501 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/aminidumpreader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9452 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/common_structs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2349 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/directory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9818 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11724 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpreader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5238 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/minidumpshell.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/streams/
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/CommentStreamA.py
+-rw-r--r--   0 runner    (1001) docker     (122)      627 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/CommentStreamW.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25274 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ContextStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11428 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ExceptionStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/FunctionTableStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8898 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/HandleDataStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/HandleOperationListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/JavaScriptDataStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      549 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/LastReservedStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3211 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/Memory64ListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12503 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MemoryInfoListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3252 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MemoryListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6684 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/MiscInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8440 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ModuleListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ProcessVmCountersStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14530 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/SystemInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       94 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/SystemMemoryInfoStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2834 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadExListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6506 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadInfoListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3308 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/ThreadListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/TokenStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4906 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/UnloadedModuleListStream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3153 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/createminidump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/privileges.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7333 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/privileges_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:59.511441 dumpulator-0.2.4/src/minidump/utils/winapi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/defines.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6286 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/kernel32.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2398 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/psapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/utils/winapi/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6137 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/win_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9188 2023-05-06 15:05:58.000000 dumpulator-0.2.4/src/minidump/writer.py
```

### Comparing `dumpulator-0.2.3/LICENSE` & `dumpulator-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/PKG-INFO` & `dumpulator-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpulator
-Version: 0.2.3
+Version: 0.2.4
 Summary: An easy-to-use library for emulating code in minidump files.
 Home-page: https://github.com/mrexodia/dumpulator
 Author: Duncan Ogilvie
 Author-email: dumpulator@mrexodia.re
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mrexodia/dumpulator/issues
 Platform: UNKNOWN
```

### Comparing `dumpulator-0.2.3/README.md` & `dumpulator-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/setup.cfg` & `dumpulator-0.2.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dumpulator
-version = v0.2.3
+version = v0.2.4
 author = Duncan Ogilvie
 author_email = dumpulator@mrexodia.re
 description = An easy-to-use library for emulating code in minidump files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mrexodia/dumpulator
 project_urls =
```

### Comparing `dumpulator-0.2.3/setup.py` & `dumpulator-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator/details.py` & `dumpulator-0.2.4/src/dumpulator/details.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import struct
 from collections import namedtuple
-from typing import List
+from typing import List, Dict, Optional, Iterable
 
 from unicorn import *
 from unicorn.x86_const import *
 
 from dumpulator.memory import MemoryProtect, PageManager
 
 def map_unicorn_perms(protect: MemoryProtect):
@@ -379,14 +379,75 @@
     def __contains__(self, name: str):
         try:
             self._resolve_reg(name)
             return True
         except Exception:
             return False
 
+    @property
+    def volatile(self):
+        if self._x64:
+            return ["rax", "rcx", "rdx", "r8", "r9", "r10", "r11"]
+        else:
+            return ["eax", "ecx", "edx"]
+
+    @property
+    def nonvolatile(self):
+        if self._x64:
+            return ["rbx", "rbp", "rsp", "rsi", "rdi",
+                    "r12", "r13", "r14", "r15"]
+        else:
+            return ["ebx", "ebp", "esp", "esi", "edi"]
+
+    @property
+    def gp(self):
+        if self._x64:
+            return ["rax", "rbx", "rcx", "rdx", "rbp", "rsp", "rsi", "rdi",
+                    "r8", "r9", "r10", "r11", "r12", "r13", "r14", "r15"]
+        else:
+            return ["eax", "ebx", "ecx", "edx", "ebp", "esp", "esi", "edi"]
+
+    @property
+    def integer(self):
+        if self._x64:
+            return ["rax", "rbx", "rcx", "rdx", "rbp", "rsi", "rdi",
+                    "r8", "r9", "r10", "r11", "r12", "r13", "r14", "r15"]
+        else:
+            return ["eax", "ebx", "ecx", "edx", "ebp", "esi", "edi"]
+
+    @property
+    def control(self):
+        if self._x64:
+            return ["rip", "rsp", "rflags"]
+        else:
+            return ["eip", "esp", "eflags"]
+
+    @property
+    def debug(self):
+        return ["dr0", "dr1", "dr2", "dr6", "dr7"]
+
+    @property
+    def fpu(self):
+        if self._x64:
+            return [f"ymm{i}" for i in range(16)]
+        else:
+            return [f"ymm{i}" for i in range(8)]
+
+    def save(self, regs: Optional[Iterable[str]] = None):
+        if regs is None:
+            if self._x64:
+                regs = self.gp + ["rip", "rflags"]
+            else:
+                regs = self.gp + ["eip", "eflags"]
+        return { reg: self[reg] for reg in regs}
+
+    def load(self, regs: Dict[str, int]):
+        for reg, value in regs.items():
+            self[reg] = value
+
 
 class Arguments:
     def __init__(self, uc: Uc, memory: PageManager, regs: Registers, x64):
         self._uc = uc
         self._memory = memory
         self._regs = regs
         self._x64 = x64
@@ -580,10 +641,13 @@
     for row in table:
         if len(result) > 0:
             result += "\n"
         line = ""
         for index, col in enumerate(row):
             if index > 0:
                 line += " "
-            line += f"{col:>{lengths[index]}}"
+            if index + 1 == len(row):
+                line += col
+            else:
+                line += f"{col:>{lengths[index]}}"
         result += line.rstrip()
     return result
```

### Comparing `dumpulator-0.2.3/src/dumpulator/dumpulator.py` & `dumpulator-0.2.4/src/dumpulator/dumpulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -299,14 +299,22 @@
         self._uc = Uc(UC_ARCH_X86, UC_MODE_64)
 
         # TODO: multiple cs instances per segment
         mode = CS_MODE_64 if self._x64 else CS_MODE_32
         self.cs = Cs(CS_ARCH_X86, mode)
         self.cs.detail = True
 
+        # Workaround for buggy implementation of https://github.com/unicorn-engine/unicorn/pull/1746
+        def __ctl_w(ctl, nr):
+            return ctl | (nr << 26) | (UC_CTL_IO_WRITE << 30)
+        try:
+            self._uc.ctl(__ctl_w(12, 1), 1)
+        except UcError:
+            pass
+
         self.regs = Registers(self._uc, self._x64)
         self._pages = LazyPageManager(UnicornPageManager(self._uc))
         self.memory = MemoryManager(self._pages)
         self.args = Arguments(self._uc, self._pages, self.regs, self._x64)
         self.modules = ModuleManager(self.memory)
         self._allocate_base = None
         self._allocate_size = 1024 * 1024 * 10  # NOTE: 10 megs
@@ -787,43 +795,55 @@
     def _setup_modules(self):
         minidump_module: minidump.MinidumpModule
         for minidump_module in self._minidump.modules.modules:
             base = minidump_module.baseaddress
             size = minidump_module.size
             path = minidump_module.name
 
-            # Parse the header to dump the sections from memory
-            header = self.read(base, PAGE_SIZE)
-            pe = PE(data=header, fast_load=True)
-            image_size = pe.OPTIONAL_HEADER.SizeOfImage
-            section_alignment = pe.OPTIONAL_HEADER.SectionAlignment
-            mapped_data = bytearray(header)
-            mapped_data += b"\0" * (image_size - len(header))
-            for section in pe.sections:
-                name = section.Name.rstrip(b"\0").decode()
-                mask = section_alignment - 1
-                rva = (section.VirtualAddress + mask) & ~mask
-                size = self.memory.align_page(section.Misc_VirtualSize)
-                va = base + rva
-                for page in range(va, va + size, PAGE_SIZE):
-                    region = self.memory.find_commit(page)
-                    if region is not None:
-                        region.info = name
-                try:
-                    data = self.read(va, size)
-                    mapped_data[rva:size] = data
-                except IndexError:
-                    self.error(f"Failed to read section {name} from module {path}")
-            # Load the PE dumped from memory
-            pe = PE(data=mapped_data, fast_load=True)
-            # Hack to adjust pefile to accept in-memory modules
-            for section in pe.sections:
-                # Potentially interesting members: Misc_PhysicalAddress, Misc_VirtualSize, SizeOfRawData
-                section.PointerToRawData = section.VirtualAddress
-                section.PointerToRawData_adj = section.VirtualAddress
+            # Read as much data from the module memory as possible
+            try:
+                mapped_data = self.read(base, size)
+            except IndexError:
+                # HACK: modules with holes between sections need to be read in chunks
+                mapped_data = bytearray(size)
+                ptr = base
+                while ptr < base + size:
+                    region = self.memory.query(ptr)
+                    if region.state == MemoryState.MEM_COMMIT:
+                        data = self.read(region.base, region.region_size)
+                        index = region.base - base
+                        mapped_data[index:index + len(data)] = data
+                    ptr += region.region_size
+                assert len(mapped_data) == size
+
+            try:
+                # Load the PE dumped from memory
+                pe = PE(data=mapped_data, fast_load=True)
+                section_alignment = pe.OPTIONAL_HEADER.SectionAlignment
+                for section in pe.sections:
+                    # Set the section in the memory region
+                    name = section.Name.rstrip(b"\0").decode(encoding="ascii", errors="backslashreplace")
+                    mask = section_alignment - 1
+                    index = (section.VirtualAddress + mask) & ~mask
+                    section_size = self.memory.align_page(section.Misc_VirtualSize)
+                    va = base + index
+                    for page in range(va, va + section_size, PAGE_SIZE):
+                        region = self.memory.find_commit(page)
+                        if region is not None:
+                            region.info = name
+                    # HACK: adjust pefile to accept in-memory modules
+                    # Potentially interesting members: Misc_PhysicalAddress, Misc_VirtualSize, SizeOfRawData
+                    section.PointerToRawData = section.VirtualAddress
+                    section.PointerToRawData_adj = section.VirtualAddress
+            except pefile.PEFormatError as e:
+                self.error(f"Failed to parse module {hex(base)}[{hex(size)}]: {path}")
+
+            # Do not trust these values from memory
+            pe.OPTIONAL_HEADER.ImageBase = base
+            pe.OPTIONAL_HEADER.SizeOfImage = size
             self.modules.add(pe, path)
 
     def _setup_syscalls(self):
         # Load the ntdll module from memory
         ntdll = self.modules["ntdll.dll"]
         self.KiUserExceptionDispatcher = ntdll.find_export("KiUserExceptionDispatcher").address
         self.LdrLoadDll = ntdll.find_export("LdrLoadDll").address
@@ -877,15 +897,15 @@
         if not isinstance(addr, int):
             addr = int(addr)
         return self._pages.read(addr, size)
 
     def write(self, addr, data):
         if not isinstance(addr, int):
             addr = int(addr)
-        self._pages.write(addr, data)
+        self._pages.write(addr, bytes(data))
 
     def call(self, addr, args: List[int] = None, regs: dict = None, count=0):
         if args is None:
             args = []
         if regs is None:
             regs = {}
 
@@ -1511,14 +1531,16 @@
         if arg.type is OBJECT_ATTRIBUTES:
             tstr = _object_attributes_to_string(dp, arg)
         elif arg.type is UNICODE_STRING:
             tstr = f"\"{_unicode_string_to_string(dp, arg)}\""
         if tstr is not None:
             str += f" /* {tstr} */"
         return str
+    elif isinstance(arg, Int):
+        return arg.__str__()
     elif isinstance(arg, int):
         return hex(arg)
     raise NotImplemented()
 
 def _arg_type_string(arg):
     if P.is_ptr(arg) and arg.type is not None:
         return arg.type.__name__ + "*"
@@ -1657,46 +1679,122 @@
                 dp.sequence_id += 1
         else:
             raise dp.raise_kill(NotImplementedError(f"{table_prefix}syscall {hex(service_number)} -> {name} not implemented!")) from None
     else:
         raise dp.raise_kill(IndexError(f"{table_prefix}syscall {hex(service_number)} (index: {hex(function_index)}) out of range")) from None
 
 def _emulate_unsupported_instruction(dp: Dumpulator, instr: CsInsn):
-    if instr.id == X86_INS_RDRAND:
-        op: X86Op = instr.operands[0]
-        regname = instr.reg_name(op.reg)
-        if dp.x64 and op.size * 8 == 32:
-            regname = "r" + regname[1:]
-        print(f"emulated rdrand {regname}:{op.size * 8}, cip = {hex(instr.address)}+{instr.size}")
-        dp.regs[regname] = 42  # TODO: PRNG based on dmp hash
+    # Get address mask
+    if dp.regs.cs == windows_user_segment.cs:
+        address_mask = 0xFFFFFFFFFFFFFFFF
+    else:
+        address_mask = 0xFFFFFFFF
+
+    def op_mem(op: X86Op, *, aligned: bool):
+        mem_address = 0
+        if op.mem.base == X86_REG_RIP:
+            mem_address += instr.address + instr.size
+            raise NotImplementedError("TODO: check if the disp is already adjusted")
+        else:
+            base = op.mem.base
+            if base != X86_REG_INVALID:
+                name = instr.reg_name(base)
+                value = dp.regs[name]
+                mem_address += value
+
+            index = op.mem.index
+            if index != X86_REG_INVALID:
+                name = instr.reg_name(index)
+                value = dp.regs[name]
+                mem_address += value * op.mem.scale
+
+        disp = op.mem.disp # TODO: negative value handling?
+        mem_address += disp
+        mem_address &= address_mask
+        if aligned:
+            alignment = op.size
+            if mem_address & (alignment - 1) != 0:
+                assert False, f"Address {hex(mem_address)} not aligned to {alignment}"
+        return mem_address
+
+    def op_read(index: int, *, aligned=False):
+        op: X86Op = instr.operands[index]
+        if op.type == CS_OP_REG:
+            name = instr.reg_name(op.value.reg)
+            return dp.regs[name]
+        elif op.type == CS_OP_MEM:
+            mem_address = op_mem(op, aligned=aligned)
+            data = dp.read(mem_address, op.size)
+            return int.from_bytes(data, "little")
+        elif op.type == CS_OP_IMM:
+            # TODO: sign extend?
+            return op.value.imm
+        else:
+            raise NotImplementedError()
+
+    def op_write(index: int, value: int, *, aligned=False):
+        op: X86Op = instr.operands[index]
+        size = op.size
+        if op.type == CS_OP_REG:
+            name = instr.reg_name(op.value.reg)
+            if size == 4 and address_mask == 0xFFFFFFFFFFFFFFFF:
+                # Extend the register
+                assert name[0] == "e"
+                name = "r" + name[1:]
+            dp.regs[name] = value
+        elif op.type == CS_OP_MEM:
+            mem_address = op_mem(op, aligned=aligned)
+            data = value.to_bytes(size, "little")
+            # TODO: handle invalid memory access
+            dp.write(mem_address, data)
+        else:
+            raise NotImplementedError()
+
+    def cip_next():
         dp.regs.cip += instr.size
+
+    if instr.id == X86_INS_RDRAND:
+        # TODO: PRNG based on dmp hash
+        op_write(0, 42)
+        cip_next()
+    elif instr.id == X86_INS_VMOVDQU:
+        src = op_read(1)
+        op_write(0, src)
+        cip_next()
+    elif instr.id in [X86_INS_VMOVDQA, X86_INS_MOVNTDQ]:
+        src = op_read(1, aligned=True)
+        op_write(0, src, aligned=True)
+        cip_next()
     else:
+        dp.error(f"unsupported: {instr.mnemonic} {instr.op_str}")
         # Unsupported instruction
         return False
+    dp.debug(f"emulated: {hex(instr.address)}|{instr.bytes.hex()}|{instr.mnemonic} {instr.op_str}")
     # Resume execution
     return True
 
 def _hook_invalid(uc: Uc, dp: Dumpulator):
     address = dp.regs.cip
     if dp.trace:
         dp.trace.flush()
     # HACK: unicorn cannot gracefully exit in all contexts
     if dp.stopped:
         dp.error(f"terminating emulation...")
         return False
-    dp.error(f"invalid instruction at {hex(address)}")
     try:
         code = dp.read(address, 15)
         instr = next(dp.cs.disasm(code, address, 1))
+        # TODO: add a hook
         if _emulate_unsupported_instruction(dp, instr):
             # Resume execution with a context switch
             assert dp._exception.type == ExceptionType.NoException
             exception = UnicornExceptionInfo()
             exception.type = ExceptionType.ContextSwitch
             exception.final = True
             dp._exception = exception
             return False  # NOTE: returning True would stop emulation
     except StopIteration:
         pass  # Unsupported instruction
     except IndexError:
         pass  # Invalid memory access (NOTE: this should not be possible actually)
+    dp.error(f"invalid instruction at {hex(address)}")
     raise NotImplementedError("TODO: throw invalid instruction exception")
```

### Comparing `dumpulator-0.2.3/src/dumpulator/handles.py` & `dumpulator-0.2.4/src/dumpulator/handles.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator/memory.py` & `dumpulator-0.2.4/src/dumpulator/memory.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,7 +408,10 @@
                 if commit is not None and commit.info is None:
                     commit.info = info
         else:
             if region.info is not None:
                 return False
             region.info = info
         return True
+
+    def __repr__(self):
+        return f"MemoryManager(regions={len(self._regions)}, committed={len(self._committed)})"
```

### Comparing `dumpulator-0.2.3/src/dumpulator/modules.py` & `dumpulator-0.2.4/src/dumpulator/modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             index = self._exports_by_name.get(key)
             if index is None:
                 return None
             return self.exports[index]
         raise TypeError()
 
     def __repr__(self):
-        return f"Module({hex(self.base)}, {hex(self.size)}, {repr(self.path)})"
+        return f"Module({hex(self.base)}, {hex(self.size)}, {self.path})"
 
     def __hash__(self):
         return hash((self.base, self.size, self.path))
 
     def __contains__(self, addr: int):
         return self.base <= addr < self.base + self.size
 
@@ -133,7 +133,10 @@
 
     def __contains__(self, key: Union[str, int]):
         return self.find(key) is not None
 
     def __iter__(self):
         for base in self._modules:
             yield self._modules[base]
+
+    def __repr__(self) -> str:
+        return f"ModuleManager(main={hex(self.main)}, modules={len(self._modules)})"
```

### Comparing `dumpulator-0.2.3/src/dumpulator/native.py` & `dumpulator-0.2.4/src/dumpulator/native.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,15 +456,14 @@
         assert regs.ss == self.SegSs & 0xFFFF
         assert regs.ds == self.SegDs & 0xFFFF
         assert regs.es == self.SegEs & 0xFFFF
         assert regs.fs == self.SegFs & 0xFFFF
         assert regs.gs == self.SegGs & 0xFFFF
 
         # TODO: implement xmm
-
 assert ctypes.sizeof(WOW64_CONTEXT) == 0x2cc
 
 class EXCEPTION_RECORD32(ctypes.Structure):
     _pack_ = 8
     _fields_ = [
         ("ExceptionCode", ctypes.c_int32),
         ("ExceptionFlags", ctypes.c_uint32),
```

### Comparing `dumpulator-0.2.3/src/dumpulator/ntdevices.py` & `dumpulator-0.2.4/src/dumpulator/ntdevices.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator/ntenums.py` & `dumpulator-0.2.4/src/dumpulator/ntenums.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator/ntprimitives.py` & `dumpulator-0.2.4/src/dumpulator/ntprimitives.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
     def read(self, size: int) -> bytes:
         return self.arch.read(self.ptr, size)
 
     def write(self, data: Union[SupportsBytes, bytes]):
         self.arch.write(self.ptr, data)
 
-    def __getitem__(self, index) -> T:
+    def __getitem__(self, index: int) -> T:
         ptype = self.type
         if ptype is None:
             raise TypeError(f"No type associated with pointer")
 
         if P.is_ptr(ptype):
             ptr = self.ptr + index * self.arch.ptr_size()
             return ptype(self.arch, self.arch.read_ptr(ptr))
@@ -133,14 +133,35 @@
             else:
                 ctype = Struct.translate_ctype(self.arch.ptr_type(), ptype)
                 size = ctypes.sizeof(ctype)
                 data = self.arch.read(ptr, size)
                 value = ctype.from_buffer(data)
                 return ptype(value)
 
+    def __setitem__(self, index: int, value: T):
+        ptype = self.type
+        if ptype is None:
+            raise TypeError(f"No type associated with pointer")
+        if P.is_ptr(ptype):
+            ptr = self.ptr + index * self.arch.ptr_size()
+            self.arch.write_ptr(ptr, int(value))
+        else:
+            size = Struct.sizeof(ptype, self.arch)
+            ptr = self.ptr + index * size
+            if issubclass(ptype, Struct):
+                if isinstance(value, ptype):
+                    raise TypeError(f"Expected {ptype}, got {type(value)}")
+                self.arch.write(ptr, value)
+            else:
+                # TODO: support bool/enum?
+                if not isinstance(value, int):
+                    raise TypeError(f"Expected int, got {type(value)}")
+                ctype = Struct.translate_ctype(self.arch.ptr_type(), ptype)
+                self.arch.write(ptr, ctype(int(value)))
+
     def deref(self) -> T:
         return self[0]
 
     def __int__(self):
         return self.ptr
 
     def __eq__(self, other):
@@ -388,14 +409,17 @@
 
 class KAFFINITY(ULONG_PTR):
     pass
 
 class KPRIORITY(ULONG_PTR):
     pass
 
+class KIRQL(UCHAR):
+    pass
+
 # TODO: should probably be bool
 class BOOLEAN(BYTE):
     pass
 
 class LOGICAL(ULONG):
     pass
 
@@ -404,19 +428,28 @@
 
 class PSID(PVOID):
     pass
 
 class PWSTR(PVOID):
     pass
 
+class CCHAR(CHAR):
+    pass
+
+class CSHORT(SHORT):
+    pass
+
+class CLONG(ULONG):
+    pass
+
 # Some unsupported enum
 class LATENCY_TIME(Enum):
     LT_DONT_CARE = 0
     LT_LOWEST_LATENCY = 1
 
 @dataclass
 class SAL:
     annotation: str
     comment: str = ""
 
     def __str__(self):
-        return self.annotation
+        return self.annotation.split(" ")[0]
```

### Comparing `dumpulator-0.2.3/src/dumpulator/ntstructs.py` & `dumpulator-0.2.4/src/dumpulator/ntstructs.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator/ntsyscalls.py` & `dumpulator-0.2.4/src/dumpulator/ntsyscalls.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/dumpulator.egg-info/PKG-INFO` & `dumpulator-0.2.4/src/dumpulator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumpulator
-Version: 0.2.3
+Version: 0.2.4
 Summary: An easy-to-use library for emulating code in minidump files.
 Home-page: https://github.com/mrexodia/dumpulator
 Author: Duncan Ogilvie
 Author-email: dumpulator@mrexodia.re
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/mrexodia/dumpulator/issues
 Platform: UNKNOWN
```

### Comparing `dumpulator-0.2.3/src/dumpulator.egg-info/SOURCES.txt` & `dumpulator-0.2.4/src/dumpulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/__amain__.py` & `dumpulator-0.2.4/src/minidump/__amain__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/__main__.py` & `dumpulator-0.2.4/src/minidump/__main__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/aminidumpfile.py` & `dumpulator-0.2.4/src/minidump/aminidumpfile.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/aminidumpreader.py` & `dumpulator-0.2.4/src/minidump/aminidumpreader.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/common_structs.py` & `dumpulator-0.2.4/src/minidump/common_structs.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/constants.py` & `dumpulator-0.2.4/src/minidump/constants.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/directory.py` & `dumpulator-0.2.4/src/minidump/directory.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/header.py` & `dumpulator-0.2.4/src/minidump/header.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/minidumpfile.py` & `dumpulator-0.2.4/src/minidump/minidumpfile.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/minidumpreader.py` & `dumpulator-0.2.4/src/minidump/minidumpreader.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/minidumpshell.py` & `dumpulator-0.2.4/src/minidump/minidumpshell.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/CommentStreamA.py` & `dumpulator-0.2.4/src/minidump/streams/CommentStreamA.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/CommentStreamW.py` & `dumpulator-0.2.4/src/minidump/streams/CommentStreamW.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ContextStream.py` & `dumpulator-0.2.4/src/minidump/streams/ContextStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ExceptionStream.py` & `dumpulator-0.2.4/src/minidump/streams/ExceptionStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/FunctionTableStream.py` & `dumpulator-0.2.4/src/minidump/streams/FunctionTableStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/HandleDataStream.py` & `dumpulator-0.2.4/src/minidump/streams/HandleDataStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/HandleOperationListStream.py` & `dumpulator-0.2.4/src/minidump/streams/HandleOperationListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/LastReservedStream.py` & `dumpulator-0.2.4/src/minidump/streams/LastReservedStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/Memory64ListStream.py` & `dumpulator-0.2.4/src/minidump/streams/Memory64ListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/MemoryInfoListStream.py` & `dumpulator-0.2.4/src/minidump/streams/MemoryInfoListStream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python3
 #
 # Author:
 #  Tamas Jos (@skelsec)
 #
 import io
 import enum
-from minidump.common_structs import * 
+from minidump.common_structs import *
 
-class AllocationProtect(enum.Enum):
+class AllocationProtect(enum.Flag):
 	NONE = 0
 	PAGE_EXECUTE = 0x10 #Enables execute access to the committed region of pages. An attempt to write to the committed region results in an access violation.
 						#This flag is not supported by the CreateFileMapping function.
 
 	PAGE_EXECUTE_READ = 0x20 #Enables execute or read-only access to the committed region of pages. An attempt to write to the committed region results in an access violation.
 							 #Windows Server 2003 and Windows XP:  This attribute is not supported by the CreateFileMapping function until Windows XP with SP2 and Windows Server 2003 with SP1.
 
@@ -47,15 +47,15 @@
 	#The PAGE_NOCACHE flag cannot be used with the PAGE_GUARD, PAGE_NOACCESS, or PAGE_WRITECOMBINE flags.
 	#The PAGE_NOCACHE flag can be used only when allocating private memory with the VirtualAlloc, VirtualAllocEx, or VirtualAllocExNuma functions. To enable non-cached memory access for shared memory, specify the SEC_NOCACHE flag when calling the CreateFileMapping function.
 	PAGE_WRITECOMBINE = 0x400 #Sets all pages to be write-combined.
 	#Applications should not use this attribute except when explicitly required for a device. Using the interlocked functions with memory that is mapped as write-combined can result in an EXCEPTION_ILLEGAL_INSTRUCTION exception.
 	#The PAGE_WRITECOMBINE flag cannot be specified with the PAGE_NOACCESS, PAGE_GUARD, and PAGE_NOCACHE flags.
 	#The PAGE_WRITECOMBINE flag can be used only when allocating private memory with the VirtualAlloc, VirtualAllocEx, or VirtualAllocExNuma functions. To enable write-combined memory access for shared memory, specify the SEC_WRITECOMBINE flag when calling the CreateFileMapping function.
 	#Windows Server 2003 and Windows XP:  This flag is not supported until Windows Server 2003 with SP1.
-	
+
 class MemoryType(enum.Enum):
 	MEM_IMAGE = 0x1000000 #Indicates that the memory pages within the region are mapped into the view of an image section.
 	MEM_MAPPED = 0x40000 #Indicates that the memory pages within the region are mapped into the view of a section.
 	MEM_PRIVATE = 0x20000 #Indicates that the memory pages within the region are private (that is, not shared by other processes).
 class MemoryState(enum.Enum):
 	MEM_COMMIT = 0x1000 #Indicates committed pages for which physical storage has been allocated, either in memory or in the paging file on disk.
 	MEM_FREE = 0x10000 #Indicates free pages not accessible to the calling process and available to be allocated. For free pages, the information in the AllocationBase, AllocationProtect, Protect, and Type members is undefined.
@@ -74,25 +74,25 @@
 		return self.SizeOfHeader + len(self.entries)*MINIDUMP_MEMORY_INFO().get_size()
 
 	def to_bytes(self):
 		t  = self.SizeOfHeader.to_bytes(4, byteorder = 'little', signed = False)
 		t += self.SizeOfEntry.to_bytes(4, byteorder = 'little', signed = False)
 		t += len(self.entries).to_bytes(8, byteorder = 'little', signed = False)
 		return t
-	
+
 	@staticmethod
 	def parse(buff):
 		mhds = MINIDUMP_MEMORY_INFO_LIST()
 		mhds.SizeOfHeader = int.from_bytes(buff.read(4), byteorder = 'little', signed = False)
 		mhds.SizeOfEntry = int.from_bytes(buff.read(4), byteorder = 'little', signed = False)
 		mhds.NumberOfEntries = int.from_bytes(buff.read(8), byteorder = 'little', signed = False)
-			
+
 		return mhds
-		
-# https://msdn.microsoft.com/en-us/library/windows/desktop/ms680386(v=vs.85).aspx	
+
+# https://msdn.microsoft.com/en-us/library/windows/desktop/ms680386(v=vs.85).aspx
 class MINIDUMP_MEMORY_INFO:
 	def __init__(self):
 		self.BaseAddress = None
 		self.AllocationBase = None
 		self.AllocationProtect = None
 		self.__alignment1 = 0
 		self.RegionSize = None
@@ -117,15 +117,15 @@
 		t += self.__alignment1.to_bytes(4, byteorder = 'little', signed = False)
 		t += self.RegionSize.to_bytes(8, byteorder = 'little', signed = False)
 		t += self.State.value.to_bytes(4, byteorder = 'little', signed = False)
 		t += self.Protect.value.to_bytes(4, byteorder = 'little', signed = False)
 		t += self.Type.value.to_bytes(4, byteorder = 'little', signed = False)
 		t += self.__alignment2.to_bytes(4, byteorder = 'little', signed = False)
 		return t
-	
+
 	@staticmethod
 	def parse(buff):
 		mmi = MINIDUMP_MEMORY_INFO()
 		mmi.BaseAddress = int.from_bytes(buff.read(8), byteorder = 'little', signed = False)
 		mmi.AllocationBase = int.from_bytes(buff.read(8), byteorder = 'little', signed = False)
 		mmi.AllocationProtect = int.from_bytes(buff.read(4), byteorder = 'little', signed = False)
 		mmi.__alignment1 = int.from_bytes(buff.read(4), byteorder = 'little', signed = False)
@@ -139,39 +139,39 @@
 		except:
 			pass
 		try:
 			mmi.Type = MemoryType(int.from_bytes(buff.read(4), byteorder = 'little', signed = False))
 		except:
 			pass
 		mmi.__alignment2 = int.from_bytes(buff.read(4), byteorder = 'little', signed = False)
-			
+
 		return mmi
-		
+
 class MinidumpMemoryInfo:
 	def __init__(self):
 		self.BaseAddress = None
 		self.AllocationBase = None
 		self.AllocationProtect = None
 		self.RegionSize = None
 		self.State = None
 		self.Protect = None
 		self.Type = None
-	
+
 	@staticmethod
 	def parse(t, buff):
 		mmi = MinidumpMemoryInfo()
 		mmi.BaseAddress = t.BaseAddress
 		mmi.AllocationBase = t.AllocationBase
 		mmi.AllocationProtect = t.AllocationProtect
 		mmi.RegionSize = t.RegionSize
 		mmi.State = t.State
 		mmi.Protect = t.Protect
 		mmi.Type = t.Type
 		return mmi
-	
+
 	@staticmethod
 	def get_header():
 		t = [
 			'BaseAddress',
 			'AllocationBase',
 			'AllocationProtect',
 			'RegionSize',
@@ -188,49 +188,49 @@
 			str(self.AllocationProtect),
 			hex(self.RegionSize),
 			self.State.name if self.State else 'N/A',
 			self.Protect.name if self.Protect else 'N/A',
 			self.Type.name if self.Type else 'N/A',
 		]
 		return t
-		
-		
+
+
 class MinidumpMemoryInfoList:
 	def __init__(self):
 		self.header = None
 		self.infos = []
-	
+
 	@staticmethod
 	def parse(dir, buff):
 		t = MinidumpMemoryInfoList()
 		buff.seek(dir.Location.Rva)
 		data = buff.read(dir.Location.DataSize)
 		chunk = io.BytesIO(data)
 		t.header = MINIDUMP_MEMORY_INFO_LIST.parse(chunk)
 		for _ in range(t.header.NumberOfEntries):
 			mi = MINIDUMP_MEMORY_INFO.parse(chunk)
 			t.infos.append(MinidumpMemoryInfo.parse(mi, buff))
-		
+
 		return t
 
 	@staticmethod
 	async def aparse(dir, buff):
 		t = MinidumpMemoryInfoList()
 		await buff.seek(dir.Location.Rva)
 		data = await buff.read(dir.Location.DataSize)
 		chunk = io.BytesIO(data)
 		t.header = MINIDUMP_MEMORY_INFO_LIST.parse(chunk)
 		for _ in range(t.header.NumberOfEntries):
 			mi = MINIDUMP_MEMORY_INFO.parse(chunk)
 			t.infos.append(MinidumpMemoryInfo.parse(mi, None))
-		
+
 		return t
-		
+
 	def to_table(self):
 		t = []
 		t.append(MinidumpMemoryInfo.get_header())
 		for info in self.infos:
 			t.append(info.to_row())
 		return t
-	
+
 	def __str__(self):
 		return '== MinidumpMemoryInfoList ==\n' + construct_table(self.to_table())
```

### Comparing `dumpulator-0.2.3/src/minidump/streams/MemoryListStream.py` & `dumpulator-0.2.4/src/minidump/streams/MemoryListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/MiscInfoStream.py` & `dumpulator-0.2.4/src/minidump/streams/MiscInfoStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ModuleListStream.py` & `dumpulator-0.2.4/src/minidump/streams/ModuleListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/SystemInfoStream.py` & `dumpulator-0.2.4/src/minidump/streams/SystemInfoStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ThreadExListStream.py` & `dumpulator-0.2.4/src/minidump/streams/ThreadExListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ThreadInfoListStream.py` & `dumpulator-0.2.4/src/minidump/streams/ThreadInfoListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/ThreadListStream.py` & `dumpulator-0.2.4/src/minidump/streams/ThreadListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/UnloadedModuleListStream.py` & `dumpulator-0.2.4/src/minidump/streams/UnloadedModuleListStream.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/streams/__init__.py` & `dumpulator-0.2.4/src/minidump/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/createminidump.py` & `dumpulator-0.2.4/src/minidump/utils/createminidump.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/privileges.py` & `dumpulator-0.2.4/src/minidump/utils/privileges.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/privileges_types.py` & `dumpulator-0.2.4/src/minidump/utils/privileges_types.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/winapi/defines.py` & `dumpulator-0.2.4/src/minidump/utils/winapi/defines.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/winapi/kernel32.py` & `dumpulator-0.2.4/src/minidump/utils/winapi/kernel32.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/winapi/psapi.py` & `dumpulator-0.2.4/src/minidump/utils/winapi/psapi.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/utils/winapi/version.py` & `dumpulator-0.2.4/src/minidump/utils/winapi/version.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/win_datatypes.py` & `dumpulator-0.2.4/src/minidump/win_datatypes.py`

 * *Files identical despite different names*

### Comparing `dumpulator-0.2.3/src/minidump/writer.py` & `dumpulator-0.2.4/src/minidump/writer.py`

 * *Files identical despite different names*

