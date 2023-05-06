# Comparing `tmp/piano_visualizer-1.0.0.tar.gz` & `tmp/piano_visualizer-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piano_visualizer-1.0.0.tar", last modified: Tue Apr  5 17:05:10 2022, max compression
+gzip compressed data, was "piano_visualizer-1.0.1.tar", last modified: Sat May  6 16:26:31 2023, max compression
```

## Comparing `piano_visualizer-1.0.0.tar` & `piano_visualizer-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 17:05:10.254908 piano_visualizer-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-04-05 17:05:10.254908 piano_visualizer-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-04-05 17:05:05.000000 piano_visualizer-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 17:05:10.254908 piano_visualizer-1.0.0/piano_visualizer/
--rw-r--r--   0 runner    (1001) docker     (121)    16026 2022-04-05 17:05:05.000000 piano_visualizer-1.0.0/piano_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 17:05:10.254908 piano_visualizer-1.0.0/piano_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-04-05 17:05:10.000000 piano_visualizer-1.0.0/piano_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-04-05 17:05:10.000000 piano_visualizer-1.0.0/piano_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 17:05:10.000000 piano_visualizer-1.0.0/piano_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-04-05 17:05:10.000000 piano_visualizer-1.0.0/piano_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-05 17:05:10.000000 piano_visualizer-1.0.0/piano_visualizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-05 17:05:10.254908 piano_visualizer-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-04-05 17:05:05.000000 piano_visualizer-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/piano_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    15961 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/piano_visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/piano_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/setup.py
```

### Comparing `piano_visualizer-1.0.0/PKG-INFO` & `piano_visualizer-1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: piano_visualizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library that allows you to export a video in which a piano is playing the music you give it.
 Home-page: https://github.com/ArjunSahlot/piano_visualizer
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
 License: GNU GPL v3
