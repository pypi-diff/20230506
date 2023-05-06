# Comparing `tmp/pyracf-0.6.1.tar.gz` & `tmp/pyracf-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.6.1.tar", last modified: Fri May  5 19:34:07 2023, max compression
+gzip compressed data, was "pyracf-0.6.2.tar", last modified: Sat May  6 08:30:34 2023, max compression
```

## Comparing `pyracf-0.6.1.tar` & `pyracf-0.6.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.1/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.1/MANIFEST.in
--rw-rw-r--   0 henri     (1000) henri     (1000)     8019 2023-05-05 19:34:07.114300 pyracf-0.6.1/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)     7494 2023-05-05 19:33:48.000000 pyracf-0.6.1/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-05 19:34:07.114300 pyracf-0.6.1/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      961 2023-05-05 19:33:03.000000 pyracf-0.6.1/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    33417 2023-05-05 10:00:54.000000 pyracf-0.6.1/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   126403 2023-05-05 19:32:44.000000 pyracf-0.6.1/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-05 19:34:07.114300 pyracf-0.6.1/src/pyracf.egg-info/
--rw-rw-r--   0 henri     (1000) henri     (1000)     8019 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       32 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-05 19:34:07.000000 pyracf-0.6.1/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.333418 pyracf-0.6.2/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.6.2/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.6.2/MANIFEST.in
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-05-06 08:30:34.333418 pyracf-0.6.2/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)     7659 2023-05-06 08:24:36.000000 pyracf-0.6.2/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-06 08:30:34.333418 pyracf-0.6.2/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2023-05-06 08:22:26.000000 pyracf-0.6.2/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.329418 pyracf-0.6.2/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.329418 pyracf-0.6.2/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    33408 2023-05-06 08:23:06.000000 pyracf-0.6.2/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   126403 2023-05-05 19:32:44.000000 pyracf-0.6.2/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2023-05-06 08:30:34.333418 pyracf-0.6.2/src/pyracf.egg-info/
+-rw-rw-r--   0 henri     (1000) henri     (1000)     8184 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      254 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2023-05-06 08:30:34.000000 pyracf-0.6.2/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.6.1/LICENSE` & `pyracf-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.1/PKG-INFO` & `pyracf-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.1
+Version: 0.6.2
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,14 +26,18 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.6.2 (Fix XLSX Creation)
+- With newer versions of XlsxWriter there's no more .save(). Changed to .close()
+- Pinned pandas and XlsxWriter versions in setup.py 
+
 ### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 - Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
```

### Comparing `pyracf-0.6.1/README.md` & `pyracf-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.6.2 (Fix XLSX Creation)
+- With newer versions of XlsxWriter there's no more .save(). Changed to .close()
+- Pinned pandas and XlsxWriter versions in setup.py 
+
 ### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 - Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
```

### Comparing `pyracf-0.6.1/setup.py` & `pyracf-0.6.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.6.1",
+    version="0.6.2",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
@@ -21,13 +21,12 @@
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     include_package_data=True,
     install_requires=[
         'wheel',
-        'pandas',
-        'xlsxwriter',
-        'anytree'
+        'pandas>=1.5.2',
+        'xlsxwriter>=3.1.0'
     ],
     python_requires=">=3.6",
 )
```

### Comparing `pyracf-0.6.1/src/pyracf/__init__.py` & `pyracf-0.6.2/src/pyracf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -656,15 +656,15 @@
                     if i>0 and j>0:
                         rdict = worksheet.table.get(j,None)
                         centry = rdict.get(i,None)
                         if centry:
                             value = shared_strings[centry.string]
                             worksheet.write(j, i, value, accessLevelFormats[value])
 
-        writer.save()   
+        writer.close()   
 
     def ownertree(self):
         if self._ownertree != None:
             return self._ownertree
         else:
             # get all owners... (group or user)
             self._ownertree = {}
@@ -677,22 +677,16 @@
             # now we gotta condense it :)
             return self._ownertree
             for supgrp in self._ownertree:
                 for subgrp in self._ownertree[supgrp]:
                     if subgrp in self._ownertree.values:
                         self._ownertree[supgrp].remove(subgrp)
                         self._ownertree[supgrp].append(self._ownertree[subgrp])
-
-
             return self._ownertree
 
-
-
-
-    
     def getdatsetrisk(self, profile=''):
         '''This will produce a dict as follows:
       
         '''
         try:
             if self._records[self.GPBD_RECORDTYPE]['parsed'] == 0 or self._records[self.USCON_RECORDTYPE]['parsed'] == 0 or self._records[self.USBD_RECORDTYPE]['parsed'] == 0 or self._records[self.DSACC_RECORDTYPE]['parsed'] == 0 or  self._records[self.DSBD_RECORDTYPE]['parsed'] == 0:
                 raise StoopidException("Need to parse DSACC and DSBD first...")
```

### Comparing `pyracf-0.6.1/src/pyracf/offsets.json` & `pyracf-0.6.2/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.6.1/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.6.2/src/pyracf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.6.1
+Version: 0.6.2
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,14 +26,18 @@
 For more information on the various records, please refer to the [IBM documentation](https://www.ibm.com/docs/en/zos/2.1.0?topic=records-irrdbu00-record-types) on IRRDBU00 record types and the [record formats](https://www.ibm.com/docs/en/zos/2.5.0?topic=records-record-formats-produced-by-database-unload-utility) produced by the database unload utility. The DataFrames generated by PyRACF feature the same 'fieldnames' as outlined in the documentation, ensuring consistency and accuracy in your analyses.
 
 To get started with PyRACF, install it using `pip install pyracf` or explore the source code on [GitHub](https://github.com/wizardofzos/pyracf/releases/latest). Use PyRACF to take control of your security data and protect your IBM Z systems from threats.
 
 
 ## Updates
 
+### 0.6.2 (Fix XLSX Creation)
+- With newer versions of XlsxWriter there's no more .save(). Changed to .close()
+- Pinned pandas and XlsxWriter versions in setup.py 
+
 ### 0.6.1 (Bug free?)
 - XLS generation fully functional again (also for z/VM unloads)
 - Oprhan detection working again
 - Conditional Dataset Access Records now parsing correctly
 - Conditional Dataset Access now correctly pickled :)
 - Fixed parsing of GRCACC records (had misparsed AUTH_ID)
 - Conditional Generic (General) Records now with correct column name (GRCACC_CLASS_NAME)
```

