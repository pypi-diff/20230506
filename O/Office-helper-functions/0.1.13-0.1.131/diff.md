# Comparing `tmp/Office_helper_functions-0.1.13.tar.gz` & `tmp/Office_helper_functions-0.1.131.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Office_helper_functions-0.1.13.tar", last modified: Fri May  5 19:58:28 2023, max compression
+gzip compressed data, was "Office_helper_functions-0.1.131.tar", last modified: Sat May  6 09:30:31 2023, max compression
```

## Comparing `Office_helper_functions-0.1.13.tar` & `Office_helper_functions-0.1.131.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.861563 Office_helper_functions-0.1.13/Office_helper_functions/
--rw-rw-rw-   0        0        0     3175 2023-05-04 20:51:57.000000 Office_helper_functions-0.1.13/Office_helper_functions/Dates.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.897244 Office_helper_functions-0.1.13/Office_helper_functions/Image/
--rw-rw-rw-   0        0        0     1418 2023-05-04 20:40:27.000000 Office_helper_functions-0.1.13/Office_helper_functions/Image/Image_operations.py
--rw-rw-rw-   0        0        0        0 2023-05-04 20:41:09.000000 Office_helper_functions-0.1.13/Office_helper_functions/Image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.902265 Office_helper_functions-0.1.13/Office_helper_functions/Word/
--rw-rw-rw-   0        0        0     2477 2023-05-05 19:33:25.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/Word_Image.py
--rw-rw-rw-   0        0        0        0 2023-05-04 20:52:17.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.902265 Office_helper_functions-0.1.13/Office_helper_functions/Word/checkbox/
--rw-rw-rw-   0        0        0        0 2023-05-04 19:59:26.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/checkbox/__init__.py
--rw-rw-rw-   0        0        0     3138 2023-05-05 19:57:26.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/form_field.py
--rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.13/Office_helper_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.891016 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/
--rw-rw-rw-   0        0        0      202 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-05-05 19:58:13.000000 Office_helper_functions-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.591873 Office_helper_functions-0.1.131/
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.535799 Office_helper_functions-0.1.131/Office_helper_functions/
+-rw-rw-rw-   0        0        0     3175 2023-05-04 20:51:57.000000 Office_helper_functions-0.1.131/Office_helper_functions/Dates.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.560398 Office_helper_functions-0.1.131/Office_helper_functions/Image/
+-rw-rw-rw-   0        0        0     1418 2023-05-04 20:40:27.000000 Office_helper_functions-0.1.131/Office_helper_functions/Image/Image_operations.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:41:09.000000 Office_helper_functions-0.1.131/Office_helper_functions/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.585220 Office_helper_functions-0.1.131/Office_helper_functions/Word/
+-rw-rw-rw-   0        0        0     2477 2023-05-06 09:30:20.000000 Office_helper_functions-0.1.131/Office_helper_functions/Word/Word_Image.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:52:17.000000 Office_helper_functions-0.1.131/Office_helper_functions/Word/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.586737 Office_helper_functions-0.1.131/Office_helper_functions/Word/checkbox/
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:26.000000 Office_helper_functions-0.1.131/Office_helper_functions/Word/checkbox/__init__.py
+-rw-rw-rw-   0        0        0     3045 2023-05-06 09:30:22.000000 Office_helper_functions-0.1.131/Office_helper_functions/Word/form_field.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.131/Office_helper_functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 09:30:31.558067 Office_helper_functions-0.1.131/Office_helper_functions.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-05-06 09:30:31.000000 Office_helper_functions-0.1.131/Office_helper_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-06 09:30:31.000000 Office_helper_functions-0.1.131/Office_helper_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 09:30:31.000000 Office_helper_functions-0.1.131/Office_helper_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-06 09:30:31.000000 Office_helper_functions-0.1.131/Office_helper_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      203 2023-05-06 09:30:31.586737 Office_helper_functions-0.1.131/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-06 09:30:31.592465 Office_helper_functions-0.1.131/setup.cfg
+-rw-rw-rw-   0        0        0      355 2023-05-06 09:30:09.000000 Office_helper_functions-0.1.131/setup.py
```

### Comparing `Office_helper_functions-0.1.13/Office_helper_functions/Dates.py` & `Office_helper_functions-0.1.131/Office_helper_functions/Dates.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.13/Office_helper_functions/Image/Image_operations.py` & `Office_helper_functions-0.1.131/Office_helper_functions/Image/Image_operations.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.13/Office_helper_functions/Word/Word_Image.py` & `Office_helper_functions-0.1.131/Office_helper_functions/Word/Word_Image.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.13/Office_helper_functions/Word/form_field.py` & `Office_helper_functions-0.1.131/Office_helper_functions/Word/form_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,22 @@
 
     Returns:
         BytesIO: Returns a BytesIO to be used in document libraries
     """
     with zipfile.ZipFile(io.BytesIO(xlsx_data), mode='r') as zf:
 
         sheet1_data = zf.read('word/document.xml').decode('utf-8')
-        print(sheet1_data.index('w:sdt'))
         soup = BeautifulSoup(sheet1_data, 'xml')
 
         std_elements_with_checkboxes = soup.find_all('w:sdt')
         x =std_elements_with_checkboxes[checkbox_location]
         if "checkbox" in str(x): 
             x.find('checked')['w14:val'] = checkbox_value
             x.find('w:t').string = ["☒" if checkbox_value==1 else "☐"][0]
                 
-        print(len(std_elements_with_checkboxes))
         
         files = {x: zf.read(x) for x in zf.namelist()}
         modified_sheet1_data = str(soup)
         files['word/document.xml'] = modified_sheet1_data
 
     # Create a new in-memory ZipFile object
     output_zip = io.BytesIO()
```

### Comparing `Office_helper_functions-0.1.13/Office_helper_functions.egg-info/SOURCES.txt` & `Office_helper_functions-0.1.131/Office_helper_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

