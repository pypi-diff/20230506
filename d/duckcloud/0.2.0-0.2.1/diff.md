# Comparing `tmp/duckcloud-0.2.0.tar.gz` & `tmp/duckcloud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckcloud-0.2.0.tar", max compression
+gzip compressed data, was "duckcloud-0.2.1.tar", max compression
```

## Comparing `duckcloud-0.2.0.tar` & `duckcloud-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1526 2023-05-05 19:40:56.200714 duckcloud-0.2.0/duckcloud/__init__.py
--rw-r--r--   0        0        0      462 2023-05-05 19:42:31.987823 duckcloud-0.2.0/duckcloud/Session.py
--rw-r--r--   0        0        0     3347 2023-05-06 19:23:52.620238 duckcloud-0.2.0/duckcloud/VM.py
--rw-r--r--   0        0        0      429 2023-05-06 19:24:58.285127 duckcloud-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-05-05 16:26:06.322101 duckcloud-0.2.0/README.md
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 duckcloud-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-05-05 19:40:56.200714 duckcloud-0.2.1/duckcloud/__init__.py
+-rw-r--r--   0        0        0      462 2023-05-05 19:42:31.987823 duckcloud-0.2.1/duckcloud/Session.py
+-rw-r--r--   0        0        0     3348 2023-05-06 19:36:19.112427 duckcloud-0.2.1/duckcloud/VM.py
+-rw-r--r--   0        0        0      429 2023-05-06 19:36:58.197446 duckcloud-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-05-05 16:26:06.322101 duckcloud-0.2.1/README.md
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 duckcloud-0.2.1/PKG-INFO
```

### Comparing `duckcloud-0.2.0/duckcloud/__init__.py` & `duckcloud-0.2.1/duckcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `duckcloud-0.2.0/duckcloud/VM.py` & `duckcloud-0.2.1/duckcloud/VM.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 	def ramset(self, mb):
 		r = requests.post("https://duckcloud.pcprojects.tk/ramset/"+str(self.index)+"?ramset="+mb, headers={"cookie": "token="+self.token}, allow_redirects=False)
 		if "Location" in r.headers:
 			return True
 		else:
 			return False
 	def resize(self, width, height):
-		r = requests.post(f"https://duckcloud.pcprojects.tk/resize/{self.index}?w={width}&h={height}" headers={"cookie": "token="+self.token}, allow_redirects=False) # notepad++ doesnt highlight f strings bruh
+		r = requests.post(f"https://duckcloud.pcprojects.tk/resize/{self.index}?w={width}&h={height}", headers={"cookie": "token="+self.token}, allow_redirects=False) # notepad++ doesnt highlight f strings bruh
 		if "Location" in r.headers:
 			return True
 		else:
 			return False
 	def rename(self, newname):
 		r = requests.post("https://duckcloud.pcprojects.tk/ren/"+str(self.index), json={"vmname": newname}, headers={"cookie": "token="+self.token}, allow_redirects=False)
 		if r.headers["Location"] == "/settings/"+str(self.index):
```

### Comparing `duckcloud-0.2.0/PKG-INFO` & `duckcloud-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckcloud
-Version: 0.2.0
+Version: 0.2.1
 Summary: A small wrapper for duckcloud.
 Author: BadPythonCoder
 Author-email: goaway@lol.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

