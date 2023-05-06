# Comparing `tmp/ndx-multichannel-volume-0.1.0.tar.gz` & `tmp/ndx-multichannel-volume-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndx-multichannel-volume-0.1.0.tar", last modified: Mon Apr  3 17:49:04 2023, max compression
+gzip compressed data, was "ndx-multichannel-volume-0.1.1.tar", last modified: Sat May  6 01:58:52 2023, max compression
```

## Comparing `ndx-multichannel-volume-0.1.0.tar` & `ndx-multichannel-volume-0.1.1.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.564499 ndx-multichannel-volume-0.1.0/
--rw-r--r--   0 danielsprague   (501) staff       (20)     1522 2023-02-23 20:11:07.000000 ndx-multichannel-volume-0.1.0/LICENSE.txt
--rw-r--r--   0 danielsprague   (501) staff       (20)      264 2023-02-23 20:11:07.000000 ndx-multichannel-volume-0.1.0/MANIFEST.in
--rw-r--r--   0 danielsprague   (501) staff       (20)      766 2023-04-03 17:49:04.564671 ndx-multichannel-volume-0.1.0/PKG-INFO
--rw-r--r--   0 danielsprague   (501) staff       (20)      220 2023-04-03 17:32:03.000000 ndx-multichannel-volume-0.1.0/README.md
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.527395 ndx-multichannel-volume-0.1.0/docs/
--rw-r--r--   0 danielsprague   (501) staff       (20)     6600 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/Makefile
--rw-r--r--   0 danielsprague   (501) staff       (20)     6196 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/README.md
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.505597 ndx-multichannel-volume-0.1.0/docs/build/
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.504979 ndx-multichannel-volume-0.1.0/docs/build/html/
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.533730 ndx-multichannel-volume-0.1.0/docs/build/html/_static/
--rw-r--r--   0 danielsprague   (501) staff       (20)    14813 2023-04-03 17:31:04.000000 ndx-multichannel-volume-0.1.0/docs/build/html/_static/basic.css
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.535630 ndx-multichannel-volume-0.1.0/docs/build/html/_static/css/
--rw-r--r--   0 danielsprague   (501) staff       (20)     3229 2023-02-23 20:09:06.000000 ndx-multichannel-volume-0.1.0/docs/build/html/_static/css/badge_only.css
--rw-r--r--   0 danielsprague   (501) staff       (20)   135235 2023-02-23 20:09:06.000000 ndx-multichannel-volume-0.1.0/docs/build/html/_static/css/theme.css
--rw-r--r--   0 danielsprague   (501) staff       (20)     4819 2023-04-03 17:31:04.000000 ndx-multichannel-volume-0.1.0/docs/build/html/_static/pygments.css
--rw-r--r--   0 danielsprague   (501) staff       (20)      365 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/build/html/_static/theme_overrides.css
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.547386 ndx-multichannel-volume-0.1.0/docs/build/latex/
--rw-r--r--   0 danielsprague   (501) staff       (20)     1549 2023-04-03 17:31:17.000000 ndx-multichannel-volume-0.1.0/docs/build/latex/Makefile
--rw-r--r--   0 danielsprague   (501) staff       (20)      473 2023-04-03 17:31:17.000000 ndx-multichannel-volume-0.1.0/docs/build/latex/make.bat
--rw-r--r--   0 danielsprague   (501) staff       (20)      804 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/make.bat
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.558402 ndx-multichannel-volume-0.1.0/docs/source/
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.559103 ndx-multichannel-volume-0.1.0/docs/source/_static/
--rw-r--r--   0 danielsprague   (501) staff       (20)      365 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 danielsprague   (501) staff       (20)     3739 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/conf.py
--rw-r--r--   0 danielsprague   (501) staff       (20)     3982 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/conf_doc_autogen.py
--rw-r--r--   0 danielsprague   (501) staff       (20)      167 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/credits.rst
--rw-r--r--   0 danielsprague   (501) staff       (20)     1602 2023-04-03 17:28:20.000000 ndx-multichannel-volume-0.1.0/docs/source/description.rst
--rw-r--r--   0 danielsprague   (501) staff       (20)      201 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/format.rst
--rw-r--r--   0 danielsprague   (501) staff       (20)      487 2023-02-23 20:11:18.000000 ndx-multichannel-volume-0.1.0/docs/source/index.rst
--rw-r--r--   0 danielsprague   (501) staff       (20)       93 2023-04-03 17:29:53.000000 ndx-multichannel-volume-0.1.0/docs/source/release_notes.rst
--rw-r--r--   0 danielsprague   (501) staff       (20)      234 2023-04-03 17:44:54.000000 ndx-multichannel-volume-0.1.0/pyproject.toml
--rw-r--r--   0 danielsprague   (501) staff       (20)       94 2023-02-23 20:11:07.000000 ndx-multichannel-volume-0.1.0/requirements.txt
--rw-r--r--   0 danielsprague   (501) staff       (20)      246 2023-04-03 17:49:04.565305 ndx-multichannel-volume-0.1.0/setup.cfg
--rw-r--r--   0 danielsprague   (501) staff       (20)     2101 2023-02-23 20:11:07.000000 ndx-multichannel-volume-0.1.0/setup.py
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.560125 ndx-multichannel-volume-0.1.0/spec/
--rw-r--r--   0 danielsprague   (501) staff       (20)     7961 2023-03-30 18:28:59.000000 ndx-multichannel-volume-0.1.0/spec/ndx-multichannel-volume.extensions.yaml
--rw-r--r--   0 danielsprague   (501) staff       (20)      556 2023-03-30 18:28:59.000000 ndx-multichannel-volume-0.1.0/spec/ndx-multichannel-volume.namespace.yaml
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.506864 ndx-multichannel-volume-0.1.0/src/
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.507489 ndx-multichannel-volume-0.1.0/src/pynwb/
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.560570 ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/
--rw-r--r--   0 danielsprague   (501) staff       (20)    11362 2023-03-30 19:43:44.000000 ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/__init__.py
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.561576 ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/spec/
--rw-r--r--   0 danielsprague   (501) staff       (20)     7961 2023-03-30 18:28:59.000000 ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/spec/ndx-multichannel-volume.extensions.yaml
--rw-r--r--   0 danielsprague   (501) staff       (20)      556 2023-03-30 18:28:59.000000 ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/spec/ndx-multichannel-volume.namespace.yaml
-drwxr-xr-x   0 danielsprague   (501) staff       (20)        0 2023-04-03 17:49:04.564122 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/
--rw-r--r--   0 danielsprague   (501) staff       (20)      766 2023-04-03 17:49:04.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/PKG-INFO
--rw-r--r--   0 danielsprague   (501) staff       (20)     1202 2023-04-03 17:49:04.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/SOURCES.txt
--rw-r--r--   0 danielsprague   (501) staff       (20)        1 2023-04-03 17:49:04.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/dependency_links.txt
--rw-r--r--   0 danielsprague   (501) staff       (20)        1 2023-02-27 22:29:18.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/not-zip-safe
--rw-r--r--   0 danielsprague   (501) staff       (20)       31 2023-04-03 17:49:04.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/requires.txt
--rw-r--r--   0 danielsprague   (501) staff       (20)       16 2023-04-03 17:49:04.000000 ndx-multichannel-volume-0.1.0/src/pynwb/ndx_multichannel_volume.egg-info/top_level.txt
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.533971 ndx-multichannel-volume-0.1.1/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     1522 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/LICENSE.txt
+-rw-r--r--   0 danielysprague   (501) staff       (20)      264 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/MANIFEST.in
+-rw-r--r--   0 danielysprague   (501) staff       (20)     2884 2023-05-06 01:58:52.534023 ndx-multichannel-volume-0.1.1/PKG-INFO
+-rw-r--r--   0 danielysprague   (501) staff       (20)     2370 2023-05-06 01:52:12.000000 ndx-multichannel-volume-0.1.1/README.md
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.529843 ndx-multichannel-volume-0.1.1/docs/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     6600 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/Makefile
+-rw-r--r--   0 danielysprague   (501) staff       (20)     6196 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/README.md
+-rw-r--r--   0 danielysprague   (501) staff       (20)      804 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/make.bat
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.531025 ndx-multichannel-volume-0.1.1/docs/source/
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.531196 ndx-multichannel-volume-0.1.1/docs/source/_static/
+-rw-r--r--   0 danielysprague   (501) staff       (20)      365 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 danielysprague   (501) staff       (20)     3739 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/conf.py
+-rw-r--r--   0 danielysprague   (501) staff       (20)     3982 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/conf_doc_autogen.py
+-rw-r--r--   0 danielysprague   (501) staff       (20)      167 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/credits.rst
+-rw-r--r--   0 danielysprague   (501) staff       (20)     1602 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/description.rst
+-rw-r--r--   0 danielysprague   (501) staff       (20)      201 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/format.rst
+-rw-r--r--   0 danielysprague   (501) staff       (20)      487 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/index.rst
+-rw-r--r--   0 danielysprague   (501) staff       (20)       93 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/docs/source/release_notes.rst
+-rw-r--r--   0 danielysprague   (501) staff       (20)       94 2023-05-05 19:54:38.000000 ndx-multichannel-volume-0.1.1/requirements.txt
+-rw-r--r--   0 danielysprague   (501) staff       (20)      246 2023-05-06 01:58:52.534240 ndx-multichannel-volume-0.1.1/setup.cfg
+-rw-r--r--   0 danielysprague   (501) staff       (20)     2117 2023-05-06 01:56:45.000000 ndx-multichannel-volume-0.1.1/setup.py
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.531576 ndx-multichannel-volume-0.1.1/spec/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     8204 2023-05-06 01:26:14.000000 ndx-multichannel-volume-0.1.1/spec/ndx-multichannel-volume.extensions.yaml
+-rw-r--r--   0 danielysprague   (501) staff       (20)      556 2023-05-06 01:26:14.000000 ndx-multichannel-volume-0.1.1/spec/ndx-multichannel-volume.namespace.yaml
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.528073 ndx-multichannel-volume-0.1.1/src/
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.528210 ndx-multichannel-volume-0.1.1/src/pynwb/
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.532125 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     1689 2023-05-05 21:29:58.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/__init__.py
+-rw-r--r--   0 danielysprague   (501) staff       (20)    11682 2023-05-06 00:37:27.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/ndx_multichannel_volume.py
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.533816 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/spec/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     8204 2023-05-06 01:26:14.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/spec/ndx-multichannel-volume.extensions.yaml
+-rw-r--r--   0 danielysprague   (501) staff       (20)      556 2023-05-06 01:26:14.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/spec/ndx-multichannel-volume.namespace.yaml
+drwxr-xr-x   0 danielysprague   (501) staff       (20)        0 2023-05-06 01:58:52.533485 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/
+-rw-r--r--   0 danielysprague   (501) staff       (20)     2884 2023-05-06 01:58:52.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/PKG-INFO
+-rw-r--r--   0 danielysprague   (501) staff       (20)     1024 2023-05-06 01:58:52.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/SOURCES.txt
+-rw-r--r--   0 danielysprague   (501) staff       (20)        1 2023-05-06 01:58:52.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/dependency_links.txt
+-rw-r--r--   0 danielysprague   (501) staff       (20)        1 2023-05-05 20:46:06.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/not-zip-safe
+-rw-r--r--   0 danielysprague   (501) staff       (20)       31 2023-05-06 01:58:52.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/requires.txt
+-rw-r--r--   0 danielysprague   (501) staff       (20)       24 2023-05-06 01:58:52.000000 ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume.egg-info/top_level.txt
```

### Comparing `ndx-multichannel-volume-0.1.0/LICENSE.txt` & `ndx-multichannel-volume-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/Makefile` & `ndx-multichannel-volume-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/README.md` & `ndx-multichannel-volume-0.1.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/make.bat` & `ndx-multichannel-volume-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/source/conf.py` & `ndx-multichannel-volume-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/source/conf_doc_autogen.py` & `ndx-multichannel-volume-0.1.1/docs/source/conf_doc_autogen.py`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/docs/source/description.rst` & `ndx-multichannel-volume-0.1.1/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/setup.py` & `ndx-multichannel-volume-0.1.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,29 +18,29 @@
     else:
         readme = ""
 except Exception:
     readme = ""
 
 setup_args = {
     'name': 'ndx-multichannel-volume',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'extension to allow use of multichannel volumetric images',
     'long_description': readme,
     'long_description_content_type': readme_type,
     'author': 'Daniel Sprague',
     'author_email': 'daniel.sprague@ucsf.edu',
     'url': '',
     'license': 'BSD-3',
     'install_requires': [
         'pynwb>=1.5.0,<3',
         'hdmf>=2.5.6,<4',
     ],
     'packages': find_packages('src/pynwb', exclude=["tests", "tests.*"]),
     'package_dir': {'': 'src/pynwb'},
-    'package_data': {'MultiChannelVol': [
+    'package_data': {'ndx_multichannel_volume': [
         'spec/ndx-multichannel-volume.namespace.yaml',
         'spec/ndx-multichannel-volume.extensions.yaml',
     ]},
     'classifiers': [
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License"
@@ -55,15 +55,15 @@
 }
 
 
 def _copy_spec_files(project_dir):
     ns_path = os.path.join(project_dir, 'spec', 'ndx-multichannel-volume.namespace.yaml')
     ext_path = os.path.join(project_dir, 'spec', 'ndx-multichannel-volume.extensions.yaml')
 
-    dst_dir = os.path.join(project_dir, 'src', 'pynwb', 'MultiChannelVol', 'spec')
+    dst_dir = os.path.join(project_dir, 'src', 'pynwb', 'ndx_multichannel_volume', 'spec')
     if not os.path.exists(dst_dir):
         os.mkdir(dst_dir)
 
     copy2(ns_path, dst_dir)
     copy2(ext_path, dst_dir)
```

