# Comparing `tmp/pyupgrade-3.3.2.tar.gz` & `tmp/pyupgrade-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrade-3.3.2.tar", last modified: Tue Apr 25 01:35:06 2023, max compression
+gzip compressed data, was "pyupgrade-3.4.0.tar", last modified: Sat May  6 21:09:25 2023, max compression
```

## Comparing `pyupgrade-3.3.2.tar` & `pyupgrade-3.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.876028 pyupgrade-3.3.2/pyupgrade/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2022-11-10 15:38:09.000000 pyupgrade-3.3.2/pyupgrade/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11784 2023-02-20 22:41:07.000000 pyupgrade-3.3.2/pyupgrade/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/pyupgrade/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/collections_abc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2022-12-02 18:20:28.000000 pyupgrade-3.3.2/pyupgrade/_plugins/datetime_utc_alias.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1231 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/default_encoding.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/dict_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1709 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/format_locals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4334 2022-11-29 16:14:49.000000 pyupgrade-3.3.2/pyupgrade/_plugins/fstrings.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1483 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/identity_equality.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-04-25 01:35:03.000000 pyupgrade-3.3.2/pyupgrade/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/io_open.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2451 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/lru_cache.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/metaclass_type.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/mock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2224 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/native_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/new_style_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3851 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/open_mode.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/oserror_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9357 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/percent_format.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/set_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_base_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6558 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_metaclasses.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_remove_decorators.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/six_simple.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/subprocess_run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1747 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/type_of_primitive.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8084 2022-12-06 22:19:56.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4836 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep563.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep585.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5610 2022-11-10 15:10:00.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep604.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2022-11-10 15:10:00.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep646_unpack.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/typing_text.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/unittest_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1189 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/unpack_list_comprehension.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6416 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_plugins/versioned_branches.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/pyupgrade/_string_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    15888 2022-10-29 19:34:22.000000 pyupgrade-3.3.2/pyupgrade/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-04-25 01:35:06.876028 pyupgrade-3.3.2/pyupgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-04-25 01:35:06.000000 pyupgrade-3.3.2/pyupgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1199 2023-04-25 01:35:06.880028 pyupgrade-3.3.2/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:39.000000 pyupgrade-3.3.2/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.927491 pyupgrade-3.4.0/pyupgrade/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11784 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/pyupgrade/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/collections_abc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/datetime_utc_alias.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/default_encoding.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/dict_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/format_locals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/fstrings.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/identity_equality.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    20494 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/io_open.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/lru_cache.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/metaclass_type.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/mock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2331 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/native_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/new_style_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/open_mode.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/oserror_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/percent_format.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/set_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_base_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_metaclasses.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_remove_decorators.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/six_simple.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/subprocess_run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/type_of_primitive.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8423 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4877 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep563.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep585.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep604.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep646_unpack.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/typing_text.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_plugins/unittest_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-05-06 20:39:40.000000 pyupgrade-3.4.0/pyupgrade/_plugins/unpack_list_comprehension.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade/_plugins/versioned_branches.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/pyupgrade/_string_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-05-06 20:39:40.000000 pyupgrade-3.4.0/pyupgrade/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-05-06 21:09:25.927491 pyupgrade-3.4.0/pyupgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-05-06 21:09:25.000000 pyupgrade-3.4.0/pyupgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1199 2023-05-06 21:09:25.931491 pyupgrade-3.4.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-05-06 20:27:38.000000 pyupgrade-3.4.0/setup.py
```

### Comparing `pyupgrade-3.3.2/LICENSE` & `pyupgrade-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/PKG-INFO` & `pyupgrade-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.3.2
+Version: 3.4.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.2/README.md` & `pyupgrade-3.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_ast_helpers.py` & `pyupgrade-3.4.0/pyupgrade/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_data.py` & `pyupgrade-3.4.0/pyupgrade/_data.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_main.py` & `pyupgrade-3.4.0/pyupgrade/_main.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/collections_abc.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/collections_abc.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/datetime_utc_alias.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/datetime_utc_alias.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/default_encoding.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/mock.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,38 +3,31 @@
 import ast
 from typing import Iterable
 
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
-from pyupgrade._ast_helpers import has_starargs
 from pyupgrade._data import register
 from pyupgrade._data import State
 from pyupgrade._data import TokenFunc
