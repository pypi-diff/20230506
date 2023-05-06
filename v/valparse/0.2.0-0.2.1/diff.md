# Comparing `tmp/valparse-0.2.0.tar.gz` & `tmp/valparse-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valparse-0.2.0.tar", last modified: Mon May  1 20:52:52 2023, max compression
+gzip compressed data, was "valparse-0.2.1.tar", last modified: Sat May  6 02:16:05 2023, max compression
```

## Comparing `valparse-0.2.0.tar` & `valparse-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-01 20:52:52.879322 valparse-0.2.0/
--rw-r--r--   0 talzuss    (501) staff       (20)     1809 2023-05-01 20:31:28.000000 valparse-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 talzuss    (501) staff       (20)     1068 2023-04-22 01:04:57.000000 valparse-0.2.0/LICENSE
--rw-r--r--   0 talzuss    (501) staff       (20)      368 2023-04-22 05:17:45.000000 valparse-0.2.0/MANIFEST.in
--rw-r--r--   0 talzuss    (501) staff       (20)     2003 2023-04-22 05:06:58.000000 valparse-0.2.0/Makefile
--rw-r--r--   0 talzuss    (501) staff       (20)     5079 2023-05-01 20:52:52.879193 valparse-0.2.0/PKG-INFO
--rw-r--r--   0 talzuss    (501) staff       (20)     3437 2023-05-01 20:31:28.000000 valparse-0.2.0/README.md
--rw-r--r--   0 talzuss    (501) staff       (20)     1571 2023-05-01 20:47:59.000000 valparse-0.2.0/pyproject.toml
--rw-r--r--   0 talzuss    (501) staff       (20)       38 2023-05-01 20:52:52.879361 valparse-0.2.0/setup.cfg
--rw-r--r--   0 talzuss    (501) staff       (20)      331 2023-05-01 20:47:59.000000 valparse-0.2.0/setup.py
-drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-01 20:52:52.877807 valparse-0.2.0/valparse/
--rw-r--r--   0 talzuss    (501) staff       (20)       67 2023-05-01 20:47:59.000000 valparse-0.2.0/valparse/__init__.py
-drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-01 20:52:52.878559 valparse-0.2.0/valparse/tests/
-drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-01 20:52:52.879006 valparse-0.2.0/valparse/tests/data/
--rw-r--r--   0 talzuss    (501) staff       (20)       10 2023-04-22 05:42:39.000000 valparse-0.2.0/valparse/tests/data/.gitignore
--rw-r--r--   0 talzuss    (501) staff       (20)     3491 2023-04-22 04:29:07.000000 valparse-0.2.0/valparse/tests/data/bad-test.xml
--rw-r--r--   0 talzuss    (501) staff       (20)       61 2023-04-22 05:42:15.000000 valparse-0.2.0/valparse/tests/data/bad.supp
--rw-r--r--   0 talzuss    (501) staff       (20)       61 2023-05-01 20:38:35.000000 valparse-0.2.0/valparse/tests/data/test.supp
--rw-r--r--   0 talzuss    (501) staff       (20)     2331 2023-05-01 20:47:59.000000 valparse-0.2.0/valparse/tests/test_parser.py
--rw-r--r--   0 talzuss    (501) staff       (20)     4656 2023-05-01 20:47:59.000000 valparse-0.2.0/valparse/tests/test_vgerror.py
--rw-r--r--   0 talzuss    (501) staff       (20)      510 2023-05-01 20:37:46.000000 valparse-0.2.0/valparse/util.py
--rw-r--r--   0 talzuss    (501) staff       (20)    14961 2023-05-01 20:47:59.000000 valparse-0.2.0/valparse/valparse.py
-drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-01 20:52:52.878334 valparse-0.2.0/valparse.egg-info/
--rw-r--r--   0 talzuss    (501) staff       (20)     5079 2023-05-01 20:52:52.000000 valparse-0.2.0/valparse.egg-info/PKG-INFO
--rw-r--r--   0 talzuss    (501) staff       (20)      480 2023-05-01 20:52:52.000000 valparse-0.2.0/valparse.egg-info/SOURCES.txt
--rw-r--r--   0 talzuss    (501) staff       (20)        1 2023-05-01 20:52:52.000000 valparse-0.2.0/valparse.egg-info/dependency_links.txt
--rw-r--r--   0 talzuss    (501) staff       (20)      156 2023-05-01 20:52:52.000000 valparse-0.2.0/valparse.egg-info/requires.txt
--rw-r--r--   0 talzuss    (501) staff       (20)        9 2023-05-01 20:52:52.000000 valparse-0.2.0/valparse.egg-info/top_level.txt
+drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-06 02:16:05.147711 valparse-0.2.1/
+-rw-r--r--   0 talzuss    (501) staff       (20)     1809 2023-05-01 20:31:28.000000 valparse-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 talzuss    (501) staff       (20)     1068 2023-04-22 01:04:57.000000 valparse-0.2.1/LICENSE
+-rw-r--r--   0 talzuss    (501) staff       (20)      368 2023-04-22 05:17:45.000000 valparse-0.2.1/MANIFEST.in
+-rw-r--r--   0 talzuss    (501) staff       (20)     2003 2023-04-22 05:06:58.000000 valparse-0.2.1/Makefile
+-rw-r--r--   0 talzuss    (501) staff       (20)     5392 2023-05-06 02:16:05.147577 valparse-0.2.1/PKG-INFO
+-rw-r--r--   0 talzuss    (501) staff       (20)     3828 2023-05-04 04:37:46.000000 valparse-0.2.1/README.md
+-rw-r--r--   0 talzuss    (501) staff       (20)     1571 2023-05-06 02:11:46.000000 valparse-0.2.1/pyproject.toml
+-rw-r--r--   0 talzuss    (501) staff       (20)       38 2023-05-06 02:16:05.147751 valparse-0.2.1/setup.cfg
+-rw-r--r--   0 talzuss    (501) staff       (20)       38 2023-05-06 01:49:57.000000 valparse-0.2.1/setup.py
+drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-06 02:16:05.146005 valparse-0.2.1/valparse/
+-rw-r--r--   0 talzuss    (501) staff       (20)       67 2023-05-06 02:11:46.000000 valparse-0.2.1/valparse/__init__.py
+drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-06 02:16:05.146893 valparse-0.2.1/valparse/tests/
+drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-06 02:16:05.147392 valparse-0.2.1/valparse/tests/data/
+-rw-r--r--   0 talzuss    (501) staff       (20)       10 2023-04-22 05:42:39.000000 valparse-0.2.1/valparse/tests/data/.gitignore
+-rw-r--r--   0 talzuss    (501) staff       (20)     3491 2023-04-22 04:29:07.000000 valparse-0.2.1/valparse/tests/data/bad-test.xml
+-rw-r--r--   0 talzuss    (501) staff       (20)       61 2023-04-22 05:42:15.000000 valparse-0.2.1/valparse/tests/data/bad.supp
+-rw-r--r--   0 talzuss    (501) staff       (20)       61 2023-05-06 01:51:00.000000 valparse-0.2.1/valparse/tests/data/test.supp
+-rw-r--r--   0 talzuss    (501) staff       (20)     3478 2023-05-06 01:49:57.000000 valparse-0.2.1/valparse/tests/test_parser.py
+-rw-r--r--   0 talzuss    (501) staff       (20)     6530 2023-05-06 01:49:57.000000 valparse-0.2.1/valparse/tests/test_vgerror.py
+-rw-r--r--   0 talzuss    (501) staff       (20)     1385 2023-05-04 04:29:11.000000 valparse-0.2.1/valparse/util.py
+-rw-r--r--   0 talzuss    (501) staff       (20)    19208 2023-05-06 01:59:23.000000 valparse-0.2.1/valparse/valparse.py
+drwxr-xr-x   0 talzuss    (501) staff       (20)        0 2023-05-06 02:16:05.146628 valparse-0.2.1/valparse.egg-info/
+-rw-r--r--   0 talzuss    (501) staff       (20)     5392 2023-05-06 02:16:05.000000 valparse-0.2.1/valparse.egg-info/PKG-INFO
+-rw-r--r--   0 talzuss    (501) staff       (20)      480 2023-05-06 02:16:05.000000 valparse-0.2.1/valparse.egg-info/SOURCES.txt
+-rw-r--r--   0 talzuss    (501) staff       (20)        1 2023-05-06 02:16:05.000000 valparse-0.2.1/valparse.egg-info/dependency_links.txt
+-rw-r--r--   0 talzuss    (501) staff       (20)      156 2023-05-06 02:16:05.000000 valparse-0.2.1/valparse.egg-info/requires.txt
+-rw-r--r--   0 talzuss    (501) staff       (20)        9 2023-05-06 02:16:05.000000 valparse-0.2.1/valparse.egg-info/top_level.txt
```

### Comparing `valparse-0.2.0/CONTRIBUTING.md` & `valparse-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `valparse-0.2.0/LICENSE` & `valparse-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valparse-0.2.0/Makefile` & `valparse-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `valparse-0.2.0/PKG-INFO` & `valparse-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: valparse
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package to parse Valgrind XML files.
-Home-page: https://github.com/tzussman/valparse
-Author: valparse contributors
 Author-email: Tal Zussman <tz2294@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Tal Zussman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,18 +29,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # *valparse,* a parser for Valgrind-generated XML files
 
