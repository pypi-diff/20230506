# Comparing `tmp/hoyo-daily-logins-helper-1.2.2.tar.gz` & `tmp/hoyo-daily-logins-helper-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyo-daily-logins-helper-1.2.2.tar", last modified: Sat May  6 21:36:48 2023, max compression
+gzip compressed data, was "hoyo-daily-logins-helper-1.2.3.tar", last modified: Sat May  6 21:50:24 2023, max compression
```

## Comparing `hoyo-daily-logins-helper-1.2.2.tar` & `hoyo-daily-logins-helper-1.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.559295 hoyo-daily-logins-helper-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.551295 hoyo-daily-logins-helper-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.555295 hoyo-daily-logins-helper-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:36:48.559295 hoyo-daily-logins-helper-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.555295 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:36:48.559295 hoyo-daily-logins-helper-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.559295 hoyo-daily-logins-helper-1.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 21:36:48.000000 hoyo-daily-logins-helper-1.2.2/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:48.559295 hoyo-daily-logins-helper-1.2.2/src/games/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/games/genshin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/games/hoyo_checkin.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/games/starrail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-06 21:36:33.000000 hoyo-daily-logins-helper-1.2.2/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.381270 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 21:50:24.000000 hoyo-daily-logins-helper-1.2.3/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:24.385270 hoyo-daily-logins-helper-1.2.3/src/games/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/genshin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/hoyo_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/games/starrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-06 21:50:09.000000 hoyo-daily-logins-helper-1.2.3/src/main.py
```

### Comparing `hoyo-daily-logins-helper-1.2.2/.github/workflows/deploy.yml` & `hoyo-daily-logins-helper-1.2.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/.github/workflows/tests.yml` & `hoyo-daily-logins-helper-1.2.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/.gitignore` & `hoyo-daily-logins-helper-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/LICENSE` & `hoyo-daily-logins-helper-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/PKG-INFO` & `hoyo-daily-logins-helper-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 1.2.2
+Version: 1.2.3
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-1.2.2/Pipfile.lock` & `hoyo-daily-logins-helper-1.2.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/README.md` & `hoyo-daily-logins-helper-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/PKG-INFO` & `hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 1.2.2
+Version: 1.2.3
 Summary: Get hoyo daily login rewards automatically!
 Author-email: Christopher Kaster <me@atomicptr.de>
 Keywords: genshin,genshin-impact,starrail,honkai-starrail,game
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `hoyo-daily-logins-helper-1.2.2/hoyo_daily_logins_helper.egg-info/SOURCES.txt` & `hoyo-daily-logins-helper-1.2.3/hoyo_daily_logins_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/pyproject.toml` & `hoyo-daily-logins-helper-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/src/config.py` & `hoyo-daily-logins-helper-1.2.3/src/config.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/src/games/hoyo_checkin.py` & `hoyo-daily-logins-helper-1.2.3/src/games/hoyo_checkin.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/src/http.py` & `hoyo-daily-logins-helper-1.2.3/src/http.py`

 * *Files identical despite different names*

### Comparing `hoyo-daily-logins-helper-1.2.2/src/main.py` & `hoyo-daily-logins-helper-1.2.3/src/main.py`

 * *Files identical despite different names*

