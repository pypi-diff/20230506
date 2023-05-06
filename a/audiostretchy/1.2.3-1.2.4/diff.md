# Comparing `tmp/audiostretchy-1.2.3.tar.gz` & `tmp/audiostretchy-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.2.3.tar", last modified: Sat May  6 15:28:17 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.4.tar", last modified: Sat May  6 15:32:39 2023, max compression
```

## Comparing `audiostretchy-1.2.3.tar` & `audiostretchy-1.2.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.586869 audiostretchy-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.578869 audiostretchy-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.578869 audiostretchy-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-06 15:32:39.586869 audiostretchy-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.578869 audiostretchy-1.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.578869 audiostretchy-1.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:32:39.586869 audiostretchy-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.578869 audiostretchy-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.582869 audiostretchy-1.2.4/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7264 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:32:39.000000 audiostretchy-1.2.4/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:32:39.586869 audiostretchy-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:32:28.000000 audiostretchy-1.2.4/tests/conftest.py
```

### Comparing `audiostretchy-1.2.3/.coveragerc` & `audiostretchy-1.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/.github/workflows/ci.yaml` & `audiostretchy-1.2.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/.gitignore` & `audiostretchy-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/.pre-commit-config.yaml` & `audiostretchy-1.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/.readthedocs.yml` & `audiostretchy-1.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/LICENSE.txt` & `audiostretchy-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/PKG-INFO` & `audiostretchy-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.3
+Version: 1.2.4
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.3
+_Version: **1.2.4**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -98,33 +98,41 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and 
+        values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` 
+        from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
+        The stretch ratio for gaps (silence) in the audio. 
+        Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks 
+        (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+        The threshold level in dB to determine if a section of audio is considered 
+        a gap (for `-g`). Default is -40 dB.
     -d, --double_range=DOUBLE_RANGE
         If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
-        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
+        If set, enables fast period detection, which may speed up processing but 
+        reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        If set, forces the algorithm to use normal period detection instead of fast period detection.
+        If set, forces the algorithm to use normal period detection instead 
+        of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed 
+        with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
@@ -135,30 +143,32 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
+# This needs [all] installation for MP3 support
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") 
 audio_stretch.stretch(
     ratio=1.1,
     gap_ratio=1.2,
     upper_freq=333,
     lower_freq=55,
     buffer_ms=25,
     threshold_gap_db=-40,
     dual_force=False,
     fast_detection=False,
     normal_detection=False,
 )
-audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
+# This needs [all] installation for soxr support
+audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
-- Written with assistance from GPT-4
+- Python code written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

### Comparing `audiostretchy-1.2.3/README.md` & `audiostretchy-1.2.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.3
+_Version: **1.2.4**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -70,33 +70,41 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and 
+        values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` 
+        from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
+        The stretch ratio for gaps (silence) in the audio. 
+        Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks 
+        (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+        The threshold level in dB to determine if a section of audio is considered 
+        a gap (for `-g`). Default is -40 dB.
     -d, --double_range=DOUBLE_RANGE
         If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
-        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
+        If set, enables fast period detection, which may speed up processing but 
+        reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        If set, forces the algorithm to use normal period detection instead of fast period detection.
+        If set, forces the algorithm to use normal period detection instead 
+        of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed 
+        with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
@@ -107,30 +115,32 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
+# This needs [all] installation for MP3 support
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") 
 audio_stretch.stretch(
     ratio=1.1,
     gap_ratio=1.2,
     upper_freq=333,
     lower_freq=55,
     buffer_ms=25,
     threshold_gap_db=-40,
     dual_force=False,
     fast_detection=False,
     normal_detection=False,
 )
-audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
+# This needs [all] installation for soxr support
+audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
-- Written with assistance from GPT-4
+- Python code written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

### Comparing `audiostretchy-1.2.3/docs/Makefile` & `audiostretchy-1.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/docs/conf.py` & `audiostretchy-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/docs/index.md` & `audiostretchy-1.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/setup.cfg` & `audiostretchy-1.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/setup.py` & `audiostretchy-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/__init__.py` & `audiostretchy-1.2.4/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.4/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.4/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.4/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.4/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy/stretch.py` & `audiostretchy-1.2.4/src/audiostretchy/stretch.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.4/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.3
+Version: 1.2.4
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,15 +26,15 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.3
+_Version: **1.2.4**_
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -98,33 +98,41 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and 
+        values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` 
+        from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
+        The stretch ratio for gaps (silence) in the audio. 
+        Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks 
+        (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+        The threshold level in dB to determine if a section of audio is considered 
+        a gap (for `-g`). Default is -40 dB.
     -d, --double_range=DOUBLE_RANGE
         If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
-        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
+        If set, enables fast period detection, which may speed up processing but 
+        reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        If set, forces the algorithm to use normal period detection instead of fast period detection.
+        If set, forces the algorithm to use normal period detection instead 
+        of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed 
+        with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
@@ -135,30 +143,32 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
+# This needs [all] installation for MP3 support
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") 
 audio_stretch.stretch(
     ratio=1.1,
     gap_ratio=1.2,
     upper_freq=333,
     lower_freq=55,
     buffer_ms=25,
     threshold_gap_db=-40,
     dual_force=False,
     fast_detection=False,
     normal_detection=False,
 )
-audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
+# This needs [all] installation for soxr support
+audio_stretch.resample(sample_rate=44100) 
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
-- Written with assistance from GPT-4
+- Python code written with assistance from GPT-4
 - Licensed under the [BSD-3-Clause license](./LICENSE.txt)
```

### Comparing `audiostretchy-1.2.3/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.4/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/tests/audio-1.2.mp3` & `audiostretchy-1.2.4/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/tests/audio-1.2.wav` & `audiostretchy-1.2.4/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/tests/audio.mp3` & `audiostretchy-1.2.4/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.3/tests/audio.wav` & `audiostretchy-1.2.4/tests/audio.wav`

 * *Files identical despite different names*

