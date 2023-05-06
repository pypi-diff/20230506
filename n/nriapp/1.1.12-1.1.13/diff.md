# Comparing `tmp/nriapp-1.1.12.tar.gz` & `tmp/nriapp-1.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.12.tar", last modified: Wed Apr 19 15:02:09 2023, max compression
+gzip compressed data, was "nriapp-1.1.13.tar", last modified: Sat May  6 05:16:40 2023, max compression
```

## Comparing `nriapp-1.1.12.tar` & `nriapp-1.1.13.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.12/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.12/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-04-19 15:02:09.499948 nriapp-1.1.12/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.12/README
--rw-rw-rw-   0        0        0      336 2023-04-19 14:16:22.000000 nriapp-1.1.12/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 15:02:09.499948 nriapp-1.1.12/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-04-19 15:01:23.000000 nriapp-1.1.12/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.484348 nriapp-1.1.12/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.12/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    13961 2023-04-19 14:54:34.000000 nriapp-1.1.12/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    25938 2023-04-19 14:57:41.000000 nriapp-1.1.12/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.484348 nriapp-1.1.12/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.790962 nriapp-1.1.13/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.13/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.13/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-05-06 05:16:40.790962 nriapp-1.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.13/README
+-rw-rw-rw-   0        0        0      325 2023-05-06 05:06:53.000000 nriapp-1.1.13/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-05-06 05:16:40.790962 nriapp-1.1.13/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-05-06 05:07:12.000000 nriapp-1.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.619362 nriapp-1.1.13/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.712962 nriapp-1.1.13/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.13/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.728562 nriapp-1.1.13/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.13/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.13/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.775362 nriapp-1.1.13/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    17188 2023-05-05 05:36:38.000000 nriapp-1.1.13/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.13/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   101629 2023-04-30 17:20:44.000000 nriapp-1.1.13/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.775362 nriapp-1.1.13/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.13/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.13/src/nriapp/helper/visualization.py
+drwxrwxrwx   0        0        0        0 2023-05-06 05:16:40.697362 nriapp-1.1.13/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-05-06 05:16:39.000000 nriapp-1.1.13/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-05-06 05:16:40.000000 nriapp-1.1.13/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 05:16:39.000000 nriapp-1.1.13/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-06 05:16:39.000000 nriapp-1.1.13/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 05:16:39.000000 nriapp-1.1.13/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    36761 2023-04-29 10:16:03.000000 nriapp-1.1.13/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.12/LICENSE` & `nriapp-1.1.13/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/setup.py` & `nriapp-1.1.13/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.12',
+   version='1.1.13',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.12/src/nriapp/changelog.txt` & `nriapp-1.1.13/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.13/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.13/src/nriapp/core/dataexplorer.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 from azure.kusto.data import KustoClient, KustoConnectionStringBuilder, ClientRequestProperties
 from azure.kusto.data.exceptions import KustoServiceError
 from azure.kusto.data.helpers import dataframe_from_result_table
 from azure.identity import DeviceCodeCredential
 import json
 import pandas as pd
 import os
+import requests
 import concurrent.futures
 from tqdm import tqdm
-import pickle, cloudpickle
-from datetime import date
+import pickle
+from datetime import date, datetime, timedelta
+from bs4 import BeautifulSoup
+import dateutil.parser as parser 
+import pytz
+from pytz import timezone
+
 
 desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop') 
 
 session_file = os.path.abspath(os.path.dirname(__file__)) + "\..\session\kusto.pkl"
 tenant_id = "bcf2d2a2-2dee-419b-971f-21e5170fbf84"
 KUSTO_URI = "https://kvcw1z66xgnuy00q1uhhzs.australiaeast.kusto.windows.net"
 KUSTO_INGEST_URI = "https://ingest-kvcw1z66xgnuy00q1uhhzs.australiaeast.kusto.windows.net"
@@ -52,15 +58,14 @@
         Raw
         | extend a = parse_json(Events)
         | distinct items= tostring(a)
         | extend a = parse_json(items)
         | project IncidentId=toint(a.IncidentId), Status=toint(a.Status)
         | sort by IncidentId desc 
         '''
-
         response = self.client_query.execute(database, check_changes)
         
         results = response.primary_results[0]
 
         set1 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"]}, sort_keys=True) for x in results) #Serialize
         set2 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"]}, sort_keys=True) for x in data)    #Serialize
 
@@ -102,25 +107,42 @@
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="RawEventMapping")
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
         return data
 
-
-    def ingest_mfastats(self, data, database="Incidents", table="Multifactor"):
-        item_list = '''
-        Multifactor
-        | extend items = parse_json(Items)
-        | project items.ID
+    def check_ingest_mfastats_tag(self, database="Incidents", table="Authentication"):
+        tag = date.today().strftime("%Y-%m-%d")
+        
+        current_tags = ''' Authentication
+        | extend tags = tostring(extent_tags())
+        | distinct tags
+        | extend item = parse_json(tags)
+        | mv-expand tag = item
+        | project trim_start("ingest-by:", tostring(tag))
         '''
