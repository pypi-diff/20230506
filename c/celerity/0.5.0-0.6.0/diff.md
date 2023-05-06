# Comparing `tmp/celerity-0.5.0.tar.gz` & `tmp/celerity-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celerity-0.5.0.tar", max compression
+gzip compressed data, was "celerity-0.6.0.tar", max compression
```

## Comparing `celerity-0.5.0.tar` & `celerity-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1075 2023-05-05 16:10:40.668348 celerity-0.5.0/LICENSE
--rw-r--r--   0        0        0     4346 2023-05-05 16:10:40.668348 celerity-0.5.0/README.md
--rw-r--r--   0        0        0     1830 2023-05-05 16:10:40.668348 celerity-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/__init__.py
--rw-r--r--   0        0        0     2501 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/astrometry.py
--rw-r--r--   0        0        0      240 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/common.py
--rw-r--r--   0        0        0      997 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/constants.py
--rw-r--r--   0        0        0     1650 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/coordinates.py
--rw-r--r--   0        0        0      468 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/epoch.py
--rw-r--r--   0        0        0     2092 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/seeing.py
--rw-r--r--   0        0        0     4129 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/temporal.py
--rw-r--r--   0        0        0      961 2023-05-05 16:10:40.668348 celerity-0.5.0/src/celerity/utilities.py
--rw-r--r--   0        0        0     4979 1970-01-01 00:00:00.000000 celerity-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-06 18:42:31.018552 celerity-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5469 2023-05-06 18:42:31.018552 celerity-0.6.0/README.md
+-rw-r--r--   0        0        0     1830 2023-05-06 18:42:31.018552 celerity-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/__init__.py
+-rw-r--r--   0        0        0     2501 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/astrometry.py
+-rw-r--r--   0        0        0      240 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/common.py
+-rw-r--r--   0        0        0      997 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/constants.py
+-rw-r--r--   0        0        0     1650 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/coordinates.py
+-rw-r--r--   0        0        0      628 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/earth.py
+-rw-r--r--   0        0        0      468 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/epoch.py
+-rw-r--r--   0        0        0      945 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/moon.py
+-rw-r--r--   0        0        0     2092 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/seeing.py
+-rw-r--r--   0        0        0     2789 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/sun.py
+-rw-r--r--   0        0        0     4129 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/temporal.py
+-rw-r--r--   0        0        0      961 2023-05-06 18:42:31.018552 celerity-0.6.0/src/celerity/utilities.py
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 celerity-0.6.0/PKG-INFO
```

### Comparing `celerity-0.5.0/LICENSE` & `celerity-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/README.md` & `celerity-0.6.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 )
 
 # Time of observation in UTC:
 time = Time(
     when=datetime(2021, 5, 14, 12, 0, 0, tzinfo=timezone.utc)
 )
 
-# Provide a Sky target in equatorial coordinates at epoch J2000:
+# Provide an equatorial target in equatorial coordinates at epoch J2000 in units of degrees:
 betelgeuse = { ra: 88.792938, dec: 7.407064 }
 
 # Observe the target:
 betelgeuse = observer.at(time).observe({ ra: 88.792938, dec: 7.407064 })
 
 # Get the horizontal coordinates:
 { alt, az } = betelgeuse.altAz()
@@ -63,14 +63,24 @@
 # What is the Local Sidereal Time at the time of observation?
 lst = observer.at(time).LST()
 
 # What is the Julian Date at the time of observation?
 jd = observer.at(time).JD()
 ```
 
+### Notes & Caveats
+
+Celerity is designed such that fundamental SI units of measurement are used, e.g., degrees, metres, seconds, etc. This is to ensure that the API is as accurate as possible, and that the user is aware of the units being used at all times.
+
+The `Observer` class requires the user to provide the latitude and longitude in degrees, and the elevation in metres. Latitude is positive for the northern hemisphere, and negative for the southern hemisphere between -90° at the southern pole and +90° at the northern pole. Longitude is always positive for the eastern hemisphere (east of the Prime Meridian), and negative for the western hemisphere (west of the Prime Meridian) representing a longitude between -180° and +180°.
+
+The `Time` class requires the user to provide the time in UTC, and not in any other timezone. The user can, once the `Time` object has been created, convert the time to any other timezone using the provided class methods.
+
+The `Target` class requires the user to provide the right ascension and declination in degrees (and not in hours and degrees).
+
 ---
 
 ## Package Development
 
 ### Project Requirements
 
 - [Python](https://www.python.org/) 3.11.*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `celerity-0.5.0/pyproject.toml` & `celerity-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celerity"
