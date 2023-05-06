# Comparing `tmp/excel_cleaner-0.0.13.tar.gz` & `tmp/excel_cleaner-0.0.14.tar.gz`

## Comparing `excel_cleaner-0.0.13.tar` & `excel_cleaner-0.0.14.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/updatePackage.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/src/excel_cleaner/__init__.py
--rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/src/excel_cleaner/_excelCleaner.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/test/MG-158427.xlsx
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/test/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/LICENSE.txt
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/README.md
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 excel_cleaner-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/updatePackage.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/src/excel_cleaner/__init__.py
+-rw-r--r--   0        0        0    33838 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/src/excel_cleaner/_excelCleaner.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/test/MG-158427.xlsx
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/test/test.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/LICENSE.txt
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/README.md
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 excel_cleaner-0.0.14/PKG-INFO
```

### Comparing `excel_cleaner-0.0.13/updatePackage.txt` & `excel_cleaner-0.0.14/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.13/src/excel_cleaner/_excelCleaner.py` & `excel_cleaner-0.0.14/src/excel_cleaner/_excelCleaner.py`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.13/test/MG-158427.xlsx` & `excel_cleaner-0.0.14/test/MG-158427.xlsx`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.13/LICENSE.txt` & `excel_cleaner-0.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excel_cleaner-0.0.13/README.md` & `excel_cleaner-0.0.14/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.13</li>
+<li>Version 0.0.14</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
@@ -52,15 +52,15 @@
 <ul><li>Disabled some bindings that belong to tksheet package.</li></ul>
 <br>
 
 <li>Version 0.0.4</li>
 
 ```python
 
-import excelcolumnizer as xl
+import excel_cleaner as xl
 
 xlpath='(excel file name with extension)'
 xl.sheet(xlpath)
 
 ```
 
 <ul><li>A tksheet window will be opened with the contents of excel file.</li>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # excel_cleaner ## What is it? A package that helps you clean and recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.13
+    * Version 0.0.14
           o Added function-key features
                1. F1: delete rows or columns
                2. F2: delete rows having a particular cell
                3. F3: combine rows or columns
                4. F4: combine selected rows
                5. F5: insert a cell to row and repeat the process to other rows
                   in the same pattern
@@ -39,15 +39,15 @@
                   next action. This selection is only a hint and should not be
                   followed unless otherwise.
     *
     * Version 0.0.5
           o Disabled some bindings that belong to tksheet package.
     *
     * Version 0.0.4
-    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+    * ```python import excel_cleaner as xl xlpath='(excel file name with
       extension)' xl.sheet(xlpath) ```
           o A tksheet window will be opened with the contents of excel file.
           o Here are recommending orders of actions to try:
                1. Remove unwanted rows (F1) first
                2. Remove unwanted columns (F1) or combine columns (F3)
                3. Click a cell to insert (F5) or delete the cell (F7)
           o
```

### Comparing `excel_cleaner-0.0.13/pyproject.toml` & `excel_cleaner-0.0.14/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excel_cleaner"
-version = "0.0.13"
+version = "0.0.14"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you clean and recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excel_cleaner-0.0.13/PKG-INFO` & `excel_cleaner-0.0.14/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_cleaner
-Version: 0.0.13
+Version: 0.0.14
 Summary: A small packages that helps you clean and recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -30,15 +30,15 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a> for opening/saving Excel file in Python.</li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a> for displaying the content of the Excel file.</li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.13</li>
+<li>Version 0.0.14</li>
 <ul><li>Added function-key features</li>
 <ol><li>F1: delete rows or columns</li>
 <li>F2: delete rows having a particular cell</li>
 <li>F3: combine rows or columns</li>
 <li>F4: combine selected rows</li>
 <li>F5: insert a cell to row and repeat the process to other rows in the same pattern</li>
 <li>F7: delete a cell to row and repeat the process to other rows in the same pattern</li>
@@ -71,15 +71,15 @@
 <ul><li>Disabled some bindings that belong to tksheet package.</li></ul>
 <br>
 
 <li>Version 0.0.4</li>
 
 ```python
 
-import excelcolumnizer as xl
+import excel_cleaner as xl
 
 xlpath='(excel file name with extension)'
 xl.sheet(xlpath)
 
 ```
 
 <ul><li>A tksheet window will be opened with the contents of excel file.</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.13 Summary: A small
+Metadata-Version: 2.1 Name: excel_cleaner Version: 0.0.14 Summary: A small
 packages that helps you clean and recover columns of Excel data converted from
 PDF files. Project-URL: Homepage, https://github.com/generateNscore/
 excelcolumnizer Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -13,15 +13,15 @@
 markdown # excel_cleaner ## What is it? A package that helps you clean and
 recover columns of Excel data converted from PDF files. ## Where to get it
 pip install excel_cleaner
 ## Dependencies
     * openpyxl for opening/saving Excel file in Python.
     * tksheet for displaying the content of the Excel file.
 ## Changes
-    * Version 0.0.13
+    * Version 0.0.14
           o Added function-key features
                1. F1: delete rows or columns
                2. F2: delete rows having a particular cell
                3. F3: combine rows or columns
                4. F4: combine selected rows
                5. F5: insert a cell to row and repeat the process to other rows
                   in the same pattern
@@ -51,15 +51,15 @@
                   next action. This selection is only a hint and should not be
                   followed unless otherwise.
     *
     * Version 0.0.5
           o Disabled some bindings that belong to tksheet package.
     *
     * Version 0.0.4
-    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+    * ```python import excel_cleaner as xl xlpath='(excel file name with
       extension)' xl.sheet(xlpath) ```
           o A tksheet window will be opened with the contents of excel file.
           o Here are recommending orders of actions to try:
                1. Remove unwanted rows (F1) first
                2. Remove unwanted columns (F1) or combine columns (F3)
                3. Click a cell to insert (F5) or delete the cell (F7)
           o
```

