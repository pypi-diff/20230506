# Comparing `tmp/FlowIO-1.1.1.tar.gz` & `tmp/FlowIO-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowIO-1.1.1.tar", last modified: Thu Jan 26 15:48:16 2023, max compression
+gzip compressed data, was "FlowIO-1.2.0.tar", last modified: Fri May  5 22:04:38 2023, max compression
```

## Comparing `FlowIO-1.1.1.tar` & `FlowIO-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-01-26 15:48:16.807551 FlowIO-1.1.1/
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-01-26 15:48:16.807551 FlowIO-1.1.1/FlowIO.egg-info/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-01-26 15:48:16.000000 FlowIO-1.1.1/FlowIO.egg-info/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      280 2023-01-26 15:48:16.000000 FlowIO-1.1.1/FlowIO.egg-info/SOURCES.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-01-26 15:48:16.000000 FlowIO-1.1.1/FlowIO.egg-info/dependency_links.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        7 2023-01-26 15:48:16.000000 FlowIO-1.1.1/FlowIO.egg-info/top_level.txt
--rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:31:25.000000 FlowIO-1.1.1/LICENSE
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       35 2022-05-19 17:10:53.000000 FlowIO-1.1.1/MANIFEST.in
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-01-26 15:48:16.807551 FlowIO-1.1.1/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     2755 2023-01-24 17:31:35.000000 FlowIO-1.1.1/README.md
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-01-26 15:48:16.807551 FlowIO-1.1.1/flowio/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      100 2022-03-24 00:00:28.000000 FlowIO-1.1.1/flowio/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       45 2023-01-26 15:45:31.000000 FlowIO-1.1.1/flowio/_version.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    14799 2023-01-24 14:19:34.000000 FlowIO-1.1.1/flowio/create_fcs.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      647 2023-01-26 14:41:38.000000 FlowIO-1.1.1/flowio/exceptions.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1573 2022-03-24 00:00:28.000000 FlowIO-1.1.1/flowio/fcs_keywords.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    21069 2023-01-26 14:46:54.000000 FlowIO-1.1.1/flowio/flowdata.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-01-26 15:48:16.807551 FlowIO-1.1.1/setup.cfg
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1130 2022-05-19 17:10:53.000000 FlowIO-1.1.1/setup.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/FlowIO.egg-info/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      296 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        7 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/top_level.txt
+-rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:31:25.000000 FlowIO-1.2.0/LICENSE
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       35 2022-05-19 17:10:53.000000 FlowIO-1.2.0/MANIFEST.in
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-05-05 22:04:38.705233 FlowIO-1.2.0/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     2755 2023-04-25 14:05:26.000000 FlowIO-1.2.0/README.md
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/flowio/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      288 2023-05-05 20:48:34.000000 FlowIO-1.2.0/flowio/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       45 2023-05-05 22:03:39.000000 FlowIO-1.2.0/flowio/_version.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    14808 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/create_fcs.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      838 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/exceptions.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1573 2022-03-24 00:00:28.000000 FlowIO-1.2.0/flowio/fcs_keywords.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    21450 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/flowdata.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3005 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-05-05 22:04:38.705233 FlowIO-1.2.0/setup.cfg
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1130 2022-05-19 17:10:53.000000 FlowIO-1.2.0/setup.py
```

### Comparing `FlowIO-1.1.1/FlowIO.egg-info/PKG-INFO` & `FlowIO-1.2.0/FlowIO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowIO
-Version: 1.1.1
+Version: 1.2.0
 Summary: FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) files
 Home-page: https://github.com/whitews/flowio
 Author: Scott White
 Author-email: whitews@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `FlowIO-1.1.1/LICENSE` & `FlowIO-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowIO-1.1.1/PKG-INFO` & `FlowIO-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowIO
-Version: 1.1.1
+Version: 1.2.0
 Summary: FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) files
 Home-page: https://github.com/whitews/flowio
 Author: Scott White
 Author-email: whitews@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `FlowIO-1.1.1/README.md` & `FlowIO-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `FlowIO-1.1.1/flowio/create_fcs.py` & `FlowIO-1.2.0/flowio/create_fcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,17 @@
             proc_metadata_dict[new_key] = v
 
     # Verify data type is float, it's the only type supported for now.
     # Supporting int type is more complicated b/c it allows setting
     # different bit allocations for event data per channel. Float is
     # easy b/c all parameters must use 32 bits per event value.
     if 'datatype' in proc_metadata_dict:
-        dtype_value = proc_metadata_dict['datatype']
-        if dtype_value != 'F':
-            raise NotImplementedError("Creating FCS files with data type %s is not supported." % dtype_value)
+        datatype_value = proc_metadata_dict['datatype']
+        if datatype_value != 'F':
+            raise NotImplementedError("Creating FCS files with data type %s is not supported." % datatype_value)
 
     for i in range(n_channels):
         chan_num = i + 1  # channel numbers in FCS are indexed at 1
 
         # Channel gain (PnG), lin/log (PnE), & range (PnR) are exceptions where we
         # look in the provided metadata to find the values. We could do this later
         # in the build_text function, but it's nicer if all the channel parameter
```

