# Comparing `tmp/excel_cleaner-0.0.15.tar.gz` & `tmp/excel_cleaner-0.0.16.tar.gz`

## Comparing `excel_cleaner-0.0.15.tar` & `excel_cleaner-0.0.16.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/updatePackage.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/src/excel_cleaner/__init__.py
--rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/src/excel_cleaner/_excelCleaner.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/test/MG-158427.xlsx
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/test/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/LICENSE.txt
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/README.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/updatePackage.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/src/excel_cleaner/__init__.py
+-rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/src/excel_cleaner/_excelCleaner.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/test/MG-158427.xlsx
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/test/test.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/LICENSE.txt
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/README.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 excel_cleaner-0.0.16/PKG-INFO
```

### Comparing `excel_cleaner-0.0.15/updatePackage.txt` & `excel_cleaner-0.0.16/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.15/src/excel_cleaner/_excelCleaner.py` & `excel_cleaner-0.0.16/src/excel_cleaner/_excelCleaner.py`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.15/test/MG-158427.xlsx` & `excel_cleaner-0.0.16/test/MG-158427.xlsx`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.15/LICENSE.txt` & `excel_cleaner-0.0.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.15/README.md` & `excel_cleaner-0.0.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.15</li>
+<li>Version 0.0.16</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
-<li>F10: split a column to two columns with a particular string</li></ol></ul>
-<ul><li>Added an option to save processes to a file</li>
+<li>F10: split a column to two columns with a particular string</li></ol>
+<li>Added an option to save processes to a file</li>
 <ul><li>The processes saved in the file can be executed to speed the process until wanted cleaning is completed.</li></ul>
-<ul><li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
+<li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
 </ul>
 <br>
 
 <li>Version 0.0.10</li>
 <ul><li>Restoring just the data before the last action is extended to data of all actions since the first action.</li>
 <li>Changed function keys for actions.</li>
 <li>Screen displays the selected row where the next action is needed.</li></ul>
```

#### html2text {}

```diff
@@ -1,83 +1,79 @@
 # excel_cleaner ## What is it? A package that helps you clean and recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.15
+    * Version 0.0.16
           o Added function-key features
                1. F1: delete rows or columns
                2. F2: delete rows having a particular cell
                3. F3: combine rows or columns
                4. F4: combine selected rows
                5. F5: insert a cell to row and repeat the process to other rows
                   in the same pattern
                6. F7: delete a cell to row and repeat the process to other rows
                   in the same pattern
                7. F10: split a column to two columns with a particular string
           o Added an option to save processes to a file
                 # The processes saved in the file can be executed to speed the
                   process until wanted cleaning is completed.
