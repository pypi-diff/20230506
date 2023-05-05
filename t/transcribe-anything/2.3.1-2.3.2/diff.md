# Comparing `tmp/transcribe-anything-2.3.1.tar.gz` & `tmp/transcribe-anything-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.3.1.tar", last modified: Fri May  5 22:25:29 2023, max compression
+gzip compressed data, was "transcribe-anything-2.3.2.tar", last modified: Fri May  5 23:05:18 2023, max compression
```

## Comparing `transcribe-anything-2.3.1.tar` & `transcribe-anything-2.3.2.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.626948 transcribe-anything-2.3.1/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     9009 2023-05-05 22:25:29.626948 transcribe-anything-2.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     7987 2023-05-05 22:23:57.000000 transcribe-anything-2.3.1/README.md
--rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/requirements.testing.txt
--rw-rw-rw-   0        0        0       71 2023-05-05 22:22:57.000000 transcribe-anything-2.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 22:25:29.627948 transcribe-anything-2.3.1/setup.cfg
--rw-rw-rw-   0        0        0     3109 2023-05-05 22:23:40.000000 transcribe-anything-2.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.594457 transcribe-anything-2.3.1/tests/
--rw-rw-rw-   0        0        0     2794 2023-05-05 18:57:48.000000 transcribe-anything-2.3.1/tests/test_transcribe_anything.py
--rw-rw-rw-   0        0        0      449 2022-12-01 20:48:45.000000 transcribe-anything-2.3.1/tests/test_whisper.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.602431 transcribe-anything-2.3.1/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.3.1/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     4868 2023-05-05 18:59:22.000000 transcribe-anything-2.3.1/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.3.1/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     2836 2023-05-05 22:22:52.000000 transcribe-anything-2.3.1/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.3.1/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.3.1/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1532 2022-12-09 00:33:26.000000 transcribe-anything-2.3.1/transcribe_anything/util.py
-drwxrwxrwx   0        0        0        0 2023-05-05 22:25:29.625426 transcribe-anything-2.3.1/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0     9009 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 22:25:29.000000 transcribe-anything-2.3.1/transcribe_anything.egg-info/top_level.txt
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-05 23:05:18.566030 transcribe-anything-2.3.2/
+-rw-r--r--   0 niteris    (501) staff       (20)     1064 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/LICENSE
+-rw-r--r--   0 niteris    (501) staff       (20)       57 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/MANIFEST.in
+-rw-r--r--   0 niteris    (501) staff       (20)     8861 2023-05-05 23:05:18.565843 transcribe-anything-2.3.2/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)     8028 2023-05-05 23:04:31.000000 transcribe-anything-2.3.2/README.md
+-rw-r--r--   0 niteris    (501) staff       (20)       24 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/requirements.testing.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       71 2023-05-05 23:02:34.000000 transcribe-anything-2.3.2/requirements.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       38 2023-05-05 23:05:18.566070 transcribe-anything-2.3.2/setup.cfg
+-rw-r--r--   0 niteris    (501) staff       (20)     3109 2023-05-05 23:04:02.000000 transcribe-anything-2.3.2/setup.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-05 23:05:18.563708 transcribe-anything-2.3.2/transcribe_anything/
+-rw-r--r--   0 niteris    (501) staff       (20)        0 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/transcribe_anything/__init__.py
+-rw-r--r--   0 niteris    (501) staff       (20)     5062 2023-05-05 23:02:34.000000 transcribe-anything-2.3.2/transcribe_anything/api.py
+-rw-r--r--   0 niteris    (501) staff       (20)     3071 2023-05-05 23:02:34.000000 transcribe-anything-2.3.2/transcribe_anything/audio.py
+-rw-r--r--   0 niteris    (501) staff       (20)     2836 2023-05-05 23:02:34.000000 transcribe-anything-2.3.2/transcribe_anything/cmd.py
+-rw-r--r--   0 niteris    (501) staff       (20)      613 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/transcribe_anything/logger.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1210 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/transcribe_anything/parse_whisper_options.py
+-rw-r--r--   0 niteris    (501) staff       (20)     1532 2022-12-15 00:53:40.000000 transcribe-anything-2.3.2/transcribe_anything/util.py
+drwxr-xr-x   0 niteris    (501) staff       (20)        0 2023-05-05 23:05:18.565617 transcribe-anything-2.3.2/transcribe_anything.egg-info/
+-rw-r--r--   0 niteris    (501) staff       (20)     8861 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/PKG-INFO
+-rw-r--r--   0 niteris    (501) staff       (20)      558 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/SOURCES.txt
+-rw-r--r--   0 niteris    (501) staff       (20)        1 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/dependency_links.txt
+-rw-r--r--   0 niteris    (501) staff       (20)      120 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/entry_points.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       71 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/requires.txt
+-rw-r--r--   0 niteris    (501) staff       (20)       20 2023-05-05 23:05:18.000000 transcribe-anything-2.3.2/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.3.1/LICENSE` & `transcribe-anything-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/PKG-INFO` & `transcribe-anything-2.3.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,189 +1,170 @@
-Metadata-Version: 2.1
-Name: transcribe-anything
-Version: 2.3.1
-Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
-Home-page: https://github.com/zackees/transcribe-anything
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# transcribe-anything
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
-
-### USES WHISPER AI
-
-Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
-
-Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
-
-Your data stays private and is not uploaded to any service.
-
-# Usage (CPU Version)
-
-```bash
-> pip install transcribe-anything
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-# Usage (GPU Accelerated Version) (works on Python 3.10.X)
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-Will output:
-
-```
-Detecting language using up to the first 30 seconds. Use `--language` to specify the language
-Detected language: English
-[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
-[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
-[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
-[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
-[00:40.000 --> 00:43.000]  Gotta make you understand
-[00:43.000 --> 00:45.000]  Never gonna give you up
-[00:45.000 --> 00:47.000]  Never gonna let you down
-[00:47.000 --> 00:51.000]  Never gonna run around and desert you
-[00:51.000 --> 00:53.000]  Never gonna make you cry
-[00:53.000 --> 00:55.000]  Never gonna say goodbye
-[00:55.000 --> 00:58.000]  Never gonna tell a lie
-[00:58.000 --> 01:00.000]  And hurt you
-[01:00.000 --> 01:04.000]  We've known each other for so long
-[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
-[01:09.000 --> 01:13.000]  Inside we both know what's been going on
-[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
-[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
-[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
-[01:25.000 --> 01:27.000]  Never gonna give you up
-[01:27.000 --> 01:29.000]  Never gonna let you down
-[01:29.000 --> 01:33.000]  Never gonna run around and desert you
-[01:33.000 --> 01:35.000]  Never gonna make you cry
-[01:35.000 --> 01:38.000]  Never gonna say goodbye
-[01:38.000 --> 01:40.000]  Never gonna tell a lie
-[01:40.000 --> 01:42.000]  And hurt you
-[01:42.000 --> 01:44.000]  Never gonna give you up
-[01:44.000 --> 01:46.000]  Never gonna let you down
-[01:46.000 --> 01:50.000]  Never gonna run around and desert you
-[01:50.000 --> 01:52.000]  Never gonna make you cry
-[01:52.000 --> 01:54.000]  Never gonna say goodbye
-[01:54.000 --> 01:57.000]  Never gonna tell a lie
-[01:57.000 --> 01:59.000]  And hurt you
-[02:08.000 --> 02:10.000]  Never gonna give
-[02:12.000 --> 02:14.000]  Never gonna give
-[02:16.000 --> 02:19.000]  We've known each other for so long
-[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
-[02:24.000 --> 02:28.000]  Inside we both know what's been going on
-[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
-[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
-[02:37.000 --> 02:40.000]  Gotta make you understand
-[02:40.000 --> 02:42.000]  Never gonna give you up
-[02:42.000 --> 02:44.000]  Never gonna let you down
-[02:44.000 --> 02:48.000]  Never gonna run around and desert you
-[02:48.000 --> 02:50.000]  Never gonna make you cry
-[02:50.000 --> 02:53.000]  Never gonna say goodbye
-[02:53.000 --> 02:55.000]  Never gonna tell a lie
-[02:55.000 --> 02:57.000]  And hurt you
-[02:57.000 --> 02:59.000]  Never gonna give you up
-[02:59.000 --> 03:01.000]  Never gonna let you down
-[03:01.000 --> 03:05.000]  Never gonna run around and desert you
-[03:05.000 --> 03:08.000]  Never gonna make you cry
-[03:08.000 --> 03:10.000]  Never gonna say goodbye
-[03:10.000 --> 03:12.000]  Never gonna tell a lie
-[03:12.000 --> 03:14.000]  And hurt you
-[03:14.000 --> 03:16.000]  Never gonna give you up
-[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
-[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
-[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
-```
-
-## Api
-
-```python
-from transcribe_anyting.api import transcribe
-
-transcribe(
-    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
-    output_dir="output_dir",
-)
-```
-
-## Install GPU/CUDA Accelerated version
-
-GPU acceleration is *much* faster than the CPU version. Install it using the following:
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# transcribe-anything should now be installed
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-## Develop
-
-Works for Ubuntu/MacOS/Win32(in git-bash)
-This will create a virtual environment
-
-```bash
-> cd transcribe_anything
-> ./install_dev.sh
-# Enter the environment:
-> source activate.sh
-```
-
-The environment is now active and the next step will only install to the local python. If the terminal
-is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
-
-## Required: Install to current python environment
-  * `pip install transcribe-anything`
-    * The command `transcribe_anything` will magically become available.
-  * `transcribe_anything <YOUTUBE_URL>`
-
-
-# Tech Stack
-  * OpenAI whisper
-  * yt-dlp: https://github.com/yt-dlp/yt-dlp
-  * static-ffmpeg
-    * github: https://github.com/zackees/static_ffmpeg
-    * pypi: https://pypi.org/project/static-ffmpeg/
-
-# Testing
-  * All tests are run by `tox`, simply go to the project directory root and run it.
-
-# Versions
-  * 2.3.1: static-ffmpeg >= 2.5 now specified
-  * 2.3.0: Now uses the official version of whisper ai
-  * 2.2.1: "test_" is now prepended to all the different output folder names.
-  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
-  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
-  * 2.1.1: Updates keywords for easier pypi finding.
-  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
-  * 2.0.13: Now works with python 3.9
-  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
-  * 2.0.11: Automatically deletes files in the out directory if they already exist.
-  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
-  * 2.0.9: fixes sanitization of path names for some youtube videos
-  * 2.0.8: fix `--output_dir` not being respected.
-  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
-  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
-  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
-  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
-  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
-  * 2.0.1: Fixes missing dependencies and adds whisper option.
-  * 2.0.0: New! Now a front end for Whisper ai!
+
+# transcribe-anything
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
+
+### USES WHISPER AI
+
+Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
+
+Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
+
+Your data stays private and is not uploaded to any service.
+
+# Usage (CPU Version)
+
+```bash
+> pip install transcribe-anything
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+Will output:
+
+```
+Detecting language using up to the first 30 seconds. Use `--language` to specify the language
+Detected language: English
+[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
+[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
+[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
+[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
+[00:40.000 --> 00:43.000]  Gotta make you understand
+[00:43.000 --> 00:45.000]  Never gonna give you up
+[00:45.000 --> 00:47.000]  Never gonna let you down
+[00:47.000 --> 00:51.000]  Never gonna run around and desert you
+[00:51.000 --> 00:53.000]  Never gonna make you cry
+[00:53.000 --> 00:55.000]  Never gonna say goodbye
+[00:55.000 --> 00:58.000]  Never gonna tell a lie
+[00:58.000 --> 01:00.000]  And hurt you
+[01:00.000 --> 01:04.000]  We've known each other for so long
+[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
+[01:09.000 --> 01:13.000]  Inside we both know what's been going on
+[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
+[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
+[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
+[01:25.000 --> 01:27.000]  Never gonna give you up
+[01:27.000 --> 01:29.000]  Never gonna let you down
+[01:29.000 --> 01:33.000]  Never gonna run around and desert you
+[01:33.000 --> 01:35.000]  Never gonna make you cry
+[01:35.000 --> 01:38.000]  Never gonna say goodbye
+[01:38.000 --> 01:40.000]  Never gonna tell a lie
+[01:40.000 --> 01:42.000]  And hurt you
+[01:42.000 --> 01:44.000]  Never gonna give you up
+[01:44.000 --> 01:46.000]  Never gonna let you down
+[01:46.000 --> 01:50.000]  Never gonna run around and desert you
+[01:50.000 --> 01:52.000]  Never gonna make you cry
+[01:52.000 --> 01:54.000]  Never gonna say goodbye
+[01:54.000 --> 01:57.000]  Never gonna tell a lie
+[01:57.000 --> 01:59.000]  And hurt you
+[02:08.000 --> 02:10.000]  Never gonna give
+[02:12.000 --> 02:14.000]  Never gonna give
+[02:16.000 --> 02:19.000]  We've known each other for so long
+[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
+[02:24.000 --> 02:28.000]  Inside we both know what's been going on
+[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
+[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
+[02:37.000 --> 02:40.000]  Gotta make you understand
+[02:40.000 --> 02:42.000]  Never gonna give you up
+[02:42.000 --> 02:44.000]  Never gonna let you down
+[02:44.000 --> 02:48.000]  Never gonna run around and desert you
+[02:48.000 --> 02:50.000]  Never gonna make you cry
+[02:50.000 --> 02:53.000]  Never gonna say goodbye
+[02:53.000 --> 02:55.000]  Never gonna tell a lie
+[02:55.000 --> 02:57.000]  And hurt you
+[02:57.000 --> 02:59.000]  Never gonna give you up
+[02:59.000 --> 03:01.000]  Never gonna let you down
+[03:01.000 --> 03:05.000]  Never gonna run around and desert you
+[03:05.000 --> 03:08.000]  Never gonna make you cry
+[03:08.000 --> 03:10.000]  Never gonna say goodbye
+[03:10.000 --> 03:12.000]  Never gonna tell a lie
+[03:12.000 --> 03:14.000]  And hurt you
+[03:14.000 --> 03:16.000]  Never gonna give you up
+[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
+[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
+[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
+```
+
+## Api
+
+```python
+from transcribe_anyting.api import transcribe
+
+transcribe(
+    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
+    output_dir="output_dir",
+)
+```
+
+## Install GPU/CUDA Accelerated version
+
+GPU acceleration is *much* faster than the CPU version. Install it using the following:
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# transcribe-anything should now be installed
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+## Develop
+
+Works for Ubuntu/MacOS/Win32(in git-bash)
+This will create a virtual environment
+
+```bash
+> cd transcribe_anything
+> ./install_dev.sh
+# Enter the environment:
+> source activate.sh
+```
+
+The environment is now active and the next step will only install to the local python. If the terminal
+is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
+
+## Required: Install to current python environment
+  * `pip install transcribe-anything`
+    * The command `transcribe_anything` will magically become available.
+  * `transcribe_anything <YOUTUBE_URL>`
+
+
+# Tech Stack
+  * OpenAI whisper
+  * yt-dlp: https://github.com/yt-dlp/yt-dlp
+  * static-ffmpeg
+    * github: https://github.com/zackees/static_ffmpeg
+    * pypi: https://pypi.org/project/static-ffmpeg/
+
+# Testing
+  * All tests are run by `tox`, simply go to the project directory root and run it.
+
+# Versions
+  * 2.3.2: Fix windows transcoding error
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
+  * 2.2.1: "test_" is now prepended to all the different output folder names.
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
+  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
+  * 2.1.1: Updates keywords for easier pypi finding.
+  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
+  * 2.0.13: Now works with python 3.9
+  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
+  * 2.0.11: Automatically deletes files in the out directory if they already exist.
+  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
+  * 2.0.9: fixes sanitization of path names for some youtube videos
+  * 2.0.8: fix `--output_dir` not being respected.
+  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
+  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
+  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
+  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
+  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
+  * 2.0.1: Fixes missing dependencies and adds whisper option.
+  * 2.0.0: New! Now a front end for Whisper ai!
```

### Comparing `transcribe-anything-2.3.1/README.md` & `transcribe-anything-2.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: transcribe-anything
+Version: 2.3.2
+Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
+Home-page: https://github.com/zackees/transcribe-anything
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # transcribe-anything
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
 [![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
 
@@ -143,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.2: Fix windows transcoding error
   * 2.3.1: static-ffmpeg >= 2.5 now specified
   * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
   * 2.1.1: Updates keywords for easier pypi finding.
   * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
```

### Comparing `transcribe-anything-2.3.1/setup.py` & `transcribe-anything-2.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "2.3.1"
+VERSION = "2.3.2"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
```

### Comparing `transcribe-anything-2.3.1/transcribe_anything/api.py` & `transcribe-anything-2.3.2/transcribe_anything/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,31 +80,38 @@
     else:
         raise ValueError(f"Unknown device {device}")
     print(f"Using device {device}")
     model_str = f" --model {model}" if model else ""
     output_dir_str = f' --output_dir "{output_dir}"' if output_dir else ""
     task_str = f" --task {task}" if task else ""
     language_str = f" --language {language}" if language else ""
-    cmd_list = [
-        "whisper",
-        f'"{tmp_mp3}"',
-        "--device",
-        device,
-        model_str,
-        output_dir_str,
-        task_str,
-        language_str,
-    ]
+    cmd_list = []
+    if sys.platform == "win32":
+        cmd_list.extend(["chcp", "65001", "&&"])
+    cmd_list.extend(
+        [
+            "whisper",
+            f'"{tmp_mp3}"',
+            "--device",
+            device,
+            model_str,
+            output_dir_str,
+            task_str,
+            language_str,
+        ]
+    )
     if other_args:
         cmd_list.extend(other_args)
     # Remove the empty strings.
     cmd_list = [x.strip() for x in cmd_list if x.strip()]
     cmd = " ".join(cmd_list)
     sys.stderr.write(f"Running:\n  {cmd}\n")
-    proc = subprocess.Popen(cmd, shell=True)  # pylint: disable=consider-using-with
+    proc = subprocess.Popen(  # pylint: disable=consider-using-with
+        cmd, shell=True, universal_newlines=True
+    )
     while True:
         rtn = proc.poll()
         if rtn is None:
             time.sleep(0.25)
             continue
         if rtn != 0:
             msg = f"Failed to execute {cmd}\n "
```

### Comparing `transcribe-anything-2.3.1/transcribe_anything/audio.py` & `transcribe-anything-2.3.2/transcribe_anything/audio.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/transcribe_anything/cmd.py` & `transcribe-anything-2.3.2/transcribe_anything/cmd.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/transcribe_anything/logger.py` & `transcribe-anything-2.3.2/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.3.2/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/transcribe_anything/util.py` & `transcribe-anything-2.3.2/transcribe_anything/util.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.1/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.3.2/transcribe_anything.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,190 @@
-Metadata-Version: 2.1
-Name: transcribe-anything
-Version: 2.3.1
-Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
-Home-page: https://github.com/zackees/transcribe-anything
-Author: Zach Vorhies
-Author-email: dont@email.me
-License: MIT
-Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Environment :: Console
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# transcribe-anything
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
-[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
-
-### USES WHISPER AI
-
-Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
-
-Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
-
-Your data stays private and is not uploaded to any service.
-
-# Usage (CPU Version)
-
-```bash
-> pip install transcribe-anything
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-# Usage (GPU Accelerated Version) (works on Python 3.10.X)
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# Outputs the srt, vtt and txt files in title/out.vtt
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-Will output:
-
-```
-Detecting language using up to the first 30 seconds. Use `--language` to specify the language
-Detected language: English
-[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
-[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
-[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
-[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
-[00:40.000 --> 00:43.000]  Gotta make you understand
-[00:43.000 --> 00:45.000]  Never gonna give you up
-[00:45.000 --> 00:47.000]  Never gonna let you down
-[00:47.000 --> 00:51.000]  Never gonna run around and desert you
-[00:51.000 --> 00:53.000]  Never gonna make you cry
-[00:53.000 --> 00:55.000]  Never gonna say goodbye
-[00:55.000 --> 00:58.000]  Never gonna tell a lie
-[00:58.000 --> 01:00.000]  And hurt you
-[01:00.000 --> 01:04.000]  We've known each other for so long
-[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
-[01:09.000 --> 01:13.000]  Inside we both know what's been going on
-[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
-[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
-[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
-[01:25.000 --> 01:27.000]  Never gonna give you up
-[01:27.000 --> 01:29.000]  Never gonna let you down
-[01:29.000 --> 01:33.000]  Never gonna run around and desert you
-[01:33.000 --> 01:35.000]  Never gonna make you cry
-[01:35.000 --> 01:38.000]  Never gonna say goodbye
-[01:38.000 --> 01:40.000]  Never gonna tell a lie
-[01:40.000 --> 01:42.000]  And hurt you
-[01:42.000 --> 01:44.000]  Never gonna give you up
-[01:44.000 --> 01:46.000]  Never gonna let you down
-[01:46.000 --> 01:50.000]  Never gonna run around and desert you
-[01:50.000 --> 01:52.000]  Never gonna make you cry
-[01:52.000 --> 01:54.000]  Never gonna say goodbye
-[01:54.000 --> 01:57.000]  Never gonna tell a lie
-[01:57.000 --> 01:59.000]  And hurt you
-[02:08.000 --> 02:10.000]  Never gonna give
-[02:12.000 --> 02:14.000]  Never gonna give
-[02:16.000 --> 02:19.000]  We've known each other for so long
-[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
-[02:24.000 --> 02:28.000]  Inside we both know what's been going on
-[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
-[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
-[02:37.000 --> 02:40.000]  Gotta make you understand
-[02:40.000 --> 02:42.000]  Never gonna give you up
-[02:42.000 --> 02:44.000]  Never gonna let you down
-[02:44.000 --> 02:48.000]  Never gonna run around and desert you
-[02:48.000 --> 02:50.000]  Never gonna make you cry
-[02:50.000 --> 02:53.000]  Never gonna say goodbye
-[02:53.000 --> 02:55.000]  Never gonna tell a lie
-[02:55.000 --> 02:57.000]  And hurt you
-[02:57.000 --> 02:59.000]  Never gonna give you up
-[02:59.000 --> 03:01.000]  Never gonna let you down
-[03:01.000 --> 03:05.000]  Never gonna run around and desert you
-[03:05.000 --> 03:08.000]  Never gonna make you cry
-[03:08.000 --> 03:10.000]  Never gonna say goodbye
-[03:10.000 --> 03:12.000]  Never gonna tell a lie
-[03:12.000 --> 03:14.000]  And hurt you
-[03:14.000 --> 03:16.000]  Never gonna give you up
-[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
-[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
-[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
-```
-
-## Api
-
-```python
-from transcribe_anyting.api import transcribe
-
-transcribe(
-    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
-    output_dir="output_dir",
-)
-```
-
-## Install GPU/CUDA Accelerated version
-
-GPU acceleration is *much* faster than the CPU version. Install it using the following:
-
-```bash
-> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
-# transcribe-anything should now be installed
-> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
-```
-
-## Develop
-
-Works for Ubuntu/MacOS/Win32(in git-bash)
-This will create a virtual environment
-
-```bash
-> cd transcribe_anything
-> ./install_dev.sh
-# Enter the environment:
-> source activate.sh
-```
-
-The environment is now active and the next step will only install to the local python. If the terminal
-is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
-
-## Required: Install to current python environment
-  * `pip install transcribe-anything`
-    * The command `transcribe_anything` will magically become available.
-  * `transcribe_anything <YOUTUBE_URL>`
-
-
-# Tech Stack
-  * OpenAI whisper
-  * yt-dlp: https://github.com/yt-dlp/yt-dlp
-  * static-ffmpeg
-    * github: https://github.com/zackees/static_ffmpeg
-    * pypi: https://pypi.org/project/static-ffmpeg/
-
-# Testing
-  * All tests are run by `tox`, simply go to the project directory root and run it.
-
-# Versions
-  * 2.3.1: static-ffmpeg >= 2.5 now specified
-  * 2.3.0: Now uses the official version of whisper ai
-  * 2.2.1: "test_" is now prepended to all the different output folder names.
-  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
-  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
-  * 2.1.1: Updates keywords for easier pypi finding.
-  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
-  * 2.0.13: Now works with python 3.9
-  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
-  * 2.0.11: Automatically deletes files in the out directory if they already exist.
-  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
-  * 2.0.9: fixes sanitization of path names for some youtube videos
-  * 2.0.8: fix `--output_dir` not being respected.
-  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
-  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
-  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
-  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
-  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
-  * 2.0.1: Fixes missing dependencies and adds whisper option.
-  * 2.0.0: New! Now a front end for Whisper ai!
+Metadata-Version: 2.1
+Name: transcribe-anything
+Version: 2.3.2
+Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
+Home-page: https://github.com/zackees/transcribe-anything
+Author: Zach Vorhies
+Author-email: dont@email.me
+License: MIT
+Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Environment :: Console
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# transcribe-anything
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/MacOS_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_macos.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Win_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_win.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Ubuntu_Tests/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/test_ubuntu.yml)
+[![Actions Status](https://github.com/zackees/transcribe-anything/workflows/Lint/badge.svg)](https://github.com/zackees/transcribe-anything/actions/workflows/lint.yml)
+
+### USES WHISPER AI
+
+Input a local file or url and this tool will transcribe it using Whisper AI into subtitle files and raw text.
+
+Uses whisper AI so this is state of the art translation service - completely free. 🤯🤯🤯
+
+Your data stays private and is not uploaded to any service.
+
+# Usage (CPU Version)
+
+```bash
+> pip install transcribe-anything
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+# Usage (GPU Accelerated Version) (works on Python 3.10.X)
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# Outputs the srt, vtt and txt files in title/out.vtt
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+Will output:
+
+```
+Detecting language using up to the first 30 seconds. Use `--language` to specify the language
+Detected language: English
+[00:00.000 --> 00:27.000]  We're no strangers to love, you know the rules, and so do I
+[00:27.000 --> 00:31.000]  I've built commitments while I'm thinking of
+[00:31.000 --> 00:35.000]  You wouldn't get this from any other guy
+[00:35.000 --> 00:40.000]  I just wanna tell you how I'm feeling
+[00:40.000 --> 00:43.000]  Gotta make you understand
+[00:43.000 --> 00:45.000]  Never gonna give you up
+[00:45.000 --> 00:47.000]  Never gonna let you down
+[00:47.000 --> 00:51.000]  Never gonna run around and desert you
+[00:51.000 --> 00:53.000]  Never gonna make you cry
+[00:53.000 --> 00:55.000]  Never gonna say goodbye
+[00:55.000 --> 00:58.000]  Never gonna tell a lie
+[00:58.000 --> 01:00.000]  And hurt you
+[01:00.000 --> 01:04.000]  We've known each other for so long
+[01:04.000 --> 01:09.000]  Your heart's been aching but you're too shy to say it
+[01:09.000 --> 01:13.000]  Inside we both know what's been going on
+[01:13.000 --> 01:17.000]  We know the game and we're gonna play it
+[01:17.000 --> 01:22.000]  And if you ask me how I'm feeling
+[01:22.000 --> 01:25.000]  Don't tell me you're too much to see
+[01:25.000 --> 01:27.000]  Never gonna give you up
+[01:27.000 --> 01:29.000]  Never gonna let you down
+[01:29.000 --> 01:33.000]  Never gonna run around and desert you
+[01:33.000 --> 01:35.000]  Never gonna make you cry
+[01:35.000 --> 01:38.000]  Never gonna say goodbye
+[01:38.000 --> 01:40.000]  Never gonna tell a lie
+[01:40.000 --> 01:42.000]  And hurt you
+[01:42.000 --> 01:44.000]  Never gonna give you up
+[01:44.000 --> 01:46.000]  Never gonna let you down
+[01:46.000 --> 01:50.000]  Never gonna run around and desert you
+[01:50.000 --> 01:52.000]  Never gonna make you cry
+[01:52.000 --> 01:54.000]  Never gonna say goodbye
+[01:54.000 --> 01:57.000]  Never gonna tell a lie
+[01:57.000 --> 01:59.000]  And hurt you
+[02:08.000 --> 02:10.000]  Never gonna give
+[02:12.000 --> 02:14.000]  Never gonna give
+[02:16.000 --> 02:19.000]  We've known each other for so long
+[02:19.000 --> 02:24.000]  Your heart's been aching but you're too shy to say it
+[02:24.000 --> 02:28.000]  Inside we both know what's been going on
+[02:28.000 --> 02:32.000]  We know the game and we're gonna play it
+[02:32.000 --> 02:37.000]  I just wanna tell you how I'm feeling
+[02:37.000 --> 02:40.000]  Gotta make you understand
+[02:40.000 --> 02:42.000]  Never gonna give you up
+[02:42.000 --> 02:44.000]  Never gonna let you down
+[02:44.000 --> 02:48.000]  Never gonna run around and desert you
+[02:48.000 --> 02:50.000]  Never gonna make you cry
+[02:50.000 --> 02:53.000]  Never gonna say goodbye
+[02:53.000 --> 02:55.000]  Never gonna tell a lie
+[02:55.000 --> 02:57.000]  And hurt you
+[02:57.000 --> 02:59.000]  Never gonna give you up
+[02:59.000 --> 03:01.000]  Never gonna let you down
+[03:01.000 --> 03:05.000]  Never gonna run around and desert you
+[03:05.000 --> 03:08.000]  Never gonna make you cry
+[03:08.000 --> 03:10.000]  Never gonna say goodbye
+[03:10.000 --> 03:12.000]  Never gonna tell a lie
+[03:12.000 --> 03:14.000]  And hurt you
+[03:14.000 --> 03:16.000]  Never gonna give you up
+[03:16.000 --> 03:23.000]  If you want, never gonna let you down Never gonna run around and desert you
+[03:23.000 --> 03:28.000]  Never gonna make you hide Never gonna say goodbye
+[03:28.000 --> 03:42.000]  Never gonna tell you I ain't ready
+```
+
+## Api
+
+```python
+from transcribe_anyting.api import transcribe
+
+transcribe(
+    url_or_file="https://www.youtube.com/watch?v=dQw4w9WgXcQ",
+    output_dir="output_dir",
+)
+```
+
+## Install GPU/CUDA Accelerated version
+
+GPU acceleration is *much* faster than the CPU version. Install it using the following:
+
+```bash
+> curl https://raw.githubusercontent.com/zackees/transcribe-anything/main/install_cuda.py | python
+# transcribe-anything should now be installed
+> transcribe_anything https://www.youtube.com/watch?v=dQw4w9WgXcQ
+```
+
+## Develop
+
+Works for Ubuntu/MacOS/Win32(in git-bash)
+This will create a virtual environment
+
+```bash
+> cd transcribe_anything
+> ./install_dev.sh
+# Enter the environment:
+> source activate.sh
+```
+
+The environment is now active and the next step will only install to the local python. If the terminal
+is closed then to get back into the environment `cd transcribe_anything` and execute `source activate.sh`
+
+## Required: Install to current python environment
+  * `pip install transcribe-anything`
+    * The command `transcribe_anything` will magically become available.
+  * `transcribe_anything <YOUTUBE_URL>`
+
+
+# Tech Stack
+  * OpenAI whisper
+  * yt-dlp: https://github.com/yt-dlp/yt-dlp
+  * static-ffmpeg
+    * github: https://github.com/zackees/static_ffmpeg
+    * pypi: https://pypi.org/project/static-ffmpeg/
+
+# Testing
+  * All tests are run by `tox`, simply go to the project directory root and run it.
+
+# Versions
+  * 2.3.2: Fix windows transcoding error
+  * 2.3.1: static-ffmpeg >= 2.5 now specified
+  * 2.3.0: Now uses the official version of whisper ai
+  * 2.2.1: "test_" is now prepended to all the different output folder names.
+  * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
+  * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
+  * 2.1.1: Updates keywords for easier pypi finding.
+  * 2.1.0: Unknown args are now assumed to be for whisper and passed to it as-is. Fixes https://github.com/zackees/transcribe-anything/issues/3
+  * 2.0.13: Now works with python 3.9
+  * 2.0.12: Adds --device to argument parameters. This will default to CUDA if available, else CPU.
+  * 2.0.11: Automatically deletes files in the out directory if they already exist.
+  * 2.0.10: fixes local file issue https://github.com/zackees/transcribe-anything/issues/2
+  * 2.0.9: fixes sanitization of path names for some youtube videos
+  * 2.0.8: fix `--output_dir` not being respected.
+  * 2.0.7: `install_cuda.sh` -> `install_cuda.py`
+  * 2.0.6: Fixes twitter video fetching. --keep-audio -> --no-keep-audio
+  * 2.0.5: Fix bad filename on trailing urls ending with /, adds --keep-audio
+  * 2.0.3: GPU support is now added. Run the `install_cuda.sh` script to enable.
+  * 2.0.2: Minor cleanup of file names (no more out.mp3.txt, it's now out.txt)
+  * 2.0.1: Fixes missing dependencies and adds whisper option.
+  * 2.0.0: New! Now a front end for Whisper ai!
```

### Comparing `transcribe-anything-2.3.1/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.3.2/transcribe_anything.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.testing.txt
 requirements.txt
 setup.py
-tests/test_transcribe_anything.py
-tests/test_whisper.py
 transcribe_anything/__init__.py
 transcribe_anything/api.py
 transcribe_anything/audio.py
 transcribe_anything/cmd.py
 transcribe_anything/logger.py
 transcribe_anything/parse_whisper_options.py
 transcribe_anything/util.py
```

