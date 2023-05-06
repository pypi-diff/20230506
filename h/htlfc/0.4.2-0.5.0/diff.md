# Comparing `tmp/htlfc-0.4.2.tar.gz` & `tmp/htlfc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htlfc-0.4.2.tar", last modified: Fri Feb 24 09:01:52 2023, max compression
+gzip compressed data, was "htlfc-0.5.0.tar", last modified: Sat May  6 08:25:24 2023, max compression
```

## Comparing `htlfc-0.4.2.tar` & `htlfc-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.188866 htlfc-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-24 09:01:37.000000 htlfc-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-24 09:01:52.188866 htlfc-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-02-24 09:01:37.000000 htlfc-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 09:01:52.188866 htlfc-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-24 09:01:37.000000 htlfc-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.180866 htlfc-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.180866 htlfc-0.4.2/src/htlfc/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/ABOUT.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.184866 htlfc-0.4.2/src/htlfc/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/codecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1859 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/filedir.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/loader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/maff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4405 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/mht.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/agents/war.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.184866 htlfc-0.4.2/src/htlfc/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/gui/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.188866 htlfc-0.4.2/src/htlfc/merger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/merger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/merger/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/merger/infobar.css
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/merger/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/merger/xmltree.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-24 09:01:37.000000 htlfc-0.4.2/src/htlfc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:01:52.184866 htlfc-0.4.2/src/htlfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 09:01:52.000000 htlfc-0.4.2/src/htlfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.574240 htlfc-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 08:25:11.000000 htlfc-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-06 08:25:24.574240 htlfc-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-06 08:25:11.000000 htlfc-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:25:24.574240 htlfc-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 08:25:11.000000 htlfc-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.566240 htlfc-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.570240 htlfc-0.5.0/src/htlfc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/ABOUT.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.574240 htlfc-0.5.0/src/htlfc/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1730 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/codecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1859 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/filedir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2151 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2521 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/maff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4405 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/mht.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/agents/war.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.574240 htlfc-0.5.0/src/htlfc/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/gui/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.574240 htlfc-0.5.0/src/htlfc/merger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/merger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/merger/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/merger/infobar.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/merger/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/merger/xmltree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-06 08:25:11.000000 htlfc-0.5.0/src/htlfc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:25:24.570240 htlfc-0.5.0/src/htlfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-06 08:25:24.000000 htlfc-0.5.0/src/htlfc.egg-info/top_level.txt
```

### Comparing `htlfc-0.4.2/LICENSE` & `htlfc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/PKG-INFO` & `htlfc-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htlfc
-Version: 0.4.2
+Version: 0.5.0
 Summary: Hypertext Legacy File Converter
 License: AGPLv3+
 Keywords: hypertext,html,mht,mhtml,maff
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `htlfc-0.4.2/pyproject.toml` & `htlfc-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/ABOUT.md` & `htlfc-0.5.0/src/htlfc/ABOUT.md`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/agents/codecs.py` & `htlfc-0.5.0/src/htlfc/agents/codecs.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 def get_text(filename):
     """Open filename, determine it's encoding and decode
     filename:str = path to file
     return@success (content,encoding)
         content:str = decoded content of filename
         encoding:str iff explicit (as defined in the meta tag)
                      or None
-    exception:
+    exceptions:
         EOFError = file is empty
+        RuntimeError("Unable to detect character set and decode file: {infile}")
     """
     with open(filename,'rb') as infile:
         raw_str = infile.read()
     if len(raw_str) == 0:
         raise EOFError(f"File is empty: {filename}")
 
     # look for "charset=word" in the meta tag (word includes - and _)
     re_charset = re.compile(b'<meta.*charset=([\w\-_]+).*>' ,flags=re.IGNORECASE)
     items = re_charset.findall(raw_str)
     encoding = None
+    content = None
     for item in items:
         try:
             found = item.decode().lower()
             content = raw_str.decode(encoding=found)
             encoding = found
             break
         except UnicodeDecodeError:
             continue
 
-    if encoding is None:
+    if content is None:
         # detect encoding with chardet
         try:
             found = chardet.detect(raw_str)['encoding']
             content = raw_str.decode(found)
-            encoding = None
         except UnicodeDecodeError:
-            raise RuntimeError(f"Unable to detect character set and decode file: {infile}")
+            # if all else fails, fallback to utf-8
+            try:
+                content = raw_str.decode(encoding='utf-8')
+            except UnicodeDecodeError:
+                raise RuntimeError(f"Unable to detect character set and decode file: {infile}")
 
     if content is not None:
         content = content.replace('&quot;','"')
     return (content,encoding)
```

### Comparing `htlfc-0.4.2/src/htlfc/agents/filedir.py` & `htlfc-0.5.0/src/htlfc/agents/filedir.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/agents/loader.py` & `htlfc-0.5.0/src/htlfc/agents/loader.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/agents/maff.py` & `htlfc-0.5.0/src/htlfc/agents/maff.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/agents/mht.py` & `htlfc-0.5.0/src/htlfc/agents/mht.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/agents/war.py` & `htlfc-0.5.0/src/htlfc/agents/war.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/gui/converter.py` & `htlfc-0.5.0/src/htlfc/gui/converter.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/gui/find.py` & `htlfc-0.5.0/src/htlfc/gui/find.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/gui/interface.py` & `htlfc-0.5.0/src/htlfc/gui/interface.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/gui/select.py` & `htlfc-0.5.0/src/htlfc/gui/select.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/gui/viewer.py` & `htlfc-0.5.0/src/htlfc/gui/viewer.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/main.py` & `htlfc-0.5.0/src/htlfc/main.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/merger/convert.py` & `htlfc-0.5.0/src/htlfc/merger/convert.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc/merger/manifest.py` & `htlfc-0.5.0/src/htlfc/merger/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         """Search for datapath (a URL string taken from html or css)
         starting at directory base
         if a match is found:
             attach to either source.frames or source.manifest
         """
         path = urllib.parse.unquote(datapath)
         path = os.path.normpath(path) # OS specific
+        if ".html#" in path:
+            # strip fragment identifier from path
+            path = path.split("#")[0]
         for dirpath, dirx, files in os.walk(base):
           for thisfile in files:
               fullpath = os.path.join(dirpath,thisfile)
               if fullpath.endswith(path):
                   source.manifest.update({datapath:fullpath})
                   return
```

### Comparing `htlfc-0.4.2/src/htlfc/merger/xmltree.py` & `htlfc-0.5.0/src/htlfc/merger/xmltree.py`

 * *Files identical despite different names*

### Comparing `htlfc-0.4.2/src/htlfc.egg-info/PKG-INFO` & `htlfc-0.5.0/src/htlfc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htlfc
-Version: 0.4.2
+Version: 0.5.0
 Summary: Hypertext Legacy File Converter
 License: AGPLv3+
 Keywords: hypertext,html,mht,mhtml,maff
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `htlfc-0.4.2/src/htlfc.egg-info/SOURCES.txt` & `htlfc-0.5.0/src/htlfc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