-                # Clicking a row provides the rows having the same pattern of
-                  the cells in row
-    *
-    * Version 0.0.10
-          o Restoring just the data before the last action is extended to data
-            of all actions since the first action.
-          o Changed function keys for actions.
-          o Screen displays the selected row where the next action is needed.
-    *
-    * Version 0.0.9
-          o A tiny bug of renaming a cleaned xlsx file was fixed.
-    *
-    * Version 0.0.7
-          o Added some help:
-               1. When a column is all None, it will be deleted without any
-                  notice.
-               2. Rows in a pattern that takes place at the least number of
-                  rows will be highlighted.
-               3. The first row of the rows will be selected and is ready for
-                  next action. This selection is only a hint and should not be
-                  followed unless otherwise.
-    *
-    * Version 0.0.5
-          o Disabled some bindings that belong to tksheet package.
-    *
-    * Version 0.0.4
-    * ```python import excel_cleaner as xl xlpath='(excel file name with
-      extension)' xl.sheet(xlpath) ```
-          o A tksheet window will be opened with the contents of excel file.
-          o Here are recommending orders of actions to try:
-               1. Remove unwanted rows (F1) first
-               2. Remove unwanted columns (F1) or combine columns (F3)
-               3. Click a cell to insert (F5) or delete the cell (F7)
-          o
-          o If the same pattern or kind of selected rows/columns is found at
-            other locations, the same action is repeated for the found rows/
-            columns.
-                # Thus, it would better try one action at the top
-                # To remove rows, click and drag the row names.
-                # To remove or combine columns, click and drag the column
-                  names.
-          o
-          o When rows or columns are to be combined, the cells of the same rows
-            or columns are combined.
-          o
-          o After every action, the contents will be saved to a file that is
-            the original name with a string "_cleaned".
-          o When a cell is inserted, all values to the right are moved to the
-            right, and an empty cell is added at the end of all other unchanged
-            rows.
-          o When a cell is deleted, all the values ââon the right are moved
-            to the left and the last column is empty.
-          o
-          o If one action is done by mistake, press comination key (control-z)
-            to restore the the data before he last action
+          o Clicking a row provides the rows having the same pattern of the
+            cells in row
+
+Version 0.0.10
+    * Restoring just the data before the last action is extended to data of all
+      actions since the first action.
+    * Changed function keys for actions.
+    * Screen displays the selected row where the next action is needed.
+
+Version 0.0.9
+    * A tiny bug of renaming a cleaned xlsx file was fixed.
+
+Version 0.0.7
+    * Added some help:
+         1. When a column is all None, it will be deleted without any notice.
+         2. Rows in a pattern that takes place at the least number of rows will
+            be highlighted.
+         3. The first row of the rows will be selected and is ready for next
+            action. This selection is only a hint and should not be followed
+            unless otherwise.
+
+Version 0.0.5
+    * Disabled some bindings that belong to tksheet package.
+
+Version 0.0.4
+```python import excel_cleaner as xl xlpath='(excel file name with extension)'
+xl.sheet(xlpath) ```
+    * A tksheet window will be opened with the contents of excel file.
+    * Here are recommending orders of actions to try:
+         1. Remove unwanted rows (F1) first
+         2. Remove unwanted columns (F1) or combine columns (F3)
+         3. Click a cell to insert (F5) or delete the cell (F7)
+    *
+    * If the same pattern or kind of selected rows/columns is found at other
+      locations, the same action is repeated for the found rows/columns.
+          o Thus, it would better try one action at the top
+          o To remove rows, click and drag the row names.
+          o To remove or combine columns, click and drag the column names.
+    *
+    * When rows or columns are to be combined, the cells of the same rows or
+      columns are combined.
+    *
+    * After every action, the contents will be saved to a file that is the
+      original name with a string "_cleaned".
+    * When a cell is inserted, all values to the right are moved to the right,
+      and an empty cell is added at the end of all other unchanged rows.
+    * When a cell is deleted, all the values ââon the right are moved to
+      the left and the last column is empty.
     *
-          o After each action is completed,
-                # the number of columns and rows and the number of patterns of
-                  rows will be displayed
-                # either a few columns or muliple rows are highlighted, which
-                  are indicative of ok to be deleted.
+    * If one action is done by mistake, press comination key (control-z) to
+      restore the the data before he last action
+
+    * After each action is completed,
+          o the number of columns and rows and the number of patterns of rows
+            will be displayed
+          o either a few columns or muliple rows are highlighted, which are
+            indicative of ok to be deleted.
```

### Comparing `excel_cleaner-0.0.15/pyproject.toml` & `excel_cleaner-0.0.16/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_cleaner"
-version = "0.0.15"
+version = "0.0.16"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you clean and recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excel_cleaner-0.0.15/PKG-INFO` & `excel_cleaner-0.0.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_cleaner
-Version: 0.0.15
+Version: 0.0.16
 Summary: A small packages that helps you clean and recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excel_cleaner
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -30,26 +30,26 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.15</li>
+<li>Version 0.0.16</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
-<li>F10: split a column to two columns with a particular string</li></ol></ul>
-<ul><li>Added an option to save processes to a file</li>
+<li>F10: split a column to two columns with a particular string</li></ol>
+<li>Added an option to save processes to a file</li>
 <ul><li>The processes saved in the file can be executed to speed the process until wanted cleaning is completed.</li></ul>
-<ul><li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
+<li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
 </ul>
 <br>
 
 <li>Version 0.0.10</li>
 <ul><li>Restoring just the data before the last action is extended to data of all actions since the first action.</li>
 <li>Changed function keys for actions.</li>
 <li>Screen displays the selected row where the next action is needed.</li></ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.15 Summary: A small
+Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.16 Summary: A small
 packages that helps you clean and recover columns of Excel data converted from
 PDF files. Project-URL: Homepage, https://github.com/generateNscore/
 excel_cleaner Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -13,83 +13,79 @@
 markdown # excel_cleaner ## What is it? A package that helps you clean and
 recover columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.15
+    * Version 0.0.16
           o Added function-key features
                1. F1: delete rows or columns
                2. F2: delete rows having a particular cell
                3. F3: combine rows or columns
                4. F4: combine selected rows
                5. F5: insert a cell to row and repeat the process to other rows
                   in the same pattern
                6. F7: delete a cell to row and repeat the process to other rows
                   in the same pattern
                7. F10: split a column to two columns with a particular string
           o Added an option to save processes to a file
                 # The processes saved in the file can be executed to speed the
                   process until wanted cleaning is completed.
