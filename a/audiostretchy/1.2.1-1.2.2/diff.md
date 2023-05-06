# Comparing `tmp/audiostretchy-1.2.1.tar.gz` & `tmp/audiostretchy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.2.1.tar", last modified: Sat May  6 15:03:43 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.2.tar", last modified: Sat May  6 15:15:26 2023, max compression
```

## Comparing `audiostretchy-1.2.1.tar` & `audiostretchy-1.2.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.222752 audiostretchy-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.226752 audiostretchy-1.2.1/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:03:42.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:03:43.000000 audiostretchy-1.2.1/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:03:43.230752 audiostretchy-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:03:31.000000 audiostretchy-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.081985 audiostretchy-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.081985 audiostretchy-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:15:25.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/conftest.py
```

### Comparing `audiostretchy-1.2.1/.coveragerc` & `audiostretchy-1.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/.github/workflows/ci.yaml` & `audiostretchy-1.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/.gitignore` & `audiostretchy-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/.pre-commit-config.yaml` & `audiostretchy-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/.readthedocs.yml` & `audiostretchy-1.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/LICENSE.txt` & `audiostretchy-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/PKG-INFO` & `audiostretchy-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.1
+Version: 1.2.2
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,49 +26,64 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.1
+Version: 1.2.2
 
 ## Features
 
-- Time stretching of audio files without changing their pitch
-- Supports WAV files, and optionally MP3 files
+- Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
-- Optional resampling
+- Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
+- With `[all]` installation, also supports resampling
 
 **Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
 The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
-### Simple installation
+### Full installation
 
 To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
