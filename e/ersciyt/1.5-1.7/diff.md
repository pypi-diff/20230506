# Comparing `tmp/ersciyt-1.5.tar.gz` & `tmp/ersciyt-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ersciyt-1.5.tar", last modified: Sat Apr 29 22:10:30 2023, max compression
+gzip compressed data, was "ersciyt-1.7.tar", last modified: Sat May  6 06:46:30 2023, max compression
```

## Comparing `ersciyt-1.5.tar` & `ersciyt-1.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.815107 ersciyt-1.5/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-29 22:10:25.000000 ersciyt-1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-29 22:10:25.000000 ersciyt-1.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-29 22:10:30.815107 ersciyt-1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      517 2023-04-29 22:10:25.000000 ersciyt-1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.813107 ersciyt-1.5/ersciyt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/__init__.py
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/admin.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.815107 ersciyt-1.5/ersciyt/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/models.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/tests.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/urls.py
--rw-r--r--   0 root         (0) root         (0)     6437 2023-04-29 22:10:25.000000 ersciyt-1.5/ersciyt/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 22:10:30.814108 ersciyt-1.5/ersciyt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      795 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      354 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-29 22:10:30.000000 ersciyt-1.5/ersciyt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      654 2023-04-29 22:10:30.816108 ersciyt-1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       36 2023-04-29 22:10:25.000000 ersciyt-1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-05-06 06:46:21.000000 ersciyt-1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-06 06:46:21.000000 ersciyt-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-06 06:46:30.692298 ersciyt-1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      517 2023-05-06 06:46:21.000000 ersciyt-1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.691298 ersciyt-1.7/ersciyt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       63 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/admin.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt/static/
+-rw-r--r--   0 root         (0) root         (0)    11852 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/static/ersci_viddown_tab2.xpi
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/tests.py
+-rw-r--r--   0 root         (0) root         (0)      412 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/urls.py
+-rw-r--r--   0 root         (0) root         (0)     6611 2023-05-06 06:46:21.000000 ersciyt-1.7/ersciyt/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 06:46:30.692298 ersciyt-1.7/ersciyt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      795 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-06 06:46:30.000000 ersciyt-1.7/ersciyt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-06 06:46:30.693298 ersciyt-1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       36 2023-05-06 06:46:21.000000 ersciyt-1.7/setup.py
```

### Comparing `ersciyt-1.5/LICENSE` & `ersciyt-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ersciyt-1.5/PKG-INFO` & `ersciyt-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.5
+Version: 1.7
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.5/README.md` & `ersciyt-1.7/README.md`

 * *Files identical despite different names*

### Comparing `ersciyt-1.5/ersciyt/views.py` & `ersciyt-1.7/ersciyt/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -150,12 +150,15 @@
     try:
         return HttpResponse ('''
         <p>Use address of youtube after watch like - for download video -  :<br>
         <b> YourSiteName/ytlink?url=<any video site link></b><br>
         or<br>
         link name like - for play in firefox -  : <br>
         <b>YourSiteName/xazlZh1lTpM</b><br>        
-        <a href="/static/ersci_viddown2.xpi">video download firefox Addon</a></br>
+        <a href="/static/ersci_viddown_tab2.xpi">Video download firefox Addon direct link</a><br>
+        or<br>
+        <a href="https://addons.mozilla.org/en-US/firefox/addon/ersci_viddown_tab2">video download firefox Addon mozilla site link</a>
+        
         </p>
         ''')
     except:
         return HttpResponse ('Youtube Url Is Mistake!!!')
```

### Comparing `ersciyt-1.5/ersciyt.egg-info/PKG-INFO` & `ersciyt-1.7/ersciyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ersciyt
-Version: 1.5
+Version: 1.7
 Summary: Youtube Downloader
 Home-page: https://github.com/epg900/yt.git
 Author: epg
 Author-email: epg900@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ersciyt-1.5/setup.cfg` & `ersciyt-1.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ersciyt
-version = 1.5
+version = 1.7
 description = Youtube Downloader
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/epg900/yt.git
 author = epg
 author_email = epg900@gmail.com
 license = GNU GENERAL PUBLIC LICENSE
```

