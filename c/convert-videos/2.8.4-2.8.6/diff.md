# Comparing `tmp/convert_videos-2.8.4.tar.gz` & `tmp/convert_videos-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_videos-2.8.4.tar", max compression
+gzip compressed data, was "convert_videos-2.8.6.tar", max compression
```

## Comparing `convert_videos-2.8.4.tar` & `convert_videos-2.8.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-06 11:21:46.786720 convert_videos-2.8.4/LICENSE.md
--rw-r--r--   0        0        0     3432 2023-05-06 11:21:46.786720 convert_videos-2.8.4/README.md
--rwxr-xr-x   0        0        0      195 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/__init__.py
--rw-r--r--   0        0        0     4431 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/cli.py
--rw-r--r--   0        0        0      219 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/colour.py
--rw-r--r--   0        0        0     2400 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/ffmpeg_converter.py
--rw-r--r--   0        0        0     2196 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/processor.py
--rw-r--r--   0        0        0     4045 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/settings.py
--rw-r--r--   0        0        0     4655 2023-05-06 11:21:46.786720 convert_videos-2.8.4/convert_videos/video_processor.py
--rw-r--r--   0        0        0      870 2023-05-06 11:21:46.786720 convert_videos-2.8.4/pyproject.toml
--rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 convert_videos-2.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 13:21:43.305393 convert_videos-2.8.6/LICENSE.md
+-rw-r--r--   0        0        0     4316 2023-05-06 13:21:43.305393 convert_videos-2.8.6/README.md
+-rwxr-xr-x   0        0        0      195 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/__init__.py
+-rw-r--r--   0        0        0     4431 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/cli.py
+-rw-r--r--   0        0        0      219 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/colour.py
+-rw-r--r--   0        0        0     2399 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/ffmpeg_converter.py
+-rw-r--r--   0        0        0     2196 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/processor.py
+-rw-r--r--   0        0        0     4045 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/settings.py
+-rw-r--r--   0        0        0     4520 2023-05-06 13:21:43.305393 convert_videos-2.8.6/convert_videos/video_processor.py
+-rw-r--r--   0        0        0      836 2023-05-06 13:21:43.309393 convert_videos-2.8.6/pyproject.toml
+-rw-r--r--   0        0        0     5262 1970-01-01 00:00:00.000000 convert_videos-2.8.6/PKG-INFO
```

### Comparing `convert_videos-2.8.4/LICENSE.md` & `convert_videos-2.8.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.4/README.md` & `convert_videos-2.8.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -13,76 +13,95 @@
 
 ### Container
 
 The default output container is `mkv` format. This can be changed with the `--container` flag to anything that is supported by FFMPEG and the chosen video and audio codecs
 
 ## Video output
 
+Default settings is HEVC/x265 at quality of 23
+
 ### Codecs
 
 Currently only HEVC (x265) and AVC (h264) are supported for video codecs.
 
 ### Resizing
 
 Videos can be resized automatically by providing a width. Height is automatically calculated to ensure that the aspect ratio is maintained.
 
 ### Hardware Acceleration
 
-Hardware acceleration is supported on nVidia devices. Caveats:
+Hardware acceleration is supported on nVidia and Intel devices.
 
-- Conversions use constqp mode for the quality setting instead of CRF, this is because nvenc does not support CRF
+Caveats for nVidia:
+- Conversions use constqp mode for the quality setting instead of CRF, as nvenc does not support CRF
 - b-frames are not currently supported; nvenc itself supports them on 20xx+ series graphics cards.
 
-Default settings:
-Audio: 160kbps 2 channel AAC
-Video: HEVC/x265 at quality of 23
+
+Caveats for Intel:
+- Conversions use global_quality mode as CRF isn't supported on Intel hardware. ICQ and LA-ICQ are apparently better, but only supported on Windows
+- Look-ahead is only supported on x264 (not HEVC)
+
+
+## Audio output
+
+Default settings is 160kbps 2 channel AAC.
+
+All audio streams will be included by default unless a language filter is specified with `--audio-language`.
+
 
 ## Subtitles
 