-from pyupgrade._string_helpers import is_codec
-from pyupgrade._token_helpers import find_closing_bracket
-from pyupgrade._token_helpers import find_open_paren
+from pyupgrade._token_helpers import find_token
 
 
-def _fix_default_encoding(i: int, tokens: list[Token]) -> None:
-    i = find_open_paren(tokens, i + 1)
-    j = find_closing_bracket(tokens, i)
-    del tokens[i + 1:j]
+def _fix_mock_mock(i: int, tokens: list[Token]) -> None:
+    j = find_token(tokens, i + 1, 'mock')
+    del tokens[i + 1:j + 1]
 
 
-@register(ast.Call)
-def visit_Call(
+@register(ast.Attribute)
+def visit_Attribute(
         state: State,
-        node: ast.Call,
+        node: ast.Attribute,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
-            isinstance(node.func, ast.Attribute) and
-            isinstance(node.func.value, (ast.Str, ast.JoinedStr)) and
-            node.func.attr == 'encode' and
-            not has_starargs(node) and
-            len(node.args) == 1 and
-            isinstance(node.args[0], ast.Str) and
-            is_codec(node.args[0].s, 'utf-8')
+            not state.settings.keep_mock and
+            isinstance(node.value, ast.Name) and
+            node.value.id == 'mock' and
+            node.attr == 'mock'
     ):
-        yield ast_to_offset(node), _fix_default_encoding
+        yield ast_to_offset(node), _fix_mock_mock
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/dict_literals.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/dict_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/format_locals.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/format_locals.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         state: State,
         node: ast.Call,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
             state.settings.min_version >= (3, 6) and
             isinstance(node.func, ast.Attribute) and
-            isinstance(node.func.value, ast.Str) and
+            isinstance(node.func.value, ast.Constant) and
+            isinstance(node.func.value.value, str) and
             node.func.attr == 'format' and
             len(node.args) == 0 and
             len(node.keywords) == 1 and
             node.keywords[0].arg is None and
             isinstance(node.keywords[0].value, ast.Call) and
             isinstance(node.keywords[0].value.func, ast.Name) and
             node.keywords[0].value.func.id == 'locals' and
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/fstrings.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/fstrings.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,20 +95,21 @@
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if state.settings.min_version < (3, 6):
         return
 
     if (
             isinstance(node.func, ast.Attribute) and
-            isinstance(node.func.value, ast.Str) and
+            isinstance(node.func.value, ast.Constant) and
+            isinstance(node.func.value.value, str) and
             node.func.attr == 'format' and
             not has_starargs(node)
     ):
         try:
-            parsed = parse_format(node.func.value.s)
+            parsed = parse_format(node.func.value.value)
         except ValueError:
             return
 
         params = _format_params(node)
         seen = set()
         i = 0
         for _, name, spec, _ in parsed:
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/identity_equality.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/identity_equality.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
 from pyupgrade._data import register
 from pyupgrade._data import State
 from pyupgrade._data import TokenFunc
 
-LITERAL_TYPES = (ast.Str, ast.Num, ast.Bytes)
-
 
 def _fix_is_literal(
         i: int,
         tokens: list[Token],
         *,
         op: ast.Is | ast.IsNot,
 ) -> None:
@@ -31,25 +29,30 @@
         i += 1
         while tokens[i].src != 'not':
             tokens[i] = Token('EMPTY', '')
             i += 1
         tokens[i] = Token('EMPTY', '')
 
 
+def _is_literal(n: ast.AST) -> bool:
+    return (
+        isinstance(n, ast.Constant) and
+        n.value not in {True, False} and
+        isinstance(n.value, (str, bytes, int, float))
+    )
+
+
 @register(ast.Compare)
 def visit_Compare(
         state: State,
         node: ast.Compare,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     left = node.left
     for op, right in zip(node.ops, node.comparators):
         if (
                 isinstance(op, (ast.Is, ast.IsNot)) and
-                (
-                    isinstance(left, LITERAL_TYPES) or
-                    isinstance(right, LITERAL_TYPES)
-                )
+                (_is_literal(left) or _is_literal(right))
         ):
             func = functools.partial(_fix_is_literal, op=op)
             yield ast_to_offset(right), func
         left = right
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/imports.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/io_open.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/io_open.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/legacy.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/lru_cache.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/lru_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 def _is_literal_kwarg(
         keyword: ast.keyword, name: str, value: bool | None,
 ) -> bool:
     return (
         keyword.arg == name and
-        isinstance(keyword.value, ast.NameConstant) and
+        isinstance(keyword.value, ast.Constant) and
         keyword.value.value is value
     )
 
 
 def _eligible(keywords: list[ast.keyword]) -> bool:
     if len(keywords) == 1:
         return _is_literal_kwarg(keywords[0], 'maxsize', None)
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/metaclass_type.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/metaclass_type.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/mock.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 from __future__ import annotations
 
 import ast
+import functools
 from typing import Iterable
 
 from tokenize_rt import Offset
-from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
 from pyupgrade._data import register
 from pyupgrade._data import State
 from pyupgrade._data import TokenFunc
-from pyupgrade._token_helpers import find_token
-
-
-def _fix_mock_mock(i: int, tokens: list[Token]) -> None:
-    j = find_token(tokens, i + 1, 'mock')
-    del tokens[i + 1:j + 1]
+from pyupgrade._token_helpers import replace_name
 
 
 @register(ast.Attribute)
 def visit_Attribute(
         state: State,
         node: ast.Attribute,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
-            not state.settings.keep_mock and
             isinstance(node.value, ast.Name) and
-            node.value.id == 'mock' and
-            node.attr == 'mock'
+            node.value.id == 'typing' and
+            node.attr == 'Text'
     ):
-        yield ast_to_offset(node), _fix_mock_mock
+        func = functools.partial(replace_name, name=node.attr, new='str')
+        yield ast_to_offset(node), func
+
+
+@register(ast.Name)
+def visit_Name(
+        state: State,
+        node: ast.Name,
+        parent: ast.AST,
+) -> Iterable[tuple[Offset, TokenFunc]]:
+    if node.id in state.from_imports['typing'] and node.id == 'Text':
+        func = functools.partial(replace_name, name=node.id, new='str')
+        yield ast_to_offset(node), func
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/native_literals.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/native_literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,19 @@
             is_name_attr(node.func, from_imports, ('six',), SIX_NATIVE_STR) or
             isinstance(node.func, ast.Name) and node.func.id == 'str'
         ) and
         not node.keywords and
         not has_starargs(node) and
         (
             len(node.args) == 0 or
-            (len(node.args) == 1 and isinstance(node.args[0], ast.Str))
+            (
+                len(node.args) == 1 and
+                isinstance(node.args[0], ast.Constant) and
+                isinstance(node.args[0].value, str)
+            )
         )
     )
 
 
 @register(ast.Call)
 def visit_Call(
         state: State,
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/new_style_classes.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/new_style_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/open_mode.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/open_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,36 +77,41 @@
                     isinstance(node.func.value, ast.Name) and
                     node.func.value.id == 'io' and
                     node.func.attr == 'open'
                 )
             ) and
             not has_starargs(node)
     ):
