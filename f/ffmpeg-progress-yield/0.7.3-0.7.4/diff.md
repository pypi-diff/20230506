# Comparing `tmp/ffmpeg-progress-yield-0.7.3.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.3.tar", last modified: Fri May  5 06:39:03 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.4.tar", last modified: Sat May  6 09:37:16 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.3.tar` & `ffmpeg-progress-yield-0.7.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.235857 ffmpeg-progress-yield-0.7.3/
--rw-r--r--   0 werner     (501) staff       (20)     2242 2023-05-05 06:39:02.000000 ffmpeg-progress-yield-0.7.3/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.3/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)     9791 2023-05-05 06:39:03.236019 ffmpeg-progress-yield-0.7.3/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.3/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.233566 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-05 06:39:01.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1279 2023-03-04 16:13:54.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7196 2023-05-05 06:35:33.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.234712 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9791 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-05 06:39:03.000000 ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-05 06:39:03.236380 ffmpeg-progress-yield-0.7.3/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.3/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-05 06:39:03.235533 ffmpeg-progress-yield-0.7.3/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.3/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-05 06:37:46.000000 ffmpeg-progress-yield-0.7.3/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.416104 ffmpeg-progress-yield-0.7.4/
+-rw-r--r--   0 werner     (501) staff       (20)     2301 2023-05-06 09:37:15.000000 ffmpeg-progress-yield-0.7.4/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.4/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)     9850 2023-05-06 09:37:16.416243 ffmpeg-progress-yield-0.7.4/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.4/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.413665 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-06 09:37:14.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1279 2023-03-04 16:13:54.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     7206 2023-05-06 09:36:51.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.415040 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)     9850 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-06 09:37:16.416642 ffmpeg-progress-yield-0.7.4/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.4/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.415940 ffmpeg-progress-yield-0.7.4/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.4/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-05 06:37:46.000000 ffmpeg-progress-yield-0.7.4/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.3/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
 
+## v0.7.4 (2023-05-06)
+
+* Fix: round percentage numbers.
+
+
 ## v0.7.3 (2023-05-05)
 
 * Update readme.
 
 * Add progress as percent, fixes #12.
```

### Comparing `ffmpeg-progress-yield-0.7.3/LICENSE` & `ffmpeg-progress-yield-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.3/PKG-INFO` & `ffmpeg-progress-yield-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.3
+Version: 0.7.4
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,19 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.4 (2023-05-06)
+
+* Fix: round percentage numbers.
+
+
 ## v0.7.3 (2023-05-05)
 
 * Update readme.
 
 * Add progress as percent, fixes #12.
```

### Comparing `ffmpeg-progress-yield-0.7.3/README.md` & `ffmpeg-progress-yield-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
                     total_dur = int(duration_override * 1000)
                     continue
 
             if total_dur:
                 progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
                 if progress_time:
                     elapsed_time = to_ms(**progress_time.groupdict())
-                    yield elapsed_time / total_dur * 100
+                    yield round(elapsed_time / total_dur * 100, 2)
 
         if self.process is None or self.process.returncode != 0:
             _pretty_stderr = "\n".join(stderr)
             raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
 
         yield 100
         self.process = None
```

### Comparing `ffmpeg-progress-yield-0.7.3/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.3
+Version: 0.7.4
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,19 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.4 (2023-05-06)
+
+* Fix: round percentage numbers.
+
+
 ## v0.7.3 (2023-05-05)
 
 * Update readme.
 
 * Add progress as percent, fixes #12.
```

### Comparing `ffmpeg-progress-yield-0.7.3/setup.py` & `ffmpeg-progress-yield-0.7.4/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.3/test/test.mp4` & `ffmpeg-progress-yield-0.7.4/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.3/test/test.py` & `ffmpeg-progress-yield-0.7.4/test/test.py`

 * *Files identical despite different names*