### Comparing `ndx-multichannel-volume-0.1.0/spec/ndx-multichannel-volume.extensions.yaml` & `ndx-multichannel-volume-0.1.1/spec/ndx-multichannel-volume.extensions.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 groups:
 - neurodata_type_def: CElegansSubject
   neurodata_type_inc: Subject
   doc: Subject object with support for C. Elegans specific attributes
   attributes:
   - name: growth_stage_time
     dtype: text
-    doc: amount of time in current growth stage in ISO duration format
+    doc: amount of time in current growth stage in ISO 8601 duration format
+    required: false
   datasets:
   - name: growth_stage
     dtype: text
     doc: Growth stage of C. elegans. One of two-fold, three-fold, L1-L4, YA, OA, duaer,
       post-dauer L4, post-dauer YA, post-dauer OA
   - name: cultivation_temp
     dtype: float32
     doc: Worm cultivation temperature in C
+    quantity: '?'
 - neurodata_type_def: MultiChannelVolumeSeries
   neurodata_type_inc: TimeSeries
   doc: Time series of volumetric data with multiple channels
   attributes:
   - name: scan_line_rate
     dtype: float32
     doc: Lines imaged per second.
@@ -69,15 +71,15 @@
     quantity: '?'
   - name: exposure_time
     dtype: float32
     dims:
     - channels
     shape:
     - null
