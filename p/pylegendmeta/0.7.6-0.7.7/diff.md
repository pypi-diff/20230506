# Comparing `tmp/pylegendmeta-0.7.6.tar.gz` & `tmp/pylegendmeta-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylegendmeta-0.7.6.tar", last modified: Thu Apr  6 14:26:23 2023, max compression
+gzip compressed data, was "pylegendmeta-0.7.7.tar", last modified: Fri Apr 21 13:53:16 2023, max compression
```

## Comparing `pylegendmeta-0.7.6.tar` & `pylegendmeta-0.7.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.596659 pylegendmeta-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.596659 pylegendmeta-0.7.6/src/legendmeta/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/legendmeta/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/jsondb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/police.py
--rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/scdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/slowcontrol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.596659 pylegendmeta-0.7.6/src/legendmeta/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/templates/geds-channel.json
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/src/legendmeta/templates/spms-channel.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.596659 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 14:26:23.000000 pylegendmeta-0.7.6/src/pylegendmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.596659 pylegendmeta-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/test_jsondb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/test_lmeta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/test_police.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/test_slowcontroldb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/tests/testdb/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/arrays.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/tests/testdb/dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/tests/testdb/dir1/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir1/dir2/file4.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir1/file3.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir1/file5.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir1/validity.jsonl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:26:23.600659 pylegendmeta-0.7.6/tests/testdb/dir2/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir2/file7.json
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/dir2/file8.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/file1.json
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/file2.json
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-06 14:26:13.000000 pylegendmeta-0.7.6/tests/testdb/file3.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.050768 pylegendmeta-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.050768 pylegendmeta-0.7.7/src/legendmeta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/legendmeta/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14443 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/jsondb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6218 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/scdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/slowcontrol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/src/legendmeta/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/templates/geds-channel.json
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/src/legendmeta/templates/spms-channel.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:53:15.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 13:53:16.000000 pylegendmeta-0.7.7/src/pylegendmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/test_jsondb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/test_lmeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/test_police.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/test_slowcontroldb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/tests/testdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/arrays.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/tests/testdb/dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/tests/testdb/dir1/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir1/dir2/file4.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir1/file3.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir1/file5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir1/validity.jsonl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:53:16.054768 pylegendmeta-0.7.7/tests/testdb/dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir2/file7.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/dir2/file8.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/file1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/file2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 13:53:07.000000 pylegendmeta-0.7.7/tests/testdb/file3.json
```

### Comparing `pylegendmeta-0.7.6/LICENSE` & `pylegendmeta-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/PKG-INFO` & `pylegendmeta-0.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylegendmeta
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python LEGEND-metadata implementation
 Home-page: https://github.com/legend-exp/pylegendmeta
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pylegendmeta-0.7.6/README.md` & `pylegendmeta-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/setup.cfg` & `pylegendmeta-0.7.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/__init__.py` & `pylegendmeta-0.7.7/src/legendmeta/__init__.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/catalog.py` & `pylegendmeta-0.7.7/src/legendmeta/catalog.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/core.py` & `pylegendmeta-0.7.7/src/legendmeta/core.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/jsondb.py` & `pylegendmeta-0.7.7/src/legendmeta/jsondb.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/police.py` & `pylegendmeta-0.7.7/src/legendmeta/police.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/scdb_tables.py` & `pylegendmeta-0.7.7/src/legendmeta/scdb_tables.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/src/legendmeta/slowcontrol.py` & `pylegendmeta-0.7.7/src/legendmeta/slowcontrol.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 
         return db.orm.Session(self.connection)
 
     def get_tables(self) -> list[str]:
         """Get tables available in the database."""
         return db.inspect(self.connection.engine).get_table_names()
 
+    def get_columns(self, table: str) -> list[str]:
+        """Get columns available on `table` in the database."""
+        return db.inspect(self.connection.engine).get_columns(table)
+
     def dataframe(self, expr: str | db.sql.Select) -> pandas.DataFrame:
         """Query the database and return a dataframe holding the result.
 
         Parameters
         ----------
         expr
             SQL table name, select SQL command text or SQLAlchemy selectable
```

### Comparing `pylegendmeta-0.7.6/src/pylegendmeta.egg-info/PKG-INFO` & `pylegendmeta-0.7.7/src/pylegendmeta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylegendmeta
-Version: 0.7.6
+Version: 0.7.7
 Summary: Python LEGEND-metadata implementation
 Home-page: https://github.com/legend-exp/pylegendmeta
 Author: Luigi Pertoldi
 Author-email: gipert@pm.me
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pylegendmeta-0.7.6/src/pylegendmeta.egg-info/SOURCES.txt` & `pylegendmeta-0.7.7/src/pylegendmeta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/tests/test_jsondb.py` & `pylegendmeta-0.7.7/tests/test_jsondb.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/tests/test_lmeta.py` & `pylegendmeta-0.7.7/tests/test_lmeta.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/tests/test_police.py` & `pylegendmeta-0.7.7/tests/test_police.py`

 * *Files identical despite different names*

### Comparing `pylegendmeta-0.7.6/tests/test_slowcontroldb.py` & `pylegendmeta-0.7.7/tests/test_slowcontroldb.py`

 * *Files identical despite different names*

