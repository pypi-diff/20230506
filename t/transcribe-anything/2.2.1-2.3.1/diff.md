# Comparing `tmp/transcribe-anything-2.2.1.tar.gz` & `tmp/transcribe-anything-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.2.1.tar", last modified: Fri May  5 19:05:17 2023, max compression
+gzip compressed data, was "transcribe-anything-2.3.1.tar", last modified: Fri May  5 22:25:29 2023, max compression
```

## Comparing `transcribe-anything-2.2.1.tar` & `transcribe-anything-2.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:05:17.903830 transcribe-anything-2.2.1/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.2.1/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8906 2023-05-05 19:05:17.903830 transcribe-anything-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     7886 2023-05-05 19:00:45.000000 transcribe-anything-2.2.1/README.md
--rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.2.1/requirements.testing.txt
--rw-rw-rw-   0        0        0       63 2023-03-20 23:48:49.000000 transcribe-anything-2.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:05:17.904831 transcribe-anything-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     3109 2023-05-05 19:01:03.000000 transcribe-anything-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:05:17.876832 transcribe-anything-2.2.1/tests/
--rw-rw-rw-   0        0        0     2794 2023-05-05 18:57:48.000000 transcribe-anything-2.2.1/tests/test_transcribe_anything.py
--rw-rw-rw-   0        0        0      449 2022-12-01 20:48:45.000000 transcribe-anything-2.2.1/tests/test_whisper.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:05:17.885830 transcribe-anything-2.2.1/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.2.1/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     4868 2023-05-05 18:59:22.000000 transcribe-anything-2.2.1/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.2.1/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     2836 2023-03-20 23:48:49.000000 transcribe-anything-2.2.1/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.2.1/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.2.1/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1532 2022-12-09 00:33:26.000000 transcribe-anything-2.2.1/transcribe_anything/util.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:05:17.902831 transcribe-anything-2.2.1/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0     8906 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 19:05:17.000000 transcribe-anything-2.2.1/transcribe_anything.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.626948 transcribe-anything-2.3.1/
+-rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9009 2023-05-05 22:25:29.626948 transcribe-anything-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7987 2023-05-05 22:23:57.000000 transcribe-anything-2.3.1/README.md
+-rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/requirements.testing.txt
+-rw-rw-rw-   0        0        0       71 2023-05-05 22:22:57.000000 transcribe-anything-2.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 22:25:29.627948 transcribe-anything-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     3109 2023-05-05 22:23:40.000000 transcribe-anything-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.594457 transcribe-anything-2.3.1/tests/
+-rw-rw-rw-   0        0        0     2794 2023-05-05 18:57:48.000000 transcribe-anything-2.3.1/tests/test_transcribe_anything.py
+-rw-rw-rw-   0        0        0      449 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/tests/test_whisper.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.602431 transcribe-anything-2.3.1/transcribe_anything/
+-rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.3.1/transcribe_anything/__init__.py
+-rw-rw-rw-   0        0        0     4868 2023-05-05 18:59:22.000000 transcribe-anything-2.3.1/transcribe_anything/api.py
+-rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.3.1/transcribe_anything/audio.py
+-rw-rw-rw-   0        0        0     2836 2023-05-05 22:22:52.000000 transcribe-anything-2.3.1/transcribe_anything/cmd.py
+-rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.3.1/transcribe_anything/logger.py
+-rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.3.1/transcribe_anything/parse_whisper_options.py
+-rw-rw-rw-   0        0        0     1532 2022-12-09 00:33:26.000000 transcribe-anything-2.3.1/transcribe_anything/util.py
+drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.625426 transcribe-anything-2.3.1/transcribe_anything.egg-info/
+-rw-rw-rw-   0        0        0     9009 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      614 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.2.1/LICENSE` & `transcribe-anything-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/PKG-INFO` & `transcribe-anything-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.2.1
+Version: 2.3.1
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -163,14 +163,16 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
```

### Comparing `transcribe-anything-2.2.1/README.md` & `transcribe-anything-2.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,16 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
```

### Comparing `transcribe-anything-2.2.1/setup.py` & `transcribe-anything-2.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "2.2.1"
+VERSION = "2.3.1"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
```

### Comparing `transcribe-anything-2.2.1/tests/test_transcribe_anything.py` & `transcribe-anything-2.3.1/tests/test_transcribe_anything.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/api.py` & `transcribe-anything-2.3.1/transcribe_anything/api.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/audio.py` & `transcribe-anything-2.3.1/transcribe_anything/audio.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/cmd.py` & `transcribe-anything-2.3.1/transcribe_anything/cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/logger.py` & `transcribe-anything-2.3.1/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.3.1/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything/util.py` & `transcribe-anything-2.3.1/transcribe_anything/util.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.2.1/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.3.1/transcribe_anything.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.2.1
+Version: 2.3.1
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -163,14 +163,16 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
   * 2.0.13: Now works with python 3.9
   * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
```

### Comparing `transcribe-anything-2.2.1/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.3.1/transcribe_anything.egg-info/SOURCES.txt`

 * *Files identical despite different names*

