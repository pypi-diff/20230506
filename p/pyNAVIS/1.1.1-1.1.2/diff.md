# Comparing `tmp/pyNAVIS-1.1.1.tar.gz` & `tmp/pyNAVIS-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyNAVIS-1.1.1.tar", last modified: Sat May  6 10:12:51 2023, max compression
+gzip compressed data, was "pyNAVIS-1.1.2.tar", last modified: Sat May  6 10:23:31 2023, max compression
```

## Comparing `pyNAVIS-1.1.1.tar` & `pyNAVIS-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/
--rw-rw-rw-   0        0        0     5225 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.899722 pyNAVIS-1.1.1/pyNAVIS/
--rw-rw-rw-   0        0        0      399 2023-05-06 10:02:02.000000 pyNAVIS-1.1.1/pyNAVIS/__init__.py
--rw-rw-rw-   0        0        0     8409 2023-05-06 10:00:39.000000 pyNAVIS-1.1.1/pyNAVIS/dataset_gen.py
--rw-rw-rw-   0        0        0    18548 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/functions.py
--rw-rw-rw-   0        0        0     8149 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/generators.py
--rw-rw-rw-   0        0        0    22338 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/loaders.py
--rw-rw-rw-   0        0        0     5287 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/main_settings.py
--rw-rw-rw-   0        0        0     2268 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/objects.py
--rw-rw-rw-   0        0        0    35380 2023-05-06 10:06:46.000000 pyNAVIS-1.1.1/pyNAVIS/plots.py
--rw-rw-rw-   0        0        0     7950 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/report_functions.py
--rw-rw-rw-   0        0        0    10205 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/savers.py
--rw-rw-rw-   0        0        0     9241 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/splitters.py
--rw-rw-rw-   0        0        0     3974 2022-03-30 06:38:38.000000 pyNAVIS-1.1.1/pyNAVIS/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 10:12:51.946938 pyNAVIS-1.1.1/pyNAVIS.egg-info/
--rw-rw-rw-   0        0        0     5225 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-06 10:12:51.000000 pyNAVIS-1.1.1/pyNAVIS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 10:12:51.962733 pyNAVIS-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-05-06 10:10:16.000000 pyNAVIS-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:31.839796 pyNAVIS-1.1.2/
+-rw-rw-rw-   0        0        0     5225 2023-05-06 10:23:31.839796 pyNAVIS-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:31.792595 pyNAVIS-1.1.2/pyNAVIS/
+-rw-rw-rw-   0        0        0      399 2023-05-06 10:02:02.000000 pyNAVIS-1.1.2/pyNAVIS/__init__.py
+-rw-rw-rw-   0        0        0     8409 2023-05-06 10:00:39.000000 pyNAVIS-1.1.2/pyNAVIS/dataset_gen.py
+-rw-rw-rw-   0        0        0    18548 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/functions.py
+-rw-rw-rw-   0        0        0     8149 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/generators.py
+-rw-rw-rw-   0        0        0    22338 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/loaders.py
+-rw-rw-rw-   0        0        0     5287 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/main_settings.py
+-rw-rw-rw-   0        0        0     2268 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/objects.py
+-rw-rw-rw-   0        0        0    35388 2023-05-06 10:22:35.000000 pyNAVIS-1.1.2/pyNAVIS/plots.py
+-rw-rw-rw-   0        0        0     7950 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/report_functions.py
+-rw-rw-rw-   0        0        0    10205 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/savers.py
+-rw-rw-rw-   0        0        0     9241 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/splitters.py
+-rw-rw-rw-   0        0        0     3974 2022-03-30 06:38:38.000000 pyNAVIS-1.1.2/pyNAVIS/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:23:31.824080 pyNAVIS-1.1.2/pyNAVIS.egg-info/
+-rw-rw-rw-   0        0        0     5225 2023-05-06 10:23:31.000000 pyNAVIS-1.1.2/pyNAVIS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-05-06 10:23:31.000000 pyNAVIS-1.1.2/pyNAVIS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:23:31.000000 pyNAVIS-1.1.2/pyNAVIS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-05-06 10:23:31.000000 pyNAVIS-1.1.2/pyNAVIS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-06 10:23:31.000000 pyNAVIS-1.1.2/pyNAVIS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:23:31.839796 pyNAVIS-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-06 10:23:07.000000 pyNAVIS-1.1.2/setup.py
```

### Comparing `pyNAVIS-1.1.1/PKG-INFO` & `pyNAVIS-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.1
+Version: 1.1.2
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Download-URL: https://pypi.org/project/pyNAVIS/
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Keywords: pyNAVIS,NAVIS,neuromorphic engineering,neuromorphic audio processing,neuromorphic sensors
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.1 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.2 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Download-URL: https://
 pypi.org/project/pyNAVIS/ Author: Juan P. Dominguez-Morales Author-email:
 jpdominguez@us.es License: GPL Keywords: pyNAVIS,NAVIS,neuromorphic
 engineering,neuromorphic audio processing,neuromorphic sensors Description-
 Content-Type: text/markdown ## pyNAVIS: an open-source cross-platform
 Neuromorphic Auditory VISualizer