-    doc: Exposure time of the sample; often the inverse of the frequency.
+    doc: Exposure time of the sample, in seconds; often the inverse of the frequency.
     quantity: '?'
   - name: power
     dtype: float32
     dims:
     - channels
     shape:
     - null
@@ -121,14 +123,18 @@
     - channel
     shape:
     - null
     - null
     - null
     - null
     doc: Volumetric multichannel data
+  groups:
+  - name: Order_optical_channels
+    neurodata_type_inc: OpticalChannelReferences
+    doc: Ordered list of names of the optical channels in the data
   links:
   - name: imaging_volume
     target_type: ImagingVolume
     doc: Link to ImagingVolume object from which this data was generated.
 - neurodata_type_def: ImagingVolume
   neurodata_type_inc: NWBDataInterface
   doc: An Imaging Volume and its Metadata
@@ -177,30 +183,30 @@
     quantity: '?'
   groups:
   - neurodata_type_inc: OpticalChannelPlus
     doc: An optical channel used to record from an imaging volume
     quantity: '*'
   - name: Order_optical_channels
     neurodata_type_inc: OpticalChannelReferences
-    doc: Order of the optical channels in the data
+    doc: Ordered list of names of the optical channels in the data
   links:
   - name: device
     target_type: Device
     doc: Link to the Device object that was used to record from this electrode.
 - neurodata_type_def: OpticalChannelReferences
   neurodata_type_inc: NWBDataInterface
   doc: wrapper for optical channel references dataset
   datasets:
-  - name: data
+  - name: channels
     dtype: text
     dims:
     - NumChannels
     shape:
     - null
-    doc: Ordered list of optical channels
+    doc: Ordered list of names of optical channels
 - neurodata_type_def: OpticalChannelPlus
   neurodata_type_inc: OpticalChannel
   doc: An optical channel used to record from an imaging volume. Contains both emission
     and excitation bands.
   datasets:
   - name: emission_range
     dtype: float32
```

### Comparing `ndx-multichannel-volume-0.1.0/spec/ndx-multichannel-volume.namespace.yaml` & `ndx-multichannel-volume-0.1.1/spec/ndx-multichannel-volume.namespace.yaml`

 * *Files identical despite different names*

### Comparing `ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/__init__.py` & `ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/ndx_multichannel_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from pynwb.ophys import OnePhotonSeries, OpticalChannel, ImageSegmentation, Fluorescence, CorrectedImageStack, MotionCorrection, RoiResponseSeries
 from datetime import datetime
 from dateutil import tz
 import pandas as pd
 import scipy.io as sio
 from datetime import datetime, timedelta
 
+
+
 # Set path of the namespace.yaml file to the expected install location
 MultiChannelVol_specpath = os.path.join(
     os.path.dirname(__file__),
     'spec',
     'ndx-multichannel-volume.namespace.yaml'
 )
 
