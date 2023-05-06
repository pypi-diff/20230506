# Comparing `tmp/excelcolumnizer-0.0.8.tar.gz` & `tmp/excelcolumnizer-0.0.9.tar.gz`

## Comparing `excelcolumnizer-0.0.8.tar` & `excelcolumnizer-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/updatePackage.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/src/excelcolumnizer/__init__.py
--rw-r--r--   0        0        0    11947 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/src/excelcolumnizer/_excelColumnizer.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/README.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/updatePackage.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/src/excelcolumnizer/__init__.py
+-rw-r--r--   0        0        0    11850 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/src/excelcolumnizer/_excelColumnizer.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 excelcolumnizer-0.0.9/PKG-INFO
```

### Comparing `excelcolumnizer-0.0.8/updatePackage.txt` & `excelcolumnizer-0.0.9/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.8/src/excelcolumnizer/_excelColumnizer.py` & `excelcolumnizer-0.0.9/src/excelcolumnizer/_excelColumnizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -273,43 +273,41 @@
             wb=load_workbook(xlpath, data_only=True)
             data = [[f.value for f in row] for row in wb.worksheets[0].rows]
             self.data=[row for row in data if row != [None for _ in range(len(data[0]))]]
         
         self.hw=tk.Tk()
         self.hw.option_add('*Font', ('Palatino Linotype',12))
         self.hw.geometry('1000x850')
-        self.hw.title(self.title+' '*10+'F1: insert cell, F3: delete cell, F5: combine columns/rows, F7: delete columns/row, F9: save, F12: restore')
+        self.hw.title(self.title+' '*10+'F1: insert cell, F3: delete cell, F5: combine cols/rows, F7: delete cols/rows, F9: save, F12: restore')
         self.hw.bind('<F1>', self.addCells)
         self.hw.bind('<F3>', self.subCells)
         self.hw.bind('<F5>', self.combineRowsColumns)
         self.hw.bind('<F7>', self.delRowsColumns)
         self.hw.bind('<F9>', self.saveCleanedData)
         self.hw.bind('<F12>', self.restore)
         
         self.hL=tk.Label(self.hw, text='...')
         self.hL.pack(pady=2)
 
         self.shtL = tksheet.Sheet(self.hw)
         self.shtL.pack(expand=1, fill='both')
         self.shtL.enable_bindings()
         self.shtL.disable_bindings(['rc_delete_row', 'rc_delete_column'])
+        self.shtL.disable_bindings(['rc_delete_row', 'rc_delete_column', 'cut', 'paste', 'copy', 'delete'])        
 
-        self.shtL.popup_menu_add_command("선택한 cell에 빈 칸 추가 - 오른쪽으로 이동 (F1)", self.addCells)
-        self.shtL.popup_menu_add_command("선택한 cell 삭제 - 왼쪽으로 이동 (F3)", self.subCells)
-        self.shtL.popup_menu_add_command("행/열 합치기 (F5)", self.combineRowsColumns)
-        self.shtL.popup_menu_add_command("행/열 삭제 (F7)", self.delRowsColumns)
-        self.shtL.popup_menu_add_command("방금 전 작업 복원 (F12)", self.restore)
+        self.shtL.popup_menu_add_command("insert cell (F1)", self.addCells)
+        self.shtL.popup_menu_add_command("delete cell (F3)", self.subCells)
+        self.shtL.popup_menu_add_command("combine rows/cols (F5)", self.combineRowsColumns)
+        self.shtL.popup_menu_add_command("delete rows/cols (F7)", self.delRowsColumns)
+        self.shtL.popup_menu_add_command("restore (F12)", self.restore)
 
         self.shtL.set_sheet_data(self.data)
         self.shtL.set_all_cell_sizes_to_text(redraw = True)
 
         self.hL.config(text=f'총 항목 수: {len(self.data[0])}×{len(self.data)}')
         self.hw.mainloop()        
     
 
 
 if __name__ == '__main__':
-    #path=r'D:/Dropbox/POS/testing/JC-OSI007413.xlsx'
-    #path=r'../ATE-207.xlsx'
-    #path=r'../KC_80968.xlsx'
     path=r'../AJ-SO007558.xlsx'
     sheet(path)
```

### Comparing `excelcolumnizer-0.0.8/LICENSE.txt` & `excelcolumnizer-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `excelcolumnizer-0.0.8/README.md` & `excelcolumnizer-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.8</li>
+<li>Version 0.0.9</li>
 <ul><li>A tiny bug is fixed:</li>
-<li>Renaming a cleaned xlsx file was fixed.</li></ul
+<li>Renaming a cleaned xlsx file was fixed.</li></ul>
 <br>
 
 <li>Version 0.0.7</li>
 <ul><li>Added some help:</li>
 <ol><li>When a column is all None, it will be deleted without any notice.</li>
 <li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
 <li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
```

