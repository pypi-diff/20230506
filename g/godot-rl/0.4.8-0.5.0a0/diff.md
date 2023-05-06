# Comparing `tmp/godot_rl-0.4.8.tar.gz` & `tmp/godot_rl-0.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "godot_rl-0.4.8.tar", last modified: Mon Mar 27 19:03:33 2023, max compression
+gzip compressed data, was "/home/edward/play/godot/godot_rl/tmp/godot_rl_agents/dist/.tmp-sg_t1odn/godot_rl-0.5.0a0.tar", last modified: Sat May  6 07:41:50 2023, max compression
```

## Comparing `godot_rl-0.4.8.tar` & `godot_rl-0.5.0a0.tar`

### file list

```diff
@@ -1,40 +1,44 @@
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1071 2023-01-10 09:17:14.000000 godot_rl-0.4.8/LICENSE
--rw-rw-r--   0 edward    (1000) edward    (1000)     6758 2023-03-27 19:03:33.989659 godot_rl-0.4.8/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)     5689 2023-03-27 18:47:11.000000 godot_rl-0.4.8/README.md
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/__init__.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl/core/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/core/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)    11880 2023-03-22 20:03:08.000000 godot_rl-0.4.8/godot_rl/core/godot_env.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     3152 2023-03-08 15:34:57.000000 godot_rl-0.4.8/godot_rl/core/utils.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl/custom_models/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/custom_models/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     3760 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/custom_models/attention_model.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl/download_utils/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/download_utils/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1191 2023-03-02 07:42:57.000000 godot_rl-0.4.8/godot_rl/download_utils/download_examples.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1746 2023-03-02 07:42:57.000000 godot_rl-0.4.8/godot_rl/download_utils/download_godot_editor.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      945 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/download_utils/from_hub.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     3595 2023-03-27 19:02:45.000000 godot_rl-0.4.8/godot_rl/main.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl/wrappers/
--rw-rw-r--   0 edward    (1000) edward    (1000)        0 2023-01-10 09:17:14.000000 godot_rl-0.4.8/godot_rl/wrappers/__init__.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     1475 2023-01-19 19:11:22.000000 godot_rl-0.4.8/godot_rl/wrappers/clean_rl_wrapper.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     5668 2023-03-22 19:53:29.000000 godot_rl-0.4.8/godot_rl/wrappers/ray_wrapper.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     5566 2023-03-27 14:33:38.000000 godot_rl-0.4.8/godot_rl/wrappers/sample_factory_wrapper.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     2349 2023-03-27 18:47:11.000000 godot_rl-0.4.8/godot_rl/wrappers/stable_baselines_wrapper.py
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/godot_rl.egg-info/
--rw-rw-r--   0 edward    (1000) edward    (1000)     6758 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/PKG-INFO
--rw-rw-r--   0 edward    (1000) edward    (1000)      932 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      242 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/entry_points.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        1 2023-01-10 09:21:07.000000 godot_rl-0.4.8/godot_rl.egg-info/not-zip-safe
--rw-rw-r--   0 edward    (1000) edward    (1000)      517 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/requires.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)        9 2023-03-27 19:03:33.000000 godot_rl-0.4.8/godot_rl.egg-info/top_level.txt
--rw-rw-r--   0 edward    (1000) edward    (1000)      886 2023-03-27 18:47:11.000000 godot_rl-0.4.8/pyproject.toml
--rw-rw-r--   0 edward    (1000) edward    (1000)     1239 2023-03-27 19:03:33.989659 godot_rl-0.4.8/setup.cfg
-drwxrwxr-x   0 edward    (1000) edward    (1000)        0 2023-03-27 19:03:33.989659 godot_rl-0.4.8/tests/
--rw-rw-r--   0 edward    (1000) edward    (1000)     1333 2023-01-17 19:48:01.000000 godot_rl-0.4.8/tests/test_action_space_proprocessor.py
--rw-rw-r--   0 edward    (1000) edward    (1000)      421 2023-01-10 09:17:14.000000 godot_rl-0.4.8/tests/test_call_method.py
--rw-rw-r--   0 edward    (1000) edward    (1000)     3358 2023-03-22 20:04:02.000000 godot_rl-0.4.8/tests/test_godot_env.py
--rw-r--r--   0 edward    (1000) edward    (1000)      588 2023-03-27 18:47:11.000000 godot_rl-0.4.8/tests/test_sb3_training.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/
+-rw-r--r--   0 edward    (1000) edward    (1000)     1071 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/LICENSE
+-rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/PKG-INFO
+-rw-r--r--   0 edward    (1000) edward    (1000)     6748 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/README.md
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.586258 godot_rl-0.5.0a0/godot_rl/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/__init__.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/core/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)    11885 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/godot_env.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3181 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/core/utils.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/custom_models/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3760 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/download_utils/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1191 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1746 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      945 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3595 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/main.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     1475 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/
+-rw-r--r--   0 edward    (1000) edward    (1000)        0 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/__init__.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     2855 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/onnx/stable_baselines_export.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     5668 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     5566 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     2349 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/godot_rl/wrappers/stable_baselines_wrapper.py
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.590258 godot_rl-0.5.0a0/godot_rl.egg-info/
+-rw-r--r--   0 edward    (1000) edward    (1000)     7819 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO
+-rw-r--r--   0 edward    (1000) edward    (1000)     1047 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)      242 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/entry_points.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        1 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/not-zip-safe
+-rw-r--r--   0 edward    (1000) edward    (1000)      534 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/requires.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)        9 2023-05-06 07:41:50.000000 godot_rl-0.5.0a0/godot_rl.egg-info/top_level.txt
+-rw-r--r--   0 edward    (1000) edward    (1000)      887 2023-05-06 07:41:12.000000 godot_rl-0.5.0a0/pyproject.toml
+-rw-r--r--   0 edward    (1000) edward    (1000)     1258 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/setup.cfg
+drwxr-xr-x   0 edward    (1000) edward    (1000)        0 2023-05-06 07:41:50.594258 godot_rl-0.5.0a0/tests/
+-rw-r--r--   0 edward    (1000) edward    (1000)     1333 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      421 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_call_method.py
+-rw-r--r--   0 edward    (1000) edward    (1000)     3358 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_godot_env.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      929 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_onnx_export.py
+-rw-r--r--   0 edward    (1000) edward    (1000)      588 2023-05-06 07:37:30.000000 godot_rl-0.5.0a0/tests/test_sb3_training.py
```

### Comparing `godot_rl-0.4.8/LICENSE` & `godot_rl-0.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/PKG-INFO` & `godot_rl-0.5.0a0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: godot_rl
-Version: 0.4.8
-Summary: A Deep Reinforcement Learning package for the Godot game engine
-Author: Edward Beeching
-Author-email: Edward Beeching <edbeeching@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
-Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: sb3
-Provides-Extra: sf
-Provides-Extra: rllib
-Provides-Extra: clean-rl
-Provides-Extra: all
-License-File: LICENSE
-
 # Godot RL Agents
 
 Feel free to join our [Discord](https://discord.gg/HMMD2J8SxY) for help and discussions about Godot RL Agents.
 
 Godot RL Agents is a fully Open Source package that allows video game creators, AI researchers and hobbyists the opportunity to learn complex behaviors for their Non Player Characters or agents.
 This repository provides:
 
@@ -57,21 +24,22 @@
 
 1. Install the Godot RL Agents library: (if you are new to python, pip and conda, read this [guide](https://www.machinelearningplus.com/deployment/conda-create-environment-and-everything-you-need-to-know-to-manage-conda-virtual-environment/))
 
 ```bash
 pip install godot-rl
 ```
 
-1. Download one, or more of [examples](https://github.com/edbeeching/godot_rl_agents_examples), such as BallChase, JumperHard, FlyBy.
+2. Download one, or more of [examples](https://github.com/edbeeching/godot_rl_agents_examples), such as BallChase, JumperHard, FlyBy.
 
 ```bash
 gdrl.env_from_hub -r edbeeching/godot_rl_JumperHard 
 ```
+You may need to example run permissions on the game executable. `chmod +x examples/godot_rl_JumperHard/bin/JumperHard.x86_64`
 
-1. Train and visualize 
+3. Train and visualize 
 
 ```bash
 gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --viz
 ```
 
 ### In editor interactive training
 
@@ -83,14 +51,20 @@
 
 ### Creating a custom environment
 
 There is a dedicated tutorial on creating custom environments [here](docs/CUSTOM_ENV.md). We recommend following this tutorial before trying to create your own environment.
 
 If you face any issues getting started, please reach out on our discord or raise a github issue.
 
+### Exporting and loading your trained agent in onnx format:
+The latest version of the library provides experimental support for onnx models with the Stable Baselines 3 and rllib training frameworks.
+1. First run train you agent using the sb3 example on the [github repo](https://github.com/edbeeching/godot_rl_agents/blob/main/examples/stable_baselines3_example.py), enabling the option `--onnx_export_path=GameModel.onnx`
+2. Then, using the **mono version** of the Godot Editor, add the onnx model path to the sync node. If you do not seen this option you may need to download the plugin from [source](https://github.com/edbeeching/godot_rl_agents_plugin)
+3. The game should now load and run using the onnx model. If you are having issues building the project, ensure that the contents of the `.csproj` and `.sln` files in you project match that those of the plugin [source](https://github.com/edbeeching/godot_rl_agents_plugin).
+
 ## Advanced usage
 [https://user-images.githubusercontent.com/7275864/209160117-cd95fa6b-67a0-40af-9d89-ea324b301795.mp4](https://user-images.githubusercontent.com/7275864/209160117-cd95fa6b-67a0-40af-9d89-ea324b301795.mp4)
 
 
 Please ensure you have successfully completed the quickstart guide before following this section.
 
 Godot RL Agents supports 4 different RL training frameworks, the links below detail a more in depth guide of how to use a particular backend:
```

### Comparing `godot_rl-0.4.8/godot_rl/core/godot_env.py` & `godot_rl-0.5.0a0/godot_rl/core/godot_env.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         suffixes = {
             "linux": ".x86_64",
             "linux2": ".x86_64",
             "darwin": ".app",
             "win32": ".exe",
         }
         suffix = suffixes[platform]
-        return pathlib.Path(env_path).with_suffix(suffix)
+        return str(pathlib.Path(env_path).with_suffix(suffix))
 
     def check_platform(self, filename: str):
         if platform == "linux" or platform == "linux2":
             # Linux
             assert (
                 pathlib.Path(filename).suffix == ".x86_64"
             ), f"Incorrect file suffix for filename {filename} suffix {pathlib.Path(filename).suffix }. Please provide a .x86_64 file"
```

### Comparing `godot_rl-0.4.8/godot_rl/core/utils.py` & `godot_rl-0.5.0a0/godot_rl/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,12 +82,13 @@
                 counter += space.shape[0]
 
             elif isinstance(space, gym.spaces.Discrete):
 
                 discrete_actions = np.greater(action[:, counter], 0.0)
                 discrete_actions = discrete_actions.astype(np.float32)
                 original_action.append(discrete_actions)
+                counter += 1
 
             else:
                 raise NotImplementedError
 
         return original_action
```

### Comparing `godot_rl-0.4.8/godot_rl/custom_models/attention_model.py` & `godot_rl-0.5.0a0/godot_rl/custom_models/attention_model.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/download_utils/download_examples.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/download_examples.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/download_utils/download_godot_editor.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/download_godot_editor.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/download_utils/from_hub.py` & `godot_rl-0.5.0a0/godot_rl/download_utils/from_hub.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/main.py` & `godot_rl-0.5.0a0/godot_rl/main.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/wrappers/clean_rl_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/clean_rl_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/wrappers/ray_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/ray_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/wrappers/sample_factory_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/sample_factory_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl/wrappers/stable_baselines_wrapper.py` & `godot_rl-0.5.0a0/godot_rl/wrappers/stable_baselines_wrapper.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/godot_rl.egg-info/PKG-INFO` & `godot_rl-0.5.0a0/godot_rl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: godot-rl
-Version: 0.4.8
+Version: 0.5.0a0
 Summary: A Deep Reinforcement Learning package for the Godot game engine
 Author: Edward Beeching
 Author-email: Edward Beeching <edbeeching@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/pypa/godot_rl_agents
 Project-URL: Bug Tracker, https://github.com/pypa/godot_rl_agents/issues
 Platform: unix
@@ -57,21 +57,22 @@
 
 1. Install the Godot RL Agents library: (if you are new to python, pip and conda, read this [guide](https://www.machinelearningplus.com/deployment/conda-create-environment-and-everything-you-need-to-know-to-manage-conda-virtual-environment/))
 
 ```bash
 pip install godot-rl
 ```
 
-1. Download one, or more of [examples](https://github.com/edbeeching/godot_rl_agents_examples), such as BallChase, JumperHard, FlyBy.
+2. Download one, or more of [examples](https://github.com/edbeeching/godot_rl_agents_examples), such as BallChase, JumperHard, FlyBy.
 
 ```bash
 gdrl.env_from_hub -r edbeeching/godot_rl_JumperHard 
 ```
+You may need to example run permissions on the game executable. `chmod +x examples/godot_rl_JumperHard/bin/JumperHard.x86_64`
 
-1. Train and visualize 
+3. Train and visualize 
 
 ```bash
 gdrl --env=gdrl --env_path=examples/godot_rl_JumperHard/bin/JumperHard.x86_64 --viz
 ```
 
 ### In editor interactive training
 
@@ -83,14 +84,20 @@
 
 ### Creating a custom environment
 
 There is a dedicated tutorial on creating custom environments [here](docs/CUSTOM_ENV.md). We recommend following this tutorial before trying to create your own environment.
 
 If you face any issues getting started, please reach out on our discord or raise a github issue.
 
+### Exporting and loading your trained agent in onnx format:
+The latest version of the library provides experimental support for onnx models with the Stable Baselines 3 and rllib training frameworks.
+1. First run train you agent using the sb3 example on the [github repo](https://github.com/edbeeching/godot_rl_agents/blob/main/examples/stable_baselines3_example.py), enabling the option `--onnx_export_path=GameModel.onnx`
+2. Then, using the **mono version** of the Godot Editor, add the onnx model path to the sync node. If you do not seen this option you may need to download the plugin from [source](https://github.com/edbeeching/godot_rl_agents_plugin)
+3. The game should now load and run using the onnx model. If you are having issues building the project, ensure that the contents of the `.csproj` and `.sln` files in you project match that those of the plugin [source](https://github.com/edbeeching/godot_rl_agents_plugin).
+
 ## Advanced usage
 [https://user-images.githubusercontent.com/7275864/209160117-cd95fa6b-67a0-40af-9d89-ea324b301795.mp4](https://user-images.githubusercontent.com/7275864/209160117-cd95fa6b-67a0-40af-9d89-ea324b301795.mp4)
 
 
 Please ensure you have successfully completed the quickstart guide before following this section.
 
 Godot RL Agents supports 4 different RL training frameworks, the links below detail a more in depth guide of how to use a particular backend:
```

### Comparing `godot_rl-0.4.8/godot_rl.egg-info/SOURCES.txt` & `godot_rl-0.5.0a0/godot_rl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,11 +21,14 @@
 godot_rl/download_utils/download_godot_editor.py
 godot_rl/download_utils/from_hub.py
 godot_rl/wrappers/__init__.py
 godot_rl/wrappers/clean_rl_wrapper.py
 godot_rl/wrappers/ray_wrapper.py
 godot_rl/wrappers/sample_factory_wrapper.py
 godot_rl/wrappers/stable_baselines_wrapper.py
+godot_rl/wrappers/onnx/__init__.py
+godot_rl/wrappers/onnx/stable_baselines_export.py
 tests/test_action_space_proprocessor.py
 tests/test_call_method.py
 tests/test_godot_env.py
+tests/test_sb3_onnx_export.py
 tests/test_sb3_training.py
```

### Comparing `godot_rl-0.4.8/godot_rl.egg-info/requires.txt` & `godot_rl-0.5.0a0/godot_rl.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 numpy
 tensorboard
 wget
 huggingface_hub>=0.10
 gym==0.26.2
 stable-baselines3
 huggingface_sb3
+onnx
+onnxruntime
 
 [all]
 numpy==1.23.5
 gym==0.26.2
 stable-baselines3
 huggingface_sb3
 sample-factory
```

### Comparing `godot_rl-0.4.8/pyproject.toml` & `godot_rl-0.5.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "godot_rl"
-version = "0.4.8"
+version = "0.5.0a"
 authors = [
   { name="Edward Beeching", email="edbeeching@gmail.com" },
 ]
 description = "A Deep Reinforcement Learning package for the Godot game engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `godot_rl-0.4.8/setup.cfg` & `godot_rl-0.5.0a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 	numpy
 	tensorboard
 	wget
 	huggingface_hub>=0.10
 	gym==0.26.2
 	stable-baselines3
 	huggingface_sb3
+	onnx
+	onnxruntime
 python_requires = >=3.8
 zip_safe = no
 
 [options.entry_points]
 console_scripts = 
 	gdrl = godot_rl.main:main
 	gdrl.interactive = godot_rl.core.godot_env:interactive
```

### Comparing `godot_rl-0.4.8/tests/test_action_space_proprocessor.py` & `godot_rl-0.5.0a0/tests/test_action_space_proprocessor.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/tests/test_godot_env.py` & `godot_rl-0.5.0a0/tests/test_godot_env.py`

 * *Files identical despite different names*

### Comparing `godot_rl-0.4.8/tests/test_sb3_training.py` & `godot_rl-0.5.0a0/tests/test_sb3_training.py`

 * *Files identical despite different names*

