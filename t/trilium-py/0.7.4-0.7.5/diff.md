# Comparing `tmp/trilium_py-0.7.4-py3-none-any.whl.zip` & `tmp/trilium_py-0.7.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27205 bytes, number of entries: 12
+Zip file size: 27426 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
--rw-r--r--  2.0 unx    27921 b- defN 23-Apr-04 07:07 trilium_py/client.py
+-rw-r--r--  2.0 unx    30967 b- defN 23-May-06 05:44 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    10488 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-Apr-13 01:18 trilium_py-0.7.4.dist-info/RECORD
-12 files, 84836 bytes uncompressed, 25535 bytes compressed:  69.9%
+-rwxrwx---  2.0 unx    35184 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    10488 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/RECORD
+12 files, 87882 bytes uncompressed, 25756 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.7.4.dist-info/LICENSE.txt
+Filename: trilium_py-0.7.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.7.4.dist-info/METADATA
+Filename: trilium_py-0.7.5.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.7.4.dist-info/WHEEL
+Filename: trilium_py-0.7.5.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.7.4.dist-info/top_level.txt
+Filename: trilium_py-0.7.5.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.7.4.dist-info/RECORD
+Filename: trilium_py-0.7.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -128,14 +128,91 @@
             "isExpanded": isExpanded,
             "noteId": noteId,
             "branchId": branchId
         }
         res = requests.post(url, json=clean_param(params), headers=self.get_header())
 
         return res.json()
+    
+    def create_file_note(self, parentNoteId: str, title: str, file_data: str, content_file: str,
+                         type: str = 'file', mime: str = None,
+                         content=None, notePosition: int = None, prefix: str = None,
+                         isExpanded: str = None, noteId: str = None,
+                         branchId: str = None):
+        '''
+        Create a note
+        set file name attribute
+        Update its content with image binary content
+        :param parentNoteId:
+        :param title:
+        :param file_data: file object from buffer.
+        :param content_file: file path in file system.
+        :param type:
+        :param mime:
+        :param content:
+        :param notePosition:
+        :param prefix:
+        :param isExpanded:
+        :param noteId:
+        :param branchId:
+        :return:
+        '''
+
+        url = f'{self.server_url}/etapi/create-note'
+
+        if not mime:
+            # if mime not specified, get mime info by python-magic package
+            if file_data:
+                mime = magic.from_buffer(file_data, mime=True)
+            elif content_file:
+                mime = magic.from_file(file_data, mime=True)
+
+        if not mime:
+            # just in case python-magic not working, give a default mime
+            mime = "image/png"
+
+        params = {
+            "parentNoteId": parentNoteId,
+            "title": title,
+            "type": type,
+            "mime": mime,
+            "content": content,
+            "notePosition": notePosition,
+            "prefix": prefix,
+            "isExpanded": isExpanded,
+            "noteId": noteId,
+            "branchId": branchId
+        }
+
+        res_file = requests.post(url, json=clean_param(params),
+                                 headers={'content-type': 'application/json', 'Authorization': self.token, })
+        res_file_json = res_file.json()
+        new_noteId = res_file_json['note']['noteId']
+
+        # set file name
+        content_file_name = os.path.basename(content_file)
+        self.create_attribute(attributeId=None, noteId=new_noteId, type='label', name='originalFileName',
+                              value=content_file_name, isInheritable=False)
+
+        # upload file, set note content
+        url = f'{self.server_url}/etapi/notes/{new_noteId}/content'
+        # content-type here will affect the result
+        # not working, encoding issue? automated force encoding to utf-8 and lost data
+        if not file_data:
+            file_data = open(content_file, 'rb').read()
+        res = requests.put(url, data=file_data,
+                           # headers={'content-type': 'text/plain', 'Authorization': self.token, })
+                           headers={
+                               'content-type': 'application/octet-stream',
+                               'Content-Transfer-Encoding': 'binary',
+                               'Authorization': self.token,
+                           })
+        if res.status_code == 204:
+            return res_file_json
+        return
 
     def create_image_note(self, parentNoteId: str, title: str, image_file: str, type: str = 'image', mime: str = None,
                           content=None,
                           notePosition: int = None, prefix: str = None,
                           isExpanded: str = None, noteId: str = None,
                           branchId: str = None):
```

## Comparing `trilium_py-0.7.4.dist-info/LICENSE.txt` & `trilium_py-0.7.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.7.4.dist-info/METADATA` & `trilium_py-0.7.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.7.4 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.7.5 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
```

## Comparing `trilium_py-0.7.4.dist-info/RECORD` & `trilium_py-0.7.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=kpSEbnEiNgxLIs9KxUf8s-OXJmt-atzeNGLgW_oTiDE,27921
+trilium_py/client.py,sha256=bY7OgceY6RAgdNv4VNXYoKh6yOnzmyNLvpYoNj0CEi4,30967
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/markdown_math.py,sha256=ORQwEXAPtcf2-NaYKx4Pr5q5B8CtupVRYt04JD-c3EY,8656
 trilium_py/utils/param_util.py,sha256=BOiblP1F-jMgggx8L_QxCH3s8-FIdG1kAM-4ykSbZ5E,675
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=U1Qn5UFzQO-Bi9DGjq2OEiVzCi6x5KXsyRKF-AOJV64,470
-trilium_py-0.7.4.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.7.4.dist-info/METADATA,sha256=6pQLG1NtC2G0YGl9wLDKhUGnP1jErTz8wi4adzXq6BE,10488
-trilium_py-0.7.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-trilium_py-0.7.4.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.7.4.dist-info/RECORD,,
+trilium_py-0.7.5.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.7.5.dist-info/METADATA,sha256=RmEkxI8yHd-Hv5zstISOfL_Ehug_oq_58nV8mxfu2xw,10488
+trilium_py-0.7.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+trilium_py-0.7.5.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.7.5.dist-info/RECORD,,
```

