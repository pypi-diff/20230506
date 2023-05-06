# Comparing `tmp/cxmlinvbot-1.0.4.tar.gz` & `tmp/cxmlinvbot-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.0.4.tar", last modified: Sat May  6 11:52:40 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.0.5.tar", last modified: Sat May  6 13:55:47 2023, max compression
```

## Comparing `cxmlinvbot-1.0.4.tar` & `cxmlinvbot-1.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.162297 cxmlinvbot-1.0.4/
--rw-rw-rw-   0        0        0      166 2023-05-06 11:52:40.161792 cxmlinvbot-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:39.995730 cxmlinvbot-1.0.4/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.0.4/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.018668 cxmlinvbot-1.0.4/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.0.4/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1483 2023-05-06 11:52:05.000000 cxmlinvbot-1.0.4/cxmlinvbot/config/base.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.031633 cxmlinvbot-1.0.4/cxmlinvbot/errors/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.0.4/cxmlinvbot/errors/__init__.py
--rw-rw-rw-   0        0        0      400 2023-05-05 17:26:49.000000 cxmlinvbot-1.0.4/cxmlinvbot/errors/errors.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.042603 cxmlinvbot-1.0.4/cxmlinvbot/filing/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.0.4/cxmlinvbot/filing/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-01 15:06:11.000000 cxmlinvbot-1.0.4/cxmlinvbot/filing/filing.py
--rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.0.4/cxmlinvbot/kill.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.054573 cxmlinvbot-1.0.4/cxmlinvbot/mail/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.0.4/cxmlinvbot/mail/__init__.py
--rw-rw-rw-   0        0        0     2784 2023-05-06 11:03:43.000000 cxmlinvbot-1.0.4/cxmlinvbot/mail/mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-06 11:06:16.000000 cxmlinvbot-1.0.4/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.087986 cxmlinvbot-1.0.4/cxmlinvbot/mapping/
--rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-05-06 09:04:07.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/action.py
--rw-rw-rw-   0        0        0     4713 2023-05-06 11:04:04.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/headermapping.py
--rw-rw-rw-   0        0        0    11461 2023-05-06 11:04:22.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/invoicedetailrequestmapping.py
--rw-rw-rw-   0        0        0      638 2023-05-06 09:04:46.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/mapping.py
--rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.0.4/cxmlinvbot/mapping/profilerequestmapping.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.108928 cxmlinvbot-1.0.4/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.0.4/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.0.4/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.0.4/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.0.4/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.156806 cxmlinvbot-1.0.4/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-05-06 09:50:28.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0      932 2023-05-06 09:06:10.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     3050 2023-05-06 11:05:43.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0     1107 2023-05-06 09:49:37.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-05-06 11:52:40.009690 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-06 11:52:39.000000 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2023-05-06 11:52:39.000000 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 11:52:39.000000 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-06 11:52:39.000000 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 11:52:39.000000 cxmlinvbot-1.0.4/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 11:52:40.162297 cxmlinvbot-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-05-06 09:55:52.000000 cxmlinvbot-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.861601 cxmlinvbot-1.0.5/
+-rw-rw-rw-   0        0        0      166 2023-05-06 13:55:47.860093 cxmlinvbot-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.709973 cxmlinvbot-1.0.5/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.0.5/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.729960 cxmlinvbot-1.0.5/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.0.5/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1483 2023-05-06 13:54:30.000000 cxmlinvbot-1.0.5/cxmlinvbot/config/base.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.740891 cxmlinvbot-1.0.5/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.0.5/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-05-05 17:26:49.000000 cxmlinvbot-1.0.5/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.752866 cxmlinvbot-1.0.5/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.0.5/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-01 15:06:11.000000 cxmlinvbot-1.0.5/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      246 2023-05-06 11:05:58.000000 cxmlinvbot-1.0.5/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.763350 cxmlinvbot-1.0.5/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.0.5/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     2784 2023-05-06 11:03:43.000000 cxmlinvbot-1.0.5/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-06 13:53:17.000000 cxmlinvbot-1.0.5/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.795264 cxmlinvbot-1.0.5/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     1925 2023-05-06 13:49:41.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4713 2023-05-06 11:04:04.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    12894 2023-05-06 13:38:46.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0      638 2023-05-06 09:04:46.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.0.5/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.815211 cxmlinvbot-1.0.5/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.0.5/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.0.5/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.0.5/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.0.5/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.856104 cxmlinvbot-1.0.5/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2231 2023-05-06 13:49:56.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0      932 2023-05-06 09:06:10.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     3050 2023-05-06 11:05:43.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0     1107 2023-05-06 09:49:37.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:55:47.723935 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-05-06 13:55:47.000000 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1116 2023-05-06 13:55:47.000000 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:55:47.000000 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-06 13:55:47.000000 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 13:55:47.000000 cxmlinvbot-1.0.5/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 13:55:47.861601 cxmlinvbot-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-05-06 09:55:52.000000 cxmlinvbot-1.0.5/setup.py
```

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/config/base.py` & `cxmlinvbot-1.0.5/cxmlinvbot/config/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidDTD' : '%sprofileresponseinvaliddtd.xml' % SAMPLE_PATH,
         'Response'                  : '%sresponse.xml' % SAMPLE_PATH,
         'ResponseWithData'          : '%sresponsewithdata.xml' % SAMPLE_PATH,
     }
     
     CSV_SAMPLE              = '%sCXML Site - Documents\\CSV Invoices\\%s' % (EnvConfig.PROJECT_ROOT, 'CSV 25th to 31st March 2023.csv')
-    VERSION                 = '1.0.4'
+    VERSION                 = '1.0.5'
```

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/filing/filing.py` & `cxmlinvbot-1.0.5/cxmlinvbot/filing/filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/mail/mail.py` & `cxmlinvbot-1.0.5/cxmlinvbot/mail/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/main.py` & `cxmlinvbot-1.0.5/cxmlinvbot/main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/mapping/action.py` & `cxmlinvbot-1.0.5/cxmlinvbot/mapping/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     def __init__(self, paths, defVal):
         super(Default, self).__init__(paths)
         self._defVal = defVal
 
     def perform(self, key, nvPairs):
         m = {}
         for p in self._paths:
