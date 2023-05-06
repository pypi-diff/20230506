# Comparing `tmp/xdrlib3-0.1.0.dev1.tar.gz` & `tmp/xdrlib3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdrlib3-0.1.0.dev1.tar", max compression
+gzip compressed data, was "xdrlib3-0.1.1.tar", max compression
```

## Comparing `xdrlib3-0.1.0.dev1.tar` & `xdrlib3-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     1215 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     6805 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/xdrlib3/__init__.py
--rw-r--r--   0        0        0       63 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/xdrlib3/py.typed
--rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 xdrlib3-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-05-06 11:45:27.919255 xdrlib3-0.1.1/README.md
+-rw-r--r--   0        0        0     1210 2023-05-06 11:45:27.919255 xdrlib3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6826 2023-05-06 11:45:27.923255 xdrlib3-0.1.1/xdrlib3/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-06 11:45:27.923255 xdrlib3-0.1.1/xdrlib3/py.typed
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 xdrlib3-0.1.1/PKG-INFO
```

### Comparing `xdrlib3-0.1.0.dev1/README.md` & `xdrlib3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xdrlib3-0.1.0.dev1/pyproject.toml` & `xdrlib3-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xdrlib3"
-version = "0.1.0.dev1"
+version = "0.1.1"
 description = "A forked version of `xdrlib`, a module for encoding and decoding XDR (External Data Representation) data in Python."
 authors = ["overcat <4catcode@gmail.com>"]
 readme = "README.md"
 maintainers = ["overcat <4catcode@gmail.com>"]
 homepage = "https://github.com/overcat/xdrlib3"
 repository = "https://github.com/overcat/xdrlib3"
 documentation = "https://github.com/overcat/xdrlib3"
```

### Comparing `xdrlib3-0.1.0.dev1/xdrlib3/__init__.py` & `xdrlib3-0.1.1/xdrlib3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 Adapted from xdrlib.py in the Python standard library, 
 you can find the LICENSE file here: https://github.com/python/cpython/blob/024ac542d738f56b36bdeb3517a10e93da5acab9/LICENSE
 """
 import struct
 from functools import wraps
 from io import BytesIO
-from typing import Callable, List, Union, TypeVar
-
+from typing import Callable, List, Union, TypeVar, Sequence
 
 __all__ = ["Error", "Packer", "Unpacker", "ConversionError"]
 
 T = TypeVar("T")
 
 
 # exceptions
@@ -120,29 +119,29 @@
         n = len(s)
         self.pack_uint(n)
         self.pack_fstring(n, s)
 
     pack_opaque = pack_string
     pack_bytes = pack_string
 
-    def pack_list(self, list: List[T], pack_item: Callable[[T], None]) -> None:
+    def pack_list(self, list: Sequence[T], pack_item: Callable[[T], None]) -> None:
         for item in list:
             self.pack_uint(1)
             pack_item(item)
         self.pack_uint(0)
 
     def pack_farray(
-        self, n: int, list: List[T], pack_item: Callable[[T], None]
+        self, n: int, list: Sequence[T], pack_item: Callable[[T], None]
     ) -> None:
         if len(list) != n:
             raise ValueError("wrong array size")
         for item in list:
             pack_item(item)
 
-    def pack_array(self, list: List[T], pack_item: Callable[[T], None]) -> None:
+    def pack_array(self, list: Sequence[T], pack_item: Callable[[T], None]) -> None:
         n = len(list)
         self.pack_uint(n)
         self.pack_farray(n, list, pack_item)
 
 
 class Unpacker:
     """Unpacks various data representations from the given buffer."""
```

### Comparing `xdrlib3-0.1.0.dev1/PKG-INFO` & `xdrlib3-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdrlib3
-Version: 0.1.0.dev1
+Version: 0.1.1
 Summary: A forked version of `xdrlib`, a module for encoding and decoding XDR (External Data Representation) data in Python.
 Home-page: https://github.com/overcat/xdrlib3
 Keywords: xdrlib,xdr
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
 Maintainer-email: 4catcode@gmail.com
```

