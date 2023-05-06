# Comparing `tmp/ols_client-0.1.3.tar.gz` & `tmp/ols_client-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ols_client-0.1.3.tar", last modified: Tue Feb 21 13:56:50 2023, max compression
+gzip compressed data, was "ols_client-0.1.4.tar", last modified: Sat May  6 10:20:27 2023, max compression
```

## Comparing `ols_client-0.1.3.tar` & `ols_client-0.1.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.097605 ols_client-0.1.3/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-09-01 14:03:59.000000 ols_client-0.1.3/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      382 2022-09-01 14:03:59.000000 ols_client-0.1.3/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     6918 2023-02-21 13:56:50.097756 ols_client-0.1.3/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     5653 2022-09-07 16:12:51.000000 ols_client-0.1.3/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.083937 ols_client-0.1.3/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.088858 ols_client-0.1.3/docs/source/
--rw-r--r--   0 cthoyt     (501) staff       (20)      231 2022-09-01 14:03:59.000000 ols_client-0.1.3/docs/source/cli.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7038 2023-02-21 13:56:48.000000 ols_client-0.1.3/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      809 2022-09-02 09:09:27.000000 ols_client-0.1.3/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       60 2022-09-02 09:09:27.000000 ols_client-0.1.3/docs/source/usage.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-09-01 14:40:12.000000 ols_client-0.1.3/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2423 2023-02-21 13:56:50.098640 ols_client-0.1.3/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.084539 ols_client-0.1.3/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.092570 ols_client-0.1.3/src/ols_client/
--rw-r--r--   0 cthoyt     (501) staff       (20)      576 2022-09-16 13:12:38.000000 ols_client-0.1.3/src/ols_client/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      327 2022-09-01 14:03:59.000000 ols_client-0.1.3/src/ols_client/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     1696 2022-09-02 11:22:05.000000 ols_client-0.1.3/src/ols_client/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13276 2023-02-21 13:52:13.000000 ols_client-0.1.3/src/ols_client/client.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-09-01 14:03:59.000000 ols_client-0.1.3/src/ols_client/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     1016 2023-02-21 13:56:48.000000 ols_client-0.1.3/src/ols_client/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.095165 ols_client-0.1.3/src/ols_client.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     6918 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)      636 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       51 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/entry_points.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-09-01 14:41:17.000000 ols_client-0.1.3/src/ols_client.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      161 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)       11 2023-02-21 13:56:50.000000 ols_client-0.1.3/src/ols_client.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-02-21 13:56:50.097155 ols_client-0.1.3/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       60 2022-09-01 14:03:59.000000 ols_client-0.1.3/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      635 2022-09-02 11:24:41.000000 ols_client-0.1.3/tests/cases.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      594 2023-02-21 13:52:33.000000 ols_client-0.1.3/tests/test_ols_client.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      404 2022-09-01 14:03:59.000000 ols_client-0.1.3/tests/test_version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.336052 ols_client-0.1.4/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2022-09-01 14:03:59.000000 ols_client-0.1.4/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      382 2022-09-01 14:03:59.000000 ols_client-0.1.4/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6918 2023-05-06 10:20:27.336208 ols_client-0.1.4/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5653 2022-09-07 16:12:51.000000 ols_client-0.1.4/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.320901 ols_client-0.1.4/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.326611 ols_client-0.1.4/docs/source/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      231 2022-09-01 14:03:59.000000 ols_client-0.1.4/docs/source/cli.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7049 2023-05-06 10:20:26.000000 ols_client-0.1.4/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      809 2022-09-02 09:09:27.000000 ols_client-0.1.4/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       60 2022-09-02 09:09:27.000000 ols_client-0.1.4/docs/source/usage.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      376 2022-09-01 14:40:12.000000 ols_client-0.1.4/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2429 2023-05-06 10:20:27.337130 ols_client-0.1.4/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.321844 ols_client-0.1.4/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.330617 ols_client-0.1.4/src/ols_client/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      576 2022-09-16 13:12:38.000000 ols_client-0.1.4/src/ols_client/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      327 2022-09-01 14:03:59.000000 ols_client-0.1.4/src/ols_client/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1696 2022-09-02 11:22:05.000000 ols_client-0.1.4/src/ols_client/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13280 2023-05-05 13:37:11.000000 ols_client-0.1.4/src/ols_client/client.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-09-01 14:03:59.000000 ols_client-0.1.4/src/ols_client/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1016 2023-05-06 10:20:26.000000 ols_client-0.1.4/src/ols_client/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.333140 ols_client-0.1.4/src/ols_client.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     6918 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)      636 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       51 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/entry_points.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2022-09-01 14:41:17.000000 ols_client-0.1.4/src/ols_client.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      161 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)       11 2023-05-06 10:20:27.000000 ols_client-0.1.4/src/ols_client.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2023-05-06 10:20:27.335556 ols_client-0.1.4/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       60 2022-09-01 14:03:59.000000 ols_client-0.1.4/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      635 2022-09-02 11:24:41.000000 ols_client-0.1.4/tests/cases.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      638 2023-05-05 13:38:03.000000 ols_client-0.1.4/tests/test_ols_client.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      404 2022-09-01 14:03:59.000000 ols_client-0.1.4/tests/test_version.py
```

### Comparing `ols_client-0.1.3/LICENSE` & `ols_client-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/PKG-INFO` & `ols_client-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ols_client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A client to the EBI Ontology Lookup Service
 Home-page: https://github.com/cthoyt/ols-client
 Download-URL: https://github.com/cthoyt/ols-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ols_client Version: 0.1.3 Summary: A client to the
