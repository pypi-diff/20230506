# Comparing `tmp/pyaipersonality-0.0.5.tar.gz` & `tmp/pyaipersonality-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-0.0.5.tar", last modified: Thu May  4 22:57:43 2023, max compression
+gzip compressed data, was "pyaipersonality-0.0.6.tar", last modified: Sat May  6 19:06:07 2023, max compression
```

## Comparing `pyaipersonality-0.0.5.tar` & `pyaipersonality-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     8362 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7869 2023-05-04 22:49:56.000000 pyaipersonality-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.899259 pyaipersonality-0.0.5/pyaipersonality/
--rw-rw-rw-   0        0        0     8393 2023-05-04 22:36:59.000000 pyaipersonality-0.0.5/pyaipersonality/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.915263 pyaipersonality-0.0.5/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0     8362 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-05-04 21:34:14.000000 pyaipersonality-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.280325 pyaipersonality-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     9224 2023-05-06 19:06:07.279325 pyaipersonality-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8731 2023-05-06 19:04:54.000000 pyaipersonality-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.254323 pyaipersonality-0.0.6/pyaipersonality/
+-rw-rw-rw-   0        0        0     8636 2023-05-06 19:04:20.000000 pyaipersonality-0.0.6/pyaipersonality/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 19:06:07.278323 pyaipersonality-0.0.6/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0     9224 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-06 19:06:07.000000 pyaipersonality-0.0.6/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 19:06:07.281324 pyaipersonality-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-06 19:04:50.000000 pyaipersonality-0.0.6/setup.py
```

### Comparing `pyaipersonality-0.0.5/LICENSE` & `pyaipersonality-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.5/PKG-INFO` & `pyaipersonality-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyAIPersonality
 
+![GitHub license](https://img.shields.io/github/license/ParisNeo/PyAIPersonality)
+![GitHub issues](https://img.shields.io/github/issues/ParisNeo/PyAIPersonality)
+![GitHub stars](https://img.shields.io/github/stars/ParisNeo/PyAIPersonality)
+![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
+[![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
+[![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
+[![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
+
+[![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
+
 ## Current version : 0.0.4 (HAL9000)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
```

### Comparing `pyaipersonality-0.0.5/README.md` & `pyaipersonality-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # PyAIPersonality
 
+![GitHub license](https://img.shields.io/github/license/ParisNeo/PyAIPersonality)
+![GitHub issues](https://img.shields.io/github/issues/ParisNeo/PyAIPersonality)
+![GitHub stars](https://img.shields.io/github/stars/ParisNeo/PyAIPersonality)
+![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
+[![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
+[![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
+[![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
+
+[![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
+
 ## Current version : 0.0.4 (HAL9000)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
```

### Comparing `pyaipersonality-0.0.5/pyaipersonality/__init__.py` & `pyaipersonality-0.0.6/pyaipersonality/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,43 +81,50 @@
             if not self.personality_package_path.exists():
                 raise ValueError("The provided path does not exist.")
 
             # Validate that the path format is OK with at least a config.yaml file present in the folder
             if not self.personality_package_path.is_dir():
                 raise ValueError("The provided path is not a folder.")
 
-            # Verify that there is at least a configuration file
-            config_file = self.personality_package_path / "config.yaml"
-            if not config_file.is_file():
-                raise ValueError("The provided folder does not contain a config.yaml file.")
-
             # Open and store the personality
-            self.load_personality(config_file)
+            self.load_personality(personality_package_path)
 
 
-    def load_personality(self, file_path):
+    def load_personality(self, package_path:Path|str=None):
         """
         Load the personality data from a YAML file and set it as attributes of the class.
 
         Parameters:
-        file_path (str or Path): The path to the YAML file containing the personality data.
+        file_path (str or Path): The path to the YAML file containing the personality data. 
+        If none, the current package path is used
 
         Returns:
         dict: A dictionary containing the personality data.
         """
-        with open(file_path, 'r', encoding='utf-8') as stream:
+        if package_path is None:
+            package_path = self.personality_package_path
+        else:
+            package_path = Path(package_path)
+        # Verify that there is at least a configuration file
+        config_file = package_path / "config.yaml"
+        if not config_file.exists():
+            raise ValueError(f"The provided folder {package_path} does not exist.")
+
+
+        with open(config_file, 'r', encoding='utf-8') as stream:
             config = yaml.safe_load(stream)
 
         # Set the personality attributes
         for key, value in config.items():
             setattr(self, key, value)
 
         # Rework the conditionning to add information
         self.personality_conditioning = self.replace_keys(self.personality_conditioning, self.Conditionning_commands)
 
+        self.personality_package_path = package_path
 
         # Check for a logo file
         logo_path = self.personality_package_path / "assets" / "logo.png"
         if logo_path.is_file():
             self._logo = Image.open(logo_path)
 
         return config
@@ -221,9 +228,7 @@
 
         def replace(match):
             key = match.group(1)
             return replacements.get(key, match.group(0))
 
         output_string = re.sub(pattern, replace, input_string)
         return output_string
-    
-
```

### Comparing `pyaipersonality-0.0.5/pyaipersonality.egg-info/PKG-INFO` & `pyaipersonality-0.0.6/pyaipersonality.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: pyaipersonality
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/PyAIPersonality
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # PyAIPersonality
 
+![GitHub license](https://img.shields.io/github/license/ParisNeo/PyAIPersonality)
+![GitHub issues](https://img.shields.io/github/issues/ParisNeo/PyAIPersonality)
+![GitHub stars](https://img.shields.io/github/stars/ParisNeo/PyAIPersonality)
+![GitHub forks](https://img.shields.io/github/forks/ParisNeo/PyAIPersonality)
+[![Discord](https://img.shields.io/discord/1092918764925882418?color=7289da&label=Discord&logo=discord&logoColor=ffffff)](https://discord.gg/4rR282WJb6)
+[![Follow me on Twitter](https://img.shields.io/twitter/follow/SpaceNerduino?style=social)](https://twitter.com/SpaceNerduino)
+[![Follow Me on YouTube](https://img.shields.io/badge/Follow%20Me%20on-YouTube-red?style=flat&logo=youtube)](https://www.youtube.com/user/Parisneo)
+
+[![PyPI](https://img.shields.io/pypi/v/pyaipersonality.svg)](https://pypi.org/project/pyaipersonality/)
+
 ## Current version : 0.0.4 (HAL9000)
 ## Main developer [ParisNeo](https://github.com/ParisNeo)
 
 PyAIPersonality is a Python library for defining AI personalities for AI-based models. With PyAIPersonality, you can define a file format, assets, and personalized scripts to create unique AI personalities.
 
 ## Installation
```

### Comparing `pyaipersonality-0.0.5/setup.py` & `pyaipersonality-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="0.0.5",
+    version="0.0.6",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
```

