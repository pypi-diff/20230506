# Comparing `tmp/ConcurrentDatabase-0.0.4.tar.gz` & `tmp/ConcurrentDatabase-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConcurrentDatabase-0.0.4.tar", last modified: Tue May  2 21:09:45 2023, max compression
+gzip compressed data, was "ConcurrentDatabase-0.0.5.tar", last modified: Sat May  6 21:49:01 2023, max compression
```

## Comparing `ConcurrentDatabase-0.0.4.tar` & `ConcurrentDatabase-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/ConcurrentDatabase/
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/ColumnWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/Database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicTable.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-02 21:09:45.000000 ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 21:09:45.753652 ConcurrentDatabase-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-02 21:09:31.000000 ConcurrentDatabase-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/ConcurrentDatabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/ColumnWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/Database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15546 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-06 21:49:01.000000 ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:49:01.785019 ConcurrentDatabase-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-06 21:48:50.000000 ConcurrentDatabase-0.0.5/setup.py
```

### Comparing `ConcurrentDatabase-0.0.4/ConcurrentDatabase/ColumnWrapper.py` & `ConcurrentDatabase-0.0.5/ConcurrentDatabase/ColumnWrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 from loguru import logger as logging
 
 
 class ColumnWrapper:
 
     def __init__(self, table, pragma):
         self.table = table
+
+        # Result of pragma table_info (position, name, type, notnull, default_value, primary_key)
         self.position = pragma[0]  # type: int
         self.name = pragma[1]  # type: str
         self.type = pragma[2].upper()  # type: str
         self.not_null = pragma[3]  # type: int
         self.default_value = pragma[4]  # type: str
         self.primary_key = pragma[5]  # type: int
 
+        # Used for foreign keys
+        self.is_foreign_key = False  # type: bool
+        self.is_child = False  # type: bool
+        self.linked_table = None  # type: DynamicTable or None
+        self.linked_column = None  # type: ColumnWrapper or None
+
         if self.primary_key:
             self.table.primary_keys.append(self)
 
+    def attach_linked_table(self, linked_table, linked_column, child: bool = False):
+        self.is_foreign_key = True
+        self.is_child = child
+        self.linked_table = linked_table
+        self.linked_column = linked_column
+
     def validate(self, value):
 
         if (self.not_null and value is None) and self.default_value == "":
             raise ValueError(f"Column {self.name} cannot be null")
         elif value is None:
             return
 
@@ -46,16 +60,17 @@
         elif self.type == "BOOLEAN":
             if not isinstance(value, bool):
                 raise ValueError(f"Column {self.name} must of exact type {self.type}")
         else:
             logging.warning(f"Unknown column type {self.type}")
 
     def __str__(self):
-        return f"[{self.position}]{'-PRIMARY KEY' if self.primary_key else ''}-{self.name}-({self.type})-" \
-               f"{'NOT NULL' if self.not_null else ''}-{'DEFAULT ' + self.default_value if self.default_value else ''}"
+        return f"[{self.position}]{'-PRIMARY KEY' if self.primary_key else ''}-{self.name}-({self.type})" \
+               f"{'-NOT NULL' if self.not_null else ''}" \
+               f"{'-DEFAULT ' + self.default_value if self.default_value else ''}"
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other):
         if isinstance(other, ColumnWrapper):
             return self.name == other.name
```

### Comparing `ConcurrentDatabase-0.0.4/ConcurrentDatabase/DynamicEntry.py` & `ConcurrentDatabase-0.0.5/ConcurrentDatabase/DynamicEntry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import time
+
+from loguru import logger as logging
+
+
 class DynamicEntry:
     """
     A class that allows you to access an entry in a database as if it were an object.
     """
 
     def __init__(self, table, load_tuple=None, **kwargs):
         self.columns = table.columns
         self.table = table
         self.database = table.database
         self.primary_keys = table.primary_keys
+        self._rowid = None
         self._values = {}
         self._previous_values = {}
         self._dirty = False
 
         if load_tuple is not None:
             for i in range(len(load_tuple)):
                 if i < len(self.columns):
@@ -50,22 +56,22 @@
         Sets the value of the entry but does not flush the changes to the database
         :param key: The column to set
         :param value: The value to set
         :return:
         """
         if isinstance(key, int):  # Select by index
             if len(self.columns) > key >= 0:
-                self._values[self.columns[key].name] = value
                 self._dirty = True
+                self._values[self.columns[key].name] = value
             else:
                 raise IndexError(f"Column index {key} is out of range for table {self.table.table_name}")
         elif isinstance(key, str):  # Select by column name
             if key in self.columns:
-                self._values[key] = value
                 self._dirty = True
+                self._values[key] = value
             else:
                 raise KeyError(f"Column {key} does not exist in table {self.table.table_name}")
         else:
             raise TypeError(f"Invalid key type {type(key)}")
 
     def set(self, **kwargs):
         """
@@ -77,28 +83,41 @@
             if key in self.columns:
                 self._dirty = True
                 self._values[key] = kwargs[key]
             else:
                 raise KeyError(f"Column {key} does not exist in table {self.table.table_name}")
         self.flush()
 
-    def get(self, key):
+    def get(self, key) -> any:
+        """
+        Gets the value of a particular column of this entry or if there is a ForeignKey constraint, gets the entry(s)
+        that this entry references
+        """
         # This form of item setting accesses the database
         if key in self.columns:
             self.refresh()
             return self._values[key]
+        # If the key is not a column, check if it is a name of a foreign table
+        elif key in [foreign_table.table_name for foreign_table in self.table.foreign_tables]:
+            foreign_table = [foreign_table for foreign_table in
+                             self.table.foreign_tables if foreign_table.table_name == key][0]
+            return foreign_table.get_related_entries(self)
         else:
             raise KeyError(f"Column {key} does not exist in table {self.table.table_name}")
 
     def flush(self):
         """
         Flushes the changes to the database if there are any
         :return:
         """
