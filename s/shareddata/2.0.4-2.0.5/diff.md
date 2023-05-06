# Comparing `tmp/shareddata-2.0.4.tar.gz` & `tmp/shareddata-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.0.4.tar", last modified: Thu May  4 14:00:35 2023, max compression
+gzip compressed data, was "shareddata-2.0.5.tar", last modified: Sat May  6 11:55:42 2023, max compression
```

## Comparing `shareddata-2.0.4.tar` & `shareddata-2.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 14:00:35.075508 shareddata-2.0.4/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     1218 2023-05-04 14:00:35.075508 shareddata-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-2.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-05-04 14:00:35.076509 shareddata-2.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-04 14:00:35.014509 shareddata-2.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-04 14:00:35.065509 shareddata-2.0.4/src/SharedData/
--rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.4/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.4/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.4/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0    11426 2023-04-14 14:51:54.000000 shareddata-2.0.4/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.4/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.4/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.4/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.4/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0    11230 2023-03-26 19:43:51.000000 shareddata-2.0.4/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     6283 2023-04-25 18:26:16.000000 shareddata-2.0.4/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    11229 2023-03-09 15:11:52.000000 shareddata-2.0.4/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.4/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.4/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.4/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    25959 2023-05-03 23:01:44.000000 shareddata-2.0.4/src/SharedData/SharedDataTable.py
--rw-rw-rw-   0        0        0    31232 2023-05-04 13:59:43.000000 shareddata-2.0.4/src/SharedData/SharedDataTableKeys.py
--rw-rw-rw-   0        0        0    18042 2023-03-20 11:50:36.000000 shareddata-2.0.4/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0     6766 2023-05-04 14:00:18.000000 shareddata-2.0.4/src/SharedData/SharedNumpy.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.4/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 14:00:35.074509 shareddata-2.0.4/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1218 2023-05-04 14:00:35.000000 shareddata-2.0.4/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-05-04 14:00:35.000000 shareddata-2.0.4/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 14:00:35.000000 shareddata-2.0.4/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-05-04 14:00:35.000000 shareddata-2.0.4/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-04 14:00:35.000000 shareddata-2.0.4/src/shareddata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 11:55:42.149711 shareddata-2.0.5/
+-rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1218 2023-05-06 11:55:42.149711 shareddata-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-2.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-05-06 11:55:42.151030 shareddata-2.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 11:55:42.120695 shareddata-2.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 11:55:42.138203 shareddata-2.0.5/src/SharedData/
+-rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.5/src/SharedData/Defaults.py
+-rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.5/src/SharedData/Logger.py
+-rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.5/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-rw-   0        0        0    11489 2023-05-06 11:54:56.000000 shareddata-2.0.5/src/SharedData/Metadata.py
+-rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.5/src/SharedData/MultiProc.py
+-rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.5/src/SharedData/SeriesLib.py
+-rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.5/src/SharedData/SharedData.py
+-rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.5/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-rw-   0        0        0    11230 2023-03-26 19:43:51.000000 shareddata-2.0.5/src/SharedData/SharedDataAWSS3.py
+-rw-rw-rw-   0        0        0     6275 2023-05-04 17:59:07.000000 shareddata-2.0.5/src/SharedData/SharedDataFeeder.py
+-rw-rw-rw-   0        0        0    11229 2023-03-09 15:11:52.000000 shareddata-2.0.5/src/SharedData/SharedDataFrame.py
+-rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.5/src/SharedData/SharedDataPeriod.py
+-rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.5/src/SharedData/SharedDataRealTime.py
+-rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.5/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-rw-   0        0        0    25959 2023-05-03 23:01:44.000000 shareddata-2.0.5/src/SharedData/SharedDataTable.py
+-rw-rw-rw-   0        0        0    31232 2023-05-04 13:59:43.000000 shareddata-2.0.5/src/SharedData/SharedDataTableKeys.py
+-rw-rw-rw-   0        0        0    18042 2023-03-20 11:50:36.000000 shareddata-2.0.5/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-rw-   0        0        0     6766 2023-05-04 14:00:18.000000 shareddata-2.0.5/src/SharedData/SharedNumpy.py
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.5/src/SharedData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 11:55:42.148710 shareddata-2.0.5/src/shareddata.egg-info/
+-rw-rw-rw-   0        0        0     1218 2023-05-06 11:55:42.000000 shareddata-2.0.5/src/shareddata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-05-06 11:55:42.000000 shareddata-2.0.5/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 11:55:42.000000 shareddata-2.0.5/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-05-06 11:55:42.000000 shareddata-2.0.5/src/shareddata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 11:55:42.000000 shareddata-2.0.5/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.0.4/LICENSE` & `shareddata-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/PKG-INFO` & `shareddata-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.4
+Version: 2.0.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.4/README.md` & `shareddata-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/setup.cfg` & `shareddata-2.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6861 7265 6464 6174 610d 0a76   = shareddata..v
-00000020: 6572 7369 6f6e 203d 2032 2e30 2e34 0d0a  ersion = 2.0.4..
+00000020: 6572 7369 6f6e 203d 2032 2e30 2e35 0d0a  ersion = 2.0.5..
 00000030: 6175 7468 6f72 203d 204a 6f73 6520 4361  author = Jose Ca
 00000040: 726c 6974 6f20 6465 204f 6c69 7665 6972  rlito de Oliveir
 00000050: 6120 4669 6c68 6f0d 0a61 7574 686f 725f  a Filho..author_
 00000060: 656d 6169 6c20 3d20 6a63 6172 6c69 746f  email = jcarlito
 00000070: 6f6c 6976 6569 7261 4067 6d61 696c 2e63  oliveira@gmail.c
 00000080: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000090: 3d20 5368 6172 6564 204d 656d 6f72 7920  = Shared Memory
