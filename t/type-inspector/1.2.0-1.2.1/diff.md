# Comparing `tmp/type_inspector-1.2.0.tar.gz` & `tmp/type_inspector-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type_inspector-1.2.0.tar", max compression
+gzip compressed data, was "type_inspector-1.2.1.tar", max compression
```

## Comparing `type_inspector-1.2.0.tar` & `type_inspector-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-02-04 22:45:21.163332 type_inspector-1.2.0/LICENSE
--rw-r--r--   0        0        0     1144 2023-05-06 12:05:56.269948 type_inspector-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5851 2023-05-06 12:05:32.116615 type_inspector-1.2.0/type_inspector/__init__.py
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 type_inspector-1.2.0/setup.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 type_inspector-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-04 22:45:21.163332 type_inspector-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1144 2023-05-06 12:08:58.759944 type_inspector-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5851 2023-05-06 12:08:50.763277 type_inspector-1.2.1/type_inspector/__init__.py
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 type_inspector-1.2.1/setup.py
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 type_inspector-1.2.1/PKG-INFO
```

### Comparing `type_inspector-1.2.0/LICENSE` & `type_inspector-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `type_inspector-1.2.0/pyproject.toml` & `type_inspector-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "type-inspector"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.10"
 pydantic = { version = "^1.10.4", optional = true }
```

### Comparing `type_inspector-1.2.0/type_inspector/__init__.py` & `type_inspector-1.2.1/type_inspector/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def __init__(self, message: str, address: str, problematic_key: object):
         super().__init__(message)
         self.message = message
         self.address = address
         self.problematic_key = problematic_key
 
     def __repr__(self):
-        return f"{self.__class__.__name__}({self.message!r}. Object: {self.address}, Key: {self.problematic_key!r})"
+        return f'{self.__class__.__name__}("{self.message}. Object: {self.address}, Key: {self.problematic_key!r}")'
 
 
 @dataclasses.dataclass(slots=True, frozen=True)
 class Inspector:
     wrapped: Any
     address_parts: list[str | int] = dataclasses.field(default_factory=list)
```

### Comparing `type_inspector-1.2.0/setup.py` & `type_inspector-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['issubclass>=0.1.2']
 
 setup_kwargs = {
     'name': 'type-inspector',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': '',
     'long_description': 'None',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