-        if len(node.args) >= 2 and isinstance(node.args[1], ast.Str):
+        if (
+                len(node.args) >= 2 and
+                isinstance(node.args[1], ast.Constant) and
+                isinstance(node.args[1].value, str)
+        ):
             if (
-                node.args[1].s in MODE_REPLACE or
-                (len(node.args) == 2 and node.args[1].s in MODE_REMOVE)
+                node.args[1].value in MODE_REPLACE or
+                (len(node.args) == 2 and node.args[1].value in MODE_REMOVE)
             ):
                 func = functools.partial(_fix_open_mode, arg_idx=1)
                 yield ast_to_offset(node), func
         elif node.keywords and (len(node.keywords) + len(node.args) > 1):
             mode = next(
                 (
                     FunctionArg(n, keyword.value)
                     for n, keyword in enumerate(node.keywords)
                     if keyword.arg == 'mode'
                 ),
                 None,
             )
             if (
                 mode is not None and
-                isinstance(mode.value, ast.Str) and
+                isinstance(mode.value, ast.Constant) and
+                isinstance(mode.value.value, str) and
                 (
-                    mode.value.s in MODE_REMOVE or
-                    mode.value.s in MODE_REPLACE
+                    mode.value.value in MODE_REMOVE or
+                    mode.value.value in MODE_REPLACE
                 )
             ):
                 func = functools.partial(
                     _fix_open_mode,
                     arg_idx=len(node.args) + mode.arg_idx,
                 )
                 yield ast_to_offset(node), func
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/oserror_aliases.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/oserror_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/percent_format.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/percent_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -180,26 +180,26 @@
         node_right: ast.Dict,
 ) -> None:
     seen_keys: set[str] = set()
     keys = {}
 
     for k in node_right.keys:
         # not a string key
