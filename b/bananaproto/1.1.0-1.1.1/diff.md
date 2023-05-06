# Comparing `tmp/bananaproto-1.1.0.tar.gz` & `tmp/bananaproto-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananaproto-1.1.0.tar", max compression
+gzip compressed data, was "bananaproto-1.1.1.tar", max compression
```

## Comparing `bananaproto-1.1.0.tar` & `bananaproto-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0    16280 2023-04-19 00:24:54.144058 bananaproto-1.1.0/README.md
--rw-r--r--   0        0        0     3369 2023-04-19 00:24:54.144058 bananaproto-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    56436 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/__init__.py
--rw-r--r--   0        0        0      295 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/_types.py
--rw-r--r--   0        0        0       99 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/_version.py
--rw-r--r--   0        0        0     3543 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/casing.py
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/__init__.py
--rw-r--r--   0        0        0     6337 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/importing.py
--rw-r--r--   0        0        0      286 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/naming.py
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/__init__.py
--rw-r--r--   0        0        0     5295 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/grpclib_client.py
--rw-r--r--   0        0        0      982 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/grpclib_server.py
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/util/__init__.py
--rw-r--r--   0        0        0     6793 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/util/async_channel.py
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/lib/google/__init__.py
--rw-r--r--   0        0        0    70836 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/__init__.py
--rw-r--r--   0        0        0     7057 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0       23 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/__init__.py
--rw-r--r--   0        0        0       32 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/__main__.py
--rw-r--r--   0        0        0     1320 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/compiler.py
--rwxr-xr-x   0        0        0     1471 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/main.py
--rw-r--r--   0        0        0    28084 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/models.py
--rw-r--r--   0        0        0     7649 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/parser.py
--rw-r--r--   0        0        0       48 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/plugin.bat
--rw-r--r--   0        0        0        0 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/py.typed
--rw-r--r--   0        0        0     8391 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/templates/template.py.j2
--rw-r--r--   0        0        0    17389 1970-01-01 00:00:00.000000 bananaproto-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16280 2023-05-06 00:10:49.508651 bananaproto-1.1.1/README.md
+-rw-r--r--   0        0        0     3451 2023-05-06 00:11:45.076772 bananaproto-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    56436 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/__init__.py
+-rw-r--r--   0        0        0      295 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/_types.py
+-rw-r--r--   0        0        0       99 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/_version.py
+-rw-r--r--   0        0        0     3543 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/casing.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/__init__.py
+-rw-r--r--   0        0        0     6337 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/importing.py
+-rw-r--r--   0        0        0      286 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/compile/naming.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/__init__.py
+-rw-r--r--   0        0        0     5295 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/grpclib_client.py
+-rw-r--r--   0        0        0      982 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/grpclib_server.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/util/__init__.py
+-rw-r--r--   0        0        0     6793 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/grpc/util/async_channel.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.508651 bananaproto-1.1.1/src/bananaproto/lib/google/__init__.py
+-rw-r--r--   0        0        0    70836 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     7057 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/__main__.py
+-rw-r--r--   0        0        0     1320 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/compiler.py
+-rwxr-xr-x   0        0        0     1471 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/main.py
+-rw-r--r--   0        0        0    28084 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/models.py
+-rw-r--r--   0        0        0     7649 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/parser.py
+-rw-r--r--   0        0        0       48 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/plugin/plugin.bat
+-rw-r--r--   0        0        0        0 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/py.typed
+-rw-r--r--   0        0        0     8391 2023-05-06 00:10:49.512652 bananaproto-1.1.1/src/bananaproto/templates/template.py.j2
+-rw-r--r--   0        0        0    18193 1970-01-01 00:00:00.000000 bananaproto-1.1.1/setup.py
+-rw-r--r--   0        0        0    17389 1970-01-01 00:00:00.000000 bananaproto-1.1.1/PKG-INFO
```

### Comparing `bananaproto-1.1.0/README.md` & `bananaproto-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/pyproject.toml` & `bananaproto-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bananaproto"
-version = "1.1.0"
+version = "v1.1.1"
 description = "A BANANA Protobuf / gRPC generator & library"
 authors = ["Daniel G. Taylor <danielgtaylor@gmail.com>"]
 maintainers = ["BananaLoaf <bananaloaf@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/BananaLoaf/python-bananaproto"
 keywords = ["protobuf", "gRPC"]
 license = "MIT"
@@ -58,30 +58,32 @@
 help = "Run tests"
 
 [tool.poe.tasks.types]
 cmd  = "mypy src --ignore-missing-imports"
 help = "Check types with mypy"
 
 [tool.poe.tasks.format]
-cmd  = "black . --exclude tests/output_"
+cmd  = "black . --exclude output_"
 help = "Apply black formatting to source code"
 
 [tool.poe.tasks.docs]
 cmd  = "sphinx-build docs docs/build"
 help = "Build the sphinx docs"
 
 [tool.poe.tasks.bench]
 shell = "asv run master^! && asv run HEAD^! && asv compare master HEAD"
 help  = "Benchmark current commit vs. master branch"
 
 [tool.poe.tasks.clean]
 cmd  = """
 rm -rf .asv .coverage .mypy_cache .pytest_cache
        dist bananaproto.egg-info **/__pycache__
-       testsoutput_*
+       testsoutput_* **/output_bananaproto
+       **/output_bananaproto_pydantic
+       **/output_reference
 """
 help = "Clean out generated files from the workspace"
 
 [tool.poe.tasks.generate_lib]
 cmd = """
 protoc
     --plugin=protoc-gen-custom=src/bananaproto/plugin/main.py
```

### Comparing `bananaproto-1.1.0/src/bananaproto/__init__.py` & `bananaproto-1.1.1/src/bananaproto/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/casing.py` & `bananaproto-1.1.1/src/bananaproto/casing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/compile/importing.py` & `bananaproto-1.1.1/src/bananaproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/grpc/grpclib_client.py` & `bananaproto-1.1.1/src/bananaproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/grpc/grpclib_server.py` & `bananaproto-1.1.1/src/bananaproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/grpc/util/async_channel.py` & `bananaproto-1.1.1/src/bananaproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/__init__.py` & `bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py` & `bananaproto-1.1.1/src/bananaproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/plugin/compiler.py` & `bananaproto-1.1.1/src/bananaproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/plugin/main.py` & `bananaproto-1.1.1/src/bananaproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/plugin/models.py` & `bananaproto-1.1.1/src/bananaproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/plugin/parser.py` & `bananaproto-1.1.1/src/bananaproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/src/bananaproto/templates/template.py.j2` & `bananaproto-1.1.1/src/bananaproto/templates/template.py.j2`

 * *Files identical despite different names*

### Comparing `bananaproto-1.1.0/PKG-INFO` & `bananaproto-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bananaproto
-Version: 1.1.0
+Version: 1.1.1
 Summary: A BANANA Protobuf / gRPC generator & library
 Home-page: https://github.com/BananaLoaf/python-bananaproto
 License: MIT
 Keywords: protobuf,gRPC
 Author: Daniel G. Taylor
 Author-email: danielgtaylor@gmail.com
 Maintainer: BananaLoaf
```

