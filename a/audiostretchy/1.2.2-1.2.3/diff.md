# Comparing `tmp/audiostretchy-1.2.2.tar.gz` & `tmp/audiostretchy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostretchy-1.2.2.tar", last modified: Sat May  6 15:15:26 2023, max compression
+gzip compressed data, was "audiostretchy-1.2.3.tar", last modified: Sat May  6 15:28:17 2023, max compression
```

## Comparing `audiostretchy-1.2.2.tar` & `audiostretchy-1.2.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.081985 audiostretchy-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.081985 audiostretchy-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/src/audiostretchy/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/linux/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/linux/_stretch.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/mac/
--rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/mac/_stretch.dylib
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/tdhs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.089985 audiostretchy-1.2.2/src/audiostretchy/interface/win/
--rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/interface/win/_stretch.dll
--rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/src/audiostretchy/stretch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.085985 audiostretchy-1.2.2/src/audiostretchy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:15:25.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:15:26.000000 audiostretchy-1.2.2/src/audiostretchy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:15:26.093985 audiostretchy-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio-1.2.mp3
--rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio-1.2.wav
--rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio.mp3
--rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/audio.wav
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:15:08.000000 audiostretchy-1.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.513349 audiostretchy-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/linux/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22664 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/linux/_stretch.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    99483 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/mac/_stretch.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/tdhs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy/interface/win/
+-rw-r--r--   0 runner    (1001) docker     (123)   104960 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/interface/win/_stretch.dll
+-rw-r--r--   0 runner    (1001) docker     (123)    13000 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/src/audiostretchy/stretch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.517349 audiostretchy-1.2.3/src/audiostretchy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-06 15:28:17.000000 audiostretchy-1.2.3/src/audiostretchy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:28:17.521349 audiostretchy-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   198991 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio-1.2.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)  1091644 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio-1.2.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   132118 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)   723534 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/audio.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 15:28:02.000000 audiostretchy-1.2.3/tests/conftest.py
```

### Comparing `audiostretchy-1.2.2/.coveragerc` & `audiostretchy-1.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/.github/workflows/ci.yaml` & `audiostretchy-1.2.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/.gitignore` & `audiostretchy-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/.pre-commit-config.yaml` & `audiostretchy-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/.readthedocs.yml` & `audiostretchy-1.2.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/LICENSE.txt` & `audiostretchy-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/PKG-INFO` & `audiostretchy-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.2
+Version: 1.2.3
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
 
-Version: 1.2.2
+Version: 1.2.3
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -98,33 +98,33 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
-    -d, --dual_force=DUAL_FORCE
-        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
+        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+    -d, --double_range=DOUBLE_RANGE
+        If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
         If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
         If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
