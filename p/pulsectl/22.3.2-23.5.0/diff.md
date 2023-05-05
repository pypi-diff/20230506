# Comparing `tmp/pulsectl-22.3.2.tar.gz` & `tmp/pulsectl-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-22.3.2.tar", last modified: Wed Mar 23 05:41:12 2022, max compression
+gzip compressed data, was "pulsectl-23.5.0.tar", last modified: Fri May  5 23:09:06 2023, max compression
```

## Comparing `pulsectl-22.3.2.tar` & `pulsectl-23.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2022-03-23 05:41:12.046604 pulsectl-22.3.2/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2022-03-23 05:40:50.000000 pulsectl-22.3.2/CHANGES.rst
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-22.3.2/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-22.3.2/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17267 2022-03-23 05:41:12.046604 pulsectl-22.3.2/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16392 2021-09-07 20:03:51.000000 pulsectl-22.3.2/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2022-03-23 05:41:12.044604 pulsectl-22.3.2/pulsectl/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-22.3.2/pulsectl/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22448 2021-10-12 22:03:30.000000 pulsectl-22.3.2/pulsectl/_pulsectl.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-22.3.2/pulsectl/lookup.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41085 2022-03-23 05:38:51.000000 pulsectl-22.3.2/pulsectl/pulsectl.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2022-03-23 05:41:12.045604 pulsectl-22.3.2/pulsectl/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-22.3.2/pulsectl/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-01-23 00:56:34.000000 pulsectl-22.3.2/pulsectl/tests/test_with_dummy_instance.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2022-03-23 05:41:12.045604 pulsectl-22.3.2/pulsectl.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17267 2022-03-23 05:41:11.000000 pulsectl-22.3.2/pulsectl.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2022-03-23 05:41:11.000000 pulsectl-22.3.2/pulsectl.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2022-03-23 05:41:11.000000 pulsectl-22.3.2/pulsectl.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2022-03-23 05:41:11.000000 pulsectl-22.3.2/pulsectl.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2022-03-23 05:41:12.047603 pulsectl-22.3.2/setup.cfg
--rw-------   0 fraggod   (1000) fraggod   (1000)     1247 2022-03-23 05:40:26.000000 pulsectl-22.3.2/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 23:09:06.527477 pulsectl-23.5.0/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2179 2022-03-23 05:40:50.000000 pulsectl-23.5.0/CHANGES.rst
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1123 2017-07-13 10:23:26.000000 pulsectl-23.5.0/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       39 2021-02-25 10:54:47.000000 pulsectl-23.5.0/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-05 23:09:06.527477 pulsectl-23.5.0/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16561 2023-05-05 23:05:28.000000 pulsectl-23.5.0/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 23:09:06.527477 pulsectl-23.5.0/pulsectl/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      665 2022-01-22 20:05:43.000000 pulsectl-23.5.0/pulsectl/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    22483 2023-05-05 23:00:11.000000 pulsectl-23.5.0/pulsectl/_pulsectl.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     4385 2018-04-23 16:48:50.000000 pulsectl-23.5.0/pulsectl/lookup.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    41085 2023-05-05 23:00:23.000000 pulsectl-23.5.0/pulsectl/pulsectl.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 23:09:06.527477 pulsectl-23.5.0/pulsectl/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2017-07-13 10:23:26.000000 pulsectl-23.5.0/pulsectl/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    25645 2022-04-09 14:42:09.000000 pulsectl-23.5.0/pulsectl/tests/test_with_dummy_instance.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 23:09:06.527477 pulsectl-23.5.0/pulsectl.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17416 2023-05-05 23:09:06.000000 pulsectl-23.5.0/pulsectl.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      342 2023-05-05 23:09:06.000000 pulsectl-23.5.0/pulsectl.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 23:09:06.000000 pulsectl-23.5.0/pulsectl.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        9 2023-05-05 23:09:06.000000 pulsectl-23.5.0/pulsectl.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2023-05-05 23:09:06.527477 pulsectl-23.5.0/setup.cfg
+-rw-------   0 fraggod   (1000) fraggod   (1000)     1247 2023-05-05 23:01:55.000000 pulsectl-23.5.0/setup.py
```

### Comparing `pulsectl-22.3.2/CHANGES.rst` & `pulsectl-23.5.0/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `pulsectl-22.3.2/COPYING` & `pulsectl-23.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `pulsectl-22.3.2/PKG-INFO` & `pulsectl-23.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 22.3.2
+Version: 23.5.0
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -39,14 +38,20 @@
 .. _pulsemixer: https://github.com/GeorgeFilipkin/pulsemixer/
 
 |
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/python-pulse-control
+- https://codeberg.org/mk-fg/python-pulse-control
+- https://fraggod.net/code/git/python-pulse-control
+
 
 
 Usage
 -----
 
 Simple example::
 
@@ -443,9 +448,7 @@
 
   Branches there have bindings for different (newer) pulseaudio versions.
 
 * `pypulseaudio <https://github.com/liamw9534/pypulseaudio/>`_ -
   high-level bindings module, rather similar to this one.
 
 * `pulseaudio-mixer-cli`_ - alsamixer-like script built on top of this module.
-
-
```

### Comparing `pulsectl-22.3.2/README.rst` & `pulsectl-23.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 .. _pulsemixer: https://github.com/GeorgeFilipkin/pulsemixer/
 
 |
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/python-pulse-control
+- https://codeberg.org/mk-fg/python-pulse-control
+- https://fraggod.net/code/git/python-pulse-control
+
 
 
 Usage
 -----
 
 Simple example::