+[![PyPI](https://img.shields.io/pypi/v/valparse)](https://pypi.org/project/valparse/)
 [![License](https://img.shields.io/github/license/tzussman/valparse)](https://github.com/tzussman/valparse)
 ![GitHub issues](https://img.shields.io/github/issues/tzussman/valparse)
 [![Build Status](https://github.com/tzussman/valparse/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/tzussman/valparse/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/tzussman/valparse/branch/main/graph/badge.svg)](https://codecov.io/gh/tzussman/valparse)
+[![Docs](https://img.shields.io/badge/-docs-blueviolet)](https://tzussman.github.io/valparse)
 
 *valparse* supports protocol version 4 with [*Memcheck*][memcheck] only, but can
 be easily modified to support [*Helgrind*][helgrind] and other protocol tools.
 
 [memcheck]: https://valgrind.org/docs/manual/mc-manual.html
 [helgrind]: https://valgrind.org/docs/manual/hg-manual.html
 
@@ -69,14 +69,26 @@
 ```
 
 Some examples of `.xml` files generated by Valgrind are included in the
 `/examples` directory.
 
 Valgrind does not support XML output for fd leaks as of version 3.18.1.
 
+## Usage
+
+Below is an example of basic `valparse` usage:
+
+```py
+import valparse
+
+xml_file = valparse.Parser('./test.xml')
+if xml_file.hasLeaks() or xml_file.hasErrors():
+    print("Leaks or errors found!")
+```
+
 ## Features
 
 -   Error generation for nonexistent/incorrectly formatted TOPLEVEL tags
 
 -   Error generation for nonexistent/incorrectly formatted PROTOCOL tags
 
 -   Basic Valgrind output parsing
```

### Comparing `valparse-0.2.0/README.md` & `valparse-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # *valparse,* a parser for Valgrind-generated XML files
 
+[![PyPI](https://img.shields.io/pypi/v/valparse)](https://pypi.org/project/valparse/)
 [![License](https://img.shields.io/github/license/tzussman/valparse)](https://github.com/tzussman/valparse)
 ![GitHub issues](https://img.shields.io/github/issues/tzussman/valparse)
 [![Build Status](https://github.com/tzussman/valparse/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/tzussman/valparse/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/tzussman/valparse/branch/main/graph/badge.svg)](https://codecov.io/gh/tzussman/valparse)
+[![Docs](https://img.shields.io/badge/-docs-blueviolet)](https://tzussman.github.io/valparse)
 
 *valparse* supports protocol version 4 with [*Memcheck*][memcheck] only, but can
 be easily modified to support [*Helgrind*][helgrind] and other protocol tools.
 
 [memcheck]: https://valgrind.org/docs/manual/mc-manual.html
 [helgrind]: https://valgrind.org/docs/manual/hg-manual.html
 
@@ -34,14 +36,26 @@
 ```
 
 Some examples of `.xml` files generated by Valgrind are included in the
 `/examples` directory.
 
 Valgrind does not support XML output for fd leaks as of version 3.18.1.
 
+## Usage
+
+Below is an example of basic `valparse` usage:
+
+```py
+import valparse
+
+xml_file = valparse.Parser('./test.xml')
+if xml_file.hasLeaks() or xml_file.hasErrors():
+    print("Leaks or errors found!")
+```
+
 ## Features
 
 -   Error generation for nonexistent/incorrectly formatted TOPLEVEL tags
 
 -   Error generation for nonexistent/incorrectly formatted PROTOCOL tags
 
 -   Basic Valgrind output parsing
```

### Comparing `valparse-0.2.0/pyproject.toml` & `valparse-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "valparse"
 authors = [{name = "Tal Zussman", email = "tz2294@columbia.edu"}]
 description="Package to parse Valgrind XML files."
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = []
 
 [project.license]
 file = "LICENSE"
```

### Comparing `valparse-0.2.0/valparse/tests/data/bad-test.xml` & `valparse-0.2.1/valparse/tests/data/bad-test.xml`

 * *Files identical despite different names*

### Comparing `valparse-0.2.0/valparse/tests/test_vgerror.py` & `valparse-0.2.1/valparse/tests/test_vgerror.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,63 +12,119 @@
         stack=[
             valparse.Frame(
                 ip="0x108706",
                 obj="/home/valparse/examples/invalid_read",
                 fn="main",
                 dir="/home/valparse/examples/",
                 file="invalid_read.c",
-                line="50",
+                line=50,
             ),
         ],
     )
 
     assert vgerr.kind == valparse.ValgrindErrorKind.INVALID_READ
     assert vgerr.msg == "Invalid read of size 4"
     assert vgerr.msg_secondary == "Address 0x4 is 4 bytes inside a block of size 8 free'd"
     assert len(vgerr.stack) == 1
 
     assert vgerr.isLeak() is False
     assert vgerr.isError() is True
 
+    vgerr_str = '''Error kind: InvalidRead
+Error message: Invalid read of size 4
+Stack:
+  Instruction Pointer: 0x108706
+  Object: /home/valparse/examples/invalid_read
+  Function: main
+  Directory: /home/valparse/examples/
+  File: invalid_read.c
+  Line: 50
+'''
+    assert str(vgerr) == vgerr_str
+
 
 def test_ValgrindError_leak():
     """Create an instance of a ValgrindError with a leak and check its fields."""
     vgerr = valparse.ValgrindError(
         kind=valparse.ValgrindErrorKind("Leak_DefinitelyLost"),
         msg="Test message",
         stack=[
             valparse.Frame(
                 ip="0x108706",
                 obj="/home/valparse/examples/fake_file",
                 fn="main",
                 dir="/home/valparse/examples/",
                 file="fake_file.c",
-                line="50",
+                line=50,
             ),
         ],
     )
 
     assert vgerr.kind == valparse.ValgrindErrorKind.LEAK_DEFINITELY_LOST
     assert vgerr.msg == "Test message"
     assert len(vgerr.stack) == 1
 
     assert vgerr.isLeak() is True
     assert vgerr.isError() is False
 
+    vgerr_str = '''Leak kind: Leak_DefinitelyLost
+Leak message: Test message
+Stack:
+  Instruction Pointer: 0x108706
+  Object: /home/valparse/examples/fake_file
+  Function: main
+  Directory: /home/valparse/examples/
+  File: fake_file.c
+  Line: 50
+'''
+    assert str(vgerr) == vgerr_str
+
+
+def test_Arguments():
+    """Create an instance of Arguments and check its fields."""
+    args = valparse.Arguments(
+        valexe="/usr/bin/valgrind.bin",
+        valargs=["--leak-check=full", "--xml=yes", "--xml-file=fake-test.xml"],
+        exe="./fake_file",
+        exeargs=["arg1", "arg2"],
+    )
+
+    assert args.valexe == "/usr/bin/valgrind.bin"
+    assert args.valargs == ["--leak-check=full", "--xml=yes", "--xml-file=fake-test.xml"]
+    assert args.exe == "./fake_file"
+    assert args.exeargs == ["arg1", "arg2"]
+
+    args_str = '''Valgrind executable: /usr/bin/valgrind.bin
+Valgrind args: --leak-check=full --xml=yes --xml-file=fake-test.xml
+Executable: ./fake_file
+Args: arg1 arg2'''
+
+    assert str(args) == args_str
+
+
+def test_Status():
+    """Create an instance of Status and check its fields."""
+    stat = valparse.Status(start="00:00:00:00.047", end="00:00:00:00.694")
+
+    assert stat.start == "00:00:00:00.047"
+    assert stat.end == "00:00:00:00.694"
+
+    assert str(stat) == "Start time: 00:00:00:00.047\nEnd time: 00:00:00:00.694\n"
+
 
 def test_SFrame():
     """Create an instance of a SFrame and check its fields."""
     sframe = valparse.SFrame(
-        obj="0x4",
+        obj="test",
         fun="main",
     )
 
-    assert sframe.obj == "0x4"
+    assert sframe.obj == "test"
     assert sframe.fun == "main"
-    assert str(sframe) == "  Object: 0x4\n  Function: main\n"
+    assert str(sframe) == "  Object: test\n  Function: main\n"
 
 
 def test_FatalSignal():
     """Create an instance of a FatalSignal and check its fields."""
     sig = valparse.FatalSignal(
         tid=5,
         signo=11,
@@ -78,61 +134,64 @@
         stack=[
             valparse.Frame(
                 ip="0x108706",
                 obj="/home/valparse/examples/invalid_read",
                 fn="main",
                 dir="/home/valparse/examples/",
                 file="invalid_read.c",
-                line="50",
+                line=50,
             ),
         ],
+        threadname="test_thread",
     )
 
     assert sig.tid == 5
     assert sig.signo == 11
     assert sig.signame == "SIGSEGV"
     assert sig.sicode == 1
     assert sig.siaddr == "0x0"
     assert len(sig.stack) == 1
+    assert sig.threadname == "test_thread"
 
     assert sig.get_signal() == signal.SIGSEGV
     sig_str = '''Thread ID: 5
 Signal number: 11
 Name: SIGSEGV
 Code: 1
 Address: 0x0
 Stack:
   Instruction Pointer: 0x108706
   Object: /home/valparse/examples/invalid_read
   Function: main
   Directory: /home/valparse/examples/
   File: invalid_read.c
   Line: 50
+Thread name: test_thread
 '''
 
     assert str(sig) == sig_str
 
 
 def test_Frame():
     """Create an instance of a Frame and check its fields."""
     frame = valparse.Frame(
         ip="0x108706",
         obj="/home/valparse/examples/invalid_read",
         fn="main",
         dir="/home/valparse/examples/",
         file="invalid_read.c",
-        line="50",
+        line=50,
     )
 
     assert frame.ip == "0x108706"
     assert frame.obj == "/home/valparse/examples/invalid_read"
     assert frame.fn == "main"
     assert frame.dir == "/home/valparse/examples/"
     assert frame.file == "invalid_read.c"
-    assert frame.line == "50"
+    assert frame.line == 50
 
     frame_str = '''  Instruction Pointer: 0x108706
   Object: /home/valparse/examples/invalid_read
   Function: main
   Directory: /home/valparse/examples/
   File: invalid_read.c
   Line: 50
@@ -158,20 +217,24 @@
 
 
 def test_Suppression():
     """Create an instance of a Suppression and check its fields."""
     supp = valparse.Suppression(
         name="test_supp",
         kind="Memcheck:Value8",
-        stack=[valparse.SFrame(fun="main")],
+        stack=[valparse.SFrame(fun="main", obj="test")],
+        auxkind="Test suppression",
     )
 
     assert supp.name == "test_supp"
     assert supp.kind == "Memcheck:Value8"
     assert len(supp.stack) == 1
+    assert supp.auxkind == "Test suppression"
 
     supp_str = '''Suppression kind: Memcheck:Value8
 Stack frame:
+  Object: test
   Function: main
+Aux kind: Test suppression
 '''
 
     assert str(supp) == supp_str
```

### Comparing `valparse-0.2.0/valparse/valparse.py` & `valparse-0.2.1/valparse/valparse.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 # Constants
 
 _SUPPORTED_VERSIONS = ['4']
 _SUPPORTED_TOOLS = ['memcheck']  # 'helgrind', 'drd', 'exp-ptrcheck'
 
 
 class ValgrindErrorKind(Enum):
+    """Enum representing Valgrind error types"""
+
     UNINIT_VALUE = 'UninitValue'
     UNINIT_CONDITION = 'UninitCondition'
     CORE_MEM_ERROR = 'CoreMemError'
     INVALID_READ = 'InvalidRead'
     INVALID_WRITE = 'InvalidWrite'
     INVALID_JUMP = 'InvalidJump'
     SYSCALL_PARAM = 'SyscallParam'
@@ -66,15 +68,35 @@
     ValgrindErrorKind.LEAK_POSSIBLY_LOST,
     ValgrindErrorKind.LEAK_STILL_REACHABLE,
 ]
 
 
 @dataclass
 class Arguments:
-    """Class to keep track of Valgrind arguments"""
+    """Class to keep track of Valgrind arguments
+
+    Parameters
+    ----------
+    valexe: str
+        Executable corresponding to the Valgrind tool
+
+    valargs: List[str]
+        Arguments passed to Valgrind
+
+    exe: str
+        Executable corresponding to the program being tested
+
+    exeargs: List[str]
+        Arguments passed to the program being tested
+
+    Raises
+    ------
+    ValgrindFormatError
+        If the <args> block does not meet Valgrind protocol specifications
+    """
 
     valexe: str
     valargs: List[str]
     exe: str
     exeargs: List[str]
 
     @classmethod
@@ -115,15 +137,29 @@
                 result += " " + exearg
 
         return result
 
 
 @dataclass
 class Status:
-    """Class to keep track of start and end time"""
+    """Class to keep track of start and end times of Valgrind run
+
+    Parameters
+    ----------
+    start: str
+        Start time of Valgrind run
+
+    end: str
+        End time of Valgrind run
+
+    Raises
+    ------
+    ValgrindFormatError
+        If the <status> block does not meet Valgrind protocol specifications
+    """
 
     start: str
     end: str
 
     @classmethod
     def from_xml_elements(cls, el: List[ET.Element]) -> 'Status':
         """Takes in list of <status> blocks"""
@@ -148,14 +184,37 @@
         result += "End time" + value(self.end)
 
         return result
 
 
 @dataclass
 class Frame:
+    """Class to keep track of Valgrind stack frame
+
+    Parameters
+    ----------
+    ip: str
+        Instruction pointer
+
+    obj: Optional[str]
+        Object name
+
+    fn: Optional[str]
+        Function name
+
+    dir: Optional[str]
+        Directory name
+
+    file: Optional[str]
+        File name
+
+    line: Optional[int]
+        Line number
+    """
+
     ip: str  # instruction pointer
     obj: Optional[str] = None
     fn: Optional[str] = None
     dir: Optional[str] = None
     file: Optional[str] = None
     line: Optional[int] = None
 
@@ -190,14 +249,25 @@
             result += indent("Line") + value(self.line)
 
         return result
 
 
 @dataclass
 class SFrame:
+    """Class to keep track of Valgrind suppression frame
+
+    Parameters
+    ----------
+    obj: Optional[str]
+        Object name
+
+    fun: Optional[str]
+        Function name
+    """
+
     obj: Optional[str] = None
     fun: Optional[str] = None
 
     @classmethod
     def from_xml_element(cls, el: ET.Element) -> 'SFrame':
         fields = {field: elem_find_text(el, field) for field in ['obj', 'fun']}
         return cls(**fields)
@@ -218,14 +288,44 @@
             result += indent("Function") + value(self.fun)
 
         return result
 
 
 @dataclass
 class ValgrindError:
+    """Class to keep track of Valgrind error
+
+    Parameters
+    ----------
+    kind: ValgrindErrorKind
+        Kind of Valgrind error
+
+    msg: str
+        Error message
+
+    stack: List[Frame]
+        Stack trace
+
+    msg_secondary: Optional[str]
+        Secondary error message
+
+    bytes_leaked: Optional[int]
+        Number of bytes leaked
+
+    blocks_leaked: Optional[int]
+        Number of blocks leaked
+
+    Methods
+    -------
+    isLeak() -> bool
+        Returns True if error is a leak, False otherwise
+    isError() -> bool
+        Returns True if error is an error, False otherwise
+    """
+
     kind: ValgrindErrorKind
     msg: str
     stack: List[Frame]
     msg_secondary: Optional[str] = None
     bytes_leaked: Optional[int] = None
     blocks_leaked: Optional[int] = None
 
@@ -267,14 +367,25 @@
             result += f"Stack:\n{frame.__str__()}"
 
         return result
 
 
 @dataclass
 class SuppCount:
+    """Class to keep track of Valgrind suppression count
+
+    Parameters
+    ----------
+    count: int
+        Number of times suppression was applied
+
+    name: str
+        Name of suppression
+    """
+
     count: int
     name: str
 
     @classmethod
     def from_xml_element(cls, el: ET.Element) -> 'SuppCount':
         count = elem_find_int(el, 'count')
         name = elem_find_text(el, 'name')
@@ -288,14 +399,36 @@
         result += "Name" + value(self.name)
 
         return result
 
 
 @dataclass
 class Suppression:
+    """Class to keep track of Valgrind suppression
+
+    Parameters
+    ----------
+    name: str
+        Name of suppression
+
+    kind: str
+        Kind of suppression
+
+    stack: List[SFrame]
+        Suppression stack trace
+
+    auxkind: Optional[str]
+        Auxiliary kind of suppression
+
+    Methods
+    -------
+    createRawText(name: str)
+        Creates raw text for suppression
+    """
+
     name: str
     kind: str
     stack: List[SFrame]
     auxkind: Optional[str] = None
 
     @classmethod
     def from_xml_element(cls, el: ET.Element) -> 'Suppression':
@@ -313,36 +446,70 @@
 
         if self.auxkind is not None:
             rawtext += line(self.auxkind)
 
         for el in self.stack:
             if el.fun is not None:
                 rawtext += line(f"fun:{el.fun}")
-            elif el.obj is not None:
+            if el.obj is not None:
                 rawtext += line(f"obj:{el.obj}")
 
         return rawtext + "}\n"
 
     def __str__(self):
         def value(val):
             return f": {val.__str__()}\n"
 
         result = "Suppression kind" + value(self.kind)
 
         for sframe in self.stack:
             result += f"Stack frame:\n{sframe.__str__()}"
 
         if self.auxkind is not None:
-            result = "Aux kind" + value(self.auxkind)
+            result += "Aux kind" + value(self.auxkind)
 
         return result
 
 
 @dataclass
 class FatalSignal:
+    """Class to keep track of fatal signal
+
+    Parameters
+    ----------
+    tid: int
+        Thread ID
+
+    signo: int
+        Signal number
+
+    signame: str
+        Signal name
+
+    sicode: int
+        Signal code
+
+    siaddr: str
+        Signal address
+
+    stack: List[Frame]
+        Stack trace
+
+    event: Optional[str]
+        Event
+
+    threadname: Optional[str]
+        Thread name
+
+    Methods
+    -------
+    get_signal() -> signal.Signals
+        Returns signal object from signal name
+    """
+
     tid: int
     signo: int
     signame: str
     sicode: int
     siaddr: str
     stack: List[Frame]
     event: Optional[str] = None
@@ -356,16 +523,15 @@
         sicode = elem_find_int(el, './sicode')
         siaddr = elem_find_text(el, './siaddr')
         stack = [Frame.from_xml_element(frame) for frame in el.findall('./stack/frame')]
         event = elem_find_text(el, './event')
         threadname = elem_find_text(el, './threadname')
         return cls(tid, signo, signame, sicode, siaddr, stack, event, threadname)
 
-    def get_signal(self):
-        """OS-specific (I think)"""
+    def get_signal(self) -> signal.Signals:
         return signal.Signals[self.signame]
 
     def __str__(self):
         def value(val):
             return f": {val.__str__()}\n"
 
         result = "Thread ID" + value(self.tid)
@@ -382,14 +548,31 @@
         if self.threadname is not None:
             result += "Thread name" + value(self.threadname)
 
         return result
 
 
 class Parser:
+    """Class to parse Valgrind XML output
+
+    Parameters
+    ----------
+    xmlfile : str
+        XML file to parse
+
+    Raises
+    ------
+    ValgrindFormatError
+        Raised if XML file is not properly formatted
+    ValgrindVersionError
+        Raised if XML file is for a schema that is not supported
+    ValgrindToolError
+        Raised if XML file is for a tool that is not supported
+    """
+
     def __init__(self, xmlfile: str) -> None:
         self.tree = ET.parse(xmlfile)
         root = self.tree.getroot()
         if root.tag != 'valgrindoutput':
             raise ValgrindFormatError("No valgrindoutput tag at top level.")
 
         # Check version
@@ -456,32 +639,68 @@
         signal = root.find('./fatal_signal')
         if signal:
             self.signal = FatalSignal.from_xml_element(signal)
 
         self.status = Status.from_xml_elements(root.findall('./status'))
 
     def hasErrors(self) -> bool:
+        """
+        Returns
+        -------
+        bool
+            True if there are errors, False otherwise
+        """
         return bool(self.errcount)
 
     def hasLeaks(self) -> bool:
+        """
+        Returns
+        -------
+        bool
+            True if there are leaks, False otherwise
+        """
         return bool(self.leakcount)
 
     def uniqueErrCount(self) -> int:
+        """
+        Returns
+        -------
+        int
+            Number of unique errors
+        """
         return len(self.errsunique)
 
     def uniqueLeakCount(self) -> int:
+        """
+        Returns
+        -------
+        int
+            Number of unique leaks
+        """
         return len(self.leaksunique)
 
     def totalBytesLeaked(self) -> int:
+        """
+        Returns
+        -------
+        int
+            Total number of bytes leaked
+        """
         count = 0
         for el in self.leaks:
             count += el.bytes_leaked
         return count
 
     def hasFatalSignal(self) -> bool:
+        """
+        Returns
+        -------
+        bool
+            True if there is a fatal signal, False otherwise
+        """
         return bool(self.signal)
 
     def __str__(self):
         result = self.args.__str__() + "\n\n"
 
         if self.hasFatalSignal():
             result += "Fatal signal:\n" + self.signal.__str__() + "\n\n"
@@ -492,30 +711,37 @@
         for err in self.errs:
             result += err.__str__() + "\n"
 
         result += "\nLeaks present: " + self.leakcount.__str__() + "\n\n"
         for leak in self.leaks:
             result += leak.__str__() + "\n"
 
-        result += "\nSuppressions: \n"
+        result += "\nSuppressions:\n"
 
         if len(self.suppressions) == 0:
             result += "none\n"
         for supp in self.suppressions:
             result += supp.__str__() + "\n"
 
         result += "\nTotal bytes leaked: " + self.totalBytesLeaked().__str__() + "\n"
 
         return result
 
 
 def dumpSuppressions(filename: str, supps: List[Tuple[str, Suppression]], append: Optional[bool] = False):
     """Dumps the raw suppression text to file with filename specified.
-    If append is specified as True, the file is opened in append mode.
-    Otherwise, the file is opened in write mode.
+
+    Parameters
+    ----------
+    filename : str
+        File to write to
+    supps : List[Tuple[str, Suppression]]
+        List of tuples of the form (name, Suppression)
+    append : Optional[bool], optional
+        If True, the file is opened in append mode, by default False
     """
     mode = 'a' if append else 'w'
 
     contents = ""
     with open(filename, mode) as file:
         for name, supp in supps:
             contents += supp.createRawText(name)
```

### Comparing `valparse-0.2.0/valparse.egg-info/PKG-INFO` & `valparse-0.2.1/valparse.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: valparse
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package to parse Valgrind XML files.
-Home-page: https://github.com/tzussman/valparse
-Author: valparse contributors
 Author-email: Tal Zussman <tz2294@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Tal Zussman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -31,18 +29,20 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: develop
 License-File: LICENSE
 
 # *valparse,* a parser for Valgrind-generated XML files
 
+[![PyPI](https://img.shields.io/pypi/v/valparse)](https://pypi.org/project/valparse/)
 [![License](https://img.shields.io/github/license/tzussman/valparse)](https://github.com/tzussman/valparse)
 ![GitHub issues](https://img.shields.io/github/issues/tzussman/valparse)
 [![Build Status](https://github.com/tzussman/valparse/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/tzussman/valparse/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/tzussman/valparse/branch/main/graph/badge.svg)](https://codecov.io/gh/tzussman/valparse)
+[![Docs](https://img.shields.io/badge/-docs-blueviolet)](https://tzussman.github.io/valparse)
 
 *valparse* supports protocol version 4 with [*Memcheck*][memcheck] only, but can
 be easily modified to support [*Helgrind*][helgrind] and other protocol tools.
 
 [memcheck]: https://valgrind.org/docs/manual/mc-manual.html
 [helgrind]: https://valgrind.org/docs/manual/hg-manual.html
 
@@ -69,14 +69,26 @@
 ```
 
 Some examples of `.xml` files generated by Valgrind are included in the
 `/examples` directory.
 
 Valgrind does not support XML output for fd leaks as of version 3.18.1.
 
+## Usage
+
+Below is an example of basic `valparse` usage:
+
+```py
+import valparse
+
+xml_file = valparse.Parser('./test.xml')
+if xml_file.hasLeaks() or xml_file.hasErrors():
+    print("Leaks or errors found!")
+```
+
 ## Features
 
 -   Error generation for nonexistent/incorrectly formatted TOPLEVEL tags
 
 -   Error generation for nonexistent/incorrectly formatted PROTOCOL tags
 
 -   Basic Valgrind output parsing
```

