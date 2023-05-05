# Comparing `tmp/django_view_manager-1.0.0-py3-none-any.whl.zip` & `tmp/django_view_manager-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 11282 bytes, number of entries: 11
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 23:39 django_view_manager/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 23:39 django_view_manager/utils/__init__.py
--rw-r--r--  2.0 unx      132 b- defN 23-Feb-17 23:39 django_view_manager/utils/apps.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 23:39 django_view_manager/utils/management/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Feb-17 23:39 django_view_manager/utils/management/commands/__init__.py
--rw-r--r--  2.0 unx    20602 b- defN 23-Feb-17 23:39 django_view_manager/utils/management/commands/makeviewmigration.py
--rw-r--r--  2.0 unx     1504 b- defN 23-Feb-17 23:40 django_view_manager-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13797 b- defN 23-Feb-17 23:40 django_view_manager-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-17 23:40 django_view_manager-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Feb-17 23:40 django_view_manager-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1049 b- defN 23-Feb-17 23:40 django_view_manager-1.0.0.dist-info/RECORD
-11 files, 37196 bytes uncompressed, 9442 bytes compressed:  74.6%
+Zip file size: 11287 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/__init__.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-05 22:06 django_view_manager/utils/apps.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/management/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 22:06 django_view_manager/utils/management/commands/__init__.py
+-rw-r--r--  2.0 unx    20602 b- defN 23-May-05 22:06 django_view_manager/utils/management/commands/makeviewmigration.py
+-rw-r--r--  2.0 unx     1504 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13800 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1049 b- defN 23-May-05 22:06 django_view_manager-1.0.1.dist-info/RECORD
+11 files, 37199 bytes uncompressed, 9447 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: django_view_manager/utils/management/commands/__init__.py
 Comment: 
 
 Filename: django_view_manager/utils/management/commands/makeviewmigration.py
 Comment: 
 
-Filename: django_view_manager-1.0.0.dist-info/LICENSE
+Filename: django_view_manager-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_view_manager-1.0.0.dist-info/METADATA
+Filename: django_view_manager-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: django_view_manager-1.0.0.dist-info/WHEEL
+Filename: django_view_manager-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_view_manager-1.0.0.dist-info/top_level.txt
+Filename: django_view_manager-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_view_manager-1.0.0.dist-info/RECORD
+Filename: django_view_manager-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `django_view_manager-1.0.0.dist-info/LICENSE` & `django_view_manager-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_view_manager-1.0.0.dist-info/METADATA` & `django_view_manager-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-view-manager
-Version: 1.0.0
+Version: 1.0.1
 Summary: A management command for django that provides diffs of sql views.
 Author-email: Arrai Innovations <support@arrai.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Arrai Innovations
         
         Redistribution and use in source and binary forms, with or without
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Environment :: Console
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django (>=3.2.0)
 
 # django-view-manager
 
 A management command for django, designed to provide a way in pull requests, to see a diff of the sql (`CREATE VIEW ...`) for unmanaged models.
```

## Comparing `django_view_manager-1.0.0.dist-info/RECORD` & `django_view_manager-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 django_view_manager/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/apps.py,sha256=fZoo89eHKqypCLKzeFxUNkGrHTBs4sWGm3ZcLDDGTi8,132
 django_view_manager/utils/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_view_manager/utils/management/commands/makeviewmigration.py,sha256=KCwaSr5YkxOgWmuobiTgqjdRS5mTJsricHGUlSRhKK8,20602
-django_view_manager-1.0.0.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
-django_view_manager-1.0.0.dist-info/METADATA,sha256=59_l6eioDRrfqRIT_41sh6PTxHtdRpWbqF9BFHSv0-k,13797
-django_view_manager-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-django_view_manager-1.0.0.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
-django_view_manager-1.0.0.dist-info/RECORD,,
+django_view_manager-1.0.1.dist-info/LICENSE,sha256=C9Y-Cr2GS0AyKcVDN7Gwj4DjjYTUdCUrFDeASp8C8fA,1504
+django_view_manager-1.0.1.dist-info/METADATA,sha256=KnedL-RzfPDhnOkhlKxm4tk0e0KH9CvLd0eI9IPgYP0,13800
+django_view_manager-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_view_manager-1.0.1.dist-info/top_level.txt,sha256=WaJvRmbbOJ7HI_7RuTxUSjULO_00vrBXScnfiFteTT8,20
+django_view_manager-1.0.1.dist-info/RECORD,,
```

