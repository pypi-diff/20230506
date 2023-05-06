# Comparing `tmp/piano_visualizer-1.0.1.tar.gz` & `tmp/piano_visualizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piano_visualizer-1.0.1.tar", last modified: Sat May  6 16:26:31 2023, max compression
+gzip compressed data, was "piano_visualizer-1.1.0.tar", last modified: Sat May  6 18:42:04 2023, max compression
```

## Comparing `piano_visualizer-1.0.1.tar` & `piano_visualizer-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/piano_visualizer/
--rw-r--r--   0 runner    (1001) docker     (123)    15961 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/piano_visualizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/piano_visualizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 16:26:31.000000 piano_visualizer-1.0.1/piano_visualizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:26:31.327204 piano_visualizer-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-06 16:26:26.000000 piano_visualizer-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:42:04.232665 piano_visualizer-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 18:41:59.000000 piano_visualizer-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-06 18:42:04.232665 piano_visualizer-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-06 18:41:59.000000 piano_visualizer-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:42:04.232665 piano_visualizer-1.1.0/piano_visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-05-06 18:42:00.000000 piano_visualizer-1.1.0/piano_visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:42:04.232665 piano_visualizer-1.1.0/piano_visualizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-06 18:42:04.000000 piano_visualizer-1.1.0/piano_visualizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-06 18:42:04.000000 piano_visualizer-1.1.0/piano_visualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:42:04.000000 piano_visualizer-1.1.0/piano_visualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 18:42:04.000000 piano_visualizer-1.1.0/piano_visualizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-06 18:42:04.000000 piano_visualizer-1.1.0/piano_visualizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 18:42:04.232665 piano_visualizer-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-06 18:42:00.000000 piano_visualizer-1.1.0/setup.py
```

### Comparing `piano_visualizer-1.0.1/LICENSE` & `piano_visualizer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piano_visualizer-1.0.1/PKG-INFO` & `piano_visualizer-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piano_visualizer
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python library that allows you to export a video in which a piano is playing the music you give it.
 Home-page: https://github.com/ArjunSahlot/piano_visualizer
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
 License: GNU GPL v3
 Keywords: piano,visualizer
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 -   Multi-core export
 -   Multiple piano support
 -   Multiple midi support
 -   Automatically generate audio for midi files
 
 ## How to
 
-`piano_visualizer` was built with the intent for it to be simple to use. You can render a piano video with simply 4 lines of code!
+`piano_visualizer` was built with the intent to for it to be simple to use. You can render a piano video with simply 4 lines of code!
 
 There are 2 main classes: `Piano` and `Video`
 `Piano` takes care of the piano rendering and the midi file parsing
 `Video` takes care of video management (fps, resolution) and exporting
 
 **INSTALL**
 `pip install piano_visualizer`
@@ -55,14 +55,19 @@
 # Create a video with resolution/fps
 video = piano_visualizer.Video((1920, 1080), 30)
 
 # Add piano to video
 video.add_piano(piano)
 
 # Export video on multiple cores (1 for single)
-video.export("your/export/path.mp4", 6)
+video.export("your/export/path.mp4", num_cores=6)
+
+# You can add music too! (although it is sometimes offset from video)
+# video.export("your/export/path.mp4", num_cores=6, music=True)
 
 # Progress bars should show up
 # Once your video is exported it will be at the path you specified!
 ```
 
+NOTE: For music to work, you need [fluidsynth](https://github.com/FluidSynth/fluidsynth/wiki/Download)
+
```

### Comparing `piano_visualizer-1.0.1/piano_visualizer/__init__.py` & `piano_visualizer-1.1.0/piano_visualizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,19 @@
 #
 
 import os
 import cv2
 import pygame
 import shutil
 import time
-import sys
 import mido
 import multiprocessing
-import ctypes
 import ffmpeg
-import threading
+from notifypy import Notify
+from midi2audio import FluidSynth
 from random_utils.colors.conversions import hsv_to_rgb
 from random_utils.funcs import crash
 from pydub import AudioSegment
 from tqdm import tqdm
 
 
 class Video:
@@ -48,15 +47,23 @@
 
     def set_audio(self, audio, overwrite=True):
         if overwrite:
             self.audio = [audio]
         else:
             self.audio.append(audio)
 