```

### Comparing `pyNAVIS-1.1.1/pyNAVIS/dataset_gen.py` & `pyNAVIS-1.1.2/pyNAVIS/dataset_gen.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/functions.py` & `pyNAVIS-1.1.2/pyNAVIS/functions.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/generators.py` & `pyNAVIS-1.1.2/pyNAVIS/generators.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/loaders.py` & `pyNAVIS-1.1.2/pyNAVIS/loaders.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/main_settings.py` & `pyNAVIS-1.1.2/pyNAVIS/main_settings.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/objects.py` & `pyNAVIS-1.1.2/pyNAVIS/objects.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/plots.py` & `pyNAVIS-1.1.2/pyNAVIS/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 A value of 10 in dot_freq means that for every 10 spikes, only 1 will be plotted. This helps reducing lag when plotting heavy files.
         """
         if verbose:
             start_time = time.time()
         # REPRESENTATION
         plt.style.use('seaborn-whitegrid')
         spk_fig = plt.figure()
-        spk_fig.canvas.set_window_title(graph_title)
+        spk_fig.canvas.manager.set_window_title(graph_title)
 
         random.seed(0)
 
         mid_address = settings.num_channels * (settings.on_off_both + 1)
 
         if start_at_zero and spikes_file.min_ts != 0:
             Functions.adapt_timestamps(spikes_file, settings)
```

### Comparing `pyNAVIS-1.1.1/pyNAVIS/report_functions.py` & `pyNAVIS-1.1.2/pyNAVIS/report_functions.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/savers.py` & `pyNAVIS-1.1.2/pyNAVIS/savers.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/splitters.py` & `pyNAVIS-1.1.2/pyNAVIS/splitters.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS/utils.py` & `pyNAVIS-1.1.2/pyNAVIS/utils.py`

 * *Files identical despite different names*

### Comparing `pyNAVIS-1.1.1/pyNAVIS.egg-info/PKG-INFO` & `pyNAVIS-1.1.2/pyNAVIS.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNAVIS
-Version: 1.1.1
+Version: 1.1.2
 Summary: Useful tools to analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS
 Download-URL: https://pypi.org/project/pyNAVIS/
 Author: Juan P. Dominguez-Morales
 Author-email: jpdominguez@us.es
 License: GPL
 Keywords: pyNAVIS,NAVIS,neuromorphic engineering,neuromorphic audio processing,neuromorphic sensors
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.1 Summary: Useful tools to
+Metadata-Version: 2.1 Name: pyNAVIS Version: 1.1.2 Summary: Useful tools to
 analyze and process spiking information from neuromorphic auditory sensors.
 Home-page: https://github.com/jpdominguez/pyNAVIS Download-URL: https://
 pypi.org/project/pyNAVIS/ Author: Juan P. Dominguez-Morales Author-email:
 jpdominguez@us.es License: GPL Keywords: pyNAVIS,NAVIS,neuromorphic
 engineering,neuromorphic audio processing,neuromorphic sensors Description-
 Content-Type: text/markdown ## pyNAVIS: an open-source cross-platform
 Neuromorphic Auditory VISualizer
```

### Comparing `pyNAVIS-1.1.1/setup.py` & `pyNAVIS-1.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     README = readme_file.read()
 """
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 """
 setup_args = dict(
     name='pyNAVIS',
-    version='1.1.1',
+    version='1.1.2',
     description='Useful tools to analyze and process spiking information from neuromorphic auditory sensors.',
     long_description_content_type="text/markdown",
     long_description=README,
     license='GPL',
     packages=find_packages(),
     author='Juan P. Dominguez-Morales',
     author_email='jpdominguez@us.es',
```