-        if not isinstance(k, ast.Str):
+        if not isinstance(k, ast.Constant) or not isinstance(k.value, str):
             return
         # duplicate key
-        elif k.s in seen_keys:
+        elif k.value in seen_keys:
             return
         # not an identifier
-        elif not k.s.isidentifier():
+        elif not k.value.isidentifier():
             return
         # a keyword
-        elif k.s in KEYWORDS:
+        elif k.value in KEYWORDS:
             return
-        seen_keys.add(k.s)
+        seen_keys.add(k.value)
         keys[ast_to_offset(k)] = k
 
     # TODO: this is overly timid
     brace = i + 4
     if tokens_to_src(tokens[i + 1:brace + 1]) != ' % {':
         return
 
@@ -208,21 +208,21 @@
 
     key_indices = []
     for j, token in enumerate(tokens[brace:brace_end], brace):
         key = keys.pop(token.offset, None)
         if key is None:
             continue
         # we found the key, but the string didn't match (implicit join?)
-        elif ast.literal_eval(token.src) != key.s:
+        elif ast.literal_eval(token.src) != key.value:
             return
         # the map uses some strange syntax that's not `'key': value`
         elif tokens[j + 1].src != ':' or tokens[j + 2].src != ' ':
             return
         else:
-            key_indices.append((j, key.s))
+            key_indices.append((j, key.value))
     assert not keys, keys
 
     tokens[brace_end] = tokens[brace_end]._replace(src=')')
     for key_index, s in reversed(key_indices):
         tokens[key_index:key_index + 3] = [Token('CODE', f'{s}=')]
     newsrc = _percent_to_format(tokens[i].src)
     tokens[i] = tokens[i]._replace(src=newsrc)
@@ -234,18 +234,19 @@
         state: State,
         node: ast.BinOp,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
             not state.settings.keep_percent_format and
             isinstance(node.op, ast.Mod) and
-            isinstance(node.left, ast.Str)
+            isinstance(node.left, ast.Constant) and
+            isinstance(node.left.value, str)
     ):
         try:
-            parsed = _parse_percent_format(node.left.s)
+            parsed = _parse_percent_format(node.left.value)
         except ValueError:
             pass
         else:
             for _, fmt in parsed:
                 if not fmt:
                     continue
                 key, conversion_flag, width, precision, conversion = fmt
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/set_literals.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/set_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/six_base_classes.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/six_base_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/six_calls.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/six_calls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import ast
 import functools
-import sys
 from typing import Iterable
 
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
 from pyupgrade._ast_helpers import has_starargs
@@ -17,18 +16,16 @@
 from pyupgrade._token_helpers import find_and_replace_call
 from pyupgrade._token_helpers import find_open_paren
 from pyupgrade._token_helpers import parse_call_args
 from pyupgrade._token_helpers import replace_call
 
 _EXPR_NEEDS_PARENS: tuple[type[ast.expr], ...] = (
     ast.Await, ast.BinOp, ast.BoolOp, ast.Compare, ast.GeneratorExp, ast.IfExp,
-    ast.Lambda, ast.UnaryOp,
+    ast.Lambda, ast.UnaryOp, ast.NamedExpr,
 )
