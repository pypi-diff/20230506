# Comparing `tmp/django_sqlite_backup-0.0.2-py3-none-any.whl.zip` & `tmp/django_sqlite_backup-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7315 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 23-May-04 10:38 django_sqlite_backup/__init__.py
--rw-r--r--  2.0 unx      450 b- defN 23-May-04 10:38 django_sqlite_backup/apps.py
--rw-r--r--  2.0 unx     1644 b- defN 23-May-04 10:38 django_sqlite_backup/aws.py
--rw-r--r--  2.0 unx      779 b- defN 23-May-04 10:38 django_sqlite_backup/backup.py
--rw-r--r--  2.0 unx      496 b- defN 23-May-04 10:38 django_sqlite_backup/decorators.py
--rw-r--r--  2.0 unx      740 b- defN 23-May-04 10:38 django_sqlite_backup/restore.py
--rw-r--r--  2.0 unx      150 b- defN 23-May-04 10:38 django_sqlite_backup/urls.py
--rw-r--r--  2.0 unx      403 b- defN 23-May-04 10:38 django_sqlite_backup/views.py
--rw-r--r--  2.0 unx     1070 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     4514 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1137 b- defN 23-May-04 10:38 django_sqlite_backup-0.0.2.dist-info/RECORD
-13 files, 11496 bytes uncompressed, 5379 bytes compressed:  53.2%
+Zip file size: 7406 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 23-May-06 10:15 django_sqlite_backup/__init__.py
+-rw-r--r--  2.0 unx      450 b- defN 23-May-06 10:15 django_sqlite_backup/apps.py
+-rw-r--r--  2.0 unx     1537 b- defN 23-May-06 10:15 django_sqlite_backup/aws.py
+-rw-r--r--  2.0 unx      779 b- defN 23-May-06 10:15 django_sqlite_backup/backup.py
+-rw-r--r--  2.0 unx      496 b- defN 23-May-06 10:15 django_sqlite_backup/decorators.py
+-rw-r--r--  2.0 unx      740 b- defN 23-May-06 10:15 django_sqlite_backup/restore.py
+-rw-r--r--  2.0 unx      150 b- defN 23-May-06 10:15 django_sqlite_backup/urls.py
+-rw-r--r--  2.0 unx      403 b- defN 23-May-06 10:15 django_sqlite_backup/views.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4621 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1137 b- defN 23-May-06 10:15 django_sqlite_backup-0.0.3.dist-info/RECORD
+13 files, 11496 bytes uncompressed, 5470 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: django_sqlite_backup/urls.py
 Comment: 
 
 Filename: django_sqlite_backup/views.py
 Comment: 
 
-Filename: django_sqlite_backup-0.0.2.dist-info/LICENSE
+Filename: django_sqlite_backup-0.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: django_sqlite_backup-0.0.2.dist-info/METADATA
+Filename: django_sqlite_backup-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: django_sqlite_backup-0.0.2.dist-info/WHEEL
+Filename: django_sqlite_backup-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: django_sqlite_backup-0.0.2.dist-info/top_level.txt
+Filename: django_sqlite_backup-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: django_sqlite_backup-0.0.2.dist-info/RECORD
+Filename: django_sqlite_backup-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_sqlite_backup/aws.py

```diff
@@ -1,58 +1,59 @@
 from datetime import datetime
+from functools import lru_cache
 from typing import Any
 
 import boto3
 from django.conf import ImproperlyConfigured
 from django.conf import settings
 
 
-class AwsSqliteBackup:
-    def __init__(self) -> None:
-        self.s3 = boto3.client("s3")
+@lru_cache
+def s3():
+    return boto3.client(
+        "s3",
+        endpoint_url=settings.SQLITE_BACKUP.get("S3_ENDPOINT"),
+    )
+
+
+def get_database_name() -> str:
+    return str(settings.DATABASES["default"]["NAME"])
 
-    def get_database_name(self) -> str:
-        return str(settings.DATABASES["default"]["NAME"])
 
+class AwsSqliteBackup:
     def _read_db(self) -> Any:
-        with open(self.get_database_name()) as f:
+        with open(get_database_name()) as f:
             return f.read()
 
     def backup_db(self) -> None:
         bucket_name = settings.SQLITE_BACKUP.get("BUCKET_NAME")
-        db_name = self.get_database_name().split("/")[-1]
+        db_name = get_database_name().split("/")[-1]
 
         if bucket_name is None:
             raise ImproperlyConfigured("`BUCKET_NAME` is not defined")
 
         full_bucket_name = f"sqlite_backup/{datetime.now().strftime('%Y-%m-%d')}/{db_name}"
 
-        self.s3.put_object(
+        s3().put_object(
             Bucket=bucket_name,
             Key=full_bucket_name,
             Body=self._read_db(),
         )
 
 
 class AwsRestoreDb:
-    def __init__(self) -> None:
-        self.s3 = boto3.client("s3")
-
-    def get_database_name(self) -> str:
-        return str(settings.DATABASES["default"]["NAME"])
-
     def restore_db(self, date_str: str) -> None:
         bucket_name = settings.SQLITE_BACKUP.get("BUCKET_NAME")
 
         if bucket_name is None:
             raise ImproperlyConfigured("`BUCKET_NAME` is not defined")
 
-        db_name = self.get_database_name()
+        db_name = get_database_name()
         key = f"sqlite_backup/{date_str}/{db_name}"
 
-        response = self.s3.get_object(
+        response = s3().get_object(
             Bucket=bucket_name,
             Key=key,
         )
 
         with open(db_name, "w") as f:
             f.write(response.get("Body").read().decode())
```