```

### Comparing `audiostretchy-1.2.2/README.md` & `audiostretchy-1.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AudioStretchy
 
 AudioStretchy is a Python library and CLI tool that which performs fast, high-quality time-stretching of WAV/MP3 files without changing their pitch. Works well for speech, can time-stretch silence separately. The library is a wrapper around David Bryant’s [audio-stretch](https://github.com/dbry/audio-stretch) C library. 
 
-Version: 1.2.2
+Version: 1.2.3
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -70,33 +70,33 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
-    -d, --dual_force=DUAL_FORCE
-        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
+        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+    -d, --double_range=DOUBLE_RANGE
+        If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
         If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
         If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
```

### Comparing `audiostretchy-1.2.2/docs/Makefile` & `audiostretchy-1.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/docs/conf.py` & `audiostretchy-1.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/docs/index.md` & `audiostretchy-1.2.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/setup.cfg` & `audiostretchy-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/setup.py` & `audiostretchy-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/__init__.py` & `audiostretchy-1.2.3/src/audiostretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/interface/linux/_stretch.so` & `audiostretchy-1.2.3/src/audiostretchy/interface/linux/_stretch.so`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/interface/mac/_stretch.dylib` & `audiostretchy-1.2.3/src/audiostretchy/interface/mac/_stretch.dylib`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/interface/tdhs.py` & `audiostretchy-1.2.3/src/audiostretchy/interface/tdhs.py`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/interface/win/_stretch.dll` & `audiostretchy-1.2.3/src/audiostretchy/interface/win/_stretch.dll`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/src/audiostretchy/stretch.py` & `audiostretchy-1.2.3/src/audiostretchy/stretch.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,42 +237,42 @@
         self,
         ratio: float = 1.0,
         gap_ratio: float = 0.0,
         upper_freq: int = 333,
         lower_freq: int = 55,
         buffer_ms: float = 25,
         threshold_gap_db: float = -40,
-        dual_force: bool = False,
+        double_range: bool = False,
         fast_detection: bool = False,
         normal_detection: bool = False,
     ):
         """
         Stretch the audio.
 
         Args:
             ratio (float): Stretch ratio. Defaults to 1.0.
             gap_ratio (float): Gap ratio. Defaults to 0.0.
             upper_freq (int): Upper frequency limit. Defaults to 333.
             lower_freq (int): Lower frequency limit. Defaults to 55.
             buffer_ms (float): Buffer size in milliseconds. Defaults to 25.
             threshold_gap_db (float): Threshold gap in dB. Defaults to -40.
-            dual_force (bool): Flag for dual force. Defaults to False.
+            double_range (bool): Flag for dual force. Defaults to False.
             fast_detection (bool): Flag for fast detection. Defaults to False.
             normal_detection (bool): Flag for normal detection. Defaults to False.
         """
         gap_ratio = gap_ratio or ratio
         flags = 0
         silence_mode = gap_ratio and gap_ratio != ratio
         buffer_samples = int(self.framerate * (buffer_ms / 1e3))
         min_period = self.framerate // upper_freq
         max_period = self.framerate // lower_freq
         max_ratio = ratio
 
         if (
-            dual_force
+            double_range
             or ratio < 0.5
             or ratio > 2.0
             or (silence_mode and (gap_ratio < 0.5 or gap_ratio > 2.0))
         ):
             flags |= TDHSAudioStretch.STRETCH_DUAL_FLAG
 
         if (fast_detection or self.framerate >= 32000) and not normal_detection:
@@ -323,54 +323,43 @@
     output_path: str,
     ratio: float = 1.0,
     gap_ratio: float = 0.0,
     upper_freq: int = 333,
     lower_freq: int = 55,
     buffer_ms: float = 25,
     threshold_gap_db: float = -40,
-    dual_force: bool = False,
+    double_range: bool = False,
     fast_detection: bool = False,
     normal_detection: bool = False,
     sample_rate: int = 0,
     ):
     """Stretches the input audio file and saves the result to the output path.
 
 Args:
     input_path (str): The path to the input WAV or MP3 audio file.
     output_path (str): The path to save the stretched WAV or MP3 audio file.
-    ratio (float, optional): The stretch ratio, where values greater than 1.0
-        will extend the audio and values less than 1.0 will shorten the audio.
-        Default is 1.0 = no stretching.
-    gap_ratio (float, optional): The stretch ratio for gaps (silence) in the audio.
-        Default is 0.0 = use ratio.
-    upper_freq (int, optional): The upper frequency limit for period detection in Hz.
-        Default is 333 Hz.
+    ratio (float, optional): The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
+    gap_ratio (float, optional): The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
+    upper_freq (int, optional): The upper frequency limit for period detection in Hz. Default is 333 Hz.
     lower_freq (int, optional): The lower frequency limit. Default is 55 Hz.
-    buffer_ms (float, optional): The buffer size in milliseconds for processing
-        the audio in chunks. Default is 25 ms.
-    threshold_gap_db (float, optional): The threshold level in dB to
-        determine if a section of audio is considered a gap (silence). Default is -40 dB.
-    dual_force (bool, optional): If True, forces the algorithm to operate in
-        dual-force mode, which may improve the quality of the stretched audio
-        but may also increase processing time. 
-    fast_detection (bool, optional): If True, enables fast period detection,
-        which may speed up processing but reduce the quality of the stretched
-        audio. 
-    normal_detection (bool, optional): If True, forces the algorithm to use
-        normal period detection instead of fast period detection.
-    sample_rate (int, optional): The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
+    buffer_ms (float, optional): The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
+    threshold_gap_db (float, optional): The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+    double_range (bool, optional): If set, doubles the min/max range of stretching from 0.5-2.0 to 0.25-4.0. 
+    fast_detection (bool, optional): If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio. 
+    normal_detection (bool, optional): If set, forces the algorithm to use normal period detection instead of fast period detection.
+    sample_rate (int, optional): The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
 """
     audio_stretch = AudioStretch()
     audio_stretch.open(input_path)
     audio_stretch.stretch(
         ratio,
         gap_ratio,
         upper_freq,
         lower_freq,
         buffer_ms,
         threshold_gap_db,
-        dual_force,
+        double_range,
         fast_detection,
         normal_detection,
     )
     audio_stretch.resample(sample_rate)
     audio_stretch.save(output_path)