-Description: # piano_visualizer
-        
-        A python library that allows you to export a video in which a piano is playing the music you give it.
-        
-        ![example gif](https://github.com/ArjunSahlot/piano_visualizer/blob/main/assets/example.gif?raw=true)
-        
-        ## Features
-        
-        -   Export a video of a custom midi file
-        -   Easy interface
-        -   Multi-core export
-        -   Multiple piano support
-        -   Multiple midi support
-        -   Automatically generate audio for midi files
-        
-        ## How to
-        
-        `piano_visualizer` was built with the intent to for it to be simple to use. You can render a piano video with simply 4 lines of code!
-        
-        There are 2 main classes: `Piano` and `Video`
-        `Piano` takes care of the piano rendering and the midi file parsing
-        `Video` takes care of video management (fps, resolution) and exporting
-        
-        **INSTALL**
-        `pip install piano_visualizer`
-        
-        Working in `example.py`
-        
-        ```py
-        # Import the library after you have installed it
-        import piano_visualizer
-        
-        # Create a piano with a midi file(s)
-        piano = piano_visualizer.Piano(["/path/to/your/midi/file.mid"])
-        
-        # Create a video with resolution/fps
-        video = piano_visualizer.Video((1920, 1080), 30)
-        
-        # Add piano to video
-        video.add_piano(piano)
-        
-        # Export video on multiple cores (1 for single)
-        video.export("your/export/path.mp4", 6)
-        
-        # Progress bars should show up
-        # Once your video is exported it will be at the path you specified!
-        ```
-        
 Keywords: piano,visualizer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# piano_visualizer
+
+A python library that allows you to export a video in which a piano is playing the music you give it.
+
+![example gif](https://github.com/ArjunSahlot/piano_visualizer/blob/main/assets/example.gif?raw=true)
+
+## Features
+
+-   Export a video of a custom midi file
+-   Easy interface
+-   Multi-core export
+-   Multiple piano support
+-   Multiple midi support
+-   Automatically generate audio for midi files
+
+## How to
+
+`piano_visualizer` was built with the intent for it to be simple to use. You can render a piano video with simply 4 lines of code!
+
+There are 2 main classes: `Piano` and `Video`
+`Piano` takes care of the piano rendering and the midi file parsing
+`Video` takes care of video management (fps, resolution) and exporting
+
+**INSTALL**
+`pip install piano_visualizer`
+
+Working in `example.py`
+
+```py
+# Import the library after you have installed it
+import piano_visualizer
+
+# Create a piano with a midi file(s)
+piano = piano_visualizer.Piano(["/path/to/your/midi/file.mid"])
+
+# Create a video with resolution/fps
+video = piano_visualizer.Video((1920, 1080), 30)
+
+# Add piano to video
+video.add_piano(piano)
+
+# Export video on multiple cores (1 for single)
+video.export("your/export/path.mp4", 6)
+
+# Progress bars should show up
+# Once your video is exported it will be at the path you specified!
+```
+
+
```

### Comparing `piano_visualizer-1.0.0/README.md` & `piano_visualizer-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 -   Multi-core export
 -   Multiple piano support
 -   Multiple midi support
 -   Automatically generate audio for midi files
 
 ## How to
 
-`piano_visualizer` was built with the intent to for it to be simple to use. You can render a piano video with simply 4 lines of code!
+`piano_visualizer` was built with the intent for it to be simple to use. You can render a piano video with simply 4 lines of code!
 
 There are 2 main classes: `Piano` and `Video`
 `Piano` takes care of the piano rendering and the midi file parsing
 `Video` takes care of video management (fps, resolution) and exporting
 
 **INSTALL**
 `pip install piano_visualizer`
```

### Comparing `piano_visualizer-1.0.0/piano_visualizer/__init__.py` & `piano_visualizer-1.0.1/piano_visualizer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import time
 import sys
 import mido
 import multiprocessing
 import ctypes
 import ffmpeg
 import threading
-from moviepy.editor import VideoFileClip, concatenate_videoclips
 from random_utils.colors.conversions import hsv_to_rgb
 from random_utils.funcs import crash
 from pydub import AudioSegment
 from tqdm import tqdm
 
 
 class Video:
```

### Comparing `piano_visualizer-1.0.0/piano_visualizer.egg-info/PKG-INFO` & `piano_visualizer-1.0.1/piano_visualizer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: piano-visualizer
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python library that allows you to export a video in which a piano is playing the music you give it.
 Home-page: https://github.com/ArjunSahlot/piano_visualizer
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
 License: GNU GPL v3
-Description: # piano_visualizer
-        
-        A python library that allows you to export a video in which a piano is playing the music you give it.
-        
-        ![example gif](https://github.com/ArjunSahlot/piano_visualizer/blob/main/assets/example.gif?raw=true)
-        
-        ## Features
-        
-        -   Export a video of a custom midi file
-        -   Easy interface
-        -   Multi-core export
-        -   Multiple piano support
-        -   Multiple midi support
-        -   Automatically generate audio for midi files
-        
-        ## How to
-        
-        `piano_visualizer` was built with the intent to for it to be simple to use. You can render a piano video with simply 4 lines of code!
-        
-        There are 2 main classes: `Piano` and `Video`
-        `Piano` takes care of the piano rendering and the midi file parsing
-        `Video` takes care of video management (fps, resolution) and exporting
-        
-        **INSTALL**
-        `pip install piano_visualizer`
-        
-        Working in `example.py`
-        
-        ```py
-        # Import the library after you have installed it
-        import piano_visualizer
-        
-        # Create a piano with a midi file(s)
-        piano = piano_visualizer.Piano(["/path/to/your/midi/file.mid"])
-        
-        # Create a video with resolution/fps
-        video = piano_visualizer.Video((1920, 1080), 30)
-        
-        # Add piano to video
-        video.add_piano(piano)
-        
-        # Export video on multiple cores (1 for single)
-        video.export("your/export/path.mp4", 6)
-        
-        # Progress bars should show up
-        # Once your video is exported it will be at the path you specified!
-        ```
-        
 Keywords: piano,visualizer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# piano_visualizer
+
+A python library that allows you to export a video in which a piano is playing the music you give it.
+
+![example gif](https://github.com/ArjunSahlot/piano_visualizer/blob/main/assets/example.gif?raw=true)
+
+## Features
+
+-   Export a video of a custom midi file
+-   Easy interface
+-   Multi-core export
+-   Multiple piano support
+-   Multiple midi support
+-   Automatically generate audio for midi files
+
+## How to
+
+`piano_visualizer` was built with the intent for it to be simple to use. You can render a piano video with simply 4 lines of code!
+
+There are 2 main classes: `Piano` and `Video`
+`Piano` takes care of the piano rendering and the midi file parsing
+`Video` takes care of video management (fps, resolution) and exporting
+
+**INSTALL**
+`pip install piano_visualizer`
+
+Working in `example.py`
+
+```py
+# Import the library after you have installed it
+import piano_visualizer
+
+# Create a piano with a midi file(s)
+piano = piano_visualizer.Piano(["/path/to/your/midi/file.mid"])
+
+# Create a video with resolution/fps
+video = piano_visualizer.Video((1920, 1080), 30)
+
+# Add piano to video
+video.add_piano(piano)
+
+# Export video on multiple cores (1 for single)
+video.export("your/export/path.mp4", 6)
+
+# Progress bars should show up
+# Once your video is exported it will be at the path you specified!
+```
+
+
```

### Comparing `piano_visualizer-1.0.0/setup.py` & `piano_visualizer-1.0.1/setup.py`

 * *Files identical despite different names*