#### html2text {}

```diff
@@ -1,58 +1,56 @@
 # excelcolumnizer ## What is it? A package that helps you recover columns of
 Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.8
+    * Version 0.0.9
           o A tiny bug is fixed:
           o Renaming a cleaned xlsx file was fixed.
-          o br>
-          o Version 0.0.7
-                # Added some help:
-                     1. When a column is all None, it will be deleted without
-                        any notice.
-                     2. Rows in a pattern that takes place at the least number
-                        of rows will be highlighted.
-                     3. The first row of the rows will be selected and is ready
-                        for next action. This selection is only a hint and
-                        should not be followed unless otherwise.
-          o
-          o Version 0.0.5
-                # Disabled some bindings that belong to tksheet package.
+    *
+    * Version 0.0.7
+          o Added some help:
+               1. When a column is all None, it will be deleted without any
+                  notice.
+               2. Rows in a pattern that takes place at the least number of
+                  rows will be highlighted.
+               3. The first row of the rows will be selected and is ready for
+                  next action. This selection is only a hint and should not be
+                  followed unless otherwise.
+    *
+    * Version 0.0.5
+          o Disabled some bindings that belong to tksheet package.
+    *
+    * Version 0.0.4
+    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+      extension)' xl.sheet(xlpath) ```
+          o A tksheet window will be opened with the contents of excel file.
+          o Here are recommending orders of actions to try:
+               1. Remove unwanted rows (F7)
+               2. Remove unwanted columns (F7) or combine columns (F5)
+               3. Click a cell to insert (F1) or delete the cell (F3)
           o
-          o Version 0.0.4
-          o ```python import excelcolumnizer as xl xlpath='(excel file name
-            with extension)' xl.sheet(xlpath) ```
-                # A tksheet window will be opened with the contents of excel
-                  file.
-                # Here are recommending orders of actions to try:
-                     1. Remove unwanted rows (F7)
-                     2. Remove unwanted columns (F7) or combine columns (F5)
-                     3. Click a cell to insert (F1) or delete the cell (F3)
-                #
-                # If the same pattern or kind of selected rows/columns is found
-                  at other locations, the same action is repeated for the found
-                  rows/columns.
-                      # Thus, it would better try one action at the top
-                      # To remove rows, click the row names.
-                      # To remove or combine columns, click the column names.
-                #
-                # After every action, the contents will be saved to a file that
-                  is the original name with a string "_cleaned".
-                # When a cell is inserted, all the cells at right will be
-                  shifted to the right and an extra column will be created with
-                  empty for all other rows that are not changed.
-                # When a cell is deleted, all the cells at right will be
-                  shifted to the left and the cell at the last column will be
-                  empty.
-                # If one action is done by mistake, press function-key F12 to
-                  restore the the data before he last action
+          o If the same pattern or kind of selected rows/columns is found at
+            other locations, the same action is repeated for the found rows/
+            columns.
+                # Thus, it would better try one action at the top
+                # To remove rows, click the row names.
+                # To remove or combine columns, click the column names.
           o
-                # After each action is completed,
-                      # the number of columns and rows and the number of
-                        patterns of rows will be displayed
-                      # either a few columns or muliple rows are highlighted,
-                        which are indicative of ok to be deleted.
+          o After every action, the contents will be saved to a file that is
+            the original name with a string "_cleaned".
+          o When a cell is inserted, all the cells at right will be shifted to
+            the right and an extra column will be created with empty for all
+            other rows that are not changed.
+          o When a cell is deleted, all the cells at right will be shifted to
+            the left and the cell at the last column will be empty.
+          o If one action is done by mistake, press function-key F12 to restore
+            the the data before he last action
     *
+          o After each action is completed,
+                # the number of columns and rows and the number of patterns of
+                  rows will be displayed
+                # either a few columns or muliple rows are highlighted, which
+                  are indicative of ok to be deleted.
+
```

### Comparing `excelcolumnizer-0.0.8/pyproject.toml` & `excelcolumnizer-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "excelcolumnizer"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
 description = "A small packages that helps you recover columns of Excel data converted from PDF files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `excelcolumnizer-0.0.8/PKG-INFO` & `excelcolumnizer-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excelcolumnizer
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -30,17 +30,17 @@
 ## Dependencies
 
 <ul><li><a href="https://openpyxl.readthedocs.io/en/stable/">openpyxl</a></li>
 <li><a href="https://github.com/ragardner/tksheet">tksheet</a></li></ul>
 
 ## Changes
 <ul>
-<li>Version 0.0.8</li>
+<li>Version 0.0.9</li>
 <ul><li>A tiny bug is fixed:</li>
