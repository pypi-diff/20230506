# Comparing `tmp/delfino-1.1.0.tar.gz` & `tmp/delfino-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino-1.1.0.tar", max compression
+gzip compressed data, was "delfino-1.1.1.tar", max compression
```

## Comparing `delfino-1.1.0.tar` & `delfino-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1067 2022-12-29 16:34:57.619143 delfino-1.1.0/LICENSE
--rw-r--r--   0        0        0     7669 2022-12-29 16:34:57.619143 delfino-1.1.0/README.md
--rw-r--r--   0        0        0     3816 2022-12-29 16:34:57.619143 delfino-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       34 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/__init__.py
--rw-r--r--   0        0        0      273 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/backports.py
--rw-r--r--   0        0        0       76 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/click_utils/__init__.py
--rw-r--r--   0        0        0    10340 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/click_utils/command.py
--rw-r--r--   0        0        0     3378 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/click_utils/set_from_config.py
--rw-r--r--   0        0        0      270 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/constants.py
--rw-r--r--   0        0        0      182 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/decorators/__init__.py
--rw-r--r--   0        0        0      545 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/decorators/files_folders.py
--rw-r--r--   0        0        0     1754 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/decorators/pass_app_context.py
--rw-r--r--   0        0        0     1545 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/decorators/pass_args.py
--rw-r--r--   0        0        0     4220 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/execution.py
--rw-r--r--   0        0        0        0 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/internal_parameters/__init__.py
--rw-r--r--   0        0        0     5402 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/internal_parameters/completion.py
--rw-r--r--   0        0        0      506 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/internal_parameters/help.py
--rw-r--r--   0        0        0      892 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/internal_parameters/verbosity.py
--rw-r--r--   0        0        0     4567 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/main.py
--rw-r--r--   0        0        0      143 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/models/__init__.py
--rw-r--r--   0        0        0      522 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/models/app_context.py
--rw-r--r--   0        0        0     1217 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/models/pyproject_toml.py
--rw-r--r--   0        0        0     1090 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/terminal_output.py
--rw-r--r--   0        0        0      618 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/utils.py
--rw-r--r--   0        0        0     1350 2022-12-29 16:34:57.619143 delfino-1.1.0/src/delfino/validation.py
--rw-r--r--   0        0        0     9059 1970-01-01 00:00:00.000000 delfino-1.1.0/setup.py
--rw-r--r--   0        0        0     9139 1970-01-01 00:00:00.000000 delfino-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-06 17:30:29.437924 delfino-1.1.1/LICENSE
+-rw-r--r--   0        0        0    17088 2023-05-06 17:30:29.437924 delfino-1.1.1/README.md
+-rw-r--r--   0        0        0     3681 2023-05-06 17:30:29.437924 delfino-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/backports.py
+-rw-r--r--   0        0        0       76 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/__init__.py
+-rw-r--r--   0        0        0    10340 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/command.py
+-rwxr-xr-x   0        0        0     2238 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/command_groups.py
+-rw-r--r--   0        0        0     3378 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/set_from_config.py
+-rw-r--r--   0        0        0      270 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/constants.py
+-rw-r--r--   0        0        0      182 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/files_folders.py
+-rw-r--r--   0        0        0     1754 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/pass_app_context.py
+-rw-r--r--   0        0        0     1545 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/pass_args.py
+-rw-r--r--   0        0        0     4220 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/execution.py
+-rw-r--r--   0        0        0        0 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/__init__.py
+-rw-r--r--   0        0        0     5402 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/completion.py
+-rw-r--r--   0        0        0      506 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/help.py
+-rw-r--r--   0        0        0      892 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/verbosity.py
+-rw-r--r--   0        0        0     4567 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/main.py
+-rw-r--r--   0        0        0      143 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/app_context.py
+-rw-r--r--   0        0        0     1407 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/pyproject_toml.py
+-rw-r--r--   0        0        0     1090 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/terminal_output.py
+-rw-r--r--   0        0        0      618 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/utils.py
+-rw-r--r--   0        0        0     1350 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/validation.py
+-rw-r--r--   0        0        0    18690 1970-01-01 00:00:00.000000 delfino-1.1.1/setup.py
+-rw-r--r--   0        0        0    18558 1970-01-01 00:00:00.000000 delfino-1.1.1/PKG-INFO
```

### Comparing `delfino-1.1.0/LICENSE` & `delfino-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/pyproject.toml` & `delfino-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delfino"
-version = "1.1.0"
+version = "1.1.1"
 description = "A collection of command line helper scripts wrapping tools used during Python development."
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -118,20 +118,14 @@
     "D1",  # Missing docstrings. We rely on code reviews. Names are often descriptive enough and don't need additional docstring.
     "D202",  # "No blank lines allowed after function docstring" is false positive caused by black formatter.
     "D204",  # "1 blank line required after class docstring"
     "D401",  # "First line should be in imperative mood"
     "D413",  # "Missing blank line after last section"
 ]
 
