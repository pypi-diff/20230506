# Comparing `tmp/tksheet-6.1.0.tar.gz` & `tmp/tksheet-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.1.0.tar", last modified: Thu May  4 18:23:08 2023, max compression
+gzip compressed data, was "tksheet-6.1.1.tar", last modified: Sat May  6 18:18:43 2023, max compression
```

## Comparing `tksheet-6.1.0.tar` & `tksheet-6.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 18:23:08.061976 tksheet-6.1.0/
--rw-rw-rw-   0        0        0     1101 2023-05-04 16:44:53.000000 tksheet-6.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3548 2023-05-04 18:23:08.061976 tksheet-6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2898 2023-05-04 17:18:34.000000 tksheet-6.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-05-04 18:23:08.061976 tksheet-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-04 18:18:39.000000 tksheet-6.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:23:08.061976 tksheet-6.1.0/tksheet/
--rw-rw-rw-   0        0        0      344 2023-05-04 16:44:53.000000 tksheet-6.1.0/tksheet/__init__.py
--rw-rw-rw-   0        0        0   169752 2023-05-04 17:01:52.000000 tksheet-6.1.0/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0   117473 2023-05-04 17:34:49.000000 tksheet-6.1.0/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0     8893 2023-05-04 17:07:18.000000 tksheet-6.1.0/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   346920 2023-05-04 17:57:20.000000 tksheet-6.1.0/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12757 2023-05-04 16:51:42.000000 tksheet-6.1.0/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0   113971 2023-05-04 18:12:11.000000 tksheet-6.1.0/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5789 2023-05-04 16:51:36.000000 tksheet-6.1.0/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    59987 2023-05-04 16:51:30.000000 tksheet-6.1.0/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-05-04 18:23:08.061976 tksheet-6.1.0/tksheet.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-05-04 18:23:08.000000 tksheet-6.1.0/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-05-04 18:23:08.000000 tksheet-6.1.0/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 18:23:08.000000 tksheet-6.1.0/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-04 18:23:08.000000 tksheet-6.1.0/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/
+-rw-rw-rw-   0        0        0     1101 2023-05-06 15:11:23.000000 tksheet-6.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3548 2023-05-06 18:18:43.812937 tksheet-6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2898 2023-05-06 15:11:23.000000 tksheet-6.1.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-06 18:18:43.828574 tksheet-6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-05-06 15:12:58.000000 tksheet-6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/tksheet/
+-rw-rw-rw-   0        0        0      344 2023-05-06 15:11:23.000000 tksheet-6.1.1/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   169752 2023-05-06 15:11:23.000000 tksheet-6.1.1/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0   117473 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0     8893 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   346731 2023-05-06 18:11:05.000000 tksheet-6.1.1/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12757 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0   113971 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5789 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    59987 2023-05-06 15:11:24.000000 tksheet-6.1.1/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:18:43.812937 tksheet-6.1.1/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 18:18:43.000000 tksheet-6.1.1/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.1.0/LICENSE.txt` & `tksheet-6.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/PKG-INFO` & `tksheet-6.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.0
+Version: 6.1.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `tksheet-6.1.0/README.md` & `tksheet-6.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/setup.py` & `tksheet-6.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.1.0',
+  version = '6.1.1',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.0.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.1.0/tksheet/_tksheet.py` & `tksheet-6.1.1/tksheet/_tksheet.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_column_headers.py` & `tksheet-6.1.1/tksheet/_tksheet_column_headers.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_formatters.py` & `tksheet-6.1.1/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_main_table.py` & `tksheet-6.1.1/tksheet/_tksheet_main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -7255,19 +7255,15 @@
         return True
 
     def set_cell_data(self, datarn, datacn, value, kwargs={}, expand_sheet=True):
         if expand_sheet:
             if datarn >= len(self.data):
                 self.fix_data_len(datarn, datacn)
             elif datacn >= len(self.data[datarn]):
-                self.data[datarn].extend(
-                    self.get_empty_row_seq(
-                        datarn, end=datacn + 1, start=len(self.data[datarn])
-                    )
-                )
+                self.fix_row_len(datarn, datacn)
         if expand_sheet or (
             len(self.data) > datarn and len(self.data[datarn]) > datacn
         ):
             if (
                 datarn,
                 datacn,
             ) in self.cell_options and "checkbox" in self.cell_options[
@@ -7310,37 +7306,30 @@
     def get_empty_row_seq(self, datarn, end, start=0, r_ops=True, c_ops=True):
         return [
             self.get_value_for_empty_cell(datarn, datacn, r_ops=r_ops, c_ops=c_ops)
             for datacn in range(start, end)
         ]
 
     def fix_row_len(self, datarn, datacn):
-        self.data[datarn].extend(
-            [
-                self.get_value_for_empty_cell(datarn, cn)
-                for cn in range(datacn + 1 - len(self.data[datarn]))
-            ]
-        )
+        self.data[datarn].extend(self.get_empty_row_seq(datarn, 
+                                                        end = datacn + 1, 
+                                                        start = len(self.data[datarn])))
 
     def fix_row_values(self, datarn, start=None, end=None):
         if datarn < len(self.data):
             for datacn, v in enumerate(islice(self.data[datarn], start, end)):
                 if not self.input_valid_for_cell(datarn, datacn, v):
                     self.data[datarn][datacn] = self.get_value_for_empty_cell(
                         datarn, datacn
                     )
 
     def fix_data_len(self, datarn, datacn):
         ncols = self.total_data_cols() if datacn is None else datacn + 1
-        self.data.extend(
-            [
-                [self.get_value_for_empty_cell(rn, cn) for cn in range(ncols)]
-                for rn in range(datarn + 1 - len(self.data))
-            ]
-        )
+        self.data.extend([self.get_empty_row_seq(rn, end = ncols, start = 0) 
+                          for rn in range(len(self.data), datarn + 1)])
 
     # internal event use
     def click_checkbox(self, r, c, datarn=None, datacn=None, undo=True, redraw=True):
         if datarn is None:
             datarn = r if self.all_rows_displayed else self.displayed_rows[r]
         if datacn is None:
             datacn = c if self.all_columns_displayed else self.displayed_columns[c]
```

### Comparing `tksheet-6.1.0/tksheet/_tksheet_other_classes.py` & `tksheet-6.1.1/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_row_index.py` & `tksheet-6.1.1/tksheet/_tksheet_row_index.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.1.1/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet/_tksheet_vars.py` & `tksheet-6.1.1/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.1.0/tksheet.egg-info/PKG-INFO` & `tksheet-6.1.1/tksheet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.1.0
+Version: 6.1.1
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.1.0.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.1.1.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

