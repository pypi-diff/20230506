# Comparing `tmp/bc125py-0.9.8.tar.gz` & `tmp/bc125py-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bc125py-0.9.8.tar", last modified: Sat Aug 20 16:02:30 2022, max compression
+gzip compressed data, was "bc125py-0.9.9.tar", last modified: Sat Apr  8 13:39:38 2023, max compression
```

## Comparing `bc125py-0.9.8.tar` & `bc125py-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-08-20 16:02:30.550547 bc125py-0.9.8/
--rw-r--r--   0 max       (1000) max       (1000)     1069 2022-05-11 17:22:41.000000 bc125py-0.9.8/LICENSE
--rw-r--r--   0 max       (1000) max       (1000)     4471 2022-08-20 16:02:30.550547 bc125py-0.9.8/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)     3835 2022-08-20 15:58:42.000000 bc125py-0.9.8/README.md
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-08-20 16:02:30.549548 bc125py-0.9.8/bc125py/
--rw-r--r--   0 max       (1000) max       (1000)      295 2022-08-20 15:58:53.000000 bc125py-0.9.8/bc125py/__init__.py
--rw-r--r--   0 max       (1000) max       (1000)      123 2022-06-19 22:04:28.000000 bc125py-0.9.8/bc125py/__main__.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-08-20 16:02:30.550547 bc125py-0.9.8/bc125py/app/
--rw-r--r--   0 max       (1000) max       (1000)        0 2022-06-19 21:29:46.000000 bc125py-0.9.8/bc125py/app/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)    13673 2022-07-02 18:59:42.000000 bc125py-0.9.8/bc125py/app/cli.py
--rw-r--r--   0 max       (1000) max       (1000)     2293 2022-06-19 22:06:01.000000 bc125py-0.9.8/bc125py/app/core.py
--rw-r--r--   0 max       (1000) max       (1000)      592 2022-05-11 17:22:41.000000 bc125py-0.9.8/bc125py/app/log.py
--rw-r--r--   0 max       (1000) max       (1000)    10600 2022-07-02 18:48:14.000000 bc125py-0.9.8/bc125py/con.py
--rw-r--r--   0 max       (1000) max       (1000)    41370 2022-06-19 21:38:48.000000 bc125py-0.9.8/bc125py/sdo.py
-drwxr-xr-x   0 max       (1000) max       (1000)        0 2022-08-20 16:02:30.550547 bc125py-0.9.8/bc125py.egg-info/
--rw-r--r--   0 max       (1000) max       (1000)     4471 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/PKG-INFO
--rw-r--r--   0 max       (1000) max       (1000)      366 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/SOURCES.txt
--rw-r--r--   0 max       (1000) max       (1000)        1 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/dependency_links.txt
--rw-r--r--   0 max       (1000) max       (1000)       50 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/entry_points.txt
--rw-r--r--   0 max       (1000) max       (1000)       19 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/requires.txt
--rw-r--r--   0 max       (1000) max       (1000)        8 2022-08-20 16:02:30.000000 bc125py-0.9.8/bc125py.egg-info/top_level.txt
--rw-r--r--   0 max       (1000) max       (1000)       38 2022-08-20 16:02:30.550547 bc125py-0.9.8/setup.cfg
--rw-r--r--   0 max       (1000) max       (1000)      939 2022-06-19 22:11:16.000000 bc125py-0.9.8/setup.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-08 13:39:38.755501 bc125py-0.9.9/
+-rw-r--r--   0 max       (1000) max       (1000)     1069 2022-05-11 17:22:41.000000 bc125py-0.9.9/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)     4471 2023-04-08 13:39:38.755501 bc125py-0.9.9/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)     3835 2022-08-20 15:58:42.000000 bc125py-0.9.9/README.md
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-08 13:39:38.754500 bc125py-0.9.9/bc125py/
+-rw-r--r--   0 max       (1000) max       (1000)      295 2023-04-08 13:32:15.000000 bc125py-0.9.9/bc125py/__init__.py
+-rw-r--r--   0 max       (1000) max       (1000)      123 2022-06-19 22:04:28.000000 bc125py-0.9.9/bc125py/__main__.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-08 13:39:38.755501 bc125py-0.9.9/bc125py/app/
+-rw-r--r--   0 max       (1000) max       (1000)        0 2022-06-19 21:29:46.000000 bc125py-0.9.9/bc125py/app/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)    13714 2023-04-08 13:34:37.000000 bc125py-0.9.9/bc125py/app/cli.py
+-rw-r--r--   0 max       (1000) max       (1000)     2293 2022-06-19 22:06:01.000000 bc125py-0.9.9/bc125py/app/core.py
+-rw-r--r--   0 max       (1000) max       (1000)      592 2022-05-11 17:22:41.000000 bc125py-0.9.9/bc125py/app/log.py
+-rw-r--r--   0 max       (1000) max       (1000)    10600 2022-07-02 18:48:14.000000 bc125py-0.9.9/bc125py/con.py
+-rw-r--r--   0 max       (1000) max       (1000)    41392 2023-04-08 13:32:15.000000 bc125py-0.9.9/bc125py/sdo.py
+drwxr-xr-x   0 max       (1000) max       (1000)        0 2023-04-08 13:39:38.755501 bc125py-0.9.9/bc125py.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)     4471 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/PKG-INFO
+-rw-r--r--   0 max       (1000) max       (1000)      366 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/SOURCES.txt
+-rw-r--r--   0 max       (1000) max       (1000)        1 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/dependency_links.txt
+-rw-r--r--   0 max       (1000) max       (1000)       50 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/entry_points.txt
+-rw-r--r--   0 max       (1000) max       (1000)       19 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/requires.txt
+-rw-r--r--   0 max       (1000) max       (1000)        8 2023-04-08 13:39:38.000000 bc125py-0.9.9/bc125py.egg-info/top_level.txt
+-rw-r--r--   0 max       (1000) max       (1000)       38 2023-04-08 13:39:38.755501 bc125py-0.9.9/setup.cfg
+-rw-r--r--   0 max       (1000) max       (1000)      939 2022-06-19 22:11:16.000000 bc125py-0.9.9/setup.py
```

### Comparing `bc125py-0.9.8/LICENSE` & `bc125py-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bc125py-0.9.8/PKG-INFO` & `bc125py-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc125py
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python-based interface for the Uniden BC125AT
 Home-page: https://github.com/itsmaxymoo/bc125py
 Author: Max Loiacono
 Author-email: max.loiacono@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/itsmaxymoo/bc125py/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bc125py-0.9.8/README.md` & `bc125py-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `bc125py-0.9.8/bc125py/app/cli.py` & `bc125py-0.9.9/bc125py/app/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # --- Program entrypoint
 def main() -> int:
 
 	# --- Command Line Arguments ---
 	# Create main cli parser
 	main_parser = argparse.ArgumentParser(
 		prog=bc125py.PACKAGE_NAME,
-		description=bc125py.PACKAGE_DESCRIPTION,
+		description=bc125py.PACKAGE_DESCRIPTION + ", version " + bc125py.PACKAGE_VERSION,
 		epilog="Please report all issues at {url} or to {email}".format(
 			url=bc125py.PACKAGE_URL,
 			email=bc125py.PACKAGE_AUTHOR_EMAIL
 		)
 	)
 
 	# Add universal cli arguments
```