-[tool.delfino]
-reports_directory = "reports"
-sources_directory = "src"
-tests_directory = "tests"
-test_types = ["unit", "integration"]
-
 [tool.delfino.plugins.delfino-core]
 disable_commands = ['build-docker']
 
 
 #[tool.delfino.dockerhub]
 #username = "radeklat"
 #build_for_platforms = [
```

### Comparing `delfino-1.1.0/src/delfino/click_utils/command.py` & `delfino-1.1.1/src/delfino/click_utils/command.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/click_utils/set_from_config.py` & `delfino-1.1.1/src/delfino/click_utils/set_from_config.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/decorators/files_folders.py` & `delfino-1.1.1/src/delfino/decorators/files_folders.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/decorators/pass_app_context.py` & `delfino-1.1.1/src/delfino/decorators/pass_app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/decorators/pass_args.py` & `delfino-1.1.1/src/delfino/decorators/pass_args.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/execution.py` & `delfino-1.1.1/src/delfino/execution.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/internal_parameters/completion.py` & `delfino-1.1.1/src/delfino/internal_parameters/completion.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/internal_parameters/verbosity.py` & `delfino-1.1.1/src/delfino/internal_parameters/verbosity.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/main.py` & `delfino-1.1.1/src/delfino/main.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/models/app_context.py` & `delfino-1.1.1/src/delfino/models/app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/models/pyproject_toml.py` & `delfino-1.1.1/src/delfino/models/pyproject_toml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from pathlib import Path
-from typing import Any, Dict, Optional, Set
+from typing import Any, Dict, List, Optional, Set
 
 from pydantic import BaseModel, Extra, Field
 
 from delfino.constants import DEFAULT_LOCAL_COMMANDS_DIRECTORY
 
 
 class PluginConfig(BaseModel):
-    enable_commands: Set[str] = set()
-    disable_commands: Set[str] = set()
+    enable_commands: Set[str] = Field(default_factory=set)
+    disable_commands: Set[str] = Field(default_factory=set)
+    command_groups: Dict[str, List[str]] = Field(default_factory=dict)
 
     @classmethod
     def empty(cls):
         return cls()
 
     class Config:
         extra = Extra.allow  # Allows arbitrary plugin-specific keys
 
 
 class Delfino(BaseModel):
     local_commands_directory: Path = DEFAULT_LOCAL_COMMANDS_DIRECTORY
     plugins: Dict[str, PluginConfig] = Field(default_factory=dict)
+    command_groups: Dict[str, List[str]] = Field(default_factory=dict)
 
     class Config:
         extra = Extra.allow
 
 
 class Poetry(BaseModel):
     name: str
```

### Comparing `delfino-1.1.0/src/delfino/terminal_output.py` & `delfino-1.1.1/src/delfino/terminal_output.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/utils.py` & `delfino-1.1.1/src/delfino/utils.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.0/src/delfino/validation.py` & `delfino-1.1.1/src/delfino/validation.py`

 * *Files identical despite different names*

