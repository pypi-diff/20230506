# Comparing `tmp/compose_chart_export-0.0.15rc4-py3-none-any.whl.zip` & `tmp/compose_chart_export-0.0.16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13232 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 10:09 compose_chart_export/__init__.py
--rw-r--r--  2.0 unx     2534 b- defN 23-May-05 10:09 compose_chart_export/chart_export.py
--rw-r--r--  2.0 unx    14200 b- defN 23-May-05 10:09 compose_chart_export/chart_file_templates.py
--rw-r--r--  2.0 unx     4967 b- defN 23-May-05 10:09 compose_chart_export/chart_mods.py
--rw-r--r--  2.0 unx     2211 b- defN 23-May-05 10:09 compose_chart_export/chart_read.py
--rw-r--r--  2.0 unx     9380 b- defN 23-May-05 10:09 compose_chart_export/compose_export.py
--rw-r--r--  2.0 unx     2359 b- defN 23-May-05 10:09 compose_chart_export/ports.py
--rw-r--r--  2.0 unx      191 b- defN 23-May-05 10:09 compose_chart_export/settings.py
--rw-r--r--  2.0 unx      586 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       21 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1214 b- defN 23-May-05 10:09 compose_chart_export-0.0.15rc4.dist-info/RECORD
-13 files, 37756 bytes uncompressed, 11146 bytes compressed:  70.5%
+Zip file size: 13196 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-06 09:53 compose_chart_export/__init__.py
+-rw-r--r--  2.0 unx     2534 b- defN 23-May-06 09:53 compose_chart_export/chart_export.py
+-rw-r--r--  2.0 unx    14200 b- defN 23-May-06 09:53 compose_chart_export/chart_file_templates.py
+-rw-r--r--  2.0 unx     4967 b- defN 23-May-06 09:53 compose_chart_export/chart_mods.py
+-rw-r--r--  2.0 unx     2211 b- defN 23-May-06 09:53 compose_chart_export/chart_read.py
+-rw-r--r--  2.0 unx     9380 b- defN 23-May-06 09:53 compose_chart_export/compose_export.py
+-rw-r--r--  2.0 unx     2359 b- defN 23-May-06 09:53 compose_chart_export/ports.py
+-rw-r--r--  2.0 unx      191 b- defN 23-May-06 09:53 compose_chart_export/settings.py
+-rw-r--r--  2.0 unx      583 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       21 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1199 b- defN 23-May-06 09:53 compose_chart_export-0.0.16.dist-info/RECORD
+13 files, 37738 bytes uncompressed, 11140 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: compose_chart_export/ports.py
 Comment: 
 
 Filename: compose_chart_export/settings.py
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc4.dist-info/METADATA
+Filename: compose_chart_export-0.0.16.dist-info/METADATA
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc4.dist-info/WHEEL
+Filename: compose_chart_export-0.0.16.dist-info/WHEEL
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt
+Filename: compose_chart_export-0.0.16.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc4.dist-info/top_level.txt
+Filename: compose_chart_export-0.0.16.dist-info/top_level.txt
 Comment: 
 
-Filename: compose_chart_export-0.0.15rc4.dist-info/RECORD
+Filename: compose_chart_export-0.0.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `compose_chart_export-0.0.15rc4.dist-info/METADATA` & `compose_chart_export-0.0.16.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: compose-chart-export
-Version: 0.0.15rc4
+Version: 0.0.16
 Summary: compose_agent_export for docker-compose -> helm chart
 Author: Espen
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
-Requires-Dist: docker-compose-parser (==0.0.15)
-Requires-Dist: model-lib (==0.0.15)
+Requires-Dist: docker-compose-parser (==0.0.16)
+Requires-Dist: model-lib (==0.0.16)
 Requires-Dist: pydantic (>=1.10.2)
 Requires-Dist: semver (==2.13.0)
-Requires-Dist: zero-3rdparty (==0.0.15)
+Requires-Dist: zero-3rdparty (==0.0.16)
 
 # Compose Chart Export
 - Uses `docker-compose.yaml` to generate a helm chart
 - Supports various customizations using labels
```

## Comparing `compose_chart_export-0.0.15rc4.dist-info/RECORD` & `compose_chart_export-0.0.16.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 compose_chart_export/chart_export.py,sha256=oDgolV_QNeF12D2xh2D9xhn45IQSbKDMmj2WRZ2UTaI,2534
 compose_chart_export/chart_file_templates.py,sha256=bG35ma5Un9_18GpPiB5MYdKtvbZOQ-4zzEn7oCv0rSs,14200
 compose_chart_export/chart_mods.py,sha256=Zn-NSYhv7jJfUtGs6V--fquIolVqFT3bwL8mSWrwgOI,4967
 compose_chart_export/chart_read.py,sha256=chwkPcucA6dLWStADbP2kpAGNbhYVMms9zmPjNIQrLs,2211
 compose_chart_export/compose_export.py,sha256=w0ionkwWLTGOz9Lf2MIZVTRrUAjj7_pzmhJOxU80ZZw,9380
 compose_chart_export/ports.py,sha256=06WBSFYTUEPUYh9x4U5BjjUeE-EPNCs1Pot6MO7zxD4,2359
 compose_chart_export/settings.py,sha256=-vo5OY1ttQUeGQwihuX2YTD-qHRgvBdMuRwP_BelWQY,191
-compose_chart_export-0.0.15rc4.dist-info/METADATA,sha256=2sFIxXvY3vSrO3mmYAoniFD49LzOIawzFpn3M7lTULk,586
-compose_chart_export-0.0.15rc4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-compose_chart_export-0.0.15rc4.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-compose_chart_export-0.0.15rc4.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
-compose_chart_export-0.0.15rc4.dist-info/RECORD,,
+compose_chart_export-0.0.16.dist-info/METADATA,sha256=R7x_HyXXnAuqa8WEXGr8vKbBkUtQg_dj6tM-Jhc-5c0,583
+compose_chart_export-0.0.16.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+compose_chart_export-0.0.16.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+compose_chart_export-0.0.16.dist-info/top_level.txt,sha256=leubfJ1d95x8SfDGSVFPIHT8AGgj9xYF0CMorIbq3uo,21
+compose_chart_export-0.0.16.dist-info/RECORD,,
```