-    def export(self, path, num_cores=4, notify=True, **kwargs):
+    def export(self, path, num_cores=4, music=False, notify=True, **kwargs):
+        """
+        Export the video to the given path.
+
+        :param path: destination to where the video will be
+        :param num_cores: number of cores to use for exporting, defaults to 4
+        :param music: whether or not you want music (it is usually not aligned with video unfortunately), defaults to False
+        :param notify: notify the user through a system notification when exporting is done, defaults to True
+        """
         if "frac_frames" in kwargs:
             frac_frames = kwargs["frac_frames"]
         else:
             frac_frames = 1
 
         def quick_export(core, start, end):
             video = cv2.VideoWriter(os.path.join(export_dir, f"video{core}.mp4"), cv2.VideoWriter_fourcc(
@@ -111,16 +118,15 @@
                             print(
                                 "Piano Visualizer is not at fault if your computer freezes...")
                         else:
                             num_cores = int(input("New core count: "))
                 num_cores = min(num_cores, multiprocessing.cpu_count())
                 processes = []
                 curr_frame = 0
-                frame_inc = (frames + self.start_offset +
-                             self.end_offset) / num_cores
+                frame_inc = (frames + self.start_offset + self.end_offset) / num_cores
 
                 print(
                     f"Exporting {int(frame_inc)} on each of {num_cores} cores...")
 
                 for i in range(num_cores):
                     p = multiprocessing.Process(target=quick_export, args=(
                         i, int(curr_frame), int(curr_frame + frame_inc)))
@@ -162,77 +168,85 @@
 
             video.release()
             cv2.destroyAllWindows()
 
             print(f"Finished in {round(time.time()-time_start, 3)} seconds.")
             print("Releasing video...")
 
-            millisecs = (frames + 1)/self.fps * 1000
-            sounds = []
-            print("Creating music...")
-            for audio_path in self.audio:
-                if audio_path == "default":
-                    for i, piano in enumerate(self.pianos):
-                        sounds.extend(piano.gen_wavs(export_dir, millisecs))
-                else:
-                    sounds.append(AudioSegment.from_file(
-                        audio_path, format=audio_path.split(".")[-1])[0:millisecs])
-            print("Created music.")
-
-            print("Combining all audios into 1...")
-            music_file = os.path.join(export_dir, "piano.wav")
-            sound = sounds.pop(sounds.index(max(sounds, key=lambda x: len(x))))
-            for i in sounds:
-                sound = sound.overlay(i)
-
-            # Compress audio to length of video
-            new_sound = sound._spawn(sound.raw_data, overrides={
-                                     "frame_rate": int(sound.frame_rate*(len(sound)/millisecs))})
-            new_sound.set_frame_rate(sound.frame_rate)
-
-            new_sound.export(music_file, format="wav")
-            print("Done")
-
-            if self.start_offset or self.end_offset:
-                print("Offsetting music...")
-                s_silent = AudioSegment.silent(
-                    self.start_offset/self.fps * 1000)
-                e_silent = AudioSegment.silent(self.end_offset/self.fps * 1000)
-                (s_silent + AudioSegment.from_wav(music_file) +
-                 e_silent).export(music_file, format="wav")
-                print("Music offsetted successfully")
-
-            print("Compiling video")
-            video = ffmpeg.input(os.path.join(export_dir, "video.mp4")).video
-            audio = ffmpeg.input(music_file).audio
-            video = ffmpeg.output(
-                video, audio, path, vcodec="copy", acodec="aac", strict="experimental")
-            if os.path.isfile(path):
-                os.remove(path)
-            ffmpeg.run(video)
+            if music:
+                millisecs = (frames + 1)/self.fps * 1000
+                sounds = []
+                print("Creating music...")
+                for audio_path in self.audio:
+                    if audio_path == "default":
+                        for i, piano in enumerate(self.pianos):
+                            sounds.extend(piano.gen_flac(export_dir, millisecs))
+                    else:
+                        sounds.append(AudioSegment.from_file(
+                            audio_path, format=audio_path.split(".")[-1])[0:millisecs])
+                print("Created music.")
+
+                print("Combining all audios into 1...")
+                music_file = os.path.join(export_dir, "piano.flac")
+                sound = sounds.pop(sounds.index(max(sounds, key=lambda x: len(x))))
+                for i in sounds:
+                    sound = sound.overlay(i)
+
+                sound.export(music_file, format="flac")
+                # Compress audio to length of video
+                # new_sound = sound._spawn(sound.raw_data, overrides={"frame_rate": int(sound.frame_rate*(len(sound)/millisecs))})
+                # new_sound.set_frame_rate(sound.frame_rate)
+
+                # new_sound.export(music_file, format="flac")
+                print("Done")
+
+                if self.start_offset or self.end_offset:
+                    print("Offsetting music...")
+                    s_silent = AudioSegment.silent(
+                        self.start_offset/self.fps * 1000)
+                    e_silent = AudioSegment.silent(self.end_offset/self.fps * 1000)
+                    (s_silent + AudioSegment.from_file(music_file, "flac") + e_silent).export(music_file, format="flac")
+                    print("Music offsetted successfully")
+
+                print("Compiling video")
+                video = ffmpeg.input(os.path.join(export_dir, "video.mp4")).video
+                audio = ffmpeg.input(music_file).audio
+                video = ffmpeg.output(
+                    video, audio, path, vcodec="copy", acodec="aac", strict="experimental")
+                if os.path.isfile(path):
+                    os.remove(path)
+                ffmpeg.run(video)
+            else:
+                print("Skipping music...")
+                os.rename(os.path.join(export_dir, "video.mp4"), path)
+
             print(f"Video Done")
             print("Cleaning up...")
 
         except (Exception, KeyboardInterrupt) as e:
-            print(f"Export interruputed due to {e}")
+            print(f"Export interrupted due to {e}")
             shutil.rmtree(export_dir)
-            if sys.platform == "linux" and notify:
-                os.system(
-                    f"notify-send 'Piano Visualizer' 'Export interrupted due to {e}'")
+            if notify:
+                notification = Notify()
+                notification.title = "Piano Visualizer"
+                notification.message = f"Export interrupted due to {e}"
+                notification.send()
             crash()
 
         shutil.rmtree(export_dir)
         total_time = time.time()-time_start
         print(
             f"Finished exporting video in {total_time//60} mins and {round(total_time%60, 3)} secs.")
         print("-"*50)
 
-        if sys.platform == "linux" and notify:
-            os.system(
-                f"notify-send 'Piano Visualizer' 'Finished exporting {path.split('/')[-1]}'")
+        if notify:
+            notification = Notify()
+            notification.title = "Piano Visualizer"
+            notification.message = f"Finished exporting {path.split('/')[-1]}"
+            notification.send()
 
     def render(self, frame):
         surf = pygame.Surface(self.resolution, pygame.SRCALPHA)
         surf.fill((0, 0, 0, 0))
         width, height = self.resolution
         max_height = height/5
         min_height = height/12
@@ -272,25 +286,23 @@
     def configure(self, datapath, value):
         if datapath in self.__dict__.keys():
             setattr(self, datapath, value)
 
     def render_rect(self, surf, x, y, width, height, color):
         s = pygame.Surface((width, height), pygame.SRCALPHA)
         for cy in range(int(height+1)):
-            pygame.draw.rect(s, list(color) +
-                             [255*((height-cy)/height)], (0, cy, width, 1))
+            pygame.draw.rect(s, list(color) + [255*((height-cy)/height)], (0, cy, width, 1))
         surf.blit(s, (x, y))
 
     def render(self, surf, frame, y, width, height, wheight, bheight, wwidth, bwidth, gap):
         counter = 0
         playing_keys = self.get_play_status(frame)
         black_keys = []
         if self.blocks:
-            self.render_blocks(surf, frame, y, width, height -
-                           wheight, wwidth, bwidth, gap)
+            self.render_blocks(surf, frame, y, width, height - wheight, wwidth, bwidth, gap)
         py = y + height - wheight
         surf.fill((0, 0, 0), (0, py, width, wheight))
 
         for key in range(88):
             if self.is_black(key):
                 x = (counter+1)*(wwidth + gap) - gap/2 - bwidth/2
                 if key in playing_keys:
@@ -304,16 +316,15 @@
                 counter += 1
                 x = counter*(wwidth + gap)
                 if key in playing_keys:
                     color = self.get_rainbow(
                         x, width) if self.color == "rainbow" else self.white_hit_col
                 else:
                     color = self.white_col
-                pygame.draw.rect(surf, self.white_col,
-                                 (x, py, wwidth, wheight))
+                pygame.draw.rect(surf, self.white_col, (x, py, wwidth, wheight))
                 self.render_rect(surf, x, py, wwidth, wheight, color)
 
         for key in black_keys:
             pygame.draw.rect(*key[0])
             self.render_rect(*key[1])
 
     def render_blocks(self, surf, frame, y, width, height, wwidth, bwidth, gap):
@@ -350,15 +361,15 @@
         for mid in self.midis:
             midi = mido.MidiFile(mid)
             for track in midi.tracks:
                 tempo = 500000
                 frame = 0
                 start_keys = [None] * 88
                 for msg in track:
-                    frame += msg.time/midi.ticks_per_beat * tempo/1000000 * self.fps
+                    frame += msg.time/midi.ticks_per_beat * tempo/1675000 * self.fps
                     if msg.is_meta:
                         if msg.type == "set_tempo":
                             tempo = msg.tempo
                     else:
                         if msg.type in ("note_on", "note_off"):
                             if not msg.velocity or msg.type == "note_off":
                                 self.notes.append(
@@ -378,26 +389,20 @@
 
     def get_min_time(self):
         return min(self.notes, key=lambda x: x["start"])["start"]
 
     def get_max_time(self):
         return max(self.notes, key=lambda x: x["end"])["end"]
 
-    def gen_wavs(self, export_dir, silent_len):
-        wavs = []
-        wav_path = os.path.join(export_dir, "pianowav.wav")
+    def gen_flac(self, export_dir, silent_len):
+        flacs = []
+        flacs_path = os.path.join(export_dir, "pianoflac.flac")
         for midi in self.midis:
-            os.system(f"timidity {midi} -Ow -o {wav_path}")
-            try:
-                wavs.append(a := AudioSegment.from_wav(wav_path))
-            except FileNotFoundError:
-                print(
-                    "You might not have timidity installed on your machine.", file=sys.stderr)
-                print(
-                    "Please have that installed if you are using the midi files as audio.", file=sys.stderr)
-                return [AudioSegment.silent(silent_len)]
-        return wavs
+            fs = FluidSynth()
+            fs.midi_to_audio(midi, flacs_path)
+            flacs.append(AudioSegment.from_file(flacs_path, format="flac"))
+        return flacs
 
     def register(self, fps, offset):
         self.fps = fps
         self.offset = offset
         self.parse_midis()
```

### Comparing `piano_visualizer-1.0.1/piano_visualizer.egg-info/PKG-INFO` & `piano_visualizer-1.1.0/piano_visualizer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piano-visualizer
-Version: 1.0.1
+Version: 1.1.0
 Summary: A python library that allows you to export a video in which a piano is playing the music you give it.
 Home-page: https://github.com/ArjunSahlot/piano_visualizer
 Author: Arjun Sahlot
 Author-email: iarjun.sahlot@gmail.com
 License: GNU GPL v3
 Keywords: piano,visualizer
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 -   Multi-core export
 -   Multiple piano support
 -   Multiple midi support
 -   Automatically generate audio for midi files
 
 ## How to
 
-`piano_visualizer` was built with the intent for it to be simple to use. You can render a piano video with simply 4 lines of code!
+`piano_visualizer` was built with the intent to for it to be simple to use. You can render a piano video with simply 4 lines of code!
 
 There are 2 main classes: `Piano` and `Video`
 `Piano` takes care of the piano rendering and the midi file parsing
 `Video` takes care of video management (fps, resolution) and exporting
 
 **INSTALL**
 `pip install piano_visualizer`
@@ -55,14 +55,19 @@
 # Create a video with resolution/fps
 video = piano_visualizer.Video((1920, 1080), 30)
 
 # Add piano to video
 video.add_piano(piano)
 
 # Export video on multiple cores (1 for single)
-video.export("your/export/path.mp4", 6)
+video.export("your/export/path.mp4", num_cores=6)
+
+# You can add music too! (although it is sometimes offset from video)
+# video.export("your/export/path.mp4", num_cores=6, music=True)
 
 # Progress bars should show up
 # Once your video is exported it will be at the path you specified!
 ```
 
+NOTE: For music to work, you need [fluidsynth](https://github.com/FluidSynth/fluidsynth/wiki/Download)
+
```

### Comparing `piano_visualizer-1.0.1/setup.py` & `piano_visualizer-1.1.0/setup.py`

 * *Files identical despite different names*