-version = "0.5.0"
+version = "0.6.0"
 description = "Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations."
 authors = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
 maintainers = [
     "Michael J. Roberts <michael@observerly.com>"
 ]
```

### Comparing `celerity-0.5.0/src/celerity/astrometry.py` & `celerity-0.6.0/src/celerity/astrometry.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/src/celerity/constants.py` & `celerity-0.6.0/src/celerity/constants.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/src/celerity/coordinates.py` & `celerity-0.6.0/src/celerity/coordinates.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/src/celerity/seeing.py` & `celerity-0.6.0/src/celerity/seeing.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/src/celerity/temporal.py` & `celerity-0.6.0/src/celerity/temporal.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/src/celerity/utilities.py` & `celerity-0.6.0/src/celerity/utilities.py`

 * *Files identical despite different names*

### Comparing `celerity-0.5.0/PKG-INFO` & `celerity-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celerity
-Version: 0.5.0
+Version: 0.6.0
 Summary: Celerity is a lightweight, zero-dependency and type-safe Python library for astronomical calculations.
 Home-page: https://github.com/michaelroberts/celerity
 Keywords: astronomy,astrometry,ephemeris
 Author: Michael J. Roberts
 Author-email: michael@observerly.com
 Maintainer: Michael J. Roberts
 Maintainer-email: michael@observerly.com
@@ -63,15 +63,15 @@
 )
 
 # Time of observation in UTC:
 time = Time(
     when=datetime(2021, 5, 14, 12, 0, 0, tzinfo=timezone.utc)
 )
 
-# Provide a Sky target in equatorial coordinates at epoch J2000:
+# Provide an equatorial target in equatorial coordinates at epoch J2000 in units of degrees:
 betelgeuse = { ra: 88.792938, dec: 7.407064 }
 
 # Observe the target:
 betelgeuse = observer.at(time).observe({ ra: 88.792938, dec: 7.407064 })
 
 # Get the horizontal coordinates:
 { alt, az } = betelgeuse.altAz()
@@ -79,14 +79,24 @@
 # What is the Local Sidereal Time at the time of observation?
 lst = observer.at(time).LST()
 
 # What is the Julian Date at the time of observation?
 jd = observer.at(time).JD()
 ```
 
+### Notes & Caveats
+
+Celerity is designed such that fundamental SI units of measurement are used, e.g., degrees, metres, seconds, etc. This is to ensure that the API is as accurate as possible, and that the user is aware of the units being used at all times.
+
+The `Observer` class requires the user to provide the latitude and longitude in degrees, and the elevation in metres. Latitude is positive for the northern hemisphere, and negative for the southern hemisphere between -90° at the southern pole and +90° at the northern pole. Longitude is always positive for the eastern hemisphere (east of the Prime Meridian), and negative for the western hemisphere (west of the Prime Meridian) representing a longitude between -180° and +180°.
+
+The `Time` class requires the user to provide the time in UTC, and not in any other timezone. The user can, once the `Time` object has been created, convert the time to any other timezone using the provided class methods.
+
+The `Target` class requires the user to provide the right ascension and declination in degrees (and not in hours and degrees).
+
 ---
 
 ## Package Development
 
 ### Project Requirements
 
 - [Python](https://www.python.org/) 3.11.*
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