@@ -39,23 +41,23 @@
     MultiChannelVol_specpath = os.path.abspath(os.path.join(
         os.path.dirname(__file__),
         '..', '..', '..',
         'spec',
         'ndx-multichannel-volume.namespace.yaml'
     ))
 
-
 # Load the namespace
 load_namespaces(MultiChannelVol_specpath)
 
 # TODO: import your classes here or define your class using get_class to make
 # them accessible at the package level
 CElegansSubject = get_class('CElegansSubject', 'ndx-multichannel-volume')
 OpticalChannelReferences = get_class('OpticalChannelReferences', 'ndx-multichannel-volume')
 OpticalChannelPlus = get_class('OpticalChannelPlus', 'ndx-multichannel-volume')
+MultiChannelVolumeSeries = get_class('MultiChannelVolumeSeries', 'ndx-multichannel-volume')
 
 @register_class('ImagingVolume', 'ndx-multichannel-volume')
 class ImagingVolume(NWBDataInterface):
     """An imaging plane and its metadata."""
 
     __nwbfields__ = ({'name': 'optical_channel_plus', 'child': True},
                      'Order_optical_channels',
@@ -210,30 +212,33 @@
 class MultiChannelVolume(NWBDataInterface):
     """An imaging plane and its metadata."""
 
     __nwbfields__ = ('resolution',
                      'description',
                      'RGBW_channels',
                      'data',
-                     'imaging_volume'
+                     'imaging_volume',
+                     'Order_optical_channels'
                      )
 
     @docval(*get_docval(NWBDataInterface.__init__, 'name'),  # required
             {'name': 'resolution', 'type': 'array_data', 'doc':'pixel resolution of the image', 'shape':[None]},
             {'name': 'imaging_volume', 'type': ImagingVolume, 'doc': 'the Imaging Volume the data was generated from'},
             {'name': 'description', 'type': str, 'doc':'description of image'},
             {'name': 'RGBW_channels', 'doc': 'which channels in image map to RGBW', 'type': 'array_data', 'shape':[None]},
             {'name': 'data', 'doc': 'Volumetric multichannel data', 'type': 'array_data', 'shape':[None]*4},
+            {'name': 'Order_optical_channels', 'type':OpticalChannelReferences, 'doc':'Order of the optical channels in the data'}
     )
     
     def __init__(self, **kwargs):
         keys_to_set = ('resolution',
                        'description',
                        'RGBW_channels',
                        'data',
-                       'imaging_volume'
+                       'imaging_volume',
+                       'Order_optical_channels'
                        )
         args_to_set = popargs_to_dict(keys_to_set, kwargs)
         super().__init__(**kwargs)
 
         for key, val in args_to_set.items():
             setattr(self, key, val)
```

### Comparing `ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/spec/ndx-multichannel-volume.extensions.yaml` & `ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/spec/ndx-multichannel-volume.extensions.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 groups:
 - neurodata_type_def: CElegansSubject
   neurodata_type_inc: Subject
   doc: Subject object with support for C. Elegans specific attributes
   attributes:
   - name: growth_stage_time
     dtype: text
-    doc: amount of time in current growth stage in ISO duration format
+    doc: amount of time in current growth stage in ISO 8601 duration format
+    required: false
   datasets:
   - name: growth_stage
     dtype: text
     doc: Growth stage of C. elegans. One of two-fold, three-fold, L1-L4, YA, OA, duaer,
       post-dauer L4, post-dauer YA, post-dauer OA
   - name: cultivation_temp
     dtype: float32
     doc: Worm cultivation temperature in C
+    quantity: '?'
 - neurodata_type_def: MultiChannelVolumeSeries
   neurodata_type_inc: TimeSeries
   doc: Time series of volumetric data with multiple channels
   attributes:
   - name: scan_line_rate
     dtype: float32
     doc: Lines imaged per second.
@@ -69,15 +71,15 @@
     quantity: '?'
   - name: exposure_time
     dtype: float32
     dims:
     - channels
     shape:
     - null
-    doc: Exposure time of the sample; often the inverse of the frequency.
+    doc: Exposure time of the sample, in seconds; often the inverse of the frequency.
     quantity: '?'
   - name: power
     dtype: float32
     dims:
     - channels
     shape:
     - null
@@ -121,14 +123,18 @@
     - channel
     shape:
     - null
     - null
     - null
     - null
     doc: Volumetric multichannel data
+  groups:
+  - name: Order_optical_channels
+    neurodata_type_inc: OpticalChannelReferences
+    doc: Ordered list of names of the optical channels in the data
   links:
   - name: imaging_volume
     target_type: ImagingVolume
     doc: Link to ImagingVolume object from which this data was generated.
 - neurodata_type_def: ImagingVolume
   neurodata_type_inc: NWBDataInterface
   doc: An Imaging Volume and its Metadata
@@ -177,30 +183,30 @@
     quantity: '?'
   groups:
   - neurodata_type_inc: OpticalChannelPlus
     doc: An optical channel used to record from an imaging volume
     quantity: '*'
   - name: Order_optical_channels
     neurodata_type_inc: OpticalChannelReferences
-    doc: Order of the optical channels in the data
+    doc: Ordered list of names of the optical channels in the data
   links:
   - name: device
     target_type: Device
     doc: Link to the Device object that was used to record from this electrode.
 - neurodata_type_def: OpticalChannelReferences
   neurodata_type_inc: NWBDataInterface
   doc: wrapper for optical channel references dataset
   datasets:
-  - name: data
+  - name: channels
     dtype: text
     dims:
     - NumChannels
     shape:
     - null
-    doc: Ordered list of optical channels
+    doc: Ordered list of names of optical channels
 - neurodata_type_def: OpticalChannelPlus
   neurodata_type_inc: OpticalChannel
   doc: An optical channel used to record from an imaging volume. Contains both emission
     and excitation bands.
   datasets:
   - name: emission_range
     dtype: float32
```

### Comparing `ndx-multichannel-volume-0.1.0/src/pynwb/MultiChannelVol/spec/ndx-multichannel-volume.namespace.yaml` & `ndx-multichannel-volume-0.1.1/src/pynwb/ndx_multichannel_volume/spec/ndx-multichannel-volume.namespace.yaml`

 * *Files identical despite different names*