### Comparing `FlowIO-1.1.1/flowio/exceptions.py` & `FlowIO-1.2.0/flowio/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,8 +22,15 @@
     """Errors relating to parsing an FCS file"""
 
 class DataOffsetDiscrepancyError(FCSParsingError):
     """
     Raised when an FCS file's HEADER & TEXT section provide different byte
     offsets for the DATA section.
     """
-    pass
+    pass
+
+class MultipleDataSetsError(FlowIOException):
+    """
+    Raised for errors related to FCS files containing more than one dataset, indicated by
+    the 'nextdata' keyword.
+    """
+    pass
```

### Comparing `FlowIO-1.1.1/flowio/fcs_keywords.py` & `FlowIO-1.2.0/flowio/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `FlowIO-1.1.1/flowio/flowdata.py` & `FlowIO-1.2.0/flowio/flowdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from operator import and_
 from struct import calcsize, iter_unpack
 from warnings import warn
 import os
 import re
 from functools import reduce
 from .create_fcs import create_fcs
-from .exceptions import FCSParsingError, DataOffsetDiscrepancyError
+from .exceptions import FCSParsingError, DataOffsetDiscrepancyError, MultipleDataSetsError
 
 try:
     # noinspection PyUnresolvedReferences, PyUnboundLocalVariable
     basestring
 except NameError:
     # noinspection PyShadowingBuiltins
     basestring = str
@@ -55,29 +55,32 @@
     :param ignore_offset_error: option to ignore data offset error (see above note), default is False
     :param ignore_offset_discrepancy: option to ignore discrepancy between the HEADER
         and TEXT values for the DATA byte offset location, default is False
     :param use_header_offsets: use the HEADER section for the data offset locations, default is False.
         Setting this option to True also suppresses an error in cases of an offset discrepancy.
     :param only_text: option to only read the "text" segment of the FCS file without loading event data,
         default is False
+    :param nextdata_offset: an integer indicating the byte offset for a data set, used for reading
+        a data set from FCS file contain multiple data sets
     """
     def __init__(
             self,
             filename_or_handle,
             ignore_offset_error=False,
             ignore_offset_discrepancy=False,
             use_header_offsets=False,
-            only_text=False
+            only_text=False,
+            nextdata_offset=None,
     ):
         if isinstance(filename_or_handle, basestring):
             self._fh = open(str(filename_or_handle), 'rb')
         else:
             self._fh = filename_or_handle
 
-        current_offset = 0
+        current_offset = nextdata_offset if nextdata_offset else 0
 
         self._ignore_offset = ignore_offset_error
 
         try:
             unused_path, self.name = os.path.split(self._fh.name)
         except (AttributeError, TypeError):
             self.name = 'InMemoryFile'
@@ -93,14 +96,17 @@
         # parse text
         self.text = self.__parse_text(
             current_offset,
             self.header['text_start'],
             self.header['text_stop']
         )
 
+        if int(self.text.get("nextdata", "0")) != 0 and nextdata_offset is None:
+            raise MultipleDataSetsError()
+
         self.channel_count = int(self.text['par'])
         self.event_count = int(self.text['tot'])
 
         # parse analysis
         try:
             a_start = int(self.text['beginanalysis'])
         except KeyError:
```

### Comparing `FlowIO-1.1.1/setup.py` & `FlowIO-1.2.0/setup.py`

 * *Files identical despite different names*

