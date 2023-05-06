# Comparing `tmp/xdrlib3-0.1.0.dev0.tar.gz` & `tmp/xdrlib3-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdrlib3-0.1.0.dev0.tar", max compression
+gzip compressed data, was "xdrlib3-0.1.0.dev1.tar", max compression
```

## Comparing `xdrlib3-0.1.0.dev0.tar` & `xdrlib3-0.1.0.dev1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      976 2023-05-06 10:38:19.243353 xdrlib3-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     1215 2023-05-06 10:38:19.230163 xdrlib3-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     6754 2023-05-06 10:04:05.147977 xdrlib3-0.1.0.dev0/xdrlib3/__init__.py
--rw-r--r--   0        0        0       63 2023-05-06 10:05:53.288203 xdrlib3-0.1.0.dev0/xdrlib3/py.typed
--rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 xdrlib3-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      976 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0     1215 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     6805 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/xdrlib3/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-06 11:26:54.943126 xdrlib3-0.1.0.dev1/xdrlib3/py.typed
+-rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 xdrlib3-0.1.0.dev1/PKG-INFO
```

### Comparing `xdrlib3-0.1.0.dev0/README.md` & `xdrlib3-0.1.0.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Usage
 `xdrlib3` has the same functions and methods as `xdrlib`. Here's an example of how to use it:
 
 ```python
 import xdrlib3
 
 packer = xdrlib3.Packer()
-packer.pack_int(42)
+packer.pack_int(16)
 packed_data = packer.get_buffer()
 
 unpacker = xdrlib3.Unpacker(packed_data)
 unpacked_data = unpacker.unpack_int()
 ```
 
 ## License
```

### Comparing `xdrlib3-0.1.0.dev0/pyproject.toml` & `xdrlib3-0.1.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xdrlib3"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 description = "A forked version of `xdrlib`, a module for encoding and decoding XDR (External Data Representation) data in Python."
 authors = ["overcat <4catcode@gmail.com>"]
 readme = "README.md"
 maintainers = ["overcat <4catcode@gmail.com>"]
 homepage = "https://github.com/overcat/xdrlib3"
 repository = "https://github.com/overcat/xdrlib3"
 documentation = "https://github.com/overcat/xdrlib3"
```

### Comparing `xdrlib3-0.1.0.dev0/xdrlib3/__init__.py` & `xdrlib3-0.1.0.dev1/xdrlib3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,18 @@
         return self.unpack_fstring(n)
 
     unpack_opaque = unpack_string
     unpack_bytes = unpack_string
 
     def unpack_list(self, unpack_item: Callable[[], T]) -> List[T]:
         list = []
-        while (x := self.unpack_uint()) != 0:
+        while 1:
+            x = self.unpack_uint()
+            if x == 0:
+                break
             if x != 1:
                 raise ConversionError("0 or 1 expected, got %r" % (x,))
             item = unpack_item()
             list.append(item)
         return list
 
     def unpack_farray(self, n: int, unpack_item: Callable[[], T]) -> List[T]:
```

### Comparing `xdrlib3-0.1.0.dev0/PKG-INFO` & `xdrlib3-0.1.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdrlib3
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: A forked version of `xdrlib`, a module for encoding and decoding XDR (External Data Representation) data in Python.
 Home-page: https://github.com/overcat/xdrlib3
 Keywords: xdrlib,xdr
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
 Maintainer-email: 4catcode@gmail.com
@@ -44,15 +44,15 @@
 ## Usage
 `xdrlib3` has the same functions and methods as `xdrlib`. Here's an example of how to use it:
 
 ```python
 import xdrlib3
 
 packer = xdrlib3.Packer()
-packer.pack_int(42)
+packer.pack_int(16)
 packed_data = packer.get_buffer()
 
 unpacker = xdrlib3.Unpacker(packed_data)
 unpacked_data = unpacker.unpack_int()
 ```
 
 ## License
```

