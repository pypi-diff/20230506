# Comparing `tmp/datalift-0.1.1-py3-none-any.whl.zip` & `tmp/datalift-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 5876 bytes, number of entries: 14
+Zip file size: 5869 bytes, number of entries: 14
 -rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:14 datalift/__init__.py
 -rw-r--r--  2.0 unx      803 b- defN 23-May-05 22:19 datalift/containers.py
--rw-r--r--  2.0 unx     2531 b- defN 23-May-05 22:21 datalift/datalift.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-May-05 22:41 datalift/datalift.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-05 20:32 datalift/storages/__init__.py
 -rw-r--r--  2.0 unx      473 b- defN 23-May-05 20:58 datalift/storages/base.py
 -rw-r--r--  2.0 unx       75 b- defN 23-May-05 22:27 datalift/storages/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-05 20:32 datalift/storages/infra/__init__.py
 -rw-r--r--  2.0 unx      570 b- defN 23-May-05 21:47 datalift/storages/infra/dummy.py
 -rw-r--r--  2.0 unx     1159 b- defN 23-May-05 21:47 datalift/storages/infra/ftp.py
--rw-r--r--  2.0 unx     2111 b- defN 23-May-05 22:33 datalift-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:33 datalift-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-May-05 22:33 datalift-0.1.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-05 22:33 datalift-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1135 b- defN 23-May-05 22:33 datalift-0.1.1.dist-info/RECORD
-14 files, 9011 bytes uncompressed, 3966 bytes compressed:  56.0%
+-rw-r--r--  2.0 unx     2077 b- defN 23-May-05 22:42 datalift-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:42 datalift-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-May-05 22:42 datalift-0.1.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-05 22:42 datalift-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1135 b- defN 23-May-05 22:42 datalift-0.1.2.dist-info/RECORD
+14 files, 8996 bytes uncompressed, 3959 bytes compressed:  56.0%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: datalift/storages/infra/dummy.py
 Comment: 
 
 Filename: datalift/storages/infra/ftp.py
 Comment: 
 
-Filename: datalift-0.1.1.dist-info/METADATA
+Filename: datalift-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: datalift-0.1.1.dist-info/WHEEL
+Filename: datalift-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: datalift-0.1.1.dist-info/entry_points.txt
+Filename: datalift-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: datalift-0.1.1.dist-info/top_level.txt
+Filename: datalift-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: datalift-0.1.1.dist-info/RECORD
+Filename: datalift-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datalift/datalift.py

```diff
@@ -71,15 +71,15 @@
         with open(args.filename, 'wb') as f:
             f.write(data)
     else:
         print(data, end='')
 
 
 def get_parser():
-    parser = argparse.ArgumentParser(description='Upload data and send notifications.')
+    parser = argparse.ArgumentParser(description='Upload and download files or stdout to a file storage.')
     parser.add_argument('filename', nargs='?', type=str, help='name of file')
     parser.add_argument('--download', action='store_true', help='download file from storage')
     parser.add_argument('--stdout', action='store_true', help='print content to stdout')
     parser.add_argument('--path', type=str, help='file uploaded file. uuid generated if not provided')
     return parser
```

## Comparing `datalift-0.1.1.dist-info/METADATA` & `datalift-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: datalift
-Version: 0.1.1
+Version: 0.1.2
 Summary: Datalift it is a command-line tool designed to tools outputs to a storage service. Users can input data either by passing a filename or through stdout from another tool.
 Home-page: UNKNOWN
 Author: Samuel López Saura
 Author-email: samuellopezsaura@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: dependency-injector (<5.0,>=4.41)
 
 # Datalift
 
-> The tool that help you store tools outputs, tag them and send notifications once uploaded.
+> The tool that help you store and retrieve tools outputs.
 
 `pip install datalift`
 
 Datalift it is a command-line tool designed to tools outputs to a storage service.
 Users can input data either by passing a filename or through stdout from another tool.
 
 The application is designed to streamline the process of uploading and
```

## Comparing `datalift-0.1.1.dist-info/RECORD` & `datalift-0.1.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 datalift/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datalift/containers.py,sha256=hlaQp29hc2mOpqMMR19cX_jOML7dJuMnnu-4fyfxedw,803
-datalift/datalift.py,sha256=x9MkfXIitGnSgMczM7WiOtVey0Atg78L9ED3a4cdSAY,2531
+datalift/datalift.py,sha256=L_R40GdPhlxGewi4Ivhc9c62YgNaN6oWBKyJef_iRN8,2550
 datalift/storages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datalift/storages/base.py,sha256=e_LrBhO_lH_cJkDXqpQXsDuhK19mlkzy7sr0Zu0SkA8,473
 datalift/storages/utils.py,sha256=0jwyTZARinF0mvNFqF4CoL--4qeXwuGZ0acf-zwCDCc,75
 datalift/storages/infra/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datalift/storages/infra/dummy.py,sha256=wprgCcpXNbZBBLhdjLRBBYUDJbxapTTfcC-xxk1_l2Y,570
 datalift/storages/infra/ftp.py,sha256=lPqktytZ7HbTZUcVTKZubZ7D38F_XAzA5sdVDcA1tX8,1159
-datalift-0.1.1.dist-info/METADATA,sha256=T8bdu7XsHaB0XL_dlxyIBAnUrqjLvTLcdVyhNc2ll_o,2111
-datalift-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-datalift-0.1.1.dist-info/entry_points.txt,sha256=wMniGJmXC6bNVrxPq32O1mVNtwZ2W3qwUL-ufzcC3MM,53
-datalift-0.1.1.dist-info/top_level.txt,sha256=D8dU7JIIO7idNTplkZHkT4xmjusJwYcn6-CvAFoD-70,9
-datalift-0.1.1.dist-info/RECORD,,
+datalift-0.1.2.dist-info/METADATA,sha256=VJgVmBxOdXdO83sQKcFgp1sTficxs5bCTmExeqexAF4,2077
+datalift-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+datalift-0.1.2.dist-info/entry_points.txt,sha256=wMniGJmXC6bNVrxPq32O1mVNtwZ2W3qwUL-ufzcC3MM,53
+datalift-0.1.2.dist-info/top_level.txt,sha256=D8dU7JIIO7idNTplkZHkT4xmjusJwYcn6-CvAFoD-70,9
+datalift-0.1.2.dist-info/RECORD,,
```