+
         if self._dirty:
+            if not self.database.open:
+                logging.warning(f"Unable to flush changes to {self.table.table_name} because the database is closed")
+                return
             # Build the query
             changed_values = {}
             for key in self._values:
                 if key in self._previous_values and self._values[key] != self._previous_values[key]:
                     changed_values[key] = self._values[key]
                 elif key not in self._previous_values:
                     changed_values[key] = self._values[key]
@@ -135,34 +154,41 @@
                 return ""
             sql = f"UPDATE {self.table.table_name} SET "
             for key, value in changed_values.items():
                 column = self.columns[self.columns.index(key)]
                 sql += f"{key} = {column.safe_value(value)}, "
             sql = sql[:-2] if sql.endswith(", ") else sql
             sql += f" WHERE {self._entry_where_clause()}"
+            self._dirty = False
             return sql
 
     def refresh(self):
         """
         Refreshes the values from the database
         :return:
         """
         sql = f"SELECT * FROM {self.table.table_name} WHERE {self._entry_where_clause()}"
-        self._values = {self.columns[i].name: value for i, value in enumerate(self.database.run(sql).fetchone())}
+        result = self.database.run(sql)
+        if result.rowcount == 0:
+            raise KeyError(f"Entry does not exist in table {self.table.table_name}")
+        self._values = {self.columns[i].name: value for i, value in enumerate(result.fetchone())}
 
     def delete(self):
         """
         Deletes the entry from the database
         :return:
         """
         primary_key_values = [self._values[column.name] for column in self.columns if column.primary_key]
         sql = f"DELETE FROM {self.table.table_name} WHERE {self._entry_where_clause()}"
         self.database.run(sql, tuple(primary_key_values))
         del self
 
+    def is_dirty(self):
+        return self._dirty
+
     def _entry_where_clause(self):
         """
         Returns a complete WHERE clause to find this entry in the database even if the table has no primary keys
         Will contain no ?'s and will be ready to be inserted into a SQL statement
         :return:
         """
         primary_keys = [column.name for column in self.columns if column.primary_key]
@@ -195,15 +221,21 @@
         return len(self.columns)
 
     def __str__(self):
         # The primary keys should be prefixed with a * to indicate that they are primary keys
         string = f"{self.table.table_name}("
         for i, column in enumerate(self.columns):
             if column.primary_key:
-                string += f"*{column.name}={self._values[column.name]}"
+                string += "*"
+            if column.is_foreign_key:
+                string += "!" if column.is_child else "¡"
+            # Check if the column is dirty
+            if column.name in self._previous_values and \
+                    self._values[column.name] != self._previous_values[column.name]:
+                string += f"*{column.name}={self._values[column.name] if column.name in self._values else None}"
             else:
                 string += f"{column.name}={self._values[column.name] if column.name in self._values else None}"
             if i != len(self.columns) - 1:
                 string += ", "
         string += ")"
         return string
 
@@ -212,17 +244,38 @@
 
     def __hash__(self):
         """Return a hash of the primary key."""
         return hash(tuple(self.primary_keys))
 
     def __eq__(self, other):
         if isinstance(other, DynamicEntry):
-            return self.primary_keys == other.primary_keys
+            if self.table.table_name != other.table.table_name:
+                raise ValueError("Cannot compare entries from different tables")
+            for column in self.columns:
+                if column not in other.columns:  # This would be unexpected as they should be from the same table
+                    raise TypeError(f"Unexpected column {column.name} in entry {other}")
+                if self._values[column.name] != other._values[column.name]:
+                    return False
+            return True
         elif isinstance(other, tuple):
-            return self.primary_keys == other
+            if len(other) != len(self.columns):
+                raise ValueError("Tuple must be the same length as the number of columns in the table")
+            for i, column in enumerate(self.columns):
+                if self._values[column.name] != other[i]:
+                    return False
+            return True
         elif isinstance(other, dict):
-            if self.primary_keys:
-                return self.primary_keys == tuple(other[key] for key in self.primary_keys)
-            else:  # compare all values
-                return self._values == other
+            for key in other:
+                if key not in self._values:
+                    raise KeyError(f"Key {key} not in entry")
+                if self._values[key] != other[key]:
+                    return False
+            return True
         else:
             raise TypeError(f"Cannot compare DynamicEntry to {type(other)}")
+
+    def __del__(self):
+        """
+        Called when the DynamicEntry object is garbage collected, flushes the entry to the database to prevent data loss
+        """
+        if self._dirty:
+            self.flush()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ConcurrentDatabase-0.0.4/ConcurrentDatabase.egg-info/PKG-INFO` & `ConcurrentDatabase-0.0.5/ConcurrentDatabase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.4/PKG-INFO` & `ConcurrentDatabase-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConcurrentDatabase
-Version: 0.0.4
+Version: 0.0.5
 Summary: A SQLite wrapper that allows for object oriented database access.
 Home-page: 
 Author: Jay S
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `ConcurrentDatabase-0.0.4/README.md` & `ConcurrentDatabase-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ConcurrentDatabase-0.0.4/pyproject.toml` & `ConcurrentDatabase-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "ConcurrentDatabase"
 author = "Jay S"
 author_email = ""
-version = "0.0.4"
+version = "0.0.5"
 description = "A simple wrapper allow for treating an SQLite database as an object oriented structure"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ConcurrentDatabase-0.0.4/setup.py` & `ConcurrentDatabase-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ConcurrentDatabase",
-    version="0.0.4",
+    version="0.0.5",
     author="Jay S",
     author_email="",
     description="A SQLite wrapper that allows for object oriented database access.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