-if sys.version_info >= (3, 8):  # pragma: >=3.8 cover
-    _EXPR_NEEDS_PARENS += (ast.NamedExpr,)
 
 SIX_CALLS = {
     'u': '{args[0]}',
     'byte2int': '{args[0]}[0]',
     'indexbytes': '{args[0]}[{rest}]',
     'iteritems': '{args[0]}.items()',
     'iterkeys': '{args[0]}.keys()',
@@ -139,15 +136,16 @@
                 state.from_imports,
                 ('six',),
                 ('b', 'ensure_binary'),
             ) and
             not node.keywords and
             not has_starargs(node) and
             len(node.args) == 1 and
-            isinstance(node.args[0], ast.Str)
+            isinstance(node.args[0], ast.Constant) and
+            isinstance(node.args[0].value, str)
     ):
         yield ast_to_offset(node), _fix_six_b
     elif (
             isinstance(parent, ast.Expr) and
             is_name_attr(
                 node.func,
                 state.from_imports,
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/six_metaclasses.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/six_metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/six_remove_decorators.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/six_remove_decorators.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/six_simple.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/six_simple.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/subprocess_run.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/type_of_primitive.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/type_of_primitive.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from pyupgrade._ast_helpers import ast_to_offset
 from pyupgrade._data import register
 from pyupgrade._data import State
 from pyupgrade._data import TokenFunc
 from pyupgrade._token_helpers import find_closing_bracket
 from pyupgrade._token_helpers import find_open_paren
 
-NUM_TYPES = {
+_TYPES = {
+    bool: 'bool',
+    bytes: 'bytes',
+    str: 'str',
     int: 'int',
     float: 'float',
     complex: 'complex',
 }
 
 
 def _rewrite_type_of_primitive(
@@ -38,27 +41,16 @@
         state: State,
         node: ast.Call,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if (
             isinstance(node.func, ast.Name) and
             node.func.id == 'type' and
-            len(node.args) == 1
+            len(node.args) == 1 and
+            isinstance(node.args[0], ast.Constant) and
+            node.args[0].value not in {Ellipsis, None}
     ):
-        if isinstance(node.args[0], ast.Str):
-            func = functools.partial(
-                _rewrite_type_of_primitive,
-                src='str',
-            )
-            yield ast_to_offset(node), func
-        elif isinstance(node.args[0], ast.Bytes):
-            func = functools.partial(
-                _rewrite_type_of_primitive,
-                src='bytes',
-            )
-            yield ast_to_offset(node), func
-        elif isinstance(node.args[0], ast.Num):
-            func = functools.partial(
-                _rewrite_type_of_primitive,
-                src=NUM_TYPES[type(node.args[0].n)],
-            )
-            yield ast_to_offset(node), func
+        func = functools.partial(
+            _rewrite_type_of_primitive,
+            src=_TYPES[type(node.args[0].value)],
+        )
+        yield ast_to_offset(node), func
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_classes.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_classes.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,21 +34,24 @@
             if len(node_slice.elts) == 1:
                 slice_s = f'{_unparse(node_slice.elts[0])},'
             else:
                 slice_s = ', '.join(_unparse(elt) for elt in node_slice.elts)
         else:
             slice_s = _unparse(node_slice)
         return f'{_unparse(node.value)}[{slice_s}]'
-    elif isinstance(node, (ast.Str, ast.Bytes)):
-        return repr(node.s)
-    elif isinstance(node, ast.Ellipsis):
+    elif (
+            isinstance(node, ast.Constant) and
+            isinstance(node.value, (str, bytes))
+    ):
+        return repr(node.value)
+    elif isinstance(node, ast.Constant) and node.value is Ellipsis:
         return '...'
     elif isinstance(node, ast.List):
         return '[{}]'.format(', '.join(_unparse(elt) for elt in node.elts))
-    elif isinstance(node, ast.NameConstant):
+    elif isinstance(node, ast.Constant) and node.value in {True, False, None}:
         return repr(node.value)
     elif isinstance(node, ast.BinOp) and isinstance(node.op, ast.BitOr):
         return f'{_unparse(node.left)} | {_unparse(node.right)}'
     else:
         raise NotImplementedError(ast.dump(node))
 
 
@@ -93,15 +96,15 @@
 
     attrs = '\n'.join(parts)
     return end, attrs
 
 
 def _fix_named_tuple(i: int, tokens: list[Token], *, call: ast.Call) -> None:
     types = {
-        tup.elts[0].s: tup.elts[1]
+        tup.elts[0].value: tup.elts[1]
         for tup in call.args[1].elts  # type: ignore  # (checked below)
     }
     end, attrs = _typed_class_replacement(tokens, i, call, types)
     src = f'class {tokens[i].src}({_unparse(call.func)}):\n{attrs}'
     tokens[i:end] = [Token('CODE', src)]
 
 
@@ -119,15 +122,15 @@
 def _fix_dict_typed_dict(
         i: int,
         tokens: list[Token],
         *,
         call: ast.Call,
 ) -> None:
     types = {
-        k.s: v
+        k.value: v
         for k, v in zip(
             call.args[1].keys,  # type: ignore  # (checked below)
             call.args[1].values,  # type: ignore  # (checked below)
         )
     }
     if call.keywords:
         total = call.keywords[0].value.value  # type: ignore # (checked below)  # noqa: E501
@@ -156,16 +159,17 @@
 
     if (
             # NT = ...("NT", ...)
             len(node.targets) == 1 and
             isinstance(node.targets[0], ast.Name) and
             isinstance(node.value, ast.Call) and
             len(node.value.args) >= 1 and
-            isinstance(node.value.args[0], ast.Str) and
-            node.targets[0].id == node.value.args[0].s and
+            isinstance(node.value.args[0], ast.Constant) and
+            isinstance(node.value.args[0].value, str) and
+            node.targets[0].id == node.value.args[0].value and
             not has_starargs(node.value)
     ):
         if (
                 is_name_attr(
                     node.value.func,
                     state.from_imports,
                     ('typing',),
@@ -174,17 +178,18 @@
                 len(node.value.args) == 2 and
                 not node.value.keywords and
                 isinstance(node.value.args[1], (ast.List, ast.Tuple)) and
                 len(node.value.args[1].elts) > 0 and
                 all(
                     isinstance(tup, ast.Tuple) and
                     len(tup.elts) == 2 and
-                    isinstance(tup.elts[0], ast.Str) and
-                    tup.elts[0].s.isidentifier() and
-                    tup.elts[0].s not in KEYWORDS
+                    isinstance(tup.elts[0], ast.Constant) and
+                    isinstance(tup.elts[0].value, str) and
+                    tup.elts[0].value.isidentifier() and
+                    tup.elts[0].value not in KEYWORDS
                     for tup in node.value.args[1].elts
                 )
         ):
             func = functools.partial(_fix_named_tuple, call=node.value)
             yield ast_to_offset(node), func
         elif (
                 is_name_attr(
@@ -220,15 +225,16 @@
                             (ast.Constant, ast.NameConstant),
                         )
                     )
                 ) and
                 isinstance(node.value.args[1], ast.Dict) and
                 node.value.args[1].keys and
                 all(
-                    isinstance(k, ast.Str) and
-                    k.s.isidentifier() and
-                    k.s not in KEYWORDS
+                    isinstance(k, ast.Constant) and
+                    isinstance(k.value, str) and
+                    k.value.isidentifier() and
+                    k.value not in KEYWORDS
                     for k in node.value.args[1].keys
                 )
         ):
             func = functools.partial(_fix_dict_typed_dict, call=node.value)
             yield ast_to_offset(node), func
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep563.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep563.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,16 +109,16 @@
     nodes: list[ast.AST] = [annotation]
     while nodes:
         node = nodes.pop()
         if isinstance(node, ast.Call):
             nodes.extend(_process_call(node))
         elif isinstance(node, ast.Subscript):
             nodes.extend(_process_subscript(node))
-        elif isinstance(node, ast.Str):
-            func = functools.partial(_dequote, new=node.s)
+        elif isinstance(node, ast.Constant) and isinstance(node.value, str):
+            func = functools.partial(_dequote, new=node.value)
             yield ast_to_offset(node), func
         else:
             for name in node._fields:
                 value = getattr(node, name)
                 if isinstance(value, ast.AST):
                     nodes.append(value)
                 elif isinstance(value, list):
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep585.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep585.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep604.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep604.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,17 +124,24 @@
             )
         )
     )
 
 
 def _any_arg_is_str(node_slice: ast.expr) -> bool:
     return (
-        isinstance(node_slice, ast.Str) or (
+        (
+            isinstance(node_slice, ast.Constant) and
+            isinstance(node_slice.value, str)
+        ) or (
             isinstance(node_slice, ast.Tuple) and
-            any(isinstance(elt, ast.Str) for elt in node_slice.elts)
+            any(
+                isinstance(elt, ast.Constant) and
+                isinstance(elt.value, str)
+                for elt in node_slice.elts
+            )
         )
     )
 
 
 @register(ast.Subscript)
 def visit_Subscript(
         state: State,
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_pep646_unpack.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/typing_pep646_unpack.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/typing_text.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/unpack_list_comprehension.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from __future__ import annotations
 
 import ast
-import functools
 from typing import Iterable
 
 from tokenize_rt import Offset
+from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
+from pyupgrade._ast_helpers import is_async_listcomp
 from pyupgrade._data import register
 from pyupgrade._data import State
 from pyupgrade._data import TokenFunc
-from pyupgrade._token_helpers import replace_name
+from pyupgrade._token_helpers import find_closing_bracket
 
 
-@register(ast.Attribute)
-def visit_Attribute(
-        state: State,
-        node: ast.Attribute,
-        parent: ast.AST,
-) -> Iterable[tuple[Offset, TokenFunc]]:
-    if (
-            isinstance(node.value, ast.Name) and
-            node.value.id == 'typing' and
-            node.attr == 'Text'
-    ):
-        func = functools.partial(replace_name, name=node.attr, new='str')
-        yield ast_to_offset(node), func
+def _replace_list_comprehension(i: int, tokens: list[Token]) -> None:
+    start = i
+    end = find_closing_bracket(tokens, start)
+    tokens[start] = tokens[start]._replace(src='(')
+    tokens[end] = tokens[end]._replace(src=')')
 
 
-@register(ast.Name)
-def visit_Name(
+@register(ast.Assign)
+def visit_Assign(
         state: State,
-        node: ast.Name,
+        node: ast.Assign,
         parent: ast.AST,
 ) -> Iterable[tuple[Offset, TokenFunc]]:
-    if node.id in state.from_imports['typing'] and node.id == 'Text':
-        func = functools.partial(replace_name, name=node.id, new='str')
-        yield ast_to_offset(node), func
+    if (
+            len(node.targets) == 1 and
+            isinstance(node.targets[0], ast.Tuple) and
+            isinstance(node.value, ast.ListComp) and
+            not is_async_listcomp(node.value)
+    ):
+        yield ast_to_offset(node.value), _replace_list_comprehension
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/unittest_aliases.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/unittest_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_plugins/versioned_branches.py` & `pyupgrade-3.4.0/pyupgrade/_plugins/versioned_branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 import ast
 from typing import cast
 from typing import Iterable
-from typing import List
 
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from pyupgrade._ast_helpers import ast_to_offset
 from pyupgrade._ast_helpers import is_name_attr
 from pyupgrade._data import register
@@ -65,36 +64,39 @@
         del tokens[if_block.end:else_block.end]
         if_block.replace_condition(tokens, [Token('NAME', 'else')])
 
 
 def _eq(test: ast.Compare, n: int) -> bool:
     return (
         isinstance(test.ops[0], ast.Eq) and
-        isinstance(test.comparators[0], ast.Num) and
-        test.comparators[0].n == n
+        isinstance(test.comparators[0], ast.Constant) and
+        test.comparators[0].value == n
     )
 
 
 def _compare_to_3(
     test: ast.Compare,
     op: type[ast.cmpop] | tuple[type[ast.cmpop], ...],
     minor: int = 0,
 ) -> bool:
     if not (
             isinstance(test.ops[0], op) and
             isinstance(test.comparators[0], ast.Tuple) and
             len(test.comparators[0].elts) >= 1 and
-            all(isinstance(n, ast.Num) for n in test.comparators[0].elts)
+            all(
+                isinstance(n, ast.Constant) and isinstance(n.value, int)
+                for n in test.comparators[0].elts
+            )
     ):
         return False
 
     # checked above but mypy needs help
-    ast_elts = cast('List[ast.Num]', test.comparators[0].elts)
+    ast_elts = cast('list[ast.Constant]', test.comparators[0].elts)
     # padding a 0 for compatibility with (3,) used as a spec
-    elts = tuple(e.n for e in ast_elts) + (0,)
+    elts = tuple(e.value for e in ast_elts) + (0,)
 
     return elts[:2] == (3, minor) and all(n == 0 for n in elts[2:])
 
 
 @register(ast.If)
 def visit_If(
         state: State,
```

### Comparing `pyupgrade-3.3.2/pyupgrade/_string_helpers.py` & `pyupgrade-3.4.0/pyupgrade/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/pyupgrade/_token_helpers.py` & `pyupgrade-3.4.0/pyupgrade/_token_helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import ast
 import keyword
-import sys
 from typing import NamedTuple
 from typing import Sequence
 
 from tokenize_rt import NON_CODING_TOKENS
 from tokenize_rt import Token
 from tokenize_rt import tokens_to_src
 from tokenize_rt import UNIMPORTANT_WS
@@ -60,36 +59,19 @@
         i -= 1
     else:
         i += 1
 
     return i
 
 
-if sys.version_info >= (3, 8):  # pragma: >=3.8 cover
-    # python 3.8 fixed the offsets of generators / tuples
-    def _arg_token_index(tokens: list[Token], i: int, arg: ast.expr) -> int:
-        idx = _search_until(tokens, i, arg) + 1
-        while idx < len(tokens) and tokens[idx].name in NON_CODING_TOKENS:
-            idx += 1
-        return idx
-else:  # pragma: <3.8 cover
-    def _arg_token_index(tokens: list[Token], i: int, arg: ast.expr) -> int:
-        # lists containing non-tuples report the first element correctly
-        if isinstance(arg, ast.List):
-            # If the first element is a tuple, the ast lies to us about its col
-            # offset.  We must find the first `(` token after the start of the
-            # list element.
-            if isinstance(arg.elts[0], ast.Tuple):
-                i = _search_until(tokens, i, arg)
-                return find_open_paren(tokens, i)
-            else:
-                return _search_until(tokens, i, arg.elts[0])
-            # others' start position points at their first child node already
-        else:
-            return _search_until(tokens, i, arg)
+def _arg_token_index(tokens: list[Token], i: int, arg: ast.expr) -> int:
+    idx = _search_until(tokens, i, arg) + 1
+    while idx < len(tokens) and tokens[idx].name in NON_CODING_TOKENS:
+        idx += 1
+    return idx
 
 
 def victims(
         tokens: list[Token],
         start: int,
         arg: ast.expr,
         gen: bool,
@@ -495,25 +477,14 @@
     start_idx, end_idx = func_args[i]
     # don't replace leading whitespace / newlines
     while tokens[start_idx].name in {'UNIMPORTANT_WS', 'NL'}:
         start_idx += 1
     tokens[start_idx:end_idx] = [Token('SRC', new)]
 
 
-def find_comprehension_opening_bracket(i: int, tokens: list[Token]) -> int:
-    """Find opening bracket of comprehension given first argument."""
-    if sys.version_info < (3, 8):  # pragma: <3.8 cover
-        i -= 1
-        while not (tokens[i].name == 'OP' and tokens[i].src == '[') and i:
-            i -= 1
-        return i
-    else:  # pragma: >=3.8 cover
-        return i
-
-
 def has_space_before(i: int, tokens: list[Token]) -> bool:
     return i >= 1 and tokens[i - 1].name in {UNIMPORTANT_WS, 'INDENT'}
 
 
 def indented_amount(i: int, tokens: list[Token]) -> str:
     if i == 0:
         return ''
```

### Comparing `pyupgrade-3.3.2/pyupgrade.egg-info/PKG-INFO` & `pyupgrade-3.4.0/pyupgrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.3.2
+Version: 3.4.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
+    rev: v3.4.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
```

### Comparing `pyupgrade-3.3.2/pyupgrade.egg-info/SOURCES.txt` & `pyupgrade-3.4.0/pyupgrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.3.2/setup.cfg` & `pyupgrade-3.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyupgrade
-version = 3.3.2
+version = 3.4.0
 description = A tool to automatically upgrade syntax for newer versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/pyupgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
 	tokenize-rt>=3.2.0
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
 [options.entry_points]
```

