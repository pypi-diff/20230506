# Comparing `tmp/convert_videos-2.8.2.tar.gz` & `tmp/convert_videos-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_videos-2.8.2.tar", max compression
+gzip compressed data, was "convert_videos-2.8.4.tar", max compression
```

## Comparing `convert_videos-2.8.2.tar` & `convert_videos-2.8.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-06 10:57:54.891562 convert_videos-2.8.2/LICENSE.md
--rw-r--r--   0        0        0     3432 2023-05-06 10:57:54.891562 convert_videos-2.8.2/README.md
--rwxr-xr-x   0        0        0      195 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/__init__.py
--rw-r--r--   0        0        0     4431 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/cli.py
--rw-r--r--   0        0        0      219 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/colour.py
--rw-r--r--   0        0        0     2400 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/ffmpeg_converter.py
--rw-r--r--   0        0        0     2195 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/processor.py
--rw-r--r--   0        0        0     4045 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/settings.py
--rw-r--r--   0        0        0     4655 2023-05-06 10:57:54.891562 convert_videos-2.8.2/convert_videos/video_processor.py
--rw-r--r--   0        0        0      870 2023-05-06 10:57:54.891562 convert_videos-2.8.2/pyproject.toml
--rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 convert_videos-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 11:21:46.786720 convert_videos-2.8.4/LICENSE.md
+-rw-r--r--   0        0        0     3432 2023-05-06 11:21:46.786720 convert_videos-2.8.4/README.md
+-rwxr-xr-x   0        0        0      195 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/__init__.py
+-rw-r--r--   0        0        0     4431 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/cli.py
+-rw-r--r--   0        0        0      219 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/colour.py
+-rw-r--r--   0        0        0     2400 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/ffmpeg_converter.py
+-rw-r--r--   0        0        0     2196 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/processor.py
+-rw-r--r--   0        0        0     4045 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/settings.py
+-rw-r--r--   0        0        0     4655 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/video_processor.py
+-rw-r--r--   0        0        0      870 2023-05-06 11:21:46.786720 convert_videos-2.8.4/pyproject.toml
+-rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 convert_videos-2.8.4/PKG-INFO
```

### Comparing `convert_videos-2.8.2/LICENSE.md` & `convert_videos-2.8.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/README.md` & `convert_videos-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/convert_videos/cli.py` & `convert_videos-2.8.4/convert_videos/cli.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/convert_videos/ffmpeg_converter.py` & `convert_videos-2.8.4/convert_videos/ffmpeg_converter.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/convert_videos/processor.py` & `convert_videos-2.8.4/convert_videos/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     force: bool
     video_settings: VideoSettings
     audio_settings: AudioSettings
     dry_run: bool = False
     in_place: bool = False
     extra_ffmpeg_input_args: str = ""
     extra_ffmpeg_output_args: str = ""
-    temp_directory: str = None # type: ignore
+    temp_directory: str = None  # type: ignore
     container: str = "mkv"
 
     def start(self):
         self._load_file_map()
         self._convert_all()
         return self.results
```

### Comparing `convert_videos-2.8.2/convert_videos/settings.py` & `convert_videos-2.8.4/convert_videos/settings.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/convert_videos/video_processor.py` & `convert_videos-2.8.4/convert_videos/video_processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.2/pyproject.toml` & `convert_videos-2.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert_videos"
-version = "2.8.2"
+version = "2.8.4"
 description = "This tool allows bulk conversion of videos using ffmpeg"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `convert_videos-2.8.2/PKG-INFO` & `convert_videos-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convert-videos
-Version: 2.8.2
+Version: 2.8.4
 Summary: This tool allows bulk conversion of videos using ffmpeg
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