-### Efficient installation
+This installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+This also installs optional dependencies: 
+
+- for MP3 support: [pydub](https://pypi.org/project/pydub/) on macOS, [pymp3](https://pypi.org/project/pymp3/) on Linux and Windows
+- for resampling: [soxr](https://pypi.org/project/soxr/)
+
+On macOS, you also need to install [HomeBrew](https://brew.sh/) and then in Terminal run: 
+
+```bash
+brew install ffmpeg
+```
+
+### Minimal installation
 
 To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
-### Development installation
+This only installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+### Full development installation
 
 To install the development version, use:
 
 ```
 python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
@@ -120,27 +135,27 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
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
-audio_stretch.resample(sample_rate=44100)
+audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.2.1/README.md` & `audiostretchy-1.2.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,61 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.1
+Version: 1.2.2
 
 ## Features
 
-- Time stretching of audio files without changing their pitch
-- Supports WAV files, and optionally MP3 files
+- Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
-- Optional resampling
+- Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
+- With `[all]` installation, also supports resampling
 
 **Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
 The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
-### Simple installation
+### Full installation
 
 To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
-### Efficient installation
+This installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+This also installs optional dependencies: 
+
+- for MP3 support: [pydub](https://pypi.org/project/pydub/) on macOS, [pymp3](https://pypi.org/project/pymp3/) on Linux and Windows
+- for resampling: [soxr](https://pypi.org/project/soxr/)
+
+On macOS, you also need to install [HomeBrew](https://brew.sh/) and then in Terminal run: 
+
+```bash
+brew install ffmpeg
+```
+
+### Minimal installation
 
 To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
-### Development installation
+This only installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+### Full development installation
 
 To install the development version, use:
 
 ```
 python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
@@ -92,27 +107,27 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
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
-audio_stretch.resample(sample_rate=44100)
+audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.2.1/docs/Makefile` & `audiostretchy-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/docs/conf.py` & `audiostretchy-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/docs/index.md` & `audiostretchy-1.2.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/setup.cfg` & `audiostretchy-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/setup.py` & `audiostretchy-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/__init__.py` & `audiostretchy-1.2.2/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.2/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.2/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.2/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.2/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy/stretch.py` & `audiostretchy-1.2.2/src/audiostretchy/stretch.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.2/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.1
+Version: 1.2.2
 Summary: AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. AudioStretchy is a wrapper around the audio-stretch C library by David Bryant.
 Home-page: https://github.com/twardoch/audiostretchy
 Author: Adam Twardoch
 Author-email: adam+github@twardoch.com
 License: BSD-3-Clause
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
@@ -26,49 +26,64 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.1
+Version: 1.2.2
 
 ## Features
 
-- Time stretching of audio files without changing their pitch
-- Supports WAV files, and optionally MP3 files
+- Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
-- Optional resampling
+- Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
+- With `[all]` installation, also supports resampling
 
 **Time-domain harmonic scaling (TDHS)** is a method for time-scale modification of speech (or other audio signals), allowing the apparent rate of speech articulation to be changed without affecting the pitch-contour and the time-evolution of the formant structure. TDHS differs from other time-scale modification algorithms in that time-scaling operations are performed in the time domain (not the frequency domain).
 
 The core functionality of this package is provided by David Bryant’s excellent [audio-stretch C library](https://github.com/dbry/audio-stretch) that performs fast, high-quality TDHS on WAV in the ratio range of 0.25 (4× slower) to 4.0 (4× faster). 
 
 The library gives very good results with speech recordings, especially with modest stretching at the ratio between 0.9 (10% slower) and 1.1 (10% faster). AudioStretchy is a Python wrapper around that library. The Python package also offers some additional, optional functionality: supports MP3 (in addition to WAV), and allows you to preform resampling.
 
 ## Installation
 
-### Simple installation
+### Full installation
 
 To be able to **stretch** and **resample** both **WAV** and **MP3** files, install AudioStretchy using `pip` like so:
 
 ```
 pip install audiostretchy[all]
 ```
 
-### Efficient installation
+This installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+This also installs optional dependencies: 
+
+- for MP3 support: [pydub](https://pypi.org/project/pydub/) on macOS, [pymp3](https://pypi.org/project/pymp3/) on Linux and Windows
+- for resampling: [soxr](https://pypi.org/project/soxr/)
+
+On macOS, you also need to install [HomeBrew](https://brew.sh/) and then in Terminal run: 
+
+```bash
+brew install ffmpeg
+```
+
+### Minimal installation
 
 To only be able to **stretch** **WAV** files (no resampling, no MP3 support), install AudioStretchy with minimal dependencies like so: 
 
 ```
 pip install audiostretchy
 ```
 
-### Development installation
+This only installs the package and the pre-compiled `audio-stretch` libraries for macOS, Windows and Linux. 
+
+### Full development installation
 
 To install the development version, use:
 
 ```
 python3 -m pip install git+https://github.com/twardoch/audiostretchy#egg=audiostretchy[all]
 ```
 
@@ -120,27 +135,27 @@
 
 For advanced usage, you can use the `AudioStretch` class that lets you open and save files provided as paths or as file-like BytesIO objects: 
 
 ```python
 from audiostretchy.stretch import AudioStretch
 
 audio_stretch = AudioStretch()
-audio_stretch.open(file=MP3DataAsBytesIO, format="mp3")
+audio_stretch.open(file=MP3DataAsBytesIO, format="mp3") # Needs [all] installation for MP3 support
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
-audio_stretch.resample(sample_rate=44100)
+audio_stretch.resample(sample_rate=44100) # Needs [all] installation for soxr support
 audio_stretch.save(file=WAVDataAsBytesIO, format="wav")
 ```
 
 
 ## License
 
 - [Original C library code](https://github.com/dbry/audio-stretch): Copyright (c) 2022 David Bryant
```

### Comparing `audiostretchy-1.2.1/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.2/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/tests/audio-1.2.mp3` & `audiostretchy-1.2.2/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/tests/audio-1.2.wav` & `audiostretchy-1.2.2/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/tests/audio.mp3` & `audiostretchy-1.2.2/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.1/tests/audio.wav` & `audiostretchy-1.2.2/tests/audio.wav`

 * *Files identical despite different names*

