# Comparing `tmp/taskAutom-7.19.3.tar.gz` & `tmp/taskAutom-7.19.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-7.19.3.tar", last modified: Fri May  5 17:31:30 2023, max compression
+gzip compressed data, was "taskAutom-7.19.4.tar", last modified: Sat May  6 14:32:46 2023, max compression
```

## Comparing `taskAutom-7.19.3.tar` & `taskAutom-7.19.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.3/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-05 17:31:30.387546 taskAutom-7.19.3/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.3/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 17:31:30.387546 taskAutom-7.19.3/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-05 13:39:44.000000 taskAutom-7.19.3/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-05 13:39:49.000000 taskAutom-7.19.3/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    65612 2023-05-05 17:29:59.000000 taskAutom-7.19.3/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 17:31:30.387546 taskAutom-7.19.3/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-05 17:31:30.000000 taskAutom-7.19.3/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-7.19.4/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-06 14:32:46.802196 taskAutom-7.19.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-7.19.4/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-06 14:32:46.802196 taskAutom-7.19.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1000 2023-05-06 14:32:36.000000 taskAutom-7.19.4/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       53 2023-05-06 14:32:25.000000 taskAutom-7.19.4/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    65695 2023-05-06 14:32:16.000000 taskAutom-7.19.4/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-06 14:32:46.802196 taskAutom-7.19.4/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      513 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-05-06 14:32:46.000000 taskAutom-7.19.4/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-7.19.3/LICENSE` & `taskAutom-7.19.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.3/PKG-INFO` & `taskAutom-7.19.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.3
+Version: 7.19.4
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-7.19.3/README.md` & `taskAutom-7.19.4/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-7.19.3/setup.py` & `taskAutom-7.19.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='7.19.3',
+    version='7.19.4',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-7.19.3/src/taskAutom/taskAutom.py` & `taskAutom-7.19.4/src/taskAutom/taskAutom.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
 #logging.basicConfig(level=logging.DEBUG,format='[%(levelname)s] (%(threadName)-10s) %(message)s')
 
-LATEST_VERSION = '7.19.3'
+LATEST_VERSION = '7.19.4'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -738,15 +738,15 @@
 	"""
 	This function renders the script, based both on the Data file (data) and the plugin (py)
 	There are several possibilities for treating the data, depending on the following.
 
 	- groupColumn: how data is filtered
 	- strictOrder: if we follow the order described inside the data file
 	- useHeader: do we pay attention the headers or use numerals instead?
-	- passByRow: do we pass to the module the complete date or only rowByRow? Only valid when strictOrder=no.
+	- passByRow: do we pass to the module the complete data or only rowByRow? Only valid when strictOrder=False.
 
 	Args:
 		IPconnect (_type_): IP of router (or eventually, the grouped data value)
 		dictParam (_type_): dictionary of parameters
 		mod (_type_):       plugin
 		data (_type_):      Pandas DataFrame
 		i (_type_):         id which identifies the IPconnect value
@@ -795,58 +795,60 @@
 		if useHeader is True:
 			pluginData = data[data[groupColumn] == IPconnect]
 		else:
 			pluginData = data[data[0] == IPconnect]
 
 		if passByRow is True:
 
-			# since passByRow is yes, we pass the data to the module row by row
+			# since passByRow is True, we pass the data to the module row by row
 			# hence we apply in here the itertuples() for-loop, which is the default mode.
 			# The length of data is len(data)
 			# The row order is 'j'
 
-			for j, item in enumerate(pluginData.itertuples()):
+			for j, row in enumerate(pluginData.itertuples()):
 				try:
-					aluCliLine = aluCliLine + mod.construir_cliLine(j, item, len(pluginData), mop)
+					aluCliLine = aluCliLine + mod.construir_cliLine(j, row, len(pluginData), mop)
 				except Exception as e:
+					print(f'\nError trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}.')
 					print('\nError: ' + str(e))
-					print('Row: ' + str(item))
-					print(f'Error trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}. Quitting...\n')
-					quit()
+					print('Row: ' + str(row))		
+					print('Quitting...')
+					sys.exit(1)
 
 		else:
 
-			# since passByRow is no, we pass the complete.
+			# since passByRow is False, we pass the complete.
 			# the itertuples() for-loop, will be needed inside the plugin.
 			# this is only possible with strictMode == no.
 			# The length of data is len(data)
 			# The row order is 'j'
 			try:
 				aluCliLine = aluCliLine + mod.construir_cliLine(i, pluginData, len(pluginData), mop)
 			except Exception as e:
-				print('\nError: ' + str(e))
-				print(f'Error trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}. Quitting...\n')
-				quit()			
+				print(f'\nError trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data structure file, {dataFile}, looking for inconsistencies.')
+				print('\nError: ' + str(e))				
+				sys.exit(1)			
 
 	else:
 
-		# Since strictOrder = yes, then we pass to the module
+		# Since strictOrder = True, then we pass to the module
 		# all the data, row by row, by id i, which comes from 
 		# fncRun(). 
 		# Then the length of data is always 1.
 		# The row order is 0
 
 		try:
 			pluginData = list(data.itertuples())[i]
 			aluCliLine = mod.construir_cliLine(0, pluginData, 1, mop)
 		except Exception as e:
+			print(f'\nError trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}.')
 			print('\nError: ' + str(e))
-			print('Row: ' + str(pluginData))
-			print(f'Error trying to use plugin {pluginFilename}.\nVerify variables inside of it, or the data file {dataFile}. Quitting...\n')
-			quit()
+			print('Row: ' + str(pluginData))			
+			print('Quitting...')
+			sys.exit(1)
 
 	return aluCliLine
 
 
 def buildScripts(dictParam):
 	"""
 	This function builds scripts per router. This function must be used
```

### Comparing `taskAutom-7.19.3/taskAutom.egg-info/PKG-INFO` & `taskAutom-7.19.4/taskAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 7.19.3
+Version: 7.19.4
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