## Comparing `django_sqlite_backup-0.0.2.dist-info/LICENSE` & `django_sqlite_backup-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_sqlite_backup-0.0.2.dist-info/METADATA` & `django_sqlite_backup-0.0.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sqlite-backup
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app to easily backup your sqlite database through an endpoint.
 Author-email: Ferran Jovell <ferran.jovell+gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ferran Jovell
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -94,20 +94,22 @@
 You must define your settings in your `settings.py`:
 
 ```
 SQLITE_BACKUP = {
     "BACKUP_CLASS": ...,
     "RESTORE_CLASS": ...,
     "BUCKET_NAME": ...,
+    "S3_ENDPOINT": ...,
 }
 ```
 
 - `BACKUP_CLASS` must point to class which follows the [`SqliteBackup`](./django_sqlite_backup/backup.py) protocol.
 - `RESTORE_CLASS` must point to class which follows the [`SqliteRestore`](./django_sqlite_backup/restore.py) protocol.
 - `BUCKET_NAME` is the name of the bucket in S3 which can be written to.
+- `S3_ENDPOINT` S3 endpoint override. Leave this blank if you use AWS S3 directly.
 
 ### Management commands
 
 This app provides two commands for carrying out operations on the backups: `backup` and `restore`.
 
 ```console
 ./manage.py backup
```

## Comparing `django_sqlite_backup-0.0.2.dist-info/RECORD` & `django_sqlite_backup-0.0.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 django_sqlite_backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_sqlite_backup/apps.py,sha256=hr_VWttIN8RVXzXXG2Vo-SjuNgCFDE5POwycNww-ixo,450
-django_sqlite_backup/aws.py,sha256=64FLQTLZV9Am8TaITgj0xkCnAbifpbEyEyZVls4alX0,1644
+django_sqlite_backup/aws.py,sha256=NvjSpndNvCTPAILKuH1EyZ5rZgPmsN5Oi8btC7gqSWM,1537
 django_sqlite_backup/backup.py,sha256=8-4QRYIWJOMYM0Deuub6P5nWiBKjW4w2Gvh-UjttcNg,779
 django_sqlite_backup/decorators.py,sha256=bXvyTazsw0xkkOJ3zNtt8tOv1GmXsmB1lbUMnzW9Mbg,496
 django_sqlite_backup/restore.py,sha256=BJTGqd0zqeTWRbk1c98OqNRweYNmOoDdUC1dsuCkKWc,740
 django_sqlite_backup/urls.py,sha256=ve4fRC0VSPi235hDc9_n973ii_jrIpeE4tPrJTBSNCA,150
 django_sqlite_backup/views.py,sha256=9evoRFbHv4dFHhMD0ntXQH4VyDfWFKNGTFUdTfoIK1Y,403
-django_sqlite_backup-0.0.2.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
-django_sqlite_backup-0.0.2.dist-info/METADATA,sha256=LUXaqUFe76p8jc_-pbHeqrRl83ACKRElWakYqvv-t5g,4514
-django_sqlite_backup-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-django_sqlite_backup-0.0.2.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
-django_sqlite_backup-0.0.2.dist-info/RECORD,,
+django_sqlite_backup-0.0.3.dist-info/LICENSE,sha256=bwE4PTk0_zgY2rrrldsrBocfua-bkc_IUxH1pr1rCFA,1070
+django_sqlite_backup-0.0.3.dist-info/METADATA,sha256=hzdU3A3kYGC40s2jbhF2aSWHM8b1A6IwtJsuLQbKsNs,4621
+django_sqlite_backup-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+django_sqlite_backup-0.0.3.dist-info/top_level.txt,sha256=hpNLepZbcHqSqEC92LAtpsd7uaey2g64SD0C0NWEDqM,21
+django_sqlite_backup-0.0.3.dist-info/RECORD,,
```

