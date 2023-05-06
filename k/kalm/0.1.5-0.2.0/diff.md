# Comparing `tmp/kalm-0.1.5.tar.gz` & `tmp/kalm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalm-0.1.5.tar", last modified: Fri Apr 21 10:42:25 2023, max compression
+gzip compressed data, was "kalm-0.2.0.tar", max compression
```

## Comparing `kalm-0.1.5.tar` & `kalm-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,9 @@
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/
--rw-rw-r--   0 jho       (1000) jho       (1000)     1081 2023-04-21 06:37:05.000000 kalm-0.1.5/LICENSE.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:42:25.813122 kalm-0.1.5/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      705 2023-04-21 06:37:05.000000 kalm-0.1.5/README.md
--rw-rw-r--   0 jho       (1000) jho       (1000)     1282 2023-04-21 10:41:59.000000 kalm-0.1.5/pyproject.toml
--rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:42:25.813122 kalm-0.1.5/setup.cfg
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.811123 kalm-0.1.5/src/
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.812122 kalm-0.1.5/src/kalm/
--rw-rw-r--   0 jho       (1000) jho       (1000)    10421 2023-04-21 10:40:56.000000 kalm-0.1.5/src/kalm/__init__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)    32279 2023-04-21 10:40:49.000000 kalm-0.1.5/src/kalm/kalm.py
--rw-rw-r--   0 jho       (1000) jho       (1000)     1296 2023-04-21 06:37:05.000000 kalm-0.1.5/src/kalm/netbox.py
--rw-rw-r--   0 jho       (1000) jho       (1000)        9 2023-04-21 06:37:05.000000 kalm-0.1.5/src/kalm/package_data.dat
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:41:48.000000 kalm-0.1.5/src/kalm/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/src/kalm.egg-info/
--rw-rw-r--   0 jho       (1000) jho       (1000)     2703 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      377 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/SOURCES.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/dependency_links.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       35 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/entry_points.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/requires.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       13 2023-04-21 10:42:25.000000 kalm-0.1.5/src/kalm.egg-info/top_level.txt
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/src/toolbox/
--rw-rw-r--   0 jho       (1000) jho       (1000)      312 2023-04-21 06:46:41.000000 kalm-0.1.5/src/toolbox/toolbox.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:42:25.813122 kalm-0.1.5/tests/
--rw-rw-r--   0 jho       (1000) jho       (1000)      417 2023-04-21 06:37:05.000000 kalm-0.1.5/tests/test_simple.py
+-rw-r--r--   0        0        0     1081 2023-05-05 20:49:24.880279 kalm-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1790 2023-05-06 18:07:36.278019 kalm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10421 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/__init__.py
+-rw-r--r--   0        0        0    32280 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/kalm.py
+-rw-r--r--   0        0        0     6484 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/kalm_api.py
+-rw-r--r--   0        0        0     1296 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/netbox.py
+-rw-r--r--   0        0        0        9 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/package_data.dat
+-rw-r--r--   0        0        0      312 2023-05-05 20:49:24.884279 kalm-0.2.0/src/kalm/toolbox.py
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 kalm-0.2.0/PKG-INFO
```

### Comparing `kalm-0.1.5/LICENSE.txt` & `kalm-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kalm-0.1.5/pyproject.toml` & `kalm-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,32 @@
+[tool.poetry]
+name = "kalm"
+version = "0.2.0"
+description = "Knowit automation lifecycle management"
+authors = ["Jakob Holst <jakob.holst@knowit.dk>"]
+license = "MIT"
+homepage = "https://kalm.openknowit.com"
+repository = "https://github.com/miracle-as/openknowit_kalm.git"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+requests = "^2.25"
+pytest = "^6.2"
+mypy = "^0.910"
+redis = "^4.5.3"
+pynetbox = "^6.6.2"
+wheel = "^0.34.2"
+hvac = "^1.1.0"
+netbox = "^0.0.2"
+
+
 [project]
 name = "kalm"  
-version = "0.1.5" 
-description = "" 
+version = "0.2.0-Development" 
+description = "Knowit automation lifecycle management"
 readme = "README.md" # Optional
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["kalm", "awx", "ansible", "automation"]  
 authors = [
   {name = "Jakob Holst", email = "jho@miracle.dk" }
 ]
```

### Comparing `kalm-0.1.5/src/kalm/__init__.py` & `kalm-0.2.0/src/kalm/__init__.py`

 * *Files identical despite different names*

### Comparing `kalm-0.1.5/src/kalm/kalm.py` & `kalm-0.2.0/src/kalm/kalm.py`

 * *Files 0% similar despite different names*

```diff
@@ -832,7 +832,8 @@
           run_every = "MINUTELY"
         if ( schedule ['end'] == "never" ):
           dtend = "null"
         awx_create_schedule(schedulename, unified_job_template_id, description,tz, dtstart, run_frequency, run_every, dtend, scheduletype, orgname, mytoken, r)
     except:
       prettyllog("config", "initialize", "schedules", orgname, "000",  "No schedules found")
 ### The end
+
```

### Comparing `kalm-0.1.5/src/kalm/netbox.py` & `kalm-0.2.0/src/kalm/netbox.py`

 * *Files identical despite different names*

