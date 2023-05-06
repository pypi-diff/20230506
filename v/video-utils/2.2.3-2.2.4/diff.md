# Comparing `tmp/video_utils-2.2.3.tar.gz` & `tmp/video_utils-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_utils-2.2.3.tar", max compression
+gzip compressed data, was "video_utils-2.2.4.tar", max compression
```

## Comparing `video_utils-2.2.3.tar` & `video_utils-2.2.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1078 2022-03-26 12:22:34.427600 video_utils-2.2.3/LICENSE.md
--rw-r--r--   0        0        0      917 2022-03-26 12:22:34.427600 video_utils-2.2.3/README.md
--rw-r--r--   0        0        0      752 2022-03-26 12:22:34.427600 video_utils-2.2.3/pyproject.toml
--rw-r--r--   0        0        0      166 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/__init__.py
--rw-r--r--   0        0        0     1684 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/codec.py
--rw-r--r--   0        0        0      258 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/colour.py
--rw-r--r--   0        0        0     5181 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/fileMap.py
--rw-r--r--   0        0        0      868 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/parse_episode.py
--rw-r--r--   0        0        0     1549 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/validators.py
--rw-r--r--   0        0        0     2649 2022-03-26 12:22:34.431600 video_utils-2.2.3/video_utils/video.py
--rw-r--r--   0        0        0     1689 2022-03-26 12:23:09.991109 video_utils-2.2.3/setup.py
--rw-r--r--   0        0        0     1765 2022-03-26 12:23:09.991514 video_utils-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-06 13:10:07.403968 video_utils-2.2.4/LICENSE.md
+-rw-r--r--   0        0        0      917 2023-05-06 13:10:07.403968 video_utils-2.2.4/README.md
+-rw-r--r--   0        0        0      726 2023-05-06 13:10:07.403968 video_utils-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/__init__.py
+-rw-r--r--   0        0        0     1626 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/codec.py
+-rw-r--r--   0        0        0      258 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/colour.py
+-rw-r--r--   0        0        0     5181 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/fileMap.py
+-rw-r--r--   0        0        0      868 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/parse_episode.py
+-rw-r--r--   0        0        0     1549 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/validators.py
+-rw-r--r--   0        0        0     2649 2023-05-06 13:10:07.407968 video_utils-2.2.4/video_utils/video.py
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 video_utils-2.2.4/PKG-INFO
```

### Comparing `video_utils-2.2.3/LICENSE.md` & `video_utils-2.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/README.md` & `video_utils-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/pyproject.toml` & `video_utils-2.2.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 [tool.poetry]
 name = "video_utils"
-version = "2.2.3"
+version = "2.2.4"
 description = "This library is used for lots of shared functionality around parsing TV shows and movies"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3 :: Only"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-colorama = "^0.4.0"
-pymediainfo = "^4.1"
-tqdm = "^4.40.2"
-ffmpy = "^0.2.2"
+python = "^3.8.1"
+colorama = "^0.4.6"
+pymediainfo = "^6.0.1"
+tqdm = "^4.65.0"
+ffmpy = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
-coverage = "^5.0"
-mock = "^3.0.5"
-pytest = "^5.3"
-flake8 = "^3.7"
-autopep8 = "^1.4"
-pylint = "^2.4.4"
-pytest-cov = "^2.8.1"
+coverage = "^7.2.5"
+mock = "^5.0.2"
+pytest = "^7.3.1"
+flake8 = "^6.0.0"
+pytest-cov = "^4.0.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `video_utils-2.2.3/video_utils/codec.py` & `video_utils-2.2.4/video_utils/codec.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,17 @@
         return f"<Codec format_name={self.format_name}>"
 
     def __str__(self):
         return self.__repr__()
 
     def _autodetect(self):
         try:
-            self._data = CODEC_DATA[next(
-                x for x in CODEC_DATA if x == self.format_name)]
+            self._data = CODEC_DATA[self.format_name]
             self.pretty_name = self.pretty_name if self.pretty_name else self._data["pretty_name"]
-        except StopIteration:
+        except KeyError:
             pass  # No match found
 
     def get_ffmpeg_name(self, encoder="software"):
         if self._ffmpeg_name:
             return self._ffmpeg_name
         try:
             return self._data["ffmpeg_names"][encoder]
```

### Comparing `video_utils-2.2.3/video_utils/fileMap.py` & `video_utils-2.2.4/video_utils/fileMap.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/video_utils/parse_episode.py` & `video_utils-2.2.4/video_utils/parse_episode.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/video_utils/validators.py` & `video_utils-2.2.4/video_utils/validators.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/video_utils/video.py` & `video_utils-2.2.4/video_utils/video.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.2.3/PKG-INFO` & `video_utils-2.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: video-utils
-Version: 2.2.3
+Version: 2.2.4
 Summary: This library is used for lots of shared functionality around parsing TV shows and movies
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: colorama (>=0.4.0,<0.5.0)
-Requires-Dist: ffmpy (>=0.2.2,<0.3.0)
-Requires-Dist: pymediainfo (>=4.1,<5.0)
-Requires-Dist: tqdm (>=4.40.2,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: ffmpy (>=0.3.0,<0.4.0)
+Requires-Dist: pymediainfo (>=6.0.1,<7.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Video Utils
 
 ![Test Status](https://github.com/justin8/video_utils/workflows/Tests/badge.svg?branch=master)
 [![codecov](https://codecov.io/gh/justin8/video_utils/branch/master/graph/badge.svg)](https://codecov.io/gh/justin8/video_utils)
```

