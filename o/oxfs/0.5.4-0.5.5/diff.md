# Comparing `tmp/oxfs-0.5.4.tar.gz` & `tmp/oxfs-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxfs-0.5.4.tar", last modified: Fri Oct 14 06:08:54 2022, max compression
+gzip compressed data, was "oxfs-0.5.5.tar", last modified: Sat May  6 04:06:35 2023, max compression
```

## Comparing `oxfs-0.5.4.tar` & `oxfs-0.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2022-10-14 06:08:54.271047 oxfs-0.5.4/
--rw-r--r--   0 bytedance   (501) staff       (20)     1068 2022-10-13 04:51:30.000000 oxfs-0.5.4/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)     1125 2022-10-14 06:08:54.270755 oxfs-0.5.4/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     9463 2022-10-13 04:51:30.000000 oxfs-0.5.4/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2022-10-14 06:08:54.266797 oxfs-0.5.4/oxfs/
--rwxr-xr-x   0 bytedance   (501) staff       (20)       14 2022-10-13 04:51:30.000000 oxfs-0.5.4/oxfs/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2022-10-14 06:08:54.270328 oxfs-0.5.4/oxfs/cache/
--rwxr-xr-x   0 bytedance   (501) staff       (20)       15 2022-10-13 04:51:30.000000 oxfs-0.5.4/oxfs/cache/__init__.py
--rwxr-xr-x   0 bytedance   (501) staff       (20)     1899 2022-10-14 03:56:22.000000 oxfs-0.5.4/oxfs/cache/fs.py
--rwxr-xr-x   0 bytedance   (501) staff       (20)      751 2022-10-14 02:59:27.000000 oxfs-0.5.4/oxfs/cache/meta.py
--rwxr-xr-x   0 bytedance   (501) staff       (20)      593 2022-10-14 03:45:04.000000 oxfs-0.5.4/oxfs/lock.py
--rwxr-xr-x   0 bytedance   (501) staff       (20)    16029 2022-10-14 03:46:55.000000 oxfs-0.5.4/oxfs/oxfs.py
--rwxr-xr-x   0 bytedance   (501) staff       (20)     3382 2022-10-14 03:10:01.000000 oxfs-0.5.4/oxfs/updater.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2022-10-14 06:08:54.269281 oxfs-0.5.4/oxfs.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)     1125 2022-10-14 06:08:53.000000 oxfs-0.5.4/oxfs.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      337 2022-10-14 06:08:54.000000 oxfs-0.5.4/oxfs.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2022-10-14 06:08:53.000000 oxfs-0.5.4/oxfs.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       40 2022-10-14 06:08:53.000000 oxfs-0.5.4/oxfs.egg-info/entry_points.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       44 2022-10-14 06:08:54.000000 oxfs-0.5.4/oxfs.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        5 2022-10-14 06:08:54.000000 oxfs-0.5.4/oxfs.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2022-10-13 04:52:50.000000 oxfs-0.5.4/oxfs.egg-info/zip-safe
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2022-10-14 06:08:54.271143 oxfs-0.5.4/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)     1562 2022-10-14 06:08:25.000000 oxfs-0.5.4/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-05-06 04:06:35.991220 oxfs-0.5.5/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1068 2022-10-13 04:51:30.000000 oxfs-0.5.5/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)     1125 2023-05-06 04:06:35.990971 oxfs-0.5.5/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     9463 2022-10-13 04:51:30.000000 oxfs-0.5.5/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-05-06 04:06:35.986958 oxfs-0.5.5/oxfs/
+-rwxr-xr-x   0 bytedance   (501) staff       (20)       14 2022-10-13 04:51:30.000000 oxfs-0.5.5/oxfs/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-05-06 04:06:35.990516 oxfs-0.5.5/oxfs/cache/
+-rwxr-xr-x   0 bytedance   (501) staff       (20)       15 2022-10-13 04:51:30.000000 oxfs-0.5.5/oxfs/cache/__init__.py
+-rwxr-xr-x   0 bytedance   (501) staff       (20)     1899 2022-10-14 03:56:22.000000 oxfs-0.5.5/oxfs/cache/fs.py
+-rwxr-xr-x   0 bytedance   (501) staff       (20)      751 2022-10-14 02:59:27.000000 oxfs-0.5.5/oxfs/cache/meta.py
+-rwxr-xr-x   0 bytedance   (501) staff       (20)      593 2022-10-14 03:45:04.000000 oxfs-0.5.5/oxfs/lock.py
+-rwxr-xr-x   0 bytedance   (501) staff       (20)    16018 2023-05-06 03:58:50.000000 oxfs-0.5.5/oxfs/oxfs.py
+-rwxr-xr-x   0 bytedance   (501) staff       (20)     3382 2022-10-14 03:10:01.000000 oxfs-0.5.5/oxfs/updater.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-05-06 04:06:35.989218 oxfs-0.5.5/oxfs.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1125 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      337 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       40 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/entry_points.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       44 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        5 2023-05-06 04:06:35.000000 oxfs-0.5.5/oxfs.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2022-10-13 04:52:50.000000 oxfs-0.5.5/oxfs.egg-info/zip-safe
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-05-06 04:06:35.991320 oxfs-0.5.5/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)     1562 2023-05-06 04:06:10.000000 oxfs-0.5.5/setup.py
```

### Comparing `oxfs-0.5.4/LICENSE` & `oxfs-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/PKG-INFO` & `oxfs-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxfs
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Fast SFTP File System
 Home-page: https://github.com/oxfs/oxfs
 Author: RainMark
 Author-email: rain.by.zhou@gmail.com
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `oxfs-0.5.4/README.md` & `oxfs-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/oxfs/cache/fs.py` & `oxfs-0.5.5/oxfs/cache/fs.py`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/oxfs/cache/meta.py` & `oxfs-0.5.5/oxfs/cache/meta.py`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/oxfs/lock.py` & `oxfs-0.5.5/oxfs/lock.py`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/oxfs/oxfs.py` & `oxfs-0.5.5/oxfs/oxfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def try_connect(self, client, password, abort_on_failed):
         try:
             # https://stackoverflow.com/questions/70565357/paramiko-authentication-fails-with-agreed-upon-rsa-sha2-512-pubkey-algorithm
             client.connect(self.host, port=self.port, disabled_algorithms=dict(pubkeys=["rsa-sha2-512", "rsa-sha2-256"]),
                            username=self.user, password=password, key_filename=self.key_filename)
             return client.open_sftp()
-        except paramiko.ssh_exception.AuthenticationException as e:
+        except paramiko.ssh_exception.SSHException as e:
             if abort_on_failed:
                 print('Permission denied.')
                 self.logger.exception(e)
                 sys.exit(1)
 
     def open_sftp(self):
         client = paramiko.SSHClient()
```

### Comparing `oxfs-0.5.4/oxfs/updater.py` & `oxfs-0.5.5/oxfs/updater.py`

 * *Files identical despite different names*

### Comparing `oxfs-0.5.4/oxfs.egg-info/PKG-INFO` & `oxfs-0.5.5/oxfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxfs
-Version: 0.5.4
+Version: 0.5.5
 Summary: A Fast SFTP File System
 Home-page: https://github.com/oxfs/oxfs
 Author: RainMark
 Author-email: rain.by.zhou@gmail.com
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `oxfs-0.5.4/setup.py` & `oxfs-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ### Get Start
 
 - https://oxfs.io
 '''
 
 setup(
     name='oxfs',
-    version='0.5.4',
+    version='0.5.5',
     author='RainMark',
     author_email='rain.by.zhou@gmail.com',
     description='A Fast SFTP File System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/oxfs/oxfs',
     classifiers=[
```

