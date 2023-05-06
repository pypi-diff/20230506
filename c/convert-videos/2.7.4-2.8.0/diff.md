# Comparing `tmp/convert_videos-2.7.4.tar.gz` & `tmp/convert_videos-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convert_videos-2.7.4.tar", max compression
+gzip compressed data, was "convert_videos-2.8.0.tar", max compression
```

## Comparing `convert_videos-2.7.4.tar` & `convert_videos-2.8.0.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1078 2022-03-26 13:29:19.834938 convert_videos-2.7.4/LICENSE.md
--rw-r--r--   0        0        0     3432 2022-03-26 13:29:19.834938 convert_videos-2.7.4/README.md
--rwxr-xr-x   0        0        0      195 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/__init__.py
--rw-r--r--   0        0        0     4293 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/cli.py
--rw-r--r--   0        0        0      219 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/colour.py
--rw-r--r--   0        0        0     2400 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/ffmpeg_converter.py
--rw-r--r--   0        0        0     2180 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/processor.py
--rw-r--r--   0        0        0     3121 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/settings.py
--rw-r--r--   0        0        0     4597 2022-03-26 13:29:19.834938 convert_videos-2.7.4/convert_videos/video_processor.py
--rw-r--r--   0        0        0      852 2022-03-26 13:29:19.838937 convert_videos-2.7.4/pyproject.toml
--rw-r--r--   0        0        0     4417 2022-03-26 13:29:54.313955 convert_videos-2.7.4/setup.py
--rw-r--r--   0        0        0     4337 2022-03-26 13:29:54.314415 convert_videos-2.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 08:16:46.036636 convert_videos-2.8.0/LICENSE.md
+-rw-r--r--   0        0        0     3432 2023-05-06 08:16:46.040636 convert_videos-2.8.0/README.md
+-rwxr-xr-x   0        0        0      195 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/__init__.py
+-rw-r--r--   0        0        0     4457 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/cli.py
+-rw-r--r--   0        0        0      219 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/colour.py
+-rw-r--r--   0        0        0     2400 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/ffmpeg_converter.py
+-rw-r--r--   0        0        0     2180 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/processor.py
+-rw-r--r--   0        0        0     3998 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/settings.py
+-rw-r--r--   0        0        0     4639 2023-05-06 08:16:46.040636 convert_videos-2.8.0/convert_videos/video_processor.py
+-rw-r--r--   0        0        0      870 2023-05-06 08:16:46.040636 convert_videos-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4527 1970-01-01 00:00:00.000000 convert_videos-2.8.0/PKG-INFO
```

### Comparing `convert_videos-2.7.4/LICENSE.md` & `convert_videos-2.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.7.4/README.md` & `convert_videos-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `convert_videos-2.7.4/convert_videos/cli.py` & `convert_videos-2.8.0/convert_videos/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,23 @@
 @click.option("--audio-codec", default="AAC", show_default=True, help="A target audio codec")
 @click.option("--audio-channels", default=2, show_default=True, type=int, help="The number of channels to mux sound in to")
 @click.option("--audio-bitrate", default=160, show_default=True, type=int, help="The bitrate to use for the audio codec")
 @click.option("--temp-dir", help="Specify a temporary directory to use during conversions instead of the system default")
 @click.option("--verbose", "-v", is_flag=True, help="Enable verbose log output")
 @click.option("--container", default="mkv", show_default=True, help="Specify a video container to convert the videos in to")
 @click.option("--dry-run", is_flag=True, help="Do not make actual changes")
-@click.option("--encoder", type=click.Choice(["software", "nvidia", "intel"]), default="software", show_default=True, help="Optionally use a harwdare encoder to speed things up.")
+@click.option(
+    "--encoder",
+    type=click.Choice(["software", "nvidia", "intel"]),
+    default="software",
+    show_default=True,
+    help="Optionally use a harwdare encoder to speed things up.",
+)
+@click.option("--audio-language", help="Only include audio streams in this language")
+@click.option("--subtitle-language", help="Only include subtitle streams in this language")
 def main(
     directories,
     force,
     in_place,
     video_codec,
     quality,
     preset,
@@ -56,25 +64,26 @@
     audio_channels,
     audio_bitrate,
     temp_dir,
     verbose,
     container,
     dry_run,
     encoder,
+    audio_language,
+    subtitle_language,
 ):
     configure_logger(verbose)
 
-    video_settings = VideoSettings(codec=Codec(video_codec), quality=quality, preset=preset, width=width, encoder=encoder)
-    audio_settings = AudioSettings(codec=Codec(audio_codec), channels=audio_channels, bitrate=audio_bitrate,)
+    print(subtitle_language)
+    video_settings = VideoSettings(
+        codec=Codec(video_codec), quality=quality, preset=preset, width=width, encoder=encoder, subtitle_language=subtitle_language
+    )
+    audio_settings = AudioSettings(codec=Codec(audio_codec), channels=audio_channels, bitrate=audio_bitrate, language=audio_language)
 
-    if video_settings.codec.get_ffmpeg_name() is None:
-        raise Exception("Invalid video codec specified")
-
-    if audio_settings.codec.get_ffmpeg_name() is None:
-        raise Exception("Invalid audio codec specified")
+    print(video_settings.codec.__dict__)
 
     results = []
     for directory in directories:
         results += Processor(
             directory=directory,
             force=force,
             video_settings=video_settings,
```

### Comparing `convert_videos-2.7.4/convert_videos/ffmpeg_converter.py` & `convert_videos-2.8.0/convert_videos/ffmpeg_converter.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.7.4/convert_videos/processor.py` & `convert_videos-2.8.0/convert_videos/processor.py`

 * *Files identical despite different names*

