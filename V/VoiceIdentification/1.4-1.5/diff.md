# Comparing `tmp/VoiceIdentification-1.4.tar.gz` & `tmp/VoiceIdentification-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoiceIdentification-1.4.tar", last modified: Mon Apr 24 16:42:20 2023, max compression
+gzip compressed data, was "VoiceIdentification-1.5.tar", last modified: Sat May  6 17:30:48 2023, max compression
```

## Comparing `VoiceIdentification-1.4.tar` & `VoiceIdentification-1.5.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 16:42:20.873555 VoiceIdentification-1.4/
--rw-rw-rw-   0        0        0    15395 2023-04-24 16:42:20.857950 VoiceIdentification-1.4/PKG-INFO
--rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 16:42:20.842469 VoiceIdentification-1.4/VoiceIdentification.egg-info/
--rw-rw-rw-   0        0        0    15395 2023-04-24 16:42:20.000000 VoiceIdentification-1.4/VoiceIdentification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-04-24 16:42:20.000000 VoiceIdentification-1.4/VoiceIdentification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 16:42:20.000000 VoiceIdentification-1.4/VoiceIdentification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      285 2023-04-24 16:42:20.000000 VoiceIdentification-1.4/VoiceIdentification.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-24 16:42:20.000000 VoiceIdentification-1.4/VoiceIdentification.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 16:42:20.873555 VoiceIdentification-1.4/setup.cfg
--rw-rw-rw-   0        0        0     2898 2023-04-24 16:41:55.000000 VoiceIdentification-1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 16:42:20.857950 VoiceIdentification-1.4/voice_identification/
--rw-rw-rw-   0        0        0     1965 2023-04-14 09:21:43.000000 VoiceIdentification-1.4/voice_identification/Container.py
--rw-rw-rw-   0        0        0     2142 2023-04-23 15:28:45.000000 VoiceIdentification-1.4/voice_identification/Engine.py
--rw-rw-rw-   0        0        0       17 2023-04-23 17:14:26.000000 VoiceIdentification-1.4/voice_identification/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/
+-rw-rw-rw-   0        0        0    15395 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.085768 VoiceIdentification-1.5/VoiceIdentification.egg-info/
+-rw-rw-rw-   0        0        0    15395 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      285 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2897 2023-05-06 17:29:26.000000 VoiceIdentification-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/voice_identification/
+-rw-rw-rw-   0        0        0      101 2023-05-06 17:28:21.000000 VoiceIdentification-1.5/voice_identification/__init___.py
+-rw-rw-rw-   0        0        0      313 2023-05-06 17:23:40.000000 VoiceIdentification-1.5/voice_identification/create.py
```

### Comparing `VoiceIdentification-1.4/PKG-INFO` & `VoiceIdentification-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.4
+Version: 1.5
 Summary: A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. 
 Home-page: https://github.com/SriBalajiSMVEC/voice_identification
 Author: BalajiSanthanam
 Author-email: sribalaji2112@gmail.com
 License: BSD 3-Clause License
 Keywords: biometric speaker recognition voice sphinx google wit bing api houndify ibm snowboy voice print identification security
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.4 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.5 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.4/README.md` & `VoiceIdentification-1.5/README.md`

 * *Files identical despite different names*

### Comparing `VoiceIdentification-1.4/VoiceIdentification.egg-info/PKG-INFO` & `VoiceIdentification-1.5/VoiceIdentification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.4
+Version: 1.5
 Summary: A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. 
 Home-page: https://github.com/SriBalajiSMVEC/voice_identification
 Author: BalajiSanthanam
 Author-email: sribalaji2112@gmail.com
 License: BSD 3-Clause License
 Keywords: biometric speaker recognition voice sphinx google wit bing api houndify ibm snowboy voice print identification security
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.4 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.5 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.4/setup.py` & `VoiceIdentification-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 
 # Use the README.md content for the long description:
 with io.open("README.md", encoding="utf-8") as fileObj:
     long_description = fileObj.read()
 
 setup(
     name='VoiceIdentification',
-    version=1.4,
+    version=1.5,
     url='https://github.com/SriBalajiSMVEC/voice_identification',
     author='BalajiSanthanam',
     author_email='sribalaji2112@gmail.com',
     description=('A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. '),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='BSD 3-Clause License',
     packages=['voice_identification'],
-    package_data={'voice_identifier': ['voice_identifier/*']},
+    package_data={'voice_identifier': ['voice_identifier/']},
     test_suite='tests',
     install_requires=['pyobjc-core;platform_system=="Darwin"',
                       'pyobjc;platform_system=="Darwin"',
                       'python3-Xlib;platform_system=="Linux" and python_version>="3.0"',
                       'python-xlib;platform_system=="Linux" and python_version<"3.0"',
                       'pymsgbox',
                       'pytweening>=1.0.4',
```

