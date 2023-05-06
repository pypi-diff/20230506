# Comparing `tmp/audiostretchy-1.2.0.tar.gz` & `tmp/audiostretchy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.2.0.tar", last modified: Thu May  4 02:29:01 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.1.tar", last modified: Sat May  6 15:03:43 2023, max compression
```

## Comparing `audiostretchy-1.2.0.tar` & `audiostretchy-1.2.1.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.157647 audiostretchy-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.165648 audiostretchy-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-04 02:29:01.185648 audiostretchy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.157647 audiostretchy-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.173648 audiostretchy-1.2.0/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.177648 audiostretchy-1.2.0/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 02:29:00.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 02:29:01.000000 audiostretchy-1.2.0/src/audiostretchy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    99491 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/temp.mp3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 02:29:01.181648 audiostretchy-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-04 02:28:48.000000 audiostretchy-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:03:42.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/conftest.py
```

### Comparing `audiostretchy-1.2.0/.coveragerc` & `audiostretchy-1.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/.github/workflows/ci.yaml` & `audiostretchy-1.2.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/.gitignore` & `audiostretchy-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/.pre-commit-config.yaml` & `audiostretchy-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/.readthedocs.yml` & `audiostretchy-1.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/LICENSE.txt` & `audiostretchy-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/PKG-INFO` & `audiostretchy-1.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,40 @@
-Metadata-Version: 2.1
-Name: audiostretchy
-Version: 1.2.0
-Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
-Home-page: https://github.com/twardoch/audiostretchy
-Author: Adam Twardoch
-Author-email: adam+github@twardoch.com
-License: BSD-3-Clause
-Project-URL: Documentation, https://pyscaffold.org/
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: all
-Provides-Extra: testing
-License-File: LICENSE.txt
-
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.0
+Version: 1.2.1
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Optional resampling
 