```

### Comparing `pulsectl-22.3.2/pulsectl/__init__.py` & `pulsectl-23.5.0/pulsectl/__init__.py`

 * *Files identical despite different names*

### Comparing `pulsectl-22.3.2/pulsectl/_pulsectl.py` & `pulsectl-23.5.0/pulsectl/_pulsectl.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 PA_SUBSCRIPTION_EVENT_CARD = 0x0009
 PA_SUBSCRIPTION_EVENT_FACILITY_MASK = 0x000F
 PA_SUBSCRIPTION_EVENT_NEW = 0x0000
 PA_SUBSCRIPTION_EVENT_CHANGE = 0x0010
 PA_SUBSCRIPTION_EVENT_REMOVE = 0x0020
 PA_SUBSCRIPTION_EVENT_TYPE_MASK = 0x0030
 
-PA_SAMPLE_FLOAT32BE = 5
+PA_SAMPLE_FLOAT32NE = dict(little=5, big=6)[sys.byteorder]
 
 PA_STREAM_DONT_MOVE = 0x0200
 PA_STREAM_PEAK_DETECT = 0x0800
 PA_STREAM_ADJUST_LATENCY = 0x2000
 PA_STREAM_DONT_INHIBIT_AUTO_SUSPEND = 0x8000
 
 def c_enum_map(**values):
```

### Comparing `pulsectl-22.3.2/pulsectl/lookup.py` & `pulsectl-23.5.0/pulsectl/lookup.py`

 * *Files identical despite different names*

### Comparing `pulsectl-22.3.2/pulsectl/pulsectl.py` & `pulsectl-23.5.0/pulsectl/pulsectl.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,25 +860,25 @@
 
 
 	def get_peak_sample(self, source, timeout, stream_idx=None):
 		'''Returns peak (max) value in 0-1.0 range for samples in source/stream within timespan.
 			"source" can be either int index of pulseaudio source
 				(i.e. source.index), its name (source.name), or None to use default source.
 			Resulting value is what pulseaudio returns as
-				PA_SAMPLE_FLOAT32BE float after "timeout" seconds.
+				PA_SAMPLE_FLOAT32NE float after "timeout" seconds.
 			If specified source does not exist, 0 should be returned after timeout.
 			This can be used to detect if there's any sound
 				on the microphone or any sound played through a sink via its monitor_source index,
 				or same for any specific stream connected to these (if "stream_idx" is passed).
 			Sample stream masquerades as
 				application.id=org.PulseAudio.pavucontrol to avoid being listed in various mixer apps.
 			Example - get peak for specific sink input "si" for 0.8 seconds:
 				pulse.get_peak_sample(pulse.sink_info(si.sink).monitor_source, 0.8, si.index)'''
 		samples, proplist = [0], c.pa.proplist_from_string('application.id=org.PulseAudio.pavucontrol')
-		ss = c.PA_SAMPLE_SPEC(format=c.PA_SAMPLE_FLOAT32BE, rate=25, channels=1)
+		ss = c.PA_SAMPLE_SPEC(format=c.PA_SAMPLE_FLOAT32NE, rate=25, channels=1)
 		s = c.pa.stream_new_with_proplist(self._ctx, 'peak detect', c.byref(ss), None, proplist)
 		c.pa.proplist_free(proplist)
 
 		@c.PA_STREAM_REQUEST_CB_T
 		def read_cb(s, bs, userdata):
 			buff, bs = c.c_void_p(), c.c_int(bs)
 			c.pa.stream_peek(s, buff, c.byref(bs))
```

### Comparing `pulsectl-22.3.2/pulsectl/tests/test_with_dummy_instance.py` & `pulsectl-23.5.0/pulsectl/tests/test_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-22.3.2/pulsectl.egg-info/PKG-INFO` & `pulsectl-23.5.0/pulsectl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pulsectl
-Version: 22.3.2
+Version: 23.5.0
 Summary: Python high-level interface and ctypes-based bindings for PulseAudio (libpulse)
 Home-page: http://github.com/mk-fg/python-pulse-control
 Author: George Filipkin, Mike Kazantsev
 Author-email: mk.fraggod@gmail.com
 License: MIT
 Keywords: pulseaudio,libpulse,pulse,pa,bindings,sound,audio,ctypes,control,mixer,volume,mute,source,sink
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
@@ -39,14 +38,20 @@
 .. _pulsemixer: https://github.com/GeorgeFilipkin/pulsemixer/
 
 |
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/python-pulse-control
+- https://codeberg.org/mk-fg/python-pulse-control
+- https://fraggod.net/code/git/python-pulse-control
+
 
 
 Usage
 -----
 
 Simple example::
 
@@ -443,9 +448,7 @@
 
   Branches there have bindings for different (newer) pulseaudio versions.
 
 * `pypulseaudio <https://github.com/liamw9534/pypulseaudio/>`_ -
   high-level bindings module, rather similar to this one.
 
 * `pulseaudio-mixer-cli`_ - alsamixer-like script built on top of this module.
-
-
```

### Comparing `pulsectl-22.3.2/setup.py` & `pulsectl-23.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	readme = open(os.path.join(
 		os.path.dirname(__file__), 'README.rst' )).read()
 except IOError: readme = ''
 
 setup(
 
 	name = 'pulsectl',
-	version = '22.3.2',
+	version = '23.5.0',
 	author = 'George Filipkin, Mike Kazantsev',
 	author_email = 'mk.fraggod@gmail.com',
 	license = 'MIT',
 	keywords = [
 		'pulseaudio', 'libpulse', 'pulse', 'pa', 'bindings',
 		'sound', 'audio',
 		'ctypes', 'control', 'mixer', 'volume', 'mute', 'source', 'sink' ],
```

