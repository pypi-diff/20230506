# Comparing `tmp/excel_cleaner-0.0.14.tar.gz` & `tmp/excel_cleaner-0.0.15.tar.gz`

## Comparing `excel_cleaner-0.0.14.tar` & `excel_cleaner-0.0.15.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/updatePackage.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/src/excel_cleaner/__init__.py
--rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/src/excel_cleaner/_excelCleaner.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/test/MG-158427.xlsx
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/test/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/LICENSE.txt
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/pyproject.toml
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/updatePackage.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/src/excel_cleaner/__init__.py
+-rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/src/excel_cleaner/_excelCleaner.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/test/MG-158427.xlsx
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/test/test.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/LICENSE.txt
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/README.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/pyproject.toml
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 excel_cleaner-0.0.15/PKG-INFO
```

### Comparing `excel_cleaner-0.0.14/updatePackage.txt` & `excel_cleaner-0.0.15/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.14/src/excel_cleaner/_excelCleaner.py` & `excel_cleaner-0.0.15/src/excel_cleaner/_excelCleaner.py`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.14/test/MG-158427.xlsx` & `excel_cleaner-0.0.15/test/MG-158427.xlsx`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.14/LICENSE.txt` & `excel_cleaner-0.0.15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.14/README.md` & `excel_cleaner-0.0.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.14</li>
+<li>Version 0.0.15</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F10: split a column to two columns with a particular string</li></ol></ul>
-<ul><li>Option to save processes to a file</li>
-<ul><li>The processes saved can be executed to speed the process until wanted cleaning is completed.</li></ul></ul>
+<ul><li>Added an option to save processes to a file</li>
+<ul><li>The processes saved in the file can be executed to speed the process until wanted cleaning is completed.</li></ul>
+<ul><li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
+</ul>
 <br>
 
 <li>Version 0.0.10</li>
 <ul><li>Restoring just the data before the last action is extended to data of all actions since the first action.</li>
 <li>Changed function keys for actions.</li>
 <li>Screen displays the selected row where the next action is needed.</li></ul>
 <br>
```

#### html2text {}

```diff
@@ -1,28 +1,30 @@
 # excel_cleaner ## What is it? A package that helps you clean and recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.14
+    * Version 0.0.15
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
-          o Option to save processes to a file
-                # The processes saved can be executed to speed the process
-                  until wanted cleaning is completed.
+          o Added an option to save processes to a file
+                # The processes saved in the file can be executed to speed the
+                  process until wanted cleaning is completed.
+                # Clicking a row provides the rows having the same pattern of
+                  the cells in row
     *
     * Version 0.0.10
           o Restoring just the data before the last action is extended to data
             of all actions since the first action.
           o Changed function keys for actions.
           o Screen displays the selected row where the next action is needed.
     *
```

### Comparing `excel_cleaner-0.0.14/pyproject.toml` & `excel_cleaner-0.0.15/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_cleaner"
-version = "0.0.14"
+version = "0.0.15"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you clean and recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -20,8 +20,8 @@
     "Operating System :: OS Independent",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: End Users/Desktop",
     "Development Status :: 5 - Production/Stable"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/generateNscore/excelcolumnizer"
+"Homepage" = "https://github.com/generateNscore/excel_cleaner"
```

### Comparing `excel_cleaner-0.0.14/PKG-INFO` & `excel_cleaner-0.0.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: excel_cleaner
-Version: 0.0.14
+Version: 0.0.15
 Summary: A small packages that helps you clean and recover columns of Excel data converted from PDF files.
-Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
+Project-URL: Homepage, https://github.com/generateNscore/excel_cleaner
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,25 +30,27 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.14</li>
+<li>Version 0.0.15</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F10: split a column to two columns with a particular string</li></ol></ul>
-<ul><li>Option to save processes to a file</li>
-<ul><li>The processes saved can be executed to speed the process until wanted cleaning is completed.</li></ul></ul>
+<ul><li>Added an option to save processes to a file</li>
+<ul><li>The processes saved in the file can be executed to speed the process until wanted cleaning is completed.</li></ul>
+<ul><li>Clicking a row provides the rows having the same pattern of the cells in row</li></ul>
+</ul>
 <br>
 
 <li>Version 0.0.10</li>
 <ul><li>Restoring just the data before the last action is extended to data of all actions since the first action.</li>
 <li>Changed function keys for actions.</li>
 <li>Screen displays the selected row where the next action is needed.</li></ul>
 <br>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.14 Summary: A small
+Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.15 Summary: A small
 packages that helps you clean and recover columns of Excel data converted from
 PDF files. Project-URL: Homepage, https://github.com/generateNscore/
-excelcolumnizer Author-email: Sukmock Lee
+excel_cleaner Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier: Topic
 :: Office/Business :: Financial :: Accounting Classifier: Topic :: Office/
 Business :: Financial :: Point-Of-Sale Classifier: Topic :: Office/Business ::
@@ -13,28 +13,30 @@
 markdown # excel_cleaner ## What is it? A package that helps you clean and
 recover columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.14
+    * Version 0.0.15
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
-          o Option to save processes to a file
-                # The processes saved can be executed to speed the process
-                  until wanted cleaning is completed.
+          o Added an option to save processes to a file
+                # The processes saved in the file can be executed to speed the
+                  process until wanted cleaning is completed.
+                # Clicking a row provides the rows having the same pattern of
+                  the cells in row
     *
     * Version 0.0.10
           o Restoring just the data before the last action is extended to data
             of all actions since the first action.
           o Changed function keys for actions.
           o Screen displays the selected row where the next action is needed.
     *
```

