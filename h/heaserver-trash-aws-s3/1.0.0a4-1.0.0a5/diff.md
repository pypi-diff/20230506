# Comparing `tmp/heaserver-trash-aws-s3-1.0.0a4.tar.gz` & `tmp/heaserver-trash-aws-s3-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a4.tar", last modified: Fri May  5 17:26:54 2023, max compression
+gzip compressed data, was "heaserver-trash-aws-s3-1.0.0a5.tar", last modified: Fri May  5 23:28:48 2023, max compression
```

## Comparing `heaserver-trash-aws-s3-1.0.0a4.tar` & `heaserver-trash-aws-s3-1.0.0a5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.631208 heaserver-trash-aws-s3-1.0.0a4/
--rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/LICENSE
--rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/MANIFEST.in
--rw-rw-rw-   0        0        0     4352 2023-05-05 17:26:54.630208 heaserver-trash-aws-s3-1.0.0a4/PKG-INFO
--rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 17:26:54.631208 heaserver-trash-aws-s3-1.0.0a4/setup.cfg
--rw-rw-rw-   0        0        0     1869 2023-05-05 17:26:10.000000 heaserver-trash-aws-s3-1.0.0a4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.574209 heaserver-trash-aws-s3-1.0.0a4/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.573208 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.593213 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    48628 2023-05-05 17:24:22.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.594209 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.626207 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4352 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 17:26:54.000000 heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.575209 heaserver-trash-aws-s3-1.0.0a4/tests/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.576209 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-05-05 17:26:54.629208 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.351024 heaserver-trash-aws-s3-1.0.0a5/
+-rw-rw-rw-   0        0        0    11625 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4352 2023-05-05 23:28:48.350023 heaserver-trash-aws-s3-1.0.0a5/PKG-INFO
+-rw-rw-rw-   0        0        0     3111 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 23:28:48.351024 heaserver-trash-aws-s3-1.0.0a5/setup.cfg
+-rw-rw-rw-   0        0        0     1869 2023-05-05 23:28:04.000000 heaserver-trash-aws-s3-1.0.0a5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    48660 2023-05-05 23:05:37.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7631 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.345024 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4352 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 23:28:48.000000 heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/tests/
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.307387 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-05-05 23:28:48.349023 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-03-08 22:56:40.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    69298 2023-04-26 23:41:02.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6276 2023-04-13 17:41:47.000000 heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver-trash-aws-s3-1.0.0a4/LICENSE` & `heaserver-trash-aws-s3-1.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a4/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a4/README.md` & `heaserver-trash-aws-s3-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a4/setup.py` & `heaserver-trash-aws-s3-1.0.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.0.0a4',
+    version='1.0.0a5',
     description="deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver>=1.0.0a116, <1.0.0a117'
+          'heaserver>=1.0.0a117, <1.0.0a118'
       ],
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
           'License :: OSI Approved :: Apache Software License',
```

### Comparing `heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/service.py` & `heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
                 if 'Size' not in resp_ and resp_['VersionId'] == version_:
                     delete_marker = resp_
                     break
     if delete_marker:
         encoded_key = encode_key(key)
         last_modified = delete_marker['LastModified']
 
-        version = next((v for v in sorted(response_['Versions'], key=lambda x: x['LastModified'],
+        version = next((v for v in sorted(response_.get('Versions', []), key=lambda x: x['LastModified'],
                         reverse=True) if v['Key'] == key and v['LastModified'] < delete_marker['LastModified']), None)
         logging.getLogger(__name__).debug('Generating trash item from delete marker %s and version %s', delete_marker, version)
         size = version['Size'] if version is not None and not is_folder(key_) else 0
         storage_class = version['StorageClass'] if version is not None else S3StorageClass.STANDARD.name
 
         item = AWSS3FolderFileTrashItem()
         item.bucket_id = bucket_id
@@ -940,22 +940,22 @@
         if not await _get_deleted_item(request):
             return response.status_not_found(f'Object {display_name(key_)} is not in the trash')
         s3_client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
         async for response_ in _get_version_objects(s3_client, bucket_name, key_, loop):
             keyfunc = lambda x: x['Key']
 
             # Preflight
-            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_['Versions'])), key=keyfunc), key=keyfunc):
+            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_.get('Versions', []))), key=keyfunc), key=keyfunc):
                 resps = sorted(versions, key=lambda x: x['LastModified'], reverse=True)
                 if resps and 'Size' in resps[0]:
                     if not is_folder(resps[0]['Key']):
                         return response.status_bad_request(f'Object {display_name(key)} has been overwritten')
 
             # Actual
-            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_['Versions'])), key=keyfunc), key=keyfunc):
+            for key, versions in itertools.groupby(sorted((resp for resp in itertools.chain(response_['DeleteMarkers'], response_.get('Versions', []))), key=keyfunc), key=keyfunc):
                 resps = sorted(versions, key=lambda x: x['LastModified'], reverse=True)
                 for resp_ in resps:
                     if 'Size' not in resp_:  # Delete the delete markers until we reach actual version objects.
                         s3_client.delete_object(Bucket=bucket_name, Key=resp_['Key'], VersionId=resp_['VersionId'])
                     else:
                         break
 
@@ -1097,15 +1097,15 @@
 
     try:
         s3_client = await request.app[HEA_DB].get_client(request, 's3', volume_id)
         async for response_ in _get_version_objects(s3_client, bucket_name, key, loop):
             delete_markers_to_delete = []
             versions_to_delete = []
             delete_marker = False
-            for resp_ in sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_['Versions']) if resp['Key'] == key), key=lambda x: x['LastModified'], reverse=True):
+            for resp_ in sorted((resp for resp in itertools.chain(response_.get('DeleteMarkers', []), response_.get('Versions', [])) if resp['Key'] == key), key=lambda x: x['LastModified'], reverse=True):
                 if not delete_marker and resp_['VersionId'] == version:
                     delete_marker = True
                     delete_markers_to_delete.append(resp_)
                     continue
                 if delete_marker and 'Size' not in resp_ and versions_to_delete:
                     delete_marker = False
                     break
```

### Comparing `heaserver-trash-aws-s3-1.0.0a4/src/heaserver/trashawss3/wstl/all.json` & `heaserver-trash-aws-s3-1.0.0a5/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `heaserver-trash-aws-s3-1.0.0a4/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver-trash-aws-s3-1.0.0a5/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/test_all.py` & `heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-trash-aws-s3-1.0.0a4/tests/heaserver/trashawss3test/testcase.py` & `heaserver-trash-aws-s3-1.0.0a5/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