-        response = self.client_query.execute(database, item_list)
-        user_ids = [i[0] for i in response.primary_results[0].raw_rows]
-        ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.JSON)
-        self.ingest_raw(data, ingestion_props)
+        response = self.client_query.execute(database, current_tags)        
+        tags = [i[0] for i in response.primary_results[0].raw_rows]
+        for i in tags:
+            if tag == i:
+                return True
+        return False
+
+    def ingest_mfastats(self, data, database="Incidents", table="Authentication"):
+        tag = date.today().strftime("%Y-%m-%d")
+
+        path = os.path.join(desktop, "authentication.tmp")
+        with open(path, "w") as file:
+            for item in data:
+                file.write(json.dumps(item) + "\n")
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="AuthenticationMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
 
     def ingest_audit_logs(self, data, database="Incidents", table="AuditHistory"):
         to_ingest = [i["id"] for i in data]
         pending = ', '.join(str(i) for i in to_ingest)
         if not pending:
             return data
         remove_list = '''
@@ -158,27 +180,14 @@
             if tag == i:
                 return True
         return False
 
     def ingest_users(self, data, database="Incidents", table="AzureAD"):
         tag = date.today().strftime("%Y-%m-%d")
 
-        current_tags = '''
-        AzureAD
-        | extend tags = tostring(extent_tags())
-        | distinct tags
-        | extend item = parse_json(tags)
-        | mv-expand tag = item
-        | project trim_start("ingest-by:", tostring(tag))
-        '''
-        response = self.client_query.execute(database, current_tags)        
-        tags = [i[0] for i in response.primary_results[0].raw_rows]
-        for i in tags:
-            if tag == i:
-                return
         path = os.path.join(desktop, "users.tmp")
         with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="FlatEventMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
@@ -201,27 +210,14 @@
             if tag == i:
                 return True
         return False
 
     def ingest_devices(self, data, database="Incidents", table="IntuneDevices"):
         tag = date.today().strftime("%Y-%m-%d")
 
-        current_tags = '''
-        IntuneDevices
-        | extend tags = tostring(extent_tags())
-        | distinct tags
-        | extend item = parse_json(tags)
-        | mv-expand tag = item
-        | project trim_start("ingest-by:", tostring(tag))
-        '''
-        response = self.client_query.execute(database, current_tags)        
-        tags = [i[0] for i in response.primary_results[0].raw_rows]
-        for i in tags:
-            if tag == i:
-                return
         path = os.path.join(desktop, "devices.tmp")
         with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="IntuneDevicesMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
@@ -244,28 +240,14 @@
             if tag == i:
                 return True
         return False
 
     def ingest_managed_devices(self, data, database="Incidents", table="ManagedDevices"):
         tag = date.today().strftime("%Y-%m-%d")
 
-        current_tags = '''
-        ManagedDevices
-        | extend tags = tostring(extent_tags())
-        | distinct tags
-        | extend item = parse_json(tags)
-        | mv-expand tag = item
-        | project trim_start("ingest-by:", tostring(tag))
-        '''
-        response = self.client_query.execute(database, current_tags)        
-        tags = [i[0] for i in response.primary_results[0].raw_rows]
-        for i in tags:
-            if tag == i:
-                return
-
         path = os.path.join(desktop, "managedDevices.tmp")
         with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="ManagedDevicesMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
             self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
@@ -276,51 +258,118 @@
         tag = date.today().strftime("%Y-%m-%d")
 
         ingestion_props =  IngestionProperties(database=database,table=table,data_format=DataFormat.CSV, ingestion_mapping_reference="DefenderAgents_mapping", additional_properties={'ignoreFirstRecord': 'true'},  ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
         result = self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
         os.remove(path)
         return result   
 
+    def check_signin_last_timestamp(self, database="Incidents", table= "SignInLogs"):
+
+        created_datetime = '''
+        let abc = SignInLogs
+        | distinct ingestion_time()
+        | summarize max($IngestionTime);
+        SignInLogs
+        | where ingestion_time() == toscalar(abc)
+        | project item = parse_json(Items)
+        | sort by todatetime(item.createdDateTime) desc 
+        | take 1
+        | project upper=todatetime(item.createdDateTime)
+        '''
+        response = self.client_query.execute(database, created_datetime)  
+        t_lower = response.primary_results[0].rows[0]["upper"]
+        lower_limit = (t_lower + timedelta(hours=1)).replace(minute=0, second=0, microsecond=0)
+        return lower_limit.strftime("%Y-%m-%dT%H:%M:%SZ")
 
+    def ingest_signin_logs(self, data, database="Incidents", table= "SignInLogs"):
+        
+        path = os.path.join(desktop, "signIns.tmp")
+        with open(path, "w") as file:
+            for item in data:
+                file.write(json.dumps(item) + "\n")
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="SignInLogsMapping") 
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
 
-    kusto_query = '''
-    let minimum = toscalar (
-    Raw
-    | extend a = parse_json(Events)
-    | top 1 by toint(a.IncidentId) asc
-    );
-    let maximum = toscalar (
-    Raw
-    | extend a = parse_json(Events)
-    | top 1 by toint(a.IncidentId) desc 
-    );
-    print highest=maximum.IncidentId,lowest=minimum.IncidentId;
-    '''
+    def get_latest_av_engines(self):
 
+        defender_updates = "https://www.microsoft.com/en-us/wdsi/defenderupdates"
+        
+        response = requests.get(defender_updates, headers={"User-Agent" : "PostmanRuntime/7.32.2"})
+        soup = BeautifulSoup(response.content, 'html.parser')
 
+        ul_tag = soup.find("ul", {"class" : "c-list list-bottom-margin"})
+        version_info = {}
+        for i in ul_tag.find_all("li"):
+                if "Version" == i.text.split(": ", 1)[0]:
+                    version_info["SignatureVersion"] =  i.text.split(": ", 1)[1]
+                elif "Engine Version" == i.text.split(": ", 1)[0]:
+                    version_info["EngineVersion"] = i.text.split(": ", 1)[1]
+                elif "Platform Version" ==  i.text.split(": ", 1)[0]:
+                    version_info["PlatformVersion"] = i.text.split(": ", 1)[1]
+                elif "Released" == i.text.split(": ", 1)[0]:
+                    dt = parser.parse(i.text.split(": ", 1)[1])
+                    local_tz = pytz.timezone('Asia/Singapore')
+                    utc_time = local_tz.localize(dt).astimezone(pytz.UTC)
+                    version_info["ReleaseDateUtc"] = utc_time.strftime("%Y-%m-%dT%H:%M")
+
+        return version_info
+
+    def check_latest_av_engines(self, database="Incidents", table= "AVEngineVersion"):
+
+        latest_release = '''
+        AVEngineVersion
+        | extend item = parse_json(Items)
+        | extend release = todatetime(item.ReleaseDateUtc)
+        | summarize latest=max(release)
+        '''
+        response = self.client_query.execute(database, latest_release)        
+        latest_date = response.primary_results[0].raw_rows[0]
+
+        if latest_date:
+            return latest_date[0]
+        else:
+            return
+
+    def ingest_latest_av_engine(self, data, database="Incidents", table= "AVEngineVersion"):
+
+        path = os.path.join(desktop, "av.tmp")
+        with open(path, "w") as file:
+            file.write(json.dumps(data))
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.JSON, ingestion_mapping_reference="AVEngineVersionMapping")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
+
+    def get_latest_compliance_ingestion_time(self, database="Incidents", table= "CompliancePolicy"):
+
+        t_latest = datetime.now(pytz.utc)
+#        latest_date = (t_latest + timedelta(days=1)).replace(hour=0, minute=0, second=0, microsecond=0)
+        latest_date = t_latest.replace(hour=0, minute=0, second=0, microsecond=0)
+#        latest_date =t_latest.replace(day=t_latest.day+1, hour=0, minute=0, second=0, microsecond=0)
+
+        latest_compliance_ingestion_time = '''
+        CompliancePolicy
+        | summarize out=max(ingestion_time())
+        | take 1
+        '''
+        response = self.client_query.execute(database, latest_compliance_ingestion_time)        
+        current_date = response.primary_results[0].rows[0]["out"]
+
+        if not current_date or (current_date.replace(hour=0, minute=0, second=0, microsecond=0) < latest_date):
+            return True 
+        else:
+            return False
+
+    def ingest_compliance_policy(self, data, database="Incidents", table = "CompliancePolicy"):
+
+        path = os.path.join(desktop, "compliance_policy.tmp")
+        with open(path, "w") as file:
+            for item in data:
+                file.write(json.dumps(item) + "\n")
+        if data:
+            ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="CompliancePolicyMapping")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)    
 
-#    for i in data[:]:
-#        if i["IncidentId"] in similar:
-#            data.remove(i)
-
-#    response = client_query.execute(DATABASE, kusto_query)
-#    row = response.primary_results[0].rows[0]
-#    highest = row[0]
-#    lowest = row[1]
-
-    #json_str = json.dumps({"Events": data})
-    #jsonFile = open("data.json", "w")
-    #jsonFile.write(json_str)
-    #jsonFile.close()
-
-#    with open("data.json", "w") as file:
-#        for i in data:
-#            file.write(json.dumps(i) + '\n')
-
-#    df = pd.DataFrame({"events": [json.dumps({"Events": data})]})
-#    df = pd.DataFrame({"events": [json.dumps(my_dict)]})
-#    df = pd.DataFrame({"events": [json.dumps(data[3])]})
-#    ingestion_props = IngestionProperties(database="Incidents",table="Raw",data_format=DataFormat.JSON, ingestion_mapping_reference="Ewan")
-#    ingestion_props = IngestionProperties(database="Incidents",table="Raw",data_format=DataFormat.JSON, ingestion_mapping_reference="RawMap")
-#    file_descriptor = FileDescriptor ("data.json", os.stat("data.json").st_size)#
-#    client_ingest.ingest_from_file(file_descriptor, ingestion_properties=ingestion_props)
```

### Comparing `nriapp-1.1.12/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.13/src/nriapp/core/msgraphapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import requests, json, pickle, ast, zipfile, re
 from urllib.parse import urlparse, parse_qs
 sys.path.append("..") # Adds higher directory to python modules path.
 from config.config import *
 from helper import login
 from loguru import logger
 from urllib.parse import parse_qs, urlsplit, parse_qsl
+from datetime import datetime, timedelta
 
 #dbgPrint = PyLog(__name__, level=logging.INFO)
 
 logger.add(f"./logs/{__name__}.log", backtrace=True, diagnose=True, filter="MSGraphApi")
 dbgPrint = logger
 #dbgPrint.disable(__name__)
 
@@ -21,15 +22,15 @@
 #        self.auth_page = 'https://portal.azure.com/api/DelegationToken?feature.cacheextensionapp=true&feature.internalgraphapiversion=true&feature.tokencaching=true'
         self.headers = kwargs.get('headers', {'content-type' : 'application/json'})
         self.cookies = kwargs.get('cookies', {})
 #        self.auth_folder = kwargs.get('output', "")
         self.body = kwargs.get('json', '')
 
         self.users_auth = ""
-        self.mfa_stats_auth = ""
+        self.iam_auth = ""
         self.devices_auth = ""
         self.email = email
 
         self._portalAuthorization = {}
         self._altPortalAuthorization = {}
         self._session.cookies.update(self.cookies)
         self._session.headers.update(self.headers)
@@ -50,24 +51,29 @@
             dbgPrint.error("Unexpected argument")
             raise("Unexpected **kwargs argument")
 #        response = requests.models.Response
         for i in range(10):
             try:
                 if params or (not data):
                     response = self._session.get(arg, headers=headers, params=params, verify=False)
-                    if response.status_code == 440 or response.status_code == 401:
+                    if response.status_code == 440:
                         login.Login().delete_session()
                         login.Login(self.email).login()
                         self.load_session()
                         continue
+                    elif response.status_code == 401:
+                        break
                     elif response.status_code == 200:
                         break
                     elif response.status_code == 500:
                         message = json.loads(response.text)
                         dbgPrint.error(message["Message"])
+                    elif response.status_code == 503:
+                        dbgPrint.error("Service Unavailable")
+                        continue
                     elif response.status_code == 504:
                         dbgPrint.error("Gateway Time-out")
                     elif response.status_code == 429:
                         message = json.loads(response.text)
                         dbgPrint.error(message["error"]["message"])
                         continue
                 else:
@@ -161,15 +167,15 @@
         'extensionName': 'Microsoft_Intune_Enrollment',
         'resourceName': 'microsoft.graph',
         'tenant': TENANT_ID,
         'portalAuthorization': self._authorization['portalAuthorization'],
         'altPortalAuthorization': self._authorization['altPortalAuthorization']        
         }
 
-        response = self._session.post(self.auth_page, json=json_data, verify=False)
+        response = self.tryrequest(self.auth_page, json=json_data)
         bearer = json.loads(response.text)
         enrollment_auth = bearer["value"]["authHeader"]
         return enrollment_auth
 
     def save_session(self):
 
         session_path = os.path.abspath(os.path.dirname(__file__)) + "\..\session"
@@ -192,15 +198,15 @@
                 cookies = pickle.load(f)
                 json_data = pickle.load(f)
             self.cookies = cookies
             self.body = json_data
             self.__init__(self.email, cookies=cookies, json=json_data)
             self.users_auth = self.get_aad_authorization()
             self.devices_auth = self.get_intune_authorization()
-            self.mfa_stats_auth = self.get_iam_authorization()
+            self.iam_auth = self.get_iam_authorization()
             self.intune_enrollment_auth = self.get_enrollment_authorization()
         else:
             session = login.Login(self.email)
             session.delete_session()
             session.login()
             self.load_session()
         return self
@@ -280,30 +286,16 @@
             skiptoken = "&skiptoken=" + skiptoken
 
         json_data = {
         'requests': [
             {
             'id': "searched_user",
             'method': "GET",
-            'url': "/users?$select=id," 
-            "displayName,"
-            "givenName,"
-            "surname,"
-            "userPrincipalName,"
-            "userType,"
-            "country,"
-            "accountEnabled,"
-            "usageLocation,"
-            "lastPasswordChangeDateTime,"
-            "officeLocation,"
-            "otherMails,"
-            "proxyAddresses,"
-            "passwordPolicies,"
-            "companyName"
-            "&$top=999"
+            'url': "/users?"
+            "$top=999"
             "&$count=true"
             "&$orderby=displayName asc"+skiptoken,
             'headers': {
                 'ConsistencyLevel': "eventual",
                 'x-ms-command-name': "UserManagement - ListUsers",
                         }
                     }
@@ -475,26 +467,14 @@
                 dbgPrint.info(len(device_list))
                 self.get_all_devices_beta(skiptoken=skiptoken+top, device_list=device_list)
             else:
                 device_list.extend(object["value"])
                 dbgPrint.info(len(device_list))
         return device_list
 
-    def check_mfa_status(self, userPrincipalName):
-        mfa_status = 'https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails'
-        params = {'$filter' : "userPrincipalName eq '" + userPrincipalName + "'"}
-        headers = {
-        'Authorization': self.mfa_stats_auth,
-        'content-type': 'application/json'
-        }
-        response = self.tryrequest(mfa_status, headers=headers, params=params)
-
-#        response = self._session.get(mfa_status, headers=headers, params=params, verify=False)
-        return json.loads(response.text).get('value', {})
-
     def get_user_groups(self, userPrincipalName):
         user_object = self.search_user(userPrincipalName)
 
         user_groups = 'https://graph.microsoft.com/beta/users/' + user_object[0]["id"] + '/memberOf/$/microsoft.graph.group'
 
 
         params = {
@@ -643,14 +623,154 @@
         status = object["status"]
         while status != "completed":
             dbgPrint.debug(status)
             result = self.tryrequest(export_job_result, headers=headers)
             object = json.loads(result.text)
             status = object["status"]        
         
+
         desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop') 
         dbgPrint.debug(status)
         agents_file = self.tryrequest(object["url"])
         dbgPrint.debug(object["url"])
         z = zipfile.ZipFile(io.BytesIO(agents_file.content))
         z.extract(id+".csv", path=desktop)
         return os.path.join(desktop, id + ".csv")
+
+
+    def check_mfa_status(self, userPrincipalName):
+        mfa_status = 'https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails'
+        params = {'$filter' : "userPrincipalName eq '" + userPrincipalName + "'"}
+        headers = {
+        'Authorization': self.iam_auth,
+        'content-type': 'application/json'
+        }
+        response = self.tryrequest(mfa_status, headers=headers, params=params)
+
+#        response = self._session.get(mfa_status, headers=headers, params=params, verify=False)
+        return json.loads(response.text).get('value', {})
+
+    def get_users_mfa(self, skiptoken="", top=50, mfa_list=[]):
+        mfa_status = 'https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails'
+        params = {'$filter' : ""}
+
+        if skiptoken:
+            params["$skiptoken"] = skiptoken
+
+        headers = {
+        'Authorization': self.iam_auth,
+        'content-type': 'application/json'
+        }
+        response = self.tryrequest(mfa_status, headers=headers, params=params)
+        while(response.status_code != 200):
+            if response.status_code == 401:
+                self.iam_auth=self.get_iam_authorization()
+                headers = {
+                'Authorization': self.iam_auth,
+                'content-type': 'application/json'
+                }
+                response = self.tryrequest(sign_ins, headers=headers, params=params)
+
+        if response.status_code == 200:
+            object = json.loads(response.text)
+            nextlink = object.get("@odata.nextLink")
+            if nextlink != None:
+                mfa_list.extend(object["value"])
+                dbgPrint.info(len(mfa_list))
+                skiptoken = dict(parse_qsl(urlsplit(nextlink).query)).get("$skiptoken") if dict(parse_qsl(urlsplit(nextlink).query)).get("$skiptoken") else dict(parse_qsl(urlsplit(nextlink).query)).get("skiptoken", "")
+                self.get_users_mfa(skiptoken=skiptoken, mfa_list=mfa_list)
+            else:
+                mfa_list.extend(object["value"])
+                dbgPrint.info(len(mfa_list))
+        return mfa_list
+
+    def get_signin_logs(self, result=[], top=1000, skiptoken="", min="", max=""):
+        
+        sign_ins = "https://graph.microsoft.com/beta/auditLogs/signIns"
+
+        params = {
+            "api-version"   : "beta", 
+            "$filter"       : "(createdDateTime ge "+ min +" and createdDateTime lt " + max + ")",
+            "$top"          : top,
+            "$orderby"      : "createdDateTime desc",
+            "source"        : "kds"
+        }
+        if skiptoken:
+            params["$skiptoken"] = skiptoken
+
+
+        headers = {
+        'Authorization': self.iam_auth,
+        'content-type': 'application/json'
+        }
+
+
+        response = self.tryrequest(sign_ins, headers=headers, params=params)
+        while(response.status_code != 200):
+            if response.status_code == 401:
+                self.iam_auth=self.get_iam_authorization()
+                headers = {
+                'Authorization': self.iam_auth,
+                'content-type': 'application/json'
+                }
+                response = self.tryrequest(sign_ins, headers=headers, params=params)
+
+        if response.status_code == 200:
+            object = json.loads(response.text)
+            nextlink = object.get("@odata.nextLink")
+            if nextlink != None:
+                result.extend(object["value"])
+                dbgPrint.info(len(result))
+                skiptoken = dict(parse_qsl(urlsplit(nextlink).query)).get("$skiptoken") if dict(parse_qsl(urlsplit(nextlink).query)).get("$skiptoken") else dict(parse_qsl(urlsplit(nextlink).query)).get("skiptoken", "")
+                return skiptoken
+            else:
+                result.extend(object["value"])
+                dbgPrint.info(len(result))
+
+    def get_all_signins(self, login_logs=[], top=1000, min="", max=""):
+        now = datetime.utcnow().replace(minute=0, second=0, microsecond=0)
+
+        if not min:
+            t_lower = now - timedelta(days=30)
+            t_lower = t_lower.replace(minute=0, second=0, microsecond=0, hour=t_lower.hour+1)
+            t_upper = t_lower + timedelta(hours=1)
+        else:
+            t_lower = datetime.strptime(min, "%Y-%m-%dT%H:%M:%SZ")
+            t_lower = t_lower.replace(minute=0, second=0, microsecond=0)
+            t_upper = t_lower + timedelta(hours=1)
+
+        if now < t_upper:
+            return None
+
+        lower_limit = t_lower.strftime("%Y-%m-%dT%H:%M:%SZ")
+        upper_limit = t_upper.strftime("%Y-%m-%dT%H:%M:%SZ")
+
+        skiptoken = self.get_signin_logs(result=login_logs, top=top, min=lower_limit, max=upper_limit)
+
+        while(skiptoken):
+            dbgPrint.info(skiptoken)
+            skiptoken = self.get_signin_logs(result=login_logs, top=top, skiptoken=skiptoken, min=lower_limit, max=upper_limit)
+
+        return upper_limit
+
+    
+    def get_compliance_policy(self):
+        device_compliance = "https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies"
+
+        headers = {
+            "Authorization" : self.devices_auth
+        }
+
+        response = self.tryrequest(device_compliance, headers=headers)
+        for i in range(3):
+            if response.status_code == 200: 
+                break
+            elif response.status_code == 401:
+                self.devices_auth = self.get_intune_authorization()
+                headers = {
+                    "Authorization" : self.devices_auth
+                }
+                response = self.tryrequest(device_compliance, headers=headers)
+
+        result = json.loads(response.text)["value"]
+        return result
+
```

### Comparing `nriapp-1.1.12/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.13/src/nriapp/core/mssentinelapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,16 @@
                     break
                 else:
                     dbgPrint.info("Sending POST request")
                     response = self._session.post(arg, headers=headers, json=data, verify=False)
                     if response.status_code == 440:
                         login.Login().delete_session()
                         login.Login(self.email).login()
-                        self.load_session()
+#                        self.load_session()
+                        break
                     elif response.status_code == 200:
                         break
                     elif response.status_code == 500:
                         message = json.loads(response.text)
                         dbgPrint.error(message["Message"])
                         sys.exit()
                     elif response.status_code == 504:
@@ -130,14 +131,19 @@
             'lookBackInDays': str(lookBackInDays),
             'isMultipleIncidents': True,
             'alertStatus': alertStatus,
             'severity': severity,
             'pageIndex': pageIndex,
             }
         response = self.tryrequest(incident_alerts, json=json_data)
+        while(response.status_code != 200):
+            if response.status_code == 440:
+                self.load_session()
+                response = self.tryrequest(incident_alerts, json=json_data)
+
         incident_list.extend(json.loads(response.text))
 
         if len(json.loads(response.text)) == pageSize:
             items = self.get_incidents(incidentId,pageIndex=pageIndex+1,lookBackInDays = 180, pageSize = 3000)
             return items
         else:
             if incidentId:
```

### Comparing `nriapp-1.1.12/src/nriapp/core/multifactor.py` & `nriapp-1.1.13/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/core/vtquery.py` & `nriapp-1.1.13/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/helper/doc.py` & `nriapp-1.1.13/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/helper/login.py` & `nriapp-1.1.13/src/nriapp/helper/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,26 +143,25 @@
         http_rqst = helper.RequestHeader(self.driver, "api/DelegationToken")         #1/27/2023 5:00:48 PM 
         cookie = http_rqst.get_param("cookie")
 
         json_data = json.loads(http_rqst.body)
 
         msgraph.MSGraphApi(cookies=cookie, json=json_data, verify=False).save_session()
 
-        self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", self.email, self.organization)
+#        self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", self.email, self.organization)
 
-        self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
-#            self.wait(driver, 20, By.XPATH, "//img[@boxtype='Image' and @title='Search']")
+#        self.wait(self.driver, 20, By.ID, "UserListGrid_ActionBarContainer")
 
-        time.sleep(2)
-        http_rqst = helper.RequestHeader(self.driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
-        cookies = http_rqst.get_param("Cookie")
-        headers = dict(http_rqst.headers._headers)
-        page = mfa.MultiFactor(cookies=cookies, headers=headers)            
+#        time.sleep(2)
+#        http_rqst = helper.RequestHeader(self.driver, "/GenericGetAvailableFilters.ajax")         #1/27/2023 5:00:48 PM 
+#        cookies = http_rqst.get_param("Cookie")
+#        headers = dict(http_rqst.headers._headers)
+#        page = mfa.MultiFactor(cookies=cookies, headers=headers)            
 
-        page.save_session()
+#        page.save_session()
 
         self.driver.quit()
 
     def mfa_login(self, email):
         self.driver = self.create_driver()  
         self.web_app(self.driver , "https://account.activedirectory.windowsazure.com/usermanagement/multifactorverification.aspx?", email, self.organization)
```

### Comparing `nriapp-1.1.12/src/nriapp/helper/pylog.py` & `nriapp-1.1.13/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/helper/requestheader.py` & `nriapp-1.1.13/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.13/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.12/src/nriapp/nriapp.py` & `nriapp-1.1.13/src/nriapp/nriapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import queue
 import re
 
 sys.path.append("..")
 
 from core import msgraphapi as graphapi 
 from core import mssentinelapi as defender
-from core import multifactor as mfaauth
-from core import dataexplorer as dex
+#from core import multifactor as mfaauth
+from core import dataexplorer as adx
 from core.abuseipdbapi import ipquery
 from helper import requestheader as helper
 from helper import login
 from helper.doc import *
 from helper.doc import WordDoc
 from helper.excel import WorkBook
 
@@ -90,15 +90,15 @@
 #        self.output = self.args.get("output",  os.path.abspath(os.path.dirname(__file__)) + "\\output")
        
         self.write_config()
         self.read_config()
 
         if self.email and not hasattr(self, "msgraph"):
             self.msgraph = graphapi.MSGraphApi(self.email).load_session()
-            self.mfa = mfaauth.MultiFactor(self.email).load_session()
+#            self.mfa = mfaauth.MultiFactor(self.email).load_session()
             self.sentinel = defender.MSSentinelApi(self.email).load_session()
 
             
     def write_config(self):
         self.config = configparser.RawConfigParser()
         self.config.read(os.path.abspath(os.path.dirname(__file__)) + '\config.ini')
         flag = False
@@ -491,31 +491,47 @@
                     for x,y in a.items():
                         if x == "userPrincipalName":
                             if y["companyName"] not in company:
                                 company.append(y["companyName"])
 
          
     def get_timely_report(self, lookBackInDays, duration=5):
-            
-
-
+        
         t_end = time.time() + 60 * duration
-        dataexplorer = dex.DataIngestion()
-        while time.time() < t_end:
+        dataexplorer = adx.DataIngestion()
 
-            dbgPrint.debug("Fetching incidents data")
-            incidents = self.sentinel.get_incidents(incidentId=0, 
-                                                    alertStatus=['New','InProgress', 'Resolved'] , 
-                                                    severity=[256,128,64,32], 
-                                                    pageIndex=1, 
-                                                    lookBackInDays=lookBackInDays, 
-                                                    pageSize=3000, 
-                                                    ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
+        utc_timezone = pytz.UTC
 
+        while time.time() < t_end:
     #        incidents_cpy = incidents[:]
+            if dataexplorer.get_latest_compliance_ingestion_time():
+                policy = self.msgraph.get_compliance_policy()
+                dataexplorer.ingest_compliance_policy(data=policy) 
+
+            av_engines = dataexplorer.get_latest_av_engines()
+            recent_date = dataexplorer.check_latest_av_engines()
+            if not recent_date:
+                dataexplorer.ingest_latest_av_engine(data=av_engines)
+
+            elif utc_timezone.localize(parser.parse(av_engines["ReleaseDateUtc"])) > parser.parse(recent_date):
+                dataexplorer.ingest_latest_av_engine(data=av_engines)
+
+            signin_logs = []
+            last_created_time = dataexplorer.check_signin_last_timestamp()        
+            lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=last_created_time)
+            dataexplorer.ingest_signin_logs(data=signin_logs)
+            del signin_logs[:]
+            while(lower_limit):
+                lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=lower_limit)
+                dataexplorer.ingest_signin_logs(data=signin_logs)
+                del signin_logs[:]
+
+            if not dataexplorer.check_ingest_mfastats_tag():
+                mfa_list = self.msgraph.get_users_mfa()
+                dataexplorer.ingest_mfastats(data=mfa_list)
 
             if not dataexplorer.check_ingest_managed_devices_tag():
                 dbgPrint.debug("Fetching all Intune devices")
                 devices = self.msgraph.get_all_devices_beta()
                 dbgPrint.debug("Ingesting data")
                 dataexplorer.ingest_managed_devices(data=devices)
                 del devices[:]
@@ -532,15 +548,22 @@
                 all_users = self.msgraph.get_all_users()
                 dbgPrint.debug("Ingesting data")  
                 dataexplorer.ingest_users(data=all_users)
                 del all_users[:]
 
             defender_agents = self.msgraph.get_defender_agents()
             dataexplorer.ingest_defender_agents(path=defender_agents)
-
+            dbgPrint.debug("Fetching incidents data")
+            incidents = self.sentinel.get_incidents(incidentId=0, 
+                                                    alertStatus=['New','InProgress', 'Resolved'] , 
+                                                    severity=[256,128,64,32], 
+                                                    pageIndex=1, 
+                                                    lookBackInDays=lookBackInDays, 
+                                                    pageSize=3000, 
+                                                    ) #sourceFilter=[16384, 1048576], titleFilter=["eDiscovery"]      #16384 == MCAS incidents 512 = eDiscovery
             dbgPrint.debug("Ingesting data")
             audit = dataexplorer.ingest_events(data=incidents)
             dbgPrint.debug("Fetching audit logs of incidents")
             audit_logs = self.sentinel.get_all_audit_logs(audit)
             dbgPrint.debug("Ingesting data")
             dataexplorer.ingest_audit_logs(data=audit_logs)
             del audit_logs[:]
@@ -658,16 +681,16 @@
                 dbgPrint.enable("core.msgraphapi")
                 dbgPrint.enable("helper.login")
             else:
                 dbgPrint.error("Unknown value")
                 sys.exit()
         if args.get("clear"):
             pass
-        if args.get("resetmfa"):
-            self.mfa.reset_session(self.email)
+#        if args.get("resetmfa"):
+#            self.mfa.reset_session(self.email)
         if args.get("user"):
             self.__init__(args)
             user_info = self.msgraph.check_mfa_status(args.get("user"))
 #            if user_info:
 #                printTable(user_info)
 #            user_info = self.msgraph.search_user(args.get("user"))
         elif args.get("incidentId"):
```