-<li>Renaming a cleaned xlsx file was fixed.</li></ul
+<li>Renaming a cleaned xlsx file was fixed.</li></ul>
 <br>
 
 <li>Version 0.0.7</li>
 <ul><li>Added some help:</li>
 <ol><li>When a column is all None, it will be deleted without any notice.</li>
 <li>Rows in a pattern that takes place at the least number of rows will be highlighted.</li>
 <li>The first row of the rows will be selected and is ready for next action. This selection is only a hint and should not be followed unless otherwise.</li></ol></ul>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.8 Summary: A small
+Metadata-Version: 2.1 Name: excelcolumnizer Version: 0.0.9 Summary: A small
 packages that helps you recover columns of Excel data converted from PDF files.
 Project-URL: Homepage, https://github.com/generateNscore/excelcolumnizer
 Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Financial and Insurance Industry Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -13,58 +13,56 @@
 markdown # excelcolumnizer ## What is it? A package that helps you recover
 columns of Excel data converted from PDF files. ## Where to get it
 pip install excelcolumnizer
 ## Dependencies
     * openpyxl
     * tksheet
 ## Changes
-    * Version 0.0.8
+    * Version 0.0.9
           o A tiny bug is fixed:
           o Renaming a cleaned xlsx file was fixed.
-          o br>
-          o Version 0.0.7
-                # Added some help:
-                     1. When a column is all None, it will be deleted without
-                        any notice.
-                     2. Rows in a pattern that takes place at the least number
-                        of rows will be highlighted.
-                     3. The first row of the rows will be selected and is ready
-                        for next action. This selection is only a hint and
-                        should not be followed unless otherwise.
-          o
-          o Version 0.0.5
-                # Disabled some bindings that belong to tksheet package.
+    *
+    * Version 0.0.7
+          o Added some help:
+               1. When a column is all None, it will be deleted without any
+                  notice.
+               2. Rows in a pattern that takes place at the least number of
+                  rows will be highlighted.
+               3. The first row of the rows will be selected and is ready for
+                  next action. This selection is only a hint and should not be
+                  followed unless otherwise.
+    *
+    * Version 0.0.5
+          o Disabled some bindings that belong to tksheet package.
+    *
+    * Version 0.0.4
+    * ```python import excelcolumnizer as xl xlpath='(excel file name with
+      extension)' xl.sheet(xlpath) ```
+          o A tksheet window will be opened with the contents of excel file.
+          o Here are recommending orders of actions to try:
+               1. Remove unwanted rows (F7)
+               2. Remove unwanted columns (F7) or combine columns (F5)
+               3. Click a cell to insert (F1) or delete the cell (F3)
           o
-          o Version 0.0.4
-          o ```python import excelcolumnizer as xl xlpath='(excel file name
-            with extension)' xl.sheet(xlpath) ```
-                # A tksheet window will be opened with the contents of excel
-                  file.
-                # Here are recommending orders of actions to try:
-                     1. Remove unwanted rows (F7)
-                     2. Remove unwanted columns (F7) or combine columns (F5)
-                     3. Click a cell to insert (F1) or delete the cell (F3)
-                #
-                # If the same pattern or kind of selected rows/columns is found
-                  at other locations, the same action is repeated for the found
-                  rows/columns.
-                      # Thus, it would better try one action at the top
-                      # To remove rows, click the row names.
-                      # To remove or combine columns, click the column names.
-                #
-                # After every action, the contents will be saved to a file that
-                  is the original name with a string "_cleaned".
-                # When a cell is inserted, all the cells at right will be
-                  shifted to the right and an extra column will be created with
-                  empty for all other rows that are not changed.
-                # When a cell is deleted, all the cells at right will be
-                  shifted to the left and the cell at the last column will be
-                  empty.
-                # If one action is done by mistake, press function-key F12 to
-                  restore the the data before he last action
+          o If the same pattern or kind of selected rows/columns is found at
+            other locations, the same action is repeated for the found rows/
+            columns.
+                # Thus, it would better try one action at the top
+                # To remove rows, click the row names.
+                # To remove or combine columns, click the column names.
           o
-                # After each action is completed,
-                      # the number of columns and rows and the number of
-                        patterns of rows will be displayed
-                      # either a few columns or muliple rows are highlighted,
-                        which are indicative of ok to be deleted.
+          o After every action, the contents will be saved to a file that is
+            the original name with a string "_cleaned".
+          o When a cell is inserted, all the cells at right will be shifted to
+            the right and an extra column will be created with empty for all
+            other rows that are not changed.
+          o When a cell is deleted, all the cells at right will be shifted to
+            the left and the cell at the last column will be empty.
+          o If one action is done by mistake, press function-key F12 to restore
+            the the data before he last action
     *
+          o After each action is completed,
+                # the number of columns and rows and the number of patterns of
+                  rows will be displayed
+                # either a few columns or muliple rows are highlighted, which
+                  are indicative of ok to be deleted.
+
```

