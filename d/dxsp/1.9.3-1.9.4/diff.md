# Comparing `tmp/dxsp-1.9.3.tar.gz` & `tmp/dxsp-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-1.9.3.tar", max compression
+gzip compressed data, was "dxsp-1.9.4.tar", max compression
```

## Comparing `dxsp-1.9.3.tar` & `dxsp-1.9.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-05-06 05:10:29.486180 dxsp-1.9.3/LICENSE
--rw-r--r--   0        0        0     3349 2023-05-06 05:10:29.486180 dxsp-1.9.3/README.md
--rw-r--r--   0        0        0       38 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/.gitignore
--rw-r--r--   0        0        0      169 2023-05-06 05:10:30.190189 dxsp-1.9.3/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      392 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/config.py
--rw-r--r--   0        0        0      556 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/default_settings.toml
--rw-r--r--   0        0        0    28346 2023-05-06 05:10:29.486180 dxsp-1.9.3/dxsp/main.py
--rw-r--r--   0        0        0     1787 2023-05-06 05:10:30.186189 dxsp-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-06 05:22:37.420173 dxsp-1.9.4/LICENSE
+-rw-r--r--   0        0        0     3349 2023-05-06 05:22:37.420173 dxsp-1.9.4/README.md
+-rw-r--r--   0        0        0       38 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/.gitignore
+-rw-r--r--   0        0        0      169 2023-05-06 05:22:38.060159 dxsp-1.9.4/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      392 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/config.py
+-rw-r--r--   0        0        0      556 2023-05-06 05:22:37.420173 dxsp-1.9.4/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    28346 2023-05-06 05:22:37.424172 dxsp-1.9.4/dxsp/main.py
+-rw-r--r--   0        0        0     1787 2023-05-06 05:22:38.060159 dxsp-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dxsp-1.9.4/PKG-INFO
```

### Comparing `dxsp-1.9.3/LICENSE` & `dxsp-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.3/README.md` & `dxsp-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.3/dxsp/assets/blockchains.py` & `dxsp-1.9.4/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.3/dxsp/default_settings.toml` & `dxsp-1.9.4/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.3/dxsp/main.py` & `dxsp-1.9.4/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-1.9.3/pyproject.toml` & `dxsp-1.9.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "1.9.3"
+version = "1.9.4"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-1.9.3/PKG-INFO` & `dxsp-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 1.9.3
+Version: 1.9.4
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

