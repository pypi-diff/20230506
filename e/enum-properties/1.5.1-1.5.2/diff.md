# Comparing `tmp/enum_properties-1.5.1.tar.gz` & `tmp/enum_properties-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_properties-1.5.1.tar", max compression
+gzip compressed data, was "enum_properties-1.5.2.tar", max compression
```

## Comparing `enum_properties-1.5.1.tar` & `enum_properties-1.5.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.5.1/LICENSE
--rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.5.1/README.rst
--rw-r--r--   0        0        0    22922 2023-04-18 06:27:52.684685 enum_properties-1.5.1/enum_properties/__init__.py
--rw-r--r--   0        0        0     1878 2023-04-18 06:27:52.693441 enum_properties-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.5.2/README.rst
+-rw-r--r--   0        0        0    22923 2023-05-06 18:11:36.844737 enum_properties-1.5.2/enum_properties/__init__.py
+-rw-r--r--   0        0        0     1878 2023-05-06 18:13:06.315400 enum_properties-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.5.2/PKG-INFO
```

### Comparing `enum_properties-1.5.1/LICENSE` & `enum_properties-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_properties-1.5.1/README.rst` & `enum_properties-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `enum_properties-1.5.1/enum_properties/__init__.py` & `enum_properties-1.5.2/enum_properties/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
     # todo remove when python 3.7 support is dropped
     cached_property = property  # pylint: disable=C0103
 
 
-VERSION = (1, 5, 1)
+VERSION = (1, 5, 2)
 
 __title__ = 'Enum Properties'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-2023 Brian Kohan'
 
@@ -231,15 +231,15 @@
                         return cls._ep_symmetric_map_[val]
                     except KeyError:
                         pass
 
                     if isinstance(val, str):
                         return cls._ep_isymmetric_map_[_do_casenorm(val)]
 
-                except (KeyError, TypeError, ValueError):
+                except Exception:  # pylint: disable=W0703
                     pass
 
         return super()._missing_(value)
 
 
 class EnumPropertiesMeta(enum.EnumMeta):
     """
```

### Comparing `enum_properties-1.5.1/pyproject.toml` & `enum_properties-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enum-properties"
-version = "1.5.1"
+version = "1.5.2"
 description = "Add properties and method specializations to Python enumeration values with a simple declarative syntax."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bckohan/enum-properties"
 homepage = "https://enum-properties.readthedocs.io"
 readme = "README.rst"
 keywords = ["enum",  "properties", "defines", "field"]
```

### Comparing `enum_properties-1.5.1/PKG-INFO` & `enum_properties-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-properties
-Version: 1.5.1
+Version: 1.5.2
 Summary: Add properties and method specializations to Python enumeration values with a simple declarative syntax.
 Home-page: https://enum-properties.readthedocs.io
 License: MIT
 Keywords: enum,properties,defines,field
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.7,<4.0
```