### Comparing `convert_videos-2.7.4/convert_videos/settings.py` & `convert_videos-2.8.0/convert_videos/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,64 @@
+from iso639 import to_iso639_2
 from dataclasses import dataclass
 
 from video_utils import Codec
 
 
 @dataclass
 class AudioSettings:
     codec: Codec
     channels: int
     bitrate: int
+    language: str = None
+
+    def __post_init__(self):
+        self.get_ffmpeg_codec()
 
     def __str__(self):
         output = ""
-        output += f" -acodec {self.codec.get_ffmpeg_name()}"
+        if self.language:
+            output = f" -map 0:a:m:language:{to_iso639_2(self.language)}"
+        else:
+            output += " -map 0:a"  # Include all audio channels
+
+        output += f" -acodec {self.get_ffmpeg_codec()}"
+        if self.get_ffmpeg_codec() == "copy":
+            return output
+
         output += f" -ab {self.bitrate}k"
         output += f" -ac {self.channels}"
-        output += f" -map 0:a"  # Include all audio channels
         return output
 
+    def get_ffmpeg_codec(self):
+        ffmpeg_codec = None
+        if self.codec.format_name == "copy":
+            ffmpeg_codec = "copy"
+        else:
+            ffmpeg_codec = self.codec.get_ffmpeg_name()
+        if not ffmpeg_codec:
+            raise Exception("Failed to find the desired audio codec!")
+        return ffmpeg_codec
+
 
 @dataclass
 class VideoSettings:
     codec: Codec
     quality: int
     preset: str
     width: int = None  # Or None
     encoder: str = "software"
+    subtitle_language: str = None
+
+    def __post_init__(self):
+        self.get_ffmpeg_codec()
 
     def __str__(self):
         output = self._get_stream_settings()
-        output += f" -vcodec {self._get_ffmpeg_codec()}"
+        output += f" -vcodec {self.get_ffmpeg_codec()}"
         if self.codec.format_name == "copy":
             return output
 
         output += f" -preset {self.preset}"
         output += self._get_quality_settings()
         output += self._get_codec_settings()
         output += self._get_scaling_settings()
@@ -65,25 +91,28 @@
         else:
             output = f" -crf {self.quality}"
         return output
 
     def _get_codec_settings(self):
         output = ""
         if self.codec == Codec("HEVC"):
-            output += f" -strict -2"
+            output += " -strict -2"
         return output
 
     def _get_stream_settings(self):
-        output = " -map 0:v:0"  # Include first video stream
-        output += " -map 0:s?"  # Include all subtitle streams, if they exist
+        output = " -map 0:v"  # Include first video stream
+        if self.subtitle_language:
+            output += f" -map 0:s:m:language:{to_iso639_2(self.subtitle_language)}?"
+        else:
+            output += " -map 0:s?"  # Include all subtitle streams, if they exist
         output += " -c:s copy"
         return output
 
-    def _get_ffmpeg_codec(self):
+    def get_ffmpeg_codec(self):
         ffmpeg_codec = None
         if self.codec.format_name == "copy":
             ffmpeg_codec = "copy"
         else:
             ffmpeg_codec = self.codec.get_ffmpeg_name(self.encoder)
         if not ffmpeg_codec:
-            raise Exception("Failed to find the desired codec!")
+            raise Exception("Failed to find the desired video codec!")
         return ffmpeg_codec
```

### Comparing `convert_videos-2.7.4/convert_videos/video_processor.py` & `convert_videos-2.8.0/convert_videos/video_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def already_processed(self):
         renamed_path = self.renamed_path()
         if os.path.exists(renamed_path):
             log.debug(f"File '{self.video.name}' appears to have already been converted to {renamed_path} exists. Skipping")
             return True
 
         split_filename = os.path.splitext(self.video.name)
-        codec_name = self.video_settings.codec.pretty_name
+        codec_name = self.video_settings.codec.pretty_name or self.video_settings.get_ffmpeg_codec()
         if split_filename[0].endswith(codec_name):
             log.debug(f"File '{self.video.name}' already matches the renaming format. Skipping")
             return True
 
         return False
 
     def renamed_path(self):
```

### Comparing `convert_videos-2.7.4/pyproject.toml` & `convert_videos-2.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convert_videos"
-version = "2.7.4"
+version = "2.8.0"
 description = "This tool allows bulk conversion of videos using ffmpeg"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -18,14 +18,15 @@
 python = "^3.6"
 colorama = "^0.4.0"
 ffmpy = "^0.2.2"
 video_utils = "^2.2.0"
 click = "^7.0"
 prettytable = "^0.7.2"
 stringcase = "^1.2.0"
+iso639 = "^0.1.4"
 
 [tool.poetry.dev-dependencies]
 coverage = "^5.0"
 mock = "^3.0.5"
 flake8 = "^3.7"
 pytest-cov = "^2.8"
 pytest = "^5.3"
```

### Comparing `convert_videos-2.7.4/PKG-INFO` & `convert_videos-2.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: convert-videos
-Version: 2.7.4
+Version: 2.8.0
 Summary: This tool allows bulk conversion of videos using ffmpeg
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: colorama (>=0.4.0,<0.5.0)
 Requires-Dist: ffmpy (>=0.2.2,<0.3.0)
+Requires-Dist: iso639 (>=0.1.4,<0.2.0)
 Requires-Dist: prettytable (>=0.7.2,<0.8.0)
 Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: video_utils (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Convert Videos
```

