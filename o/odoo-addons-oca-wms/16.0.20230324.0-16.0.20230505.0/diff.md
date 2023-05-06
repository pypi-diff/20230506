# Comparing `tmp/odoo_addons_oca_wms-16.0.20230324.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_wms-16.0.20230505.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1371 bytes, number of entries: 4
--rw-r--r--  2.0 unx      673 b- defN 23-Mar-25 08:52 odoo_addons_oca_wms-16.0.20230324.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-25 08:52 odoo_addons_oca_wms-16.0.20230324.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Mar-25 08:52 odoo_addons_oca_wms-16.0.20230324.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      384 b- defN 23-Mar-25 08:52 odoo_addons_oca_wms-16.0.20230324.0.dist-info/RECORD
-4 files, 1150 bytes uncompressed, 613 bytes compressed:  46.7%
+Zip file size: 1401 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      854 b- defN 23-May-06 08:00 odoo_addons_oca_wms-16.0.20230505.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 08:00 odoo_addons_oca_wms-16.0.20230505.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-06 08:00 odoo_addons_oca_wms-16.0.20230505.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      384 b- defN 23-May-06 08:00 odoo_addons_oca_wms-16.0.20230505.0.dist-info/RECORD
+4 files, 1331 bytes uncompressed, 643 bytes compressed:  51.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_wms-16.0.20230324.0.dist-info/METADATA
+Filename: odoo_addons_oca_wms-16.0.20230505.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20230324.0.dist-info/WHEEL
+Filename: odoo_addons_oca_wms-16.0.20230505.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20230324.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_wms-16.0.20230505.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_wms-16.0.20230324.0.dist-info/RECORD
+Filename: odoo_addons_oca_wms-16.0.20230505.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_wms-16.0.20230324.0.dist-info/METADATA` & `odoo_addons_oca_wms-16.0.20230505.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-wms
-Version: 16.0.20230324.0
+Version: 16.0.20230505.0
 Summary: Meta package for oca-wms Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-stock-available-to-promise-release (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-dynamic-routing (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-completion-info (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-picking-type-shipping-policy (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-stock-release-channel (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-stock-release-channel-auto-release (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-stock-release-channel-batch-mode-commercial-partner (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

