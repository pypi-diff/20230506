# Comparing `tmp/cxmlinvbot-1.0.1.tar.gz` & `tmp/cxmlinvbot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxmlinvbot-1.0.1.tar", last modified: Sat May  6 09:57:33 2023, max compression
+gzip compressed data, was "cxmlinvbot-1.0.2.tar", last modified: Sat May  6 10:23:26 2023, max compression
```

## Comparing `cxmlinvbot-1.0.1.tar` & `cxmlinvbot-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.533538 cxmlinvbot-1.0.1/
--rw-rw-rw-   0        0        0      166 2023-05-06 09:57:33.532538 cxmlinvbot-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.438264 cxmlinvbot-1.0.1/cxmlinvbot/
--rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.0.1/cxmlinvbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.467709 cxmlinvbot-1.0.1/cxmlinvbot/config/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.0.1/cxmlinvbot/config/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-05-06 09:56:30.000000 cxmlinvbot-1.0.1/cxmlinvbot/config/base.py
--rw-rw-rw-   0        0        0      876 2023-05-06 09:02:35.000000 cxmlinvbot-1.0.1/cxmlinvbot/config/env.py
--rw-rw-rw-   0        0        0      561 2023-05-02 10:35:18.000000 cxmlinvbot-1.0.1/cxmlinvbot/config/mail.py
--rw-rw-rw-   0        0        0      251 2023-05-06 09:07:11.000000 cxmlinvbot-1.0.1/cxmlinvbot/kill.py
--rw-rw-rw-   0        0        0     7371 2023-05-06 09:07:34.000000 cxmlinvbot-1.0.1/cxmlinvbot/main.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.485666 cxmlinvbot-1.0.1/cxmlinvbot/objects/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.0.1/cxmlinvbot/objects/__init__.py
--rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.0.1/cxmlinvbot/objects/cxmlobject.py
--rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.0.1/cxmlinvbot/objects/profileresponse.py
--rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.0.1/cxmlinvbot/objects/response.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.527554 cxmlinvbot-1.0.1/cxmlinvbot/unittests/
--rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-05-06 09:50:28.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_action.py
--rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_cxmlobject.py
--rw-rw-rw-   0        0        0      932 2023-05-06 09:06:10.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_errors.py
--rw-rw-rw-   0        0        0     3048 2023-05-06 09:06:15.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_filing.py
--rw-rw-rw-   0        0        0     1107 2023-05-06 09:49:37.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_mapping.py
--rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_profileresponse.py
--rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_response.py
-drwxrwxrwx   0        0        0        0 2023-05-06 09:57:33.451231 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/
--rw-rw-rw-   0        0        0      166 2023-05-06 09:57:33.000000 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-05-06 09:57:33.000000 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 09:57:33.000000 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-06 09:57:33.000000 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 09:57:33.000000 cxmlinvbot-1.0.1/cxmlinvbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 09:57:33.533538 cxmlinvbot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      639 2023-05-06 09:55:52.000000 cxmlinvbot-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.462148 cxmlinvbot-1.0.2/
+-rw-rw-rw-   0        0        0      166 2023-05-06 10:23:26.461151 cxmlinvbot-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.331967 cxmlinvbot-1.0.2/cxmlinvbot/
+-rw-rw-rw-   0        0        0        0 2023-05-06 08:44:56.000000 cxmlinvbot-1.0.2/cxmlinvbot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.355878 cxmlinvbot-1.0.2/cxmlinvbot/config/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:14:10.000000 cxmlinvbot-1.0.2/cxmlinvbot/config/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-05-06 10:22:26.000000 cxmlinvbot-1.0.2/cxmlinvbot/config/base.py
+-rw-rw-rw-   0        0        0      876 2023-05-06 09:02:35.000000 cxmlinvbot-1.0.2/cxmlinvbot/config/env.py
+-rw-rw-rw-   0        0        0      561 2023-05-02 10:35:18.000000 cxmlinvbot-1.0.2/cxmlinvbot/config/mail.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.364854 cxmlinvbot-1.0.2/cxmlinvbot/errors/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:45.000000 cxmlinvbot-1.0.2/cxmlinvbot/errors/__init__.py
+-rw-rw-rw-   0        0        0      400 2023-05-05 17:26:49.000000 cxmlinvbot-1.0.2/cxmlinvbot/errors/errors.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.372833 cxmlinvbot-1.0.2/cxmlinvbot/filing/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:19:57.000000 cxmlinvbot-1.0.2/cxmlinvbot/filing/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-01 15:06:11.000000 cxmlinvbot-1.0.2/cxmlinvbot/filing/filing.py
+-rw-rw-rw-   0        0        0      251 2023-05-06 09:07:11.000000 cxmlinvbot-1.0.2/cxmlinvbot/kill.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.381364 cxmlinvbot-1.0.2/cxmlinvbot/mail/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:09.000000 cxmlinvbot-1.0.2/cxmlinvbot/mail/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-05-06 09:03:54.000000 cxmlinvbot-1.0.2/cxmlinvbot/mail/mail.py
+-rw-rw-rw-   0        0        0     7371 2023-05-06 09:07:34.000000 cxmlinvbot-1.0.2/cxmlinvbot/main.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.405299 cxmlinvbot-1.0.2/cxmlinvbot/mapping/
+-rw-rw-rw-   0        0        0        0 2023-05-06 10:20:19.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-05-06 09:04:07.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/action.py
+-rw-rw-rw-   0        0        0     4716 2023-05-06 09:51:52.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/headermapping.py
+-rw-rw-rw-   0        0        0    11468 2023-05-06 09:51:24.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/invoicedetailrequestmapping.py
+-rw-rw-rw-   0        0        0      638 2023-05-06 09:04:46.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/mapping.py
+-rw-rw-rw-   0        0        0      464 2023-05-06 09:52:03.000000 cxmlinvbot-1.0.2/cxmlinvbot/mapping/profilerequestmapping.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.421258 cxmlinvbot-1.0.2/cxmlinvbot/objects/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:11:56.000000 cxmlinvbot-1.0.2/cxmlinvbot/objects/__init__.py
+-rw-rw-rw-   0        0        0     5144 2023-05-06 09:08:47.000000 cxmlinvbot-1.0.2/cxmlinvbot/objects/cxmlobject.py
+-rw-rw-rw-   0        0        0     1359 2023-05-06 09:05:33.000000 cxmlinvbot-1.0.2/cxmlinvbot/objects/profileresponse.py
+-rw-rw-rw-   0        0        0      803 2023-05-06 09:05:41.000000 cxmlinvbot-1.0.2/cxmlinvbot/objects/response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.456163 cxmlinvbot-1.0.2/cxmlinvbot/unittests/
+-rw-rw-rw-   0        0        0        0 2023-04-19 11:22:52.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/__init__.py
+-rw-rw-rw-   0        0        0     2176 2023-05-06 09:50:28.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_action.py
+-rw-rw-rw-   0        0        0     2947 2023-05-06 09:06:03.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_cxmlobject.py
+-rw-rw-rw-   0        0        0      932 2023-05-06 09:06:10.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_errors.py
+-rw-rw-rw-   0        0        0     3048 2023-05-06 09:06:15.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_filing.py
+-rw-rw-rw-   0        0        0     1107 2023-05-06 09:49:37.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_mapping.py
+-rw-rw-rw-   0        0        0     2164 2023-05-06 09:46:38.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_profileresponse.py
+-rw-rw-rw-   0        0        0     1123 2023-05-06 09:07:06.000000 cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_response.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:26.342955 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/
+-rw-rw-rw-   0        0        0      166 2023-05-06 10:23:26.000000 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-06 10:23:26.000000 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:23:26.000000 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-06 10:23:26.000000 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-06 10:23:26.000000 cxmlinvbot-1.0.2/cxmlinvbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:23:26.462148 cxmlinvbot-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      639 2023-05-06 09:55:52.000000 cxmlinvbot-1.0.2/setup.py
```

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/config/base.py` & `cxmlinvbot-1.0.2/cxmlinvbot/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,8 @@
         'ProfileResponseInvalidXML' : '%sprofileresponseinvalidxml.xml' % SAMPLE_PATH,
         'ProfileResponseInvalidDTD' : '%sprofileresponseinvaliddtd.xml' % SAMPLE_PATH,
         'Response'                  : '%sresponse.xml' % SAMPLE_PATH,
         'ResponseWithData'          : '%sresponsewithdata.xml' % SAMPLE_PATH,
     }
     
     CSV_SAMPLE              = '%sCXML Site - Documents\\CSV Invoices\\%s' % (EnvConfig.PROJECT_ROOT, 'CSV 25th to 31st March 2023.csv')
-    VERSION                 = '1.0.1'
+    VERSION                 = '1.0.2'
```

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/config/env.py` & `cxmlinvbot-1.0.2/cxmlinvbot/config/env.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/config/mail.py` & `cxmlinvbot-1.0.2/cxmlinvbot/config/mail.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/main.py` & `cxmlinvbot-1.0.2/cxmlinvbot/main.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/objects/cxmlobject.py` & `cxmlinvbot-1.0.2/cxmlinvbot/objects/cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/objects/profileresponse.py` & `cxmlinvbot-1.0.2/cxmlinvbot/objects/profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/objects/response.py` & `cxmlinvbot-1.0.2/cxmlinvbot/objects/response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_action.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_action.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_cxmlobject.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_cxmlobject.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_errors.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_filing.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_filing.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_mapping.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_profileresponse.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_profileresponse.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/cxmlinvbot/unittests/test_response.py` & `cxmlinvbot-1.0.2/cxmlinvbot/unittests/test_response.py`

 * *Files identical despite different names*

### Comparing `cxmlinvbot-1.0.1/setup.py` & `cxmlinvbot-1.0.2/setup.py`

 * *Files identical despite different names*