+Metadata-Version: 2.1 Name: ols_client Version: 0.1.4 Summary: A client to the
 EBI Ontology Lookup Service Home-page: https://github.com/cthoyt/ols-client
 Download-URL: https://github.com/cthoyt/ols-client/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/ols-client/issues Project-URL: Source Code, https://
 github.com/cthoyt/ols-client Keywords: snekpack,cookiecutter Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
```

### Comparing `ols_client-0.1.3/README.md` & `ols_client-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/docs/source/conf.py` & `ols_client-0.1.4/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "ols_client"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.1.3"
+release = "0.1.4"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
@@ -225,15 +225,15 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/3/": None,
+    "python": ("https://docs.python.org/3", None),
 }
 
 autoclass_content = "both"
 
 # Don't sort alphabetically, explained at:
 # https://stackoverflow.com/questions/37209921/python-how-not-to-sort-sphinx-output-in-alphabetical-order
 autodoc_member_order = "bysource"
```

### Comparing `ols_client-0.1.3/docs/source/index.rst` & `ols_client-0.1.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/setup.cfg` & `ols_client-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ols_client
-version = 0.1.3
+version = 0.1.4
 description = A client to the EBI Ontology Lookup Service
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/ols-client
 download_url = https://github.com/cthoyt/ols-client/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/ols-client/issues
@@ -100,14 +100,15 @@
 ignore = 
 	S301 # pickle
 	S403 # pickle
 	S404
 	S603
 	W503 # Line break before binary operator (flake8 is wrong)
 	E203  # whitespace before ':'
+	S113
 exclude = 
 	.tox,
 	.git,
 	__pycache__,
 	docs/source/conf.py,
 	build,
 	dist,
```

### Comparing `ols_client-0.1.3/src/ols_client/__init__.py` & `ols_client-0.1.4/src/ols_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/src/ols_client/cli.py` & `ols_client-0.1.4/src/ols_client/cli.py`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/src/ols_client/client.py` & `ols_client-0.1.4/src/ols_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,20 +294,20 @@
         response = self.get_ontology(ontology)
         return response["config"].get("description")
 
 
 class EBIClient(Client):
     """The first-party instance of the OLS.
 
-    .. seealso:: http://www.ebi.ac.uk/ols
+    .. seealso:: https://www.ebi.ac.uk/ols4
     """
 
     def __init__(self):
         """Initialize the client."""
-        super().__init__(base_url="http://www.ebi.ac.uk/ols")
+        super().__init__(base_url="https://www.ebi.ac.uk/ols4")
 
 
 class TIBClient(Client):
     """The TIB instance of the OLS.
 
     With its new Terminology Service, TIB – Leibniz Information Centre
     for Science and Technology and University Library provides a single
```

### Comparing `ols_client-0.1.3/src/ols_client/version.py` & `ols_client-0.1.4/src/ols_client/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`ols_client` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `ols_client-0.1.3/src/ols_client.egg-info/PKG-INFO` & `ols_client-0.1.4/src/ols_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ols-client
-Version: 0.1.3
+Version: 0.1.4
 Summary: A client to the EBI Ontology Lookup Service
 Home-page: https://github.com/cthoyt/ols-client
 Download-URL: https://github.com/cthoyt/ols-client/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ols-client Version: 0.1.3 Summary: A client to the
+Metadata-Version: 2.1 Name: ols-client Version: 0.1.4 Summary: A client to the
 EBI Ontology Lookup Service Home-page: https://github.com/cthoyt/ols-client
 Download-URL: https://github.com/cthoyt/ols-client/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/ols-client/issues Project-URL: Source Code, https://
 github.com/cthoyt/ols-client Keywords: snekpack,cookiecutter Classifier:
 Development Status :: 1 - Planning Classifier: Environment :: Console
```

### Comparing `ols_client-0.1.3/src/ols_client.egg-info/SOURCES.txt` & `ols_client-0.1.4/src/ols_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/tests/cases.py` & `ols_client-0.1.4/tests/cases.py`

 * *Files identical despite different names*

### Comparing `ols_client-0.1.3/tests/test_ols_client.py` & `ols_client-0.1.4/tests/test_ols_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class TestEbi(cases.TestClient):
     """Tests for the EBI client."""
 
     client_cls = EBIClient
     test_ontology = "aro"
-    test_label = "CMY-167"
+    test_label = "tetracycline-resistant ribosomal protection protein"
 
     def test_get_term(self):
         """Test getting a term."""
         iri = "http://biomodels.net/SBO/SBO_0000150"
         res_json = self.client.get_term("sbo", iri)
         terms = res_json["_embedded"]["terms"]
         self.assertEqual(1, len(terms))
```

