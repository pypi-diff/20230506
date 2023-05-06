# Comparing `tmp/fabricauthenticator-1.2rc0.tar.gz` & `tmp/fabricauthenticator-1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabricauthenticator-1.2rc0.tar", last modified: Fri May  5 18:07:31 2023, max compression
+gzip compressed data, was "fabricauthenticator-1.2rc1.tar", last modified: Fri May  5 18:57:13 2023, max compression
```

## Comparing `fabricauthenticator-1.2rc0.tar` & `fabricauthenticator-1.2rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-05-05 18:03:14.733463 fabricauthenticator-1.2rc0/.gitignore
--rw-r--r--   0        0        0     1072 2023-05-03 18:37:04.862085 fabricauthenticator-1.2rc0/LICENSE
--rw-r--r--   0        0        0     1164 2023-05-03 18:37:04.862450 fabricauthenticator-1.2rc0/README.md
--rw-r--r--   0        0        0       23 2023-05-05 18:00:19.782657 fabricauthenticator-1.2rc0/fabricauthenticator/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-05 15:56:19.372834 fabricauthenticator-1.2rc0/fabricauthenticator/fabricauthenticator.py
--rw-r--r--   0        0        0      798 2023-05-05 17:59:47.733357 fabricauthenticator-1.2rc0/pyproject.toml
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 fabricauthenticator-1.2rc0/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-05-05 18:03:14.733463 fabricauthenticator-1.2rc1/.gitignore
+-rw-r--r--   0        0        0     1072 2023-05-03 18:37:04.862085 fabricauthenticator-1.2rc1/LICENSE
+-rw-r--r--   0        0        0     1164 2023-05-03 18:37:04.862450 fabricauthenticator-1.2rc1/README.md
+-rw-r--r--   0        0        0       23 2023-05-05 18:57:10.603727 fabricauthenticator-1.2rc1/fabricauthenticator/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-05 15:56:19.372834 fabricauthenticator-1.2rc1/fabricauthenticator/fabricauthenticator.py
+-rw-r--r--   0        0        0      798 2023-05-05 18:54:59.452005 fabricauthenticator-1.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 fabricauthenticator-1.2rc1/PKG-INFO
```

### Comparing `fabricauthenticator-1.2rc0/.gitignore` & `fabricauthenticator-1.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.2rc0/LICENSE` & `fabricauthenticator-1.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.2rc0/README.md` & `fabricauthenticator-1.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.2rc0/fabricauthenticator/fabricauthenticator.py` & `fabricauthenticator-1.2rc1/fabricauthenticator/fabricauthenticator.py`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.2rc0/pyproject.toml` & `fabricauthenticator-1.2rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                "License :: OSI Approved :: MIT License",
                "Operating System :: OS Independent"]
 description = "Fabric OAuth Authenticator"
 dynamic = ["version"]
 
 keywords = ["Swagger", "Fabric OAuth Authenticator"]
 
-requires-python = '>=3.9'
+requires-python = '>=3.7'
 dependencies = [
     "jupyterhub>=1.0",
     "oauthenticator",
     "ldap3"
     ]
 
 [project.urls]
```

### Comparing `fabricauthenticator-1.2rc0/PKG-INFO` & `fabricauthenticator-1.2rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: fabricauthenticator
-Version: 1.2rc0
+Version: 1.2rc1
 Summary: Fabric OAuth Authenticator
 Keywords: Swagger,Fabric OAuth Authenticator
 Author-email: Komal Thareja <kthare10@renci.org>
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: jupyterhub>=1.0
 Requires-Dist: oauthenticator
 Requires-Dist: ldap3
```

