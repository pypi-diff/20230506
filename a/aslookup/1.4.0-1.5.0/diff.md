# Comparing `tmp/aslookup-1.4.0.tar.gz` & `tmp/aslookup-1.5.0.tar.gz`

## Comparing `aslookup-1.4.0.tar` & `aslookup-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 aslookup-1.4.0/tox.ini
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/__init__.py
--rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/exceptions.py
--rwxr-xr-x   0        0        0     7887 2020-02-02 00:00:00.000000 aslookup-1.4.0/aslookup/lookup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/.keep
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/test_input.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aslookup-1.4.0/tests/test_nop.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aslookup-1.4.0/.gitignore
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aslookup-1.4.0/LICENSE
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 aslookup-1.4.0/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 aslookup-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 aslookup-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 aslookup-1.5.0/tox.ini
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 aslookup-1.5.0/aslookup/__init__.py
+-rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 aslookup-1.5.0/aslookup/cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 aslookup-1.5.0/aslookup/exceptions.py
+-rwxr-xr-x   0        0        0     7882 2020-02-02 00:00:00.000000 aslookup-1.5.0/aslookup/lookup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aslookup-1.5.0/tests/.keep
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aslookup-1.5.0/tests/test_input.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 aslookup-1.5.0/tests/test_nop.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 aslookup-1.5.0/.gitignore
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aslookup-1.5.0/LICENSE
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 aslookup-1.5.0/README.md
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 aslookup-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 aslookup-1.5.0/PKG-INFO
```

### Comparing `aslookup-1.4.0/tox.ini` & `aslookup-1.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `aslookup-1.4.0/aslookup/cli.py` & `aslookup-1.5.0/aslookup/cli.py`

 * *Files identical despite different names*

### Comparing `aslookup-1.4.0/aslookup/lookup.py` & `aslookup-1.5.0/aslookup/lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Lookup routines."""
 
-import re
 import logging
+import re
 from collections import namedtuple
 
-import pytricia
 import dns.resolver
 import dns.reversename
+import pytricia
 
 from .exceptions import (
+    AddressFormatError,
     NoASDataError,
     NonroutableAddressError,
-    AddressFormatError,
 )
 
-
 logger = logging.getLogger(__name__)
 
 AS_SERVICES = {
     "shadowserver": {
         "origin_suffix": "origin.asn.shadowserver.org",
     },
     "cymru": {
@@ -103,15 +102,15 @@
         "15133 | US | arin | 2007-03-19 | EDGECAST, US"
 
     """
     s = s.strip('"')
     # Cymru results began to append a comma and country code to the end of the
     # AS name, polluting the data. Strip it off.
     s = re.sub(r", [A-Z]{2}$", "", s)
-    fields = s.split(" | ")
+    fields = s.split("|")
     fields = [x.strip() for x in fields]
     as_data = ASData(
         asn=fields[0],
         handle=f"AS{fields[0]}",
         as_name=fields[4],
         prefix=extra.get("ip_prefix"),
         domain=None,
@@ -134,15 +133,15 @@
         "12876 | 212.129.0.0/18 |  | FR | Online SAS"
 
     """
     s = s.strip('"')
     # Shadowserver results at one point appended a comma and country code to
     # the end of the AS name, polluting the data. Strip it off.
     s = re.sub(r", [A-Z]{2}$", "", s)
-    fields = s.split(" | ")
+    fields = s.split("|")
     fields = [x.strip() for x in fields]
     # For any response that returned AS data but no AS name, alert user.
     if fields[0] and not fields[2]:
         logger.warning("no value for AS name; overriding with ISP")
 
     as_data = ASData(
         asn=fields[0],
```

### Comparing `aslookup-1.4.0/.gitignore` & `aslookup-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aslookup-1.4.0/LICENSE` & `aslookup-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aslookup-1.4.0/README.md` & `aslookup-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aslookup-1.4.0/pyproject.toml` & `aslookup-1.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aslookup"
-version = "1.4.0"
+version = "1.5.0"
 authors = [
     { name="Darren Spruell", email="phatbuckett@gmail.com" },
 ]
 description = "IP to ASN routing data query script"
 readme = "README.md"
 dependencies = [
     "dnspython",
     "pytricia",
 ]
 classifiers = [
     # "Development Status :: 3 - Alpha",
-    "Development Status :: 4 - Beta",
-    # "Development Status :: 5 - Production/Stable",
+    # "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     # "Development Status :: 6 - Mature",
     "License :: OSI Approved :: ISC License (ISCL)",
     "Programming Language :: Python :: 3",
 ]
 
 [project.scripts]
 as-lookup = "aslookup.cli:main"
 
 [project.urls]
-"Homepage" = "https://github.com/dspruell/aslookup/"
+"Bug Tracker" = "https://github.com/dspruell/aslookup/issues"
+"Homepage" = "https://github.com/dspruell/aslookup"
```

### Comparing `aslookup-1.4.0/PKG-INFO` & `aslookup-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: aslookup
-Version: 1.4.0
+Version: 1.5.0
 Summary: IP to ASN routing data query script
-Project-URL: Homepage, https://github.com/dspruell/aslookup/
+Project-URL: Bug Tracker, https://github.com/dspruell/aslookup/issues
+Project-URL: Homepage, https://github.com/dspruell/aslookup
 Author-email: Darren Spruell <phatbuckett@gmail.com>
 License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: dnspython
 Requires-Dist: pytricia
 Description-Content-Type: text/markdown
 
 # aslookup
```