-                # Clicking a row provides the rows having the same pattern of
-                  the cells in row
-    *
-    * Version 0.0.10
-          o Restoring just the data before the last action is extended to data
-            of all actions since the first action.
-          o Changed function keys for actions.
-          o Screen displays the selected row where the next action is needed.
-    *
-    * Version 0.0.9
-          o A tiny bug of renaming a cleaned xlsx file was fixed.
-    *
-    * Version 0.0.7
-          o Added some help:
-               1. When a column is all None, it will be deleted without any
-                  notice.
-               2. Rows in a pattern that takes place at the least number of
-                  rows will be highlighted.
-               3. The first row of the rows will be selected and is ready for
-                  next action. This selection is only a hint and should not be
-                  followed unless otherwise.
-    *
-    * Version 0.0.5
-          o Disabled some bindings that belong to tksheet package.
-    *
-    * Version 0.0.4
-    * ```python import excel_cleaner as xl xlpath='(excel file name with
-      extension)' xl.sheet(xlpath) ```
-          o A tksheet window will be opened with the contents of excel file.
-          o Here are recommending orders of actions to try:
-               1. Remove unwanted rows (F1) first
-               2. Remove unwanted columns (F1) or combine columns (F3)
-               3. Click a cell to insert (F5) or delete the cell (F7)
-          o
-          o If the same pattern or kind of selected rows/columns is found at
-            other locations, the same action is repeated for the found rows/
-            columns.
-                # Thus, it would better try one action at the top
-                # To remove rows, click and drag the row names.
-                # To remove or combine columns, click and drag the column
-                  names.
-          o
-          o When rows or columns are to be combined, the cells of the same rows
-            or columns are combined.
-          o
-          o After every action, the contents will be saved to a file that is
-            the original name with a string "_cleaned".
-          o When a cell is inserted, all values to the right are moved to the
-            right, and an empty cell is added at the end of all other unchanged
-            rows.
-          o When a cell is deleted, all the values ââon the right are moved
-            to the left and the last column is empty.
-          o
-          o If one action is done by mistake, press comination key (control-z)
-            to restore the the data before he last action
+          o Clicking a row provides the rows having the same pattern of the
+            cells in row
+
+Version 0.0.10
+    * Restoring just the data before the last action is extended to data of all
+      actions since the first action.
+    * Changed function keys for actions.
+    * Screen displays the selected row where the next action is needed.
+
+Version 0.0.9
+    * A tiny bug of renaming a cleaned xlsx file was fixed.
+
+Version 0.0.7
+    * Added some help:
+         1. When a column is all None, it will be deleted without any notice.
+         2. Rows in a pattern that takes place at the least number of rows will
+            be highlighted.
+         3. The first row of the rows will be selected and is ready for next
+            action. This selection is only a hint and should not be followed
+            unless otherwise.
+
+Version 0.0.5
+    * Disabled some bindings that belong to tksheet package.
+
+Version 0.0.4
+```python import excel_cleaner as xl xlpath='(excel file name with extension)'
+xl.sheet(xlpath) ```
+    * A tksheet window will be opened with the contents of excel file.
+    * Here are recommending orders of actions to try:
+         1. Remove unwanted rows (F1) first
+         2. Remove unwanted columns (F1) or combine columns (F3)
+         3. Click a cell to insert (F5) or delete the cell (F7)
+    *
+    * If the same pattern or kind of selected rows/columns is found at other
+      locations, the same action is repeated for the found rows/columns.
+          o Thus, it would better try one action at the top
+          o To remove rows, click and drag the row names.
+          o To remove or combine columns, click and drag the column names.
+    *
+    * When rows or columns are to be combined, the cells of the same rows or
+      columns are combined.
+    *
+    * After every action, the contents will be saved to a file that is the
+      original name with a string "_cleaned".
+    * When a cell is inserted, all values to the right are moved to the right,
+      and an empty cell is added at the end of all other unchanged rows.
+    * When a cell is deleted, all the values ââon the right are moved to
+      the left and the last column is empty.
     *
-          o After each action is completed,
-                # the number of columns and rows and the number of patterns of
-                  rows will be displayed
-                # either a few columns or muliple rows are highlighted, which
-                  are indicative of ok to be deleted.
+    * If one action is done by mistake, press comination key (control-z) to
+      restore the the data before he last action
+
+    * After each action is completed,
+          o the number of columns and rows and the number of patterns of rows
+            will be displayed
+          o either a few columns or muliple rows are highlighted, which are
+            indicative of ok to be deleted.
```