-The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+**Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
-Time-domain harmonic scaling (TDHS) is a method for time-scale
-modification of speech (or other audio signals), allowing the apparent
-rate of speech articulation to be changed without affecting the
-pitch-contour and the time-evolution of the formant structure. TDHS
-differs from other time-scale modification algorithms in that
-time-scaling operations are performed in the time domain (not the
-frequency domain).
-
-This project is a Python wrapper around a a TDHS library to utilize it with standard WAV files. 
-
-There are two effects possible with TDHS and the audio-stretch demo. The
-first is the more obvious mentioned above of changing the duration (or
-speed) of a speech (or other audio) sample without modifying its pitch.
-The other effect is similar, but after applying the duration change we
-change the sampling rate in a complimentary manner to restore the original
-duration and timing, which then results in the pitch being altered.
-
-So when a ratio is supplied to the audio-stretch program, the default
-operation is for the total duration of the audio file to be scaled by
-exactly that ratio (0.5X to 2.0X), with the pitches remaining constant.
-If the option to scale the sample-rate proportionally is specified (-s)
-then the total duration and timing of the audio file will be preserved,
-but the pitches will be scaled by the specified ratio instead. This is
-useful for creating a "helium voice" effect and lots of other fun stuff.
-
-Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
-non-standard sampling rates will probably result. Many programs will still
-properly play these files, and audio editing programs will likely import
-them correctly (by resampling), but it is possible that some applications
-will barf on them. They can also be resampled to a standard rate using
-[audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
+The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
-_Note: The Python package does not expose all command-line options of the original library._
+The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
 ### Simple installation
 
-To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
+To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
 ### Efficient installation
 
-To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
-
+To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
 ### Development installation
 
@@ -97,51 +48,73 @@
 
 ### CLI
 
 ```
 audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INPUT_WAV
-    OUTPUT_WAV
+    INPUT_PATH
+        The path to the input WAV or MP3 audio file.
+    OUTPUT_PATH
+        The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        Default: 1.0
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        Default: 0.0
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
     -u, --upper_freq=UPPER_FREQ
-        Default: 333
+        The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
-        Default: 55
+        The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        Default: 25
+        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        Default: -40
+        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
     -d, --dual_force=DUAL_FORCE
-        Default: False
+        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
     -f, --fast_detection=FAST_DETECTION
-        Default: False
+        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        Default: False
+        If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        Default: 0
+        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
-stretch_audio("input.wav", "output.wav", ratio=ratio)
+stretch_audio("input.wav", "output.wav", ratio=1.1)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-For advanced usage, you can use the `AudioStretch` class (docs to be provided).
+For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
+
+```python
+from audiostretchy.stretch import AudioStretch
+
+audio_stretch = AudioStretch()
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.stretch(
+    ratio=1.1,
+    gap_ratio=1.2,
+    upper_freq=333,
+    lower_freq=55,
+    buffer_ms=25,
+    threshold_gap_db=-40,
+    dual_force=False,
+    fast_detection=False,
+    normal_detection=False,
+)
+audio_stretch.resample(sample_rate=44100)
+audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
+```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
 - Written with assistance from GPT-4
```

### Comparing `audiostretchy-1.2.0/README.md` & `audiostretchy-1.2.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,68 @@
+Metadata-Version: 2.1
+Name: audiostretchy
+Version: 1.2.1
+Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
+Home-page: https://github.com/twardoch/audiostretchy
+Author: Adam Twardoch
+Author-email: adam+github@twardoch.com
+License: BSD-3-Clause
+Project-URL: Documentation, https://pyscaffold.org/
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: all
+Provides-Extra: testing
+License-File: LICENSE.txt
+
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.0
+Version: 1.2.1
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Optional resampling
 
-The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+**Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
-Time-domain harmonic scaling (TDHS) is a method for time-scale
-modification of speech (or other audio signals), allowing the apparent
-rate of speech articulation to be changed without affecting the
-pitch-contour and the time-evolution of the formant structure. TDHS
-differs from other time-scale modification algorithms in that
-time-scaling operations are performed in the time domain (not the
-frequency domain).
-
-This project is a Python wrapper around a a TDHS library to utilize it with standard WAV files. 
-
-There are two effects possible with TDHS and the audio-stretch demo. The
-first is the more obvious mentioned above of changing the duration (or
-speed) of a speech (or other audio) sample without modifying its pitch.
-The other effect is similar, but after applying the duration change we
-change the sampling rate in a complimentary manner to restore the original
-duration and timing, which then results in the pitch being altered.
-
-So when a ratio is supplied to the audio-stretch program, the default
-operation is for the total duration of the audio file to be scaled by
-exactly that ratio (0.5X to 2.0X), with the pitches remaining constant.
-If the option to scale the sample-rate proportionally is specified (-s)
-then the total duration and timing of the audio file will be preserved,
-but the pitches will be scaled by the specified ratio instead. This is
-useful for creating a "helium voice" effect and lots of other fun stuff.
-
-Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
-non-standard sampling rates will probably result. Many programs will still
-properly play these files, and audio editing programs will likely import
-them correctly (by resampling), but it is possible that some applications
-will barf on them. They can also be resampled to a standard rate using
-[audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
+The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
-_Note: The Python package does not expose all command-line options of the original library._
+The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
 ### Simple installation
 
-To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
+To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
 ### Efficient installation
 
-To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
-
+To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
 ### Development installation
 
@@ -79,51 +76,73 @@
 
 ### CLI
 
 ```
 audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INPUT_WAV
-    OUTPUT_WAV
+    INPUT_PATH
+        The path to the input WAV or MP3 audio file.
+    OUTPUT_PATH
+        The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        Default: 1.0
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        Default: 0.0
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
     -u, --upper_freq=UPPER_FREQ
-        Default: 333
+        The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
-        Default: 55
+        The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        Default: 25
+        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        Default: -40
+        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
     -d, --dual_force=DUAL_FORCE
-        Default: False
+        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
     -f, --fast_detection=FAST_DETECTION
-        Default: False
+        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        Default: False
+        If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        Default: 0
+        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
-stretch_audio("input.wav", "output.wav", ratio=ratio)
+stretch_audio("input.wav", "output.wav", ratio=1.1)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-For advanced usage, you can use the `AudioStretch` class (docs to be provided).
+For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
+
+```python
+from audiostretchy.stretch import AudioStretch
+
+audio_stretch = AudioStretch()
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.stretch(
+    ratio=1.1,
+    gap_ratio=1.2,
+    upper_freq=333,
+    lower_freq=55,
+    buffer_ms=25,
+    threshold_gap_db=-40,
+    dual_force=False,
+    fast_detection=False,
+    normal_detection=False,
+)
+audio_stretch.resample(sample_rate=44100)
+audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
+```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
 - Written with assistance from GPT-4
```

### Comparing `audiostretchy-1.2.0/docs/Makefile` & `audiostretchy-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/docs/conf.py` & `audiostretchy-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/docs/index.md` & `audiostretchy-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/setup.cfg` & `audiostretchy-1.2.1/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [metadata]
 name = audiostretchy
-description = Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
+description = AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 author = Adam Twardoch
 author_email = adam+github@twardoch.com
 license = BSD-3-Clause
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/twardoch/audiostretchy
 project_urls = 
 	Documentation = https://pyscaffold.org/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
+	Operating System :: MacOS
+	Operating System :: Microsoft :: Windows
+	Operating System :: POSIX
+	Programming Language :: C
 	Programming Language :: Python
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Topic :: Multimedia :: Sound/Audio
+	Topic :: Multimedia :: Sound/Audio :: Conversion
+	Topic :: Multimedia :: Sound/Audio :: Speech
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
```

### Comparing `audiostretchy-1.2.0/setup.py` & `audiostretchy-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/__init__.py` & `audiostretchy-1.2.1/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.1/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.1/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.1/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.1/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/src/audiostretchy/stretch.py` & `audiostretchy-1.2.1/src/audiostretchy/stretch.py`

 * *Files 17% similar despite different names*

```diff
@@ -315,27 +315,54 @@
             )
 
         num_samples += stretcher.flush(self.samples[num_samples:])
         stretcher.deinit()
 
 
 def stretch_audio(
-    input_path,
-    output_path,
-    ratio=1.0,
-    gap_ratio=0.0,
-    upper_freq=333,
-    lower_freq=55,
-    buffer_ms=25,
-    threshold_gap_db=-40,
-    dual_force=False,
-    fast_detection=False,
-    normal_detection=False,
-    sample_rate=0,
-):
+    input_path: str,
+    output_path: str,
+    ratio: float = 1.0,
+    gap_ratio: float = 0.0,
+    upper_freq: int = 333,
+    lower_freq: int = 55,
+    buffer_ms: float = 25,
+    threshold_gap_db: float = -40,
+    dual_force: bool = False,
+    fast_detection: bool = False,
+    normal_detection: bool = False,
+    sample_rate: int = 0,
+    ):
+    """Stretches the input audio file and saves the result to the output path.
+
+Args:
+    input_path (str): The path to the input WAV or MP3 audio file.
+    output_path (str): The path to save the stretched WAV or MP3 audio file.
+    ratio (float, optional): The stretch ratio, where values greater than 1.0
+        will extend the audio and values less than 1.0 will shorten the audio.
+        Default is 1.0 = no stretching.
+    gap_ratio (float, optional): The stretch ratio for gaps (silence) in the audio.
+        Default is 0.0 = use ratio.
+    upper_freq (int, optional): The upper frequency limit for period detection in Hz.
+        Default is 333 Hz.
+    lower_freq (int, optional): The lower frequency limit. Default is 55 Hz.
+    buffer_ms (float, optional): The buffer size in milliseconds for processing
+        the audio in chunks. Default is 25 ms.
+    threshold_gap_db (float, optional): The threshold level in dB to
+        determine if a section of audio is considered a gap (silence). Default is -40 dB.
+    dual_force (bool, optional): If True, forces the algorithm to operate in
+        dual-force mode, which may improve the quality of the stretched audio
+        but may also increase processing time. 
+    fast_detection (bool, optional): If True, enables fast period detection,
+        which may speed up processing but reduce the quality of the stretched
+        audio. 
+    normal_detection (bool, optional): If True, forces the algorithm to use
+        normal period detection instead of fast period detection.
+    sample_rate (int, optional): The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
+"""
     audio_stretch = AudioStretch()
     audio_stretch.open(input_path)
     audio_stretch.stretch(
         ratio,
         gap_ratio,
         upper_freq,
         lower_freq,
```

### Comparing `audiostretchy-1.2.0/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.1/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,89 +1,68 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.0
-Summary: Wrapper around the audio-stretch C library to time-stretch WAV files without changing their pitch
+Version: 1.2.1
+Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: all
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
-AudioStretchy is a Python library that allows you to time-stretch audio signals without changing their pitch. It is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) library by David Bryant, which implements a sophisticated time-stretching algorithm for high-quality results. 
+AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.0
+Version: 1.2.1
 
 ## Features
 
 - Time stretching of audio files without changing their pitch
 - Supports WAV files, and optionally MP3 files
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Optional resampling
 