```

### Comparing `shareddata-2.0.4/src/SharedData/Defaults.py` & `shareddata-2.0.5/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/Logger.py` & `shareddata-2.0.5/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.0.5/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/Metadata.py` & `shareddata-2.0.5/src/SharedData/Metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,29 +49,30 @@
         self.load()
 
     @property
     def static(self):
         if self.records_chg:
             self.records_chg = False
             self._static = self.records2df(self._records)
+        self.static_chg = True
         return self._static
     
     @static.setter
     def static(self, df):
         self.static_chg = True
         self.records_chg = False
         self._index_columns = np.array(df.index.names)
         self._static = df
-        
-        
+                
     @property
     def records(self):
         if self.static_chg:
             self.static_chg = False
             self._records = self.df2records(self._static)
+        self.records_chg = True
         return self._records
     
     @records.setter
     def records(self, value):
         self.records_chg = True
         self._records = value
```

### Comparing `shareddata-2.0.4/src/SharedData/MultiProc.py` & `shareddata-2.0.5/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SeriesLib.py` & `shareddata-2.0.5/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedData.py` & `shareddata-2.0.5/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.0.5/src/SharedData/SharedDataAWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.0.5/src/SharedData/SharedDataAWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataFeeder.py` & `shareddata-2.0.5/src/SharedData/SharedDataFeeder.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 self.data[period] = SharedDataPeriod(self, period)        
             else:
                 self.data[dataset] = SharedDataTable(self, dataset)
 
         if (dataset in SharedDataFeeder.dense_datasets.keys()):
             return self.data[dataset]    
         else:
-            return self.data[dataset].records        
+            return self.data[dataset].records
         
     def load(self, period='D1', tags=None):
             
         if not self.default_collections is None:
             for c in self.default_collections.replace('\n','').split(','):
                 self.sharedData.getMetadata(c)
```

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataFrame.py` & `shareddata-2.0.5/src/SharedData/SharedDataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataPeriod.py` & `shareddata-2.0.5/src/SharedData/SharedDataPeriod.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataRealTime.py` & `shareddata-2.0.5/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.0.5/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataTable.py` & `shareddata-2.0.5/src/SharedData/SharedDataTable.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataTableKeys.py` & `shareddata-2.0.5/src/SharedData/SharedDataTableKeys.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.0.5/src/SharedData/SharedDataTimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/SharedData/SharedNumpy.py` & `shareddata-2.0.5/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.0.4/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.0.5/src/shareddata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.0.4
+Version: 2.0.5
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.0.4/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.0.5/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