-            m[p] = nvPairs.get(key, self._defVal)
+            tmp = nvPairs.get(key, '')
+            m[p] = tmp if len(tmp) else self._defVal
         return m
             
 
 class Ignore(MapAction):
     pass
```

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/mapping/headermapping.py` & `cxmlinvbot-1.0.5/cxmlinvbot/mapping/headermapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/mapping/invoicedetailrequestmapping.py` & `cxmlinvbot-1.0.5/cxmlinvbot/mapping/invoicedetailrequestmapping.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 class InvoiceDetailRequestMapping(Mapping):
   
   DTD_URL = BaseConfig.INVOICE_DETAIL_DTD_URL
 
   STRUCTURE = HeaderMapping.STRUCTURE + [
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailHeaderIndicator',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoiceDetailLineIndicator',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name',
+    'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress',
     'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitOfMeasure',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/UnitPrice/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Money',
@@ -35,14 +38,20 @@
     #'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/GrossAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
     'Request/InvoiceDetailRequest/InvoiceDetailSummary/DueAmount/Money',
   ]
 
   FIELD_TO_ACTION_MAPS = HeaderMapping.FIELD_TO_ACTION_MAPS + [dict(
+    BillToAddressID=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@addressID', '357122'),
+    ContactName=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name', 'CBRE MANAGED SERVICES LIMITED'),
+    POAddressLine1=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Street', '61 SOUTHWARK STREET'),
+    POCity=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/City', 'London'),
+    POPostalCode=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/PostalCode', 'SE1 0HL'),
+    POCountry=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/PostalAddress/Country@isoCountryCode', 'GB'),
     # This first set of fields come directly from the CSV and in the same order
     #SAVATRegNO=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Extrinsic',
     #                                'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic'),
     #                                '775685765'),
     InvoiceNumber=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceID'),
     Reference=cxmlinvbot.mapping.action.Required('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailOrderInfo/OrderReference/DocumentReference@payloadID'),      
     InvoiceDate=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceDate', lambda d : d.isoformat(), ('InvoiceDate',)),
@@ -98,18 +107,19 @@
     #                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Extrinsic@name'),
     #                                      'ProdoorVatRegNO'),
     InvoiceLineNum=cxmlinvbot.mapping.action.Default(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem@invoiceLineNumber',
                                           'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference@lineNumber'),
                                           '1'), # There is only ever 1 PO per Invoice hence defaulting to 1
     InvoiceOp=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@operation', 'new'),
     InvoiceOrigin=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@invoiceOrigin', 'supplier'),
-    InvoicePurpose=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader@purpose', 'standard'),
+    IPRole=cxmlinvbot.mapping.action.Default('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact@role', 'remitTo'),
     Language=cxmlinvbot.mapping.action.Default(( 'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/InvoiceDetailItemReference/Description@xml:lang',
                                       'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/Description@xml:lang',
-                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang'), 
+                                      'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/Description@xml:lang',
+                                      'Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/InvoicePartner/Contact/Name@xml:lang'), 
                                       'en'), # Standard xmlLangCode
     PayInNumDays=cxmlinvbot.mapping.action.Lambda('Request/InvoiceDetailRequest/InvoiceDetailRequestHeader/PaymentTerm@payInNumberOfDays', lambda d1, d2 : str((d1-d2).days), ('DueDate', 'InvoiceDate')),
     SubTotalAmount=cxmlinvbot.mapping.action.Lambda(('Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/SubtotalAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailOrder/InvoiceDetailItem/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/Tax/TaxDetail/TaxableAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/NetAmount/Money',
                                           'Request/InvoiceDetailRequest/InvoiceDetailSummary/SubtotalAmount/Money'),
```

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/mapping/mapping.py` & `cxmlinvbot-1.0.5/cxmlinvbot/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.0.5/cxmlinvbot/objects/cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.0.5/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.0.5/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,33 @@
             'another path': '999'
         }
 
         expectedRes3 = {
             'a path': '666'
         }
 