-The following explanation is adapted from the [original audio-stretch C library](https://github.com/dbry/audio-stretch): 
+**Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
-Time-domain harmonic scaling (TDHS) is a method for time-scale
-modification of speech (or other audio signals), allowing the apparent
-rate of speech articulation to be changed without affecting the
-pitch-contour and the time-evolution of the formant structure. TDHS
-differs from other time-scale modification algorithms in that
-time-scaling operations are performed in the time domain (not the
-frequency domain).
-
-This project is a Python wrapper around a a TDHS library to utilize it with standard WAV files. 
-
-There are two effects possible with TDHS and the audio-stretch demo. The
-first is the more obvious mentioned above of changing the duration (or
-speed) of a speech (or other audio) sample without modifying its pitch.
-The other effect is similar, but after applying the duration change we
-change the sampling rate in a complimentary manner to restore the original
-duration and timing, which then results in the pitch being altered.
-
-So when a ratio is supplied to the audio-stretch program, the default
-operation is for the total duration of the audio file to be scaled by
-exactly that ratio (0.5X to 2.0X), with the pitches remaining constant.
-If the option to scale the sample-rate proportionally is specified (-s)
-then the total duration and timing of the audio file will be preserved,
-but the pitches will be scaled by the specified ratio instead. This is
-useful for creating a "helium voice" effect and lots of other fun stuff.
-
-Note that unless ratios of exactly 0.5 or 2.0 are used with the -s option,
-non-standard sampling rates will probably result. Many programs will still
-properly play these files, and audio editing programs will likely import
-them correctly (by resampling), but it is possible that some applications
-will barf on them. They can also be resampled to a standard rate using
-[audio-resampler](https://github.com/dbry/audio-resampler) by David Bryant. 
+The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
-_Note: The Python package does not expose all command-line options of the original library._
+The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
 ### Simple installation
 
-To be able to stretch and resample WAV and MP3 files, install AudioStretchy using `pip` like so:
+To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
 ### Efficient installation
 
-To only be able to stretch WAV files, install AudioStretchy without dependencies like so: 
-
+To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
 ### Development installation
 
@@ -97,51 +76,73 @@
 
 ### CLI
 
 ```
 audiostretchy INPUT_WAV OUTPUT_WAV <flags>
 
 POSITIONAL ARGUMENTS
-    INPUT_WAV
-    OUTPUT_WAV
+    INPUT_PATH
+        The path to the input WAV or MP3 audio file.
+    OUTPUT_PATH
+        The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        Default: 1.0
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        Default: 0.0
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
     -u, --upper_freq=UPPER_FREQ
-        Default: 333
+        The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
-        Default: 55
+        The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        Default: 25
+        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        Default: -40
+        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
     -d, --dual_force=DUAL_FORCE
-        Default: False
+        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
     -f, --fast_detection=FAST_DETECTION
-        Default: False
+        If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
-        Default: False
+        If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        Default: 0
+        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
 
-stretch_audio("input.wav", "output.wav", ratio=ratio)
+stretch_audio("input.wav", "output.wav", ratio=1.1)
 ```
 
 In this example, the `input.wav` file will be time-stretched by a factor of 1.1, meaning it will be 10% longer, and the result will be saved in the `output.wav` file.
 
-For advanced usage, you can use the `AudioStretch` class (docs to be provided).
+For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
+
+```python
+from audiostretchy.stretch import AudioStretch
+
+audio_stretch = AudioStretch()
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.stretch(
+    ratio=1.1,
+    gap_ratio=1.2,
+    upper_freq=333,
+    lower_freq=55,
+    buffer_ms=25,
+    threshold_gap_db=-40,
+    dual_force=False,
+    fast_detection=False,
+    normal_detection=False,
+)
+audio_stretch.resample(sample_rate=44100)
+audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
+```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
 - [Python code](https://github.com/twardoch/audiostretchy): Copyright (c) 2023 Adam Twardoch
 - Written with assistance from GPT-4
```

### Comparing `audiostretchy-1.2.0/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.1/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 .readthedocs.yml
 AUTHORS.md
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-temp.mp3
 .github/workflows/ci.yaml
 docs/Makefile
 docs/authors.md
 docs/changelog.md
 docs/conf.py
 docs/contributing.md
 docs/index.md
```

### Comparing `audiostretchy-1.2.0/tests/audio-1.2.mp3` & `audiostretchy-1.2.1/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/tests/audio-1.2.wav` & `audiostretchy-1.2.1/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/tests/audio.mp3` & `audiostretchy-1.2.1/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.0/tests/audio.wav` & `audiostretchy-1.2.1/tests/audio.wav`

 * *Files identical despite different names*