```

### Comparing `audiostretchy-1.2.2/src/audiostretchy.egg-info/PKG-INFO` & `audiostretchy-1.2.3/src/audiostretchy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiostretchy
-Version: 1.2.2
+Version: 1.2.3
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
 
-Version: 1.2.2
+Version: 1.2.3
 
 ## Features
 
 - Fast, high-quality time stretching of audio files without changing their pitch
 - Adjustable stretching ratio from 0.25 to 4.0
 - Cross-platform: Windows, macOS, and Linux
 - Supports WAV files and file-like objects. With `[all]` installation, also supports MP3 files and file-like objects
@@ -98,33 +98,33 @@
     INPUT_PATH
         The path to the input WAV or MP3 audio file.
     OUTPUT_PATH
         The path to save the stretched WAV or MP3 audio file.
 
 FLAGS
     -r, --ratio=RATIO
-        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. Default is 1.0 = no stretching.
+        The stretch ratio, where values greater than 1.0 will extend the audio and values less than 1.0 will shorten the audio. From 0.5 to 2.0, or with `-d` from 0.25 to 4.0. Default is 1.0 = no stretching.
     -g, --gap_ratio=GAP_RATIO
-        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = use ratio.
+        The stretch ratio for gaps (silence) in the audio. Default is 0.0 = uses ratio.
     -u, --upper_freq=UPPER_FREQ
         The upper frequency limit for period detection in Hz. Default is 333 Hz.
     -l, --lower_freq=LOWER_FREQ
         The lower frequency limit. Default is 55 Hz.
     -b, --buffer_ms=BUFFER_MS
-        The buffer size in milliseconds for processing the audio in chunks. Default is 25 ms.
+        The buffer size in milliseconds for processing the audio in chunks (useful with `-g`). Default is 25 ms.
     -t, --threshold_gap_db=THRESHOLD_GAP_DB
-        The threshold level in dB to determine if a section of audio is considered a gap (silence). Default is -40 dB.
-    -d, --dual_force=DUAL_FORCE
-        If set, forces the algorithm to operate in dual-force mode, which may improve the quality of the stretched audio but may also increase processing time.
+        The threshold level in dB to determine if a section of audio is considered a gap (for `-g`). Default is -40 dB.
+    -d, --double_range=DOUBLE_RANGE
+        If set, doubles the min/max range of stretching.
     -f, --fast_detection=FAST_DETECTION
         If set, enables fast period detection, which may speed up processing but reduce the quality of the stretched audio.
     -n, --normal_detection=NORMAL_DETECTION
         If set, forces the algorithm to use normal period detection instead of fast period detection.
     -s, --sample_rate=SAMPLE_RATE
-        The target sample rate for resampling the stretched audio in Hz. Default is 0 = use sample rate of the input audio.
+        The target sample rate for resampling the stretched audio in Hz (if installed with `[all]`). Default is 0 = use sample rate of the input audio.
 ```
 
 ### Python
 
 ```python
 from audiostretchy.stretch import stretch_audio
```

### Comparing `audiostretchy-1.2.2/src/audiostretchy.egg-info/SOURCES.txt` & `audiostretchy-1.2.3/src/audiostretchy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/tests/audio-1.2.mp3` & `audiostretchy-1.2.3/tests/audio-1.2.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/tests/audio-1.2.wav` & `audiostretchy-1.2.3/tests/audio-1.2.wav`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/tests/audio.mp3` & `audiostretchy-1.2.3/tests/audio.mp3`

 * *Files identical despite different names*

### Comparing `audiostretchy-1.2.2/tests/audio.wav` & `audiostretchy-1.2.3/tests/audio.wav`

 * *Files identical despite different names*