-All subtitles will be copied from the source if they exist
+All subtitles will be copied from the source if they exist unless a language filter is specified with `--subtitle-language`.
 
 ## Usage
 
 ```
 Usage: convert-videos [OPTIONS] DIRECTORIES...
 
 Options:
-  -i, --in-place            Replace the original files instead of appending
-                            the new codec name
+  -i, --in-place                  Replace the original files instead of
+                                  appending the new codec name
+
+  -f, --force                     Force conversion even if the format of the
+                                  file already matches the desired format
+
+  --video-codec TEXT              A target video codec. Supported codecs:
+                                  HEVC, AVC  [default: HEVC]
 
-  -f, --force               Force conversion even if the format of the file
-                            already matches the desired format
+  -q, --quality INTEGER           The quantizer quality level to use.
+                                  [default: 24]
 
-  --video-codec TEXT        A target video codec. Supported codecs: HEVC, AVC
-                            [default: HEVC]
+  -p, --preset TEXT               FFmpeg preset to use.  [default: medium]
+  -w, --width INTEGER             Specify a new width to enable resizing of
+                                  the video
 
-  -q, --quality INTEGER     The quantizer quality level to use  [default: 23]
-  -p, --preset TEXT         FFmpeg preset to use.  [default: medium]
-  -w, --width INTEGER       Specify a new width to enable resizing of the
-                            video
+  --extra-input-args TEXT         Specify any extra arguments you would like
+                                  to pass to FFMpeg input here
 
-  --extra-input-args TEXT   Specify any extra arguments you would like to pass
-                            to FFMpeg input here
+  --extra-output-args TEXT        Specify any extra arguments you would like
+                                  to pass to FFMpeg output here
 
-  --extra-output-args TEXT  Specify any extra arguments you would like to pass
-                            to FFMpeg output here
+  --audio-codec TEXT              A target audio codec  [default: AAC]
+  --audio-channels INTEGER        The number of channels to mux sound in to
+                                  [default: 2]
 
-  --audio-codec TEXT        A target audio codec  [default: AAC]
-  --audio-channels INTEGER  The number of channels to mux sound in to
-                            [default: 2]
+  --audio-bitrate INTEGER         The bitrate to use for the audio codec
+                                  [default: 160]
 
-  --audio-bitrate INTEGER   The bitrate to use for the audio codec  [default:
-                            160]
+  --temp-dir TEXT                 Specify a temporary directory to use during
+                                  conversions instead of the system default
 
-  --temp-dir TEXT           Specify a temporary directory to use during
-                            conversions instead of the system default
+  -v, --verbose                   Enable verbose log output
+  --container TEXT                Specify a video container to convert the
+                                  videos in to  [default: mkv]
 
-  -v, --verbose             Enable verbose log output
-  --container TEXT          Specify a video container to convert the videos in
-                            to  [default: mkv]
+  --dry-run                       Do not make actual changes
+  --encoder [software|nvidia|intel]
+                                  Optionally use a harwdare encoder to speed
+                                  things up.  [default: software]
 
-  --dry-run                 Do not make actual changes
-  --nvidia-hw-accel         Use Nvidia HW acceleration instead of software
-                            encoding
+  --audio-language TEXT           Only include audio streams in this language
+  --subtitle-language TEXT        Only include subtitle streams in this
+                                  language
 
-  -h, --help                Show this message and exit.
+  -h, --help                      Show this message and exit.
 ```
```

### Comparing `convert_videos-2.8.4/convert_videos/cli.py` & `convert_videos-2.8.6/convert_videos/cli.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.4/convert_videos/ffmpeg_converter.py` & `convert_videos-2.8.6/convert_videos/ffmpeg_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     destination_file_path: str
     extra_ffmpeg_input_args: str
     extra_ffmpeg_output_args: str
     dry_run: bool
     video_settings: VideoSettings
     audio_settings: AudioSettings
 
-    def __post__init__(self):
+    def __post_init__(self):
         self._validate_destination()
 
     def process(self):
         input_settings = self._generate_ffmpeg_settings("input")
         output_settings = self._generate_ffmpeg_settings("output")
 
         ff = ffmpy.FFmpeg(inputs={self.source_file_path: input_settings}, outputs={self.destination_file_path: output_settings})
```

### Comparing `convert_videos-2.8.4/convert_videos/processor.py` & `convert_videos-2.8.6/convert_videos/processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.4/convert_videos/settings.py` & `convert_videos-2.8.6/convert_videos/settings.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.8.4/convert_videos/video_processor.py` & `convert_videos-2.8.6/convert_videos/video_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,20 +34,14 @@
     IN_DESIRED_FORMAT = auto()
 
     FAILED = auto()
 
     def __str__(self):
         return titlecase(lowercase(self.name))
 
-    def colour(self):
-        c = "green"
-        if self == Status.FAILED:
-            c = "red"
-        return colour(c, str(self))
-
 
 @dataclass
 class VideoProcessor:
     video: Video
     video_settings: VideoSettings
     audio_settings: AudioSettings
     container: str
```

### Comparing `convert_videos-2.8.4/pyproject.toml` & `convert_videos-2.8.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "convert_videos"
-version = "2.8.4"
+version = "2.8.6"
 description = "This tool allows bulk conversion of videos using ffmpeg"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3 :: Only"
 ]
 
 [tool.poetry.scripts]
 convert-videos = "convert_videos.cli:main"
 
 [tool.poetry.dependencies]
-python = "^3.6"
-colorama = "^0.4.0"
-ffmpy = "^0.2.2"
-video_utils = "^2.2.0"
-click = "^7.0"
-prettytable = "^0.7.2"
+python = "^3.8.1"
+colorama = "^0.4.6"
+ffmpy = "^0.3.0"
+video-utils = "2.2.4"
+click = "^8.1.3"
+prettytable = "^3.7.0"
 stringcase = "^1.2.0"
 iso639 = "^0.1.4"
 
 [tool.poetry.dev-dependencies]
-coverage = "^5.0"
-mock = "^3.0.5"
-flake8 = "^3.7"
-pytest-cov = "^2.8"
-pytest = "^5.3"
-black = {version = "^19.10b0", allow-prereleases = true}
+coverage = "^7.2.5"
+mock = "^5.0.2"
+flake8 = "^6.0"
+pytest-cov = "^4.0"
+pytest = "^7.3"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