### Comparing `bc125py-0.9.8/bc125py/app/core.py` & `bc125py-0.9.9/bc125py/app/core.py`

 * *Files identical despite different names*

### Comparing `bc125py-0.9.8/bc125py/app/log.py` & `bc125py-0.9.9/bc125py/app/log.py`

 * *Files identical despite different names*

### Comparing `bc125py-0.9.8/bc125py/con.py` & `bc125py-0.9.9/bc125py/con.py`

 * *Files identical despite different names*

### Comparing `bc125py-0.9.8/bc125py/sdo.py` & `bc125py-0.9.9/bc125py/sdo.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,15 +736,15 @@
 
 	def __init__(self, index: int = 1) -> None:
 		self.index = index
 
 
 	def to_write_command(self) -> tuple:
 		return self.to_fetch_command() + (
-			self.name,
+			self.name if self.name else " ",
 			freq_to_scanner(self.frequency),
 			self.modulation.value,
 			self.ctcss,
 			self.delay,
 			self.locked_out.value,
 			self.priority.value
 		)
```

### Comparing `bc125py-0.9.8/bc125py.egg-info/PKG-INFO` & `bc125py-0.9.9/bc125py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bc125py
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Python-based interface for the Uniden BC125AT
 Home-page: https://github.com/itsmaxymoo/bc125py
 Author: Max Loiacono
 Author-email: max.loiacono@protonmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/itsmaxymoo/bc125py/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bc125py-0.9.8/setup.py` & `bc125py-0.9.9/setup.py`

 * *Files identical despite different names*

