# Comparing `tmp/sopel-8ball-0.4.0.tar.gz` & `tmp/sopel-8ball-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-8ball-0.4.0.tar", last modified: Tue Apr 18 22:39:35 2023, max compression
+gzip compressed data, was "sopel-8ball-0.4.1.tar", last modified: Sat May  6 14:02:36 2023, max compression
```

## Comparing `sopel-8ball-0.4.0.tar` & `sopel-8ball-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:39:35.656575 sopel-8ball-0.4.0/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.4.0/LICENSE.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2559 2023-04-18 22:39:35.656575 sopel-8ball-0.4.0/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1380 2023-04-18 22:09:45.000000 sopel-8ball-0.4.0/README.rst
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1732 2023-04-18 22:38:04.000000 sopel-8ball-0.4.0/pyproject.toml
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      218 2023-04-18 22:39:35.656575 sopel-8ball-0.4.0/setup.cfg
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:39:35.656575 sopel-8ball-0.4.0/sopel_8ball/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.4.0/sopel_8ball/__init__.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6253 2023-04-18 22:19:57.000000 sopel-8ball-0.4.0/sopel_8ball/choices.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.4.0/sopel_8ball/config.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.4.0/sopel_8ball/managers.py
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.4.0/sopel_8ball/plugin.py
-drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-04-18 22:39:35.656575 sopel-8ball-0.4.0/sopel_8ball.egg-info/
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2559 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/PKG-INFO
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      374 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/SOURCES.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/dependency_links.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      216 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/entry_points.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       11 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/requires.txt
--rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       12 2023-04-18 22:39:35.000000 sopel-8ball-0.4.0/sopel_8ball.egg-info/top_level.txt
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-05-06 14:02:36.162012 sopel-8ball-0.4.1/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1021 2021-07-10 22:27:18.000000 sopel-8ball-0.4.1/LICENSE.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2559 2023-05-06 14:02:36.162012 sopel-8ball-0.4.1/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1380 2023-04-18 22:09:45.000000 sopel-8ball-0.4.1/README.rst
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1732 2023-05-06 13:58:25.000000 sopel-8ball-0.4.1/pyproject.toml
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      218 2023-05-06 14:02:36.162012 sopel-8ball-0.4.1/setup.cfg
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-05-06 14:02:36.162012 sopel-8ball-0.4.1/sopel_8ball/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      178 2021-07-08 21:33:17.000000 sopel-8ball-0.4.1/sopel_8ball/__init__.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     6254 2023-05-06 13:57:23.000000 sopel-8ball-0.4.1/sopel_8ball/choices.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      472 2021-07-09 13:37:34.000000 sopel-8ball-0.4.1/sopel_8ball/config.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2480 2021-07-09 15:59:39.000000 sopel-8ball-0.4.1/sopel_8ball/managers.py
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     1315 2022-01-20 13:17:00.000000 sopel-8ball-0.4.1/sopel_8ball/plugin.py
+drwxrwxr-x   0 fstrzelecki  (1000) fstrzelecki  (1000)        0 2023-05-06 14:02:36.162012 sopel-8ball-0.4.1/sopel_8ball.egg-info/
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)     2559 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/PKG-INFO
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      374 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/SOURCES.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)        1 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/dependency_links.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)      216 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/entry_points.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       11 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/requires.txt
+-rw-rw-r--   0 fstrzelecki  (1000) fstrzelecki  (1000)       12 2023-05-06 14:02:36.000000 sopel-8ball-0.4.1/sopel_8ball.egg-info/top_level.txt
```

### Comparing `sopel-8ball-0.4.0/LICENSE.txt` & `sopel-8ball-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.4.0/PKG-INFO` & `sopel-8ball-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-8ball
-Version: 0.4.0
+Version: 0.4.1
 Summary: Magic 8 ball plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>, Florian Strzelecki <florian.strzelecki@gmail.com>
 Maintainer-email: Florian Strzelecki <florian.strzelecki@gmail.com>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/Exirel/sopel-8ball
 Project-URL: Bug Tracker, https://github.com/Exirel/sopel-8ball/issues
 Keywords: sopel,plugin,height-ball,bot,irc
```

### Comparing `sopel-8ball-0.4.0/README.rst` & `sopel-8ball-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.4.0/pyproject.toml` & `sopel-8ball-0.4.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["sopel_8ball", "sopel_8ball.*"]
 namespaces = false
 
 [project]
 name = "sopel-8ball"
-version = "0.4.0"
+version = "0.4.1"
 description = "Magic 8 ball plugin for Sopel"
 keywords = [
   "sopel",
   "plugin",
   "height-ball",
   "bot",
   "irc",
```

### Comparing `sopel-8ball-0.4.0/sopel_8ball/choices.py` & `sopel-8ball-0.4.1/sopel_8ball/choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             "Mendokusai. (＃￣0￣)",
             "Omae kankei nai. (ಠ_ಠ)",
             "Osoraku. ┐(°ヮ°)┌",
             "Tsumaranai. ┐( ˘ ､ ˘ )┌",
             "Urusai! (╬`益´)",
 
             # negative answers
-            "Arienai. (|||❛︵❛。)"
+            "Arienai. (|||❛︵❛。)",
             "Chigau. (◞ ‸ ◟ㆀ)",
             "Dame! o(╥﹏╥)",
             "Iie. (ᗒᗩᗕ)",
             "Masaka! (╯︵╰)",
             "Muri. ▄█▀█●",
             "Zannen. _|￣|○",
         )
```

### Comparing `sopel-8ball-0.4.0/sopel_8ball/managers.py` & `sopel-8ball-0.4.1/sopel_8ball/managers.py`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.4.0/sopel_8ball/plugin.py` & `sopel-8ball-0.4.1/sopel_8ball/plugin.py`

 * *Files identical despite different names*

### Comparing `sopel-8ball-0.4.0/sopel_8ball.egg-info/PKG-INFO` & `sopel-8ball-0.4.1/sopel_8ball.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopel-8ball
-Version: 0.4.0
+Version: 0.4.1
 Summary: Magic 8 ball plugin for Sopel
 Author-email: dgw <dgw@technobabbl.es>, Florian Strzelecki <florian.strzelecki@gmail.com>
 Maintainer-email: Florian Strzelecki <florian.strzelecki@gmail.com>
 License: EFL-2.0
 Project-URL: Homepage, https://github.com/Exirel/sopel-8ball
 Project-URL: Bug Tracker, https://github.com/Exirel/sopel-8ball/issues
 Keywords: sopel,plugin,height-ball,bot,irc
```