+        expectedRes4 = {
+            'a path': '999'
+        }
+        
         t = cxmlinvbot.mapping.action.Default(['a path', 'another path'], '999')
         res = t.perform('a key', {'a key' : '666'})
         self.assertEqual(res, expectedRes1)
 
-        t = cxmlinvbot.mapping.action.Default(('a path', 'another path'), '999')
-        res = t.perform('a key', {'a key' : '666'})
-        self.assertEqual(res, expectedRes1)
-
         res = t.perform('a key', {'no key': '666'})
         self.assertEqual(res, expectedRes2)
 
         t = cxmlinvbot.mapping.action.Default('a path', '999')
         res = t.perform('a key', {'a key' : '666'})
         self.assertEqual(res, expectedRes3)
 
+        t = cxmlinvbot.mapping.action.Default('a path', '999')
+        res = t.perform('a key', {'a key' : ''})
+        self.assertEqual(res, expectedRes4)
+
     def test_Lambda(self):
         expectedRes1 = {
             'a path': '25',
             'another path': '25'
         }
 
         t = cxmlinvbot.mapping.action.Lambda(['a path', 'another path'], operator.add, ('this key', 'that key'))
```

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.0.5/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/cxmlinvbot.egg-info/SOURCES.txt` & `cxmlinvbot-1.0.5/cxmlinvbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.4/setup.py` & `cxmlinvbot-1.0.5/setup.py`

 * *Files identical despite different names*

