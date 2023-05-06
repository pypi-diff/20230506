# Comparing `tmp/delfino-1.1.1.tar.gz` & `tmp/delfino-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino-1.1.1.tar", max compression
+gzip compressed data, was "delfino-1.2.0.tar", max compression
```

## Comparing `delfino-1.1.1.tar` & `delfino-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1067 2023-05-06 17:30:29.437924 delfino-1.1.1/LICENSE
--rw-r--r--   0        0        0    17088 2023-05-06 17:30:29.437924 delfino-1.1.1/README.md
--rw-r--r--   0        0        0     3681 2023-05-06 17:30:29.437924 delfino-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/__init__.py
--rw-r--r--   0        0        0      273 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/backports.py
--rw-r--r--   0        0        0       76 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/__init__.py
--rw-r--r--   0        0        0    10340 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/command.py
--rwxr-xr-x   0        0        0     2238 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/command_groups.py
--rw-r--r--   0        0        0     3378 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/click_utils/set_from_config.py
--rw-r--r--   0        0        0      270 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/constants.py
--rw-r--r--   0        0        0      182 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/__init__.py
--rw-r--r--   0        0        0      545 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/files_folders.py
--rw-r--r--   0        0        0     1754 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/pass_app_context.py
--rw-r--r--   0        0        0     1545 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/decorators/pass_args.py
--rw-r--r--   0        0        0     4220 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/execution.py
--rw-r--r--   0        0        0        0 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/__init__.py
--rw-r--r--   0        0        0     5402 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/completion.py
--rw-r--r--   0        0        0      506 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/help.py
--rw-r--r--   0        0        0      892 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/internal_parameters/verbosity.py
--rw-r--r--   0        0        0     4567 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/main.py
--rw-r--r--   0        0        0      143 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/__init__.py
--rw-r--r--   0        0        0      522 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/app_context.py
--rw-r--r--   0        0        0     1407 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/models/pyproject_toml.py
--rw-r--r--   0        0        0     1090 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/terminal_output.py
--rw-r--r--   0        0        0      618 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/utils.py
--rw-r--r--   0        0        0     1350 2023-05-06 17:30:29.437924 delfino-1.1.1/src/delfino/validation.py
--rw-r--r--   0        0        0    18690 1970-01-01 00:00:00.000000 delfino-1.1.1/setup.py
--rw-r--r--   0        0        0    18558 1970-01-01 00:00:00.000000 delfino-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-06 20:40:51.841157 delfino-1.2.0/LICENSE
+-rw-r--r--   0        0        0    17473 2023-05-06 20:40:51.841157 delfino-1.2.0/README.md
+-rw-r--r--   0        0        0     3681 2023-05-06 20:40:51.841157 delfino-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/backports.py
+-rw-r--r--   0        0        0       76 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/click_utils/__init__.py
+-rw-r--r--   0        0        0    10340 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/click_utils/command.py
+-rwxr-xr-x   0        0        0     2238 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/click_utils/command_groups.py
+-rw-r--r--   0        0        0     3378 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/click_utils/set_from_config.py
+-rw-r--r--   0        0        0     1343 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/config.py
+-rw-r--r--   0        0        0      270 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/constants.py
+-rw-r--r--   0        0        0      182 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/decorators/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/decorators/files_folders.py
+-rw-r--r--   0        0        0     1754 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/decorators/pass_app_context.py
+-rw-r--r--   0        0        0     1545 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/decorators/pass_args.py
+-rw-r--r--   0        0        0     4220 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/execution.py
+-rw-r--r--   0        0        0        0 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/internal_parameters/__init__.py
+-rw-r--r--   0        0        0     5402 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/internal_parameters/completion.py
+-rw-r--r--   0        0        0      506 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/internal_parameters/help.py
+-rw-r--r--   0        0        0      892 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/internal_parameters/verbosity.py
+-rw-r--r--   0        0        0     4284 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/main.py
+-rw-r--r--   0        0        0      143 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/models/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/models/app_context.py
+-rw-r--r--   0        0        0     1370 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/models/pyproject_toml.py
+-rw-r--r--   0        0        0     1090 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/terminal_output.py
+-rw-r--r--   0        0        0      618 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/utils.py
+-rw-r--r--   0        0        0     1350 2023-05-06 20:40:51.841157 delfino-1.2.0/src/delfino/validation.py
+-rw-r--r--   0        0        0    19083 1970-01-01 00:00:00.000000 delfino-1.2.0/setup.py
+-rw-r--r--   0        0        0    18943 1970-01-01 00:00:00.000000 delfino-1.2.0/PKG-INFO
```

### Comparing `delfino-1.1.1/LICENSE` & `delfino-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/README.md` & `delfino-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,23 @@
 - Poetry: `poetry add --group=dev delfino[completion]`
 - Pipenv: `pipenv install -d delfino[completion]`
 
 to enable [auto-completion](#auto-completion).
 
 # Configuration
 
-All configuration is expected to live in the `pyproject.toml` file.
+All configuration is expected to live in one of the following files:
+
+- `pyproject.toml` in the project root
+- `.pylintrc` in the project root - to allow dev specific config, not source controlled or for non-Python projects
+- `.pylintrc` in the user home directory - for user tools available in the system
+
+If multiple files are discovered, only the highest one in the list will be used.
+
+The format for `.pylintrc` is the same as for `pyproject.toml`.
 
 ## Enabling a plugin
 
 For security reasons, plugins are disabled by default. To enable a plugin, you have to include it in the `pyproject.toml` file:
 
 ```toml
 [tool.delfino.plugins.<PLUGIN_NAME>]
```

### Comparing `delfino-1.1.1/pyproject.toml` & `delfino-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "delfino"
-version = "1.1.1"
+version = "1.2.0"
 description = "A collection of command line helper scripts wrapping tools used during Python development."
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `delfino-1.1.1/src/delfino/click_utils/command.py` & `delfino-1.2.0/src/delfino/click_utils/command.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/click_utils/command_groups.py` & `delfino-1.2.0/src/delfino/click_utils/command_groups.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/click_utils/set_from_config.py` & `delfino-1.2.0/src/delfino/click_utils/set_from_config.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/decorators/files_folders.py` & `delfino-1.2.0/src/delfino/decorators/files_folders.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/decorators/pass_app_context.py` & `delfino-1.2.0/src/delfino/decorators/pass_app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/decorators/pass_args.py` & `delfino-1.2.0/src/delfino/decorators/pass_args.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/execution.py` & `delfino-1.2.0/src/delfino/execution.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/internal_parameters/completion.py` & `delfino-1.2.0/src/delfino/internal_parameters/completion.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/internal_parameters/verbosity.py` & `delfino-1.2.0/src/delfino/internal_parameters/verbosity.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/main.py` & `delfino-1.2.0/src/delfino/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import Any, List, Optional
 
 import click
-import toml
-from pydantic import ValidationError
 
 from delfino.click_utils.command import CommandRegistry
+from delfino.config import ConfigValidationError, load_config
 from delfino.constants import ENTRY_POINT, PYPROJECT_TOML_FILENAME
 from delfino.internal_parameters.completion import install_completion_option, show_completion_option
 from delfino.internal_parameters.help import extended_help_option
 from delfino.internal_parameters.verbosity import log_level_option
 from delfino.models.app_context import AppContext
 from delfino.models.pyproject_toml import PyprojectToml
 from delfino.utils import get_package_manager
@@ -21,27 +20,24 @@
 class Commands(click.MultiCommand):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         sys.path.append(os.getcwd())
 
         self._project_root = Path(os.getcwd())
-        pyproject_toml_path = (self._project_root / PYPROJECT_TOML_FILENAME).relative_to(self._project_root)
 
         # When evaluating available commands, the program should not fail. We save the exception
         # to show it only when a command is executed.
-        self._pyproject_toml_validation_error: Optional[ValidationError] = None
+        self._pyproject_toml_validation_error: Optional[ConfigValidationError] = None
 
         try:
-            self._pyproject_toml = PyprojectToml(file_path=pyproject_toml_path, **toml.load(pyproject_toml_path))
-        except ValidationError as exc:
+            self._pyproject_toml = load_config(self._project_root)
+        except ConfigValidationError as exc:
             self._pyproject_toml = PyprojectToml()
             self._pyproject_toml_validation_error = exc
-        except FileNotFoundError:
-            self._pyproject_toml = PyprojectToml()
 
         self._command_registry = CommandRegistry(
             plugins_configs=self._pyproject_toml.tool.delfino.plugins,
             local_commands_directory=self._pyproject_toml.tool.delfino.local_commands_directory,
         )
 
     def list_commands(self, ctx: click.Context) -> List[str]:
@@ -55,17 +51,15 @@
         if cmd is None:
             return None  # command doesn't exist
 
         if ctx.resilient_parsing:  # do not fail on auto-completion
             return cmd.command
 
         if self._pyproject_toml_validation_error:
-            click.secho(
-                f"Delfino appears to be misconfigured: {self._pyproject_toml_validation_error}", fg="red", err=True
-            )
+            click.secho(str(self._pyproject_toml_validation_error), fg="red", err=True)
             raise click.Abort() from self._pyproject_toml_validation_error
 
         ctx.obj = AppContext(
             project_root=self._project_root,
             pyproject_toml=self._pyproject_toml,
             package_manager=get_package_manager(self._project_root, self._pyproject_toml),
             plugin_config=cmd.package.plugin_config,
```

### Comparing `delfino-1.1.1/src/delfino/models/app_context.py` & `delfino-1.2.0/src/delfino/models/app_context.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/models/pyproject_toml.py` & `delfino-1.2.0/src/delfino/models/pyproject_toml.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,11 @@
     delfino: Delfino = Field(default_factory=Delfino)
 
     class Config:
         allow_population_by_field_name = True
 
 
 class PyprojectToml(BaseModel):
-    file_path: Optional[Path] = None
     tool: Tool = Field(default_factory=Tool)
 
     class Config:
         extra = Extra.allow
```

### Comparing `delfino-1.1.1/src/delfino/terminal_output.py` & `delfino-1.2.0/src/delfino/terminal_output.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/utils.py` & `delfino-1.2.0/src/delfino/utils.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/src/delfino/validation.py` & `delfino-1.2.0/src/delfino/validation.py`

 * *Files identical despite different names*

### Comparing `delfino-1.1.1/setup.py` & `delfino-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 {':python_version < "3.10"': ['importlib-metadata']}
 
 entry_points = \
 {'console_scripts': ['delfino = delfino.main:main', 'mike = delfino.main:main']}
 
 setup_kwargs = {
     'name': 'delfino',
-    'version': '1.1.1',
+    'version': '1.2.0',
     'description': 'A collection of command line helper scripts wrapping tools used during Python development.',
-    'long_description': '<h1 align="center" style="border-bottom: none;">🧰&nbsp;&nbsp;Delfino&nbsp;&nbsp;🧰</h1>\n<h3 align="center">Plugable Click command finder/loader/executor.</h3>\n\n<p align="center">\n    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino?branch=main">\n        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino">\n    </a>\n    <a href="https://app.codecov.io/gh/radeklat/delfino/">\n        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino">\n    </a>\n    <a href="https://github.com/radeklat/delfino/tags">\n        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino">\n    </a>\n    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2023">\n    <a href="https://github.com/radeklat/delfino/commits/main">\n        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino">\n    </a>\n    <a href="https://www.python.org/doc/versions/">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino">\n    </a>\n    <a href="https://pypistats.org/packages/delfino">\n        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino">\n    </a>\n</p>\n\n<!--\n    How to generate TOC from PyCharm:\n    https://github.com/vsch/idea-multimarkdown/wiki/Table-of-Contents-Extension\n-->\n[TOC levels=1,2 markdown formatted bullet hierarchy]: # "Table of content"\n\n# Table of content\n- [What is Delfino](#what-is-delfino)\n  - [Plugins](#plugins)\n- [Installation](#installation)\n- [Configuration](#configuration)\n  - [Enabling a plugin](#enabling-a-plugin)\n  - [Enabling/disabling commands](#enablingdisabling-commands)\n- [Usage](#usage)\n- [Development](#development)\n  - [Commands discovery](#commands-discovery)\n  - [Minimal command](#minimal-command)\n  - [Minimal plugin](#minimal-plugin)\n- [Advanced usage](#advanced-usage)\n  - [Auto-completion](#auto-completion)\n  - [Running external programs](#running-external-programs)\n  - [Optional dependencies](#optional-dependencies)\n  - [Project settings](#project-settings)\n  - [Plugin settings](#plugin-settings)\n  - [Project specific overrides](#project-specific-overrides)\n  - [Grouping commands](#grouping-commands)\n\n# What is Delfino\n\nDelfino is a wrapper around [Click](https://click.palletsprojects.com) command line scripts. It automatically discovers instances of [Click commands](https://click.palletsprojects.com/quickstart/#basic-concepts-creating-a-command) and offers them for execution. However, the biggest power comes from the possibility of creating [plugins](#plugins), which can be distributed as standard Python packages.\n\n## Plugins\n\nPlugins can greatly reduce code duplication and/or promote your own standards in multiple places. For example, you can create a plugin wrapping common linting tools that you use on your projects, including their default configuration. Keeping the rules and creating new projects with the same style suddenly becomes a matter of installing one Python library.\n\nEach plugin can contain one or more Click commands that are automatically discovered and exposed by Delfino. See [`delfino-demo`](https://github.com/radeklat/delfino-demo) for a minimal plugin, which provide a `demo` command printing out a message.\n\nExisting plugins:\n\n| Plugin name                                                  | Description                                                                                        |\n|:-------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|\n| [delfino-demo](https://github.com/radeklat/delfino-demo)     | A minimal plugin example for Delfino. Contains one command printing a message.                     |\n| [delfino-core](https://github.com/radeklat/delfino-core)     | Commands wrapping tools used during every day development (linting, testing, dependencies update). |\n| [delfino-docker](https://github.com/radeklat/delfino-docker) | Docker build helper script.                                                                        |\n\n# Installation\n\n- pip: `pip install delfino`\n- Poetry: `poetry add --group=dev delfino`\n- Pipenv: `pipenv install -d delfino`\n\nor \n\n- pip: `pip install delfino[completion]`\n- Poetry: `poetry add --group=dev delfino[completion]`\n- Pipenv: `pipenv install -d delfino[completion]`\n\nto enable [auto-completion](#auto-completion).\n\n# Configuration\n\nAll configuration is expected to live in the `pyproject.toml` file.\n\n## Enabling a plugin\n\nFor security reasons, plugins are disabled by default. To enable a plugin, you have to include it in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN_NAME>]\n```\n\n## Enabling/disabling commands\n\nBy default, all commands are enabled. Use `enable_commands` or `disable_commands`  to show only a subset of commands. If both used, disabled commands are subtracted from the set of enabled commands.\n\n```toml\n# [tool.delfino.plugins.<PLUGIN_NAME_A>]\n# enable_commands = [<COMMAND_NAME>]\n# disable_commands = [<COMMAND_NAME>]\n\n# [tool.delfino.plugins.<PLUGIN_NAME_B>]\n# enable_commands = [<COMMAND_NAME>]\n# disable_commands = [<COMMAND_NAME>]\n```\n\n# Usage\n\nRun `delfino --help` to see all available commands and their usage.\n\n# Development\n\nDelfino is a simple wrapper around [Click commands](https://click.palletsprojects.com/quickstart/#basic-concepts-creating-a-command). Any Click command will be accepted by Delfino.\n\n## Commands discovery\n\nDelfino looks for any [`click.Command`](https://click.palletsprojects.com/en/8.0.x/api/#click.Command) sub-class in the following locations:\n\n- `commands` folder in the root of the project (next to the `pyproject.toml` file). This location is useful for commands that don\'t need to be replicated in multiple locations/projects.\n- python module import path (`<IMPORT_PATH>`) specified by `entry_point` of [a plugin](#minimal-plugin):\n  ```toml\n  [tool.poetry.plugins] # Optional super table\n\n  [tool.poetry.plugins."delfino.plugin"]\n  "delfino-<PLUGIN_NAME>" = "<IMPORT_PATH>"\n  ```\n\nAny files starting with an underscore, except for `__init__.py`, will be ignored.\n\n> **Warning**\n> Folders are NOT inspected recursively. If you place any commands into nested folders, they will not be loaded by Delfino.\n\n\n## Minimal command\n\n<!-- TODO(Radek): Delfino expects `pyproject.toml` configured. -->\n<!-- TODO(Radek): Delfino expects Poetry or Pipenv to be available. -->\n\n1. Create a `commands` folder:\n   ```shell script\n   mkdir commands\n   ```\n2. Create a `commands/__init__.py` file, with the following content:\n   ```python\n   import click\n   \n   @click.command()\n   def command_test():\n       """Tests commands placed in the `commands` folder are loaded."""\n       print("✨ This command works! ✨")\n   ```\n3. See if Delfino loads the command. Open a terminal and in the root of the project, call: `delfino --help`. You should see something like this:\n   ```text\n   Usage: delfino [OPTIONS] COMMAND [ARGS]...\n   \n   Options:\n     --help  Show this message and exit.\n   \n   Commands:\n     ...\n     command-test            Tests commands placed in the `commands` folder...\n     ...\n   ```\n4. Run the command with `delfino command-test`\n\n## Minimal plugin\n\nIf you\'d like to use one or more commands in multiple places, you can create a plugin. A plugin is just a regular Python package with specific entry point telling Delfino it should use it. It can also be distributed as any other Python packages, for example via Pypi.\n\nThe quickest way to create one is to use a [Delfino plugin cookiecutter template](https://github.com/radeklat/delfino-plugin-cookiecutter-template), which asks you several questions and sets up the whole project.\n\nAlternatively, you can get inspired by [the demo plugin](https://github.com/radeklat/delfino-demo) or any of the other [existing plugins](#plugins).\n\n# Advanced usage\n\n<!--\n## Advanced Command\n\nDelfino adds optional bits of functionality on top of Click. The following example demonstrates some of those:\n\n```python\n# commands/__init__.py\n\nimport click\n\nfrom delfino.contexts import pass_app_context, AppContext\nfrom delfino.validation import assert_pip_package_installed, pyproject_toml_key_missing\n\n@click.command()\n# The `pass_app_context` decorator adds `AppContext` as the first parameter.\n@pass_app_context\ndef command_test(app_context: AppContext):\n   """Tests commands placed in the `commands` folder are loaded."""\n   # Test optional dependencies. Any failing assertion will be printed as:\n   # Command \'<NAME>\' is misconfigured. <ASSERTION ERROR MESSAGE>\n   assert_pip_package_installed("delfino")\n\n   # AppContext contain a parsed `pyproject.toml` file.\n   # Commands can add their config under `[tool.delfino.commands.<COMMAND_NAME>]`.\n   assert "command_test" in app_context.pyproject_toml.tool.delfino.commands, \\\n       pyproject_toml_key_missing("tool.delfino.commands.command_test")\n\n   print(app_context.pyproject_toml.tool.delfino.commands["command-test"])\n```\n-->\n\n## Auto-completion\n\nYou can either attempt to install completions automatically with:\n\n```shell script\ndelfino --install-completion\n```\n\nor generate it with:\n\n```shell script\ndelfino --show-completion\n```\n\nand manually put it in the relevant RC file.\n\nThe auto-completion implementation is dynamic so that every time it is invoked, it uses the current project. Each project can have different commands or disable certain commands it doesn\'t use. And dynamic auto-completion makes sure only the currently available commands will be suggested.\n\nThe downside of this approach is that evaluating what is available each time is slower than a static list of commands.\n\n## Running external programs\n\nIt is up to you how you want to execute external processes as part of commands (if you need to at all). A common way in Python is to use `subprocess.run`. Delfino comes with its own [`run` implementation](https://github.com/radeklat/delfino/blob/main/src/delfino/execution.py#L94), which wraps and simplifies `subprocess.run` for the most common use cases:\n\n- Normalizing `subprocess.run` arguments - you can pass in either a string or a list. Either way, `subprocess.run` will be executed correctly.\n- Handling errors from the execution via the `on_error` argument. Giving the option to either ignore the errors and continue (`PASS`), not continue and clean exit (`EXIT`) or not continue and abort with error code (`ABORT`).\n- Setting environment variables.\n- Logging what is being executed in the debug level.\n\nExample:\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.execution import run, OnError\n\n@click.command()\ndef test():\n    run("pytest tests", on_error=OnError.ABORT)\n```\n\n## Optional dependencies\n\nIf you put several commands into one [plugin](#plugins), you can make some dependencies of some commands [optional](https://python-poetry.org/docs/pyproject#extras). This is useful when a command is not always used, and you don\'t want to install unnecessary dependencies. Instead, you can check if a dependency is installed only when the command is executed with `delfino.validation.assert_pip_package_installed`:\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.validation import assert_pip_package_installed\n\ntry:\n    from git import Repo\nexcept ImportError:\n    pass\n\n@click.command()\ndef git_active_branch():\n    assert_pip_package_installed("gitpython")\n    print(Repo(".").active_branch)\n```\n\nIn the example above, if `gitpython` is not installed, delfino will show the command but will fail with suggestion to install `gitpython` only when the command is executed. You can also add `git_active_branch` into [`disable_commands` config](#enablingdisabling-commands) in places where you don\'t intend to use it.\n\nThis way you can greatly reduce the number of dependencies a plugin brings into a project without a need to have many small plugins.\n\n## Project settings\n\nYou can store an arbitrary object in the Click context as [`click.Context.obj`](https://click.palletsprojects.com/api/#click.Context.obj). Delfino utilizes this object to store an instance of [`AppContext`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/app_context.py), which provides access to project related information. If you need to, you can still attach arbitrary attributes to this object later.\n\nYou can pass this object to your commands by decorating them with [`click.pass_obj`](https://click.palletsprojects.com/api/#click.pass_obj):\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.models.app_context import AppContext\n\n@click.command()\n@click.pass_obj\ndef print_app_version(obj: AppContext):\n    print(obj.pyproject_toml.tool.poetry.version)\n```\n\n## Plugin settings\n\nPlugin settings are expected to live in the `pyproject.toml` file. To prevent naming conflicts, each plugin must put its settings under `tool.delfino.plugins.<PLUGIN_NAME>`. It also allows Delfino to pass these settings directly to commands from these plugins.\n\nDelfino loads, parses, validates and stores plugin settings in [`AppContext.plugin_config`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/app_context.py). If not specified otherwise (see below), it will be an instance of [`PluginConfig`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/pyproject_toml.py), with any extra keys unvalidated and in JSON-like Python objects.\n\nYou can add additional validation to your plugin settings by sub-classing the `PluginConfig` , defining expected keys, default values and/or validation. Delfino utilizes [`pydantic`](https://docs.pydantic.dev/) to create data classes.\n\nDelfino also needs to know, which class to use for the validation. To do that, switch to `delfino.decorators.pass_app_context` instead of [`click.pass_obj`](https://click.palletsprojects.com/api/#click.pass_obj):\n\n```toml\n# pyproject.toml\n\n[tool.delfino.plugins.delfino_login_plugin]\nusername = "user"\n```\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.models.pyproject_toml import PluginConfig\nfrom delfino.models.app_context import AppContext\nfrom delfino.decorators import pass_app_context\n\n\nclass LoginPluginConfig(PluginConfig):\n    login: str\n\n\n@click.command()\n@pass_app_context(LoginPluginConfig)\ndef login(app_context: AppContext[LoginPluginConfig]):\n    print(app_context.plugin_config.login)\n```\n\nThe `AppContext` class is generic. Defining the `PluginConfigType` (such as `AppContext[LoginPluginConfig]` in the example above) enables introspection and type checks.\n\n## Project specific overrides\n\nIt is likely your projects will require slight divergence to the defaults you encode in your scripts. The following sections cover the most common use cases.\n\n### Pass-through arguments\n\nYou can pass additional arguments to downstream tools by decorating commands with the [`decorators.pass_args`](https://github.com/radeklat/delfino/blob/main/src/delfino/decorators/pass_args.py) decorator:\n\n```python\n# commands/__init__.py\n\nfrom typing import Tuple\n\nimport click\nfrom delfino.decorators import pass_args\nfrom delfino.execution import run, OnError\n\n@click.command()\n@pass_args\ndef test(passed_args: Tuple[str, ...]):\n    run(["pytest", "tests", *passed_args], on_error=OnError.ABORT)\n```\n\nThen additional arguments can be passed either via command line after `--`:\n\n```shell script\ndelfino test -- --capture=no\n```\n\nOr via configuration in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN>.test]\npass_args = [\'--capture=no\']\n```\n\nEither way, both will result in executing `pytest tests --capture=no`.\n\n### Files override\n\nYou can override files passed to downstream tools by decorating commands with the [`decorators.files_folders_option`](https://github.com/radeklat/delfino/blob/main/src/delfino/decorators/files_folders.py) decorator:\n\n```python\n# commands/__init__.py\n\nfrom typing import Tuple\n\nimport click\nfrom delfino.decorators import files_folders_option\nfrom delfino.execution import run, OnError\n\n@click.command()\n@files_folders_option\ndef test(files_folders: Tuple[str, ...]):\n    if not files_folders:\n        files_folders = ("tests/unit", "tests/integration")\n    run(["pytest", *files_folders], on_error=OnError.ABORT)\n```\n\nThen the default `"tests/unit", "tests/integration"` folders can be overridden either via command line options `-f`/`--file`/`--folder`:\n\n```shell script\ndelfino test -f tests/other\n```\n\nOr via configuration in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN>.test]\nfiles_folders = [\'tests/other\']\n```\n\nEither way, both will result in executing `pytest tests/other`.\n\n## Grouping commands\n\nOften it is useful to run several commands as a group with a different command name. Click supports calling other commands with [`click.Context.forward`](https://click.palletsprojects.com/api/#click.Context.forward) or [`click.Context.invoke`](https://click.palletsprojects.com/api/#click.Context.invoke).\n\n<!-- TODO(Radek): Add description of `execute_commands_group` once migrated from `delfino-core`. -->\n',
+    'long_description': '<h1 align="center" style="border-bottom: none;">🧰&nbsp;&nbsp;Delfino&nbsp;&nbsp;🧰</h1>\n<h3 align="center">Plugable Click command finder/loader/executor.</h3>\n\n<p align="center">\n    <a href="https://app.circleci.com/pipelines/github/radeklat/delfino?branch=main">\n        <img alt="CircleCI" src="https://img.shields.io/circleci/build/github/radeklat/delfino">\n    </a>\n    <a href="https://app.codecov.io/gh/radeklat/delfino/">\n        <img alt="Codecov" src="https://img.shields.io/codecov/c/github/radeklat/delfino">\n    </a>\n    <a href="https://github.com/radeklat/delfino/tags">\n        <img alt="GitHub tag (latest SemVer)" src="https://img.shields.io/github/tag/radeklat/delfino">\n    </a>\n    <img alt="Maintenance" src="https://img.shields.io/maintenance/yes/2023">\n    <a href="https://github.com/radeklat/delfino/commits/main">\n        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/radeklat/delfino">\n    </a>\n    <a href="https://www.python.org/doc/versions/">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/delfino">\n    </a>\n    <a href="https://pypistats.org/packages/delfino">\n        <img alt="Downloads" src="https://img.shields.io/pypi/dm/delfino">\n    </a>\n</p>\n\n<!--\n    How to generate TOC from PyCharm:\n    https://github.com/vsch/idea-multimarkdown/wiki/Table-of-Contents-Extension\n-->\n[TOC levels=1,2 markdown formatted bullet hierarchy]: # "Table of content"\n\n# Table of content\n- [What is Delfino](#what-is-delfino)\n  - [Plugins](#plugins)\n- [Installation](#installation)\n- [Configuration](#configuration)\n  - [Enabling a plugin](#enabling-a-plugin)\n  - [Enabling/disabling commands](#enablingdisabling-commands)\n- [Usage](#usage)\n- [Development](#development)\n  - [Commands discovery](#commands-discovery)\n  - [Minimal command](#minimal-command)\n  - [Minimal plugin](#minimal-plugin)\n- [Advanced usage](#advanced-usage)\n  - [Auto-completion](#auto-completion)\n  - [Running external programs](#running-external-programs)\n  - [Optional dependencies](#optional-dependencies)\n  - [Project settings](#project-settings)\n  - [Plugin settings](#plugin-settings)\n  - [Project specific overrides](#project-specific-overrides)\n  - [Grouping commands](#grouping-commands)\n\n# What is Delfino\n\nDelfino is a wrapper around [Click](https://click.palletsprojects.com) command line scripts. It automatically discovers instances of [Click commands](https://click.palletsprojects.com/quickstart/#basic-concepts-creating-a-command) and offers them for execution. However, the biggest power comes from the possibility of creating [plugins](#plugins), which can be distributed as standard Python packages.\n\n## Plugins\n\nPlugins can greatly reduce code duplication and/or promote your own standards in multiple places. For example, you can create a plugin wrapping common linting tools that you use on your projects, including their default configuration. Keeping the rules and creating new projects with the same style suddenly becomes a matter of installing one Python library.\n\nEach plugin can contain one or more Click commands that are automatically discovered and exposed by Delfino. See [`delfino-demo`](https://github.com/radeklat/delfino-demo) for a minimal plugin, which provide a `demo` command printing out a message.\n\nExisting plugins:\n\n| Plugin name                                                  | Description                                                                                        |\n|:-------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|\n| [delfino-demo](https://github.com/radeklat/delfino-demo)     | A minimal plugin example for Delfino. Contains one command printing a message.                     |\n| [delfino-core](https://github.com/radeklat/delfino-core)     | Commands wrapping tools used during every day development (linting, testing, dependencies update). |\n| [delfino-docker](https://github.com/radeklat/delfino-docker) | Docker build helper script.                                                                        |\n\n# Installation\n\n- pip: `pip install delfino`\n- Poetry: `poetry add --group=dev delfino`\n- Pipenv: `pipenv install -d delfino`\n\nor \n\n- pip: `pip install delfino[completion]`\n- Poetry: `poetry add --group=dev delfino[completion]`\n- Pipenv: `pipenv install -d delfino[completion]`\n\nto enable [auto-completion](#auto-completion).\n\n# Configuration\n\nAll configuration is expected to live in one of the following files:\n\n- `pyproject.toml` in the project root\n- `.pylintrc` in the project root - to allow dev specific config, not source controlled or for non-Python projects\n- `.pylintrc` in the user home directory - for user tools available in the system\n\nIf multiple files are discovered, only the highest one in the list will be used.\n\nThe format for `.pylintrc` is the same as for `pyproject.toml`.\n\n## Enabling a plugin\n\nFor security reasons, plugins are disabled by default. To enable a plugin, you have to include it in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN_NAME>]\n```\n\n## Enabling/disabling commands\n\nBy default, all commands are enabled. Use `enable_commands` or `disable_commands`  to show only a subset of commands. If both used, disabled commands are subtracted from the set of enabled commands.\n\n```toml\n# [tool.delfino.plugins.<PLUGIN_NAME_A>]\n# enable_commands = [<COMMAND_NAME>]\n# disable_commands = [<COMMAND_NAME>]\n\n# [tool.delfino.plugins.<PLUGIN_NAME_B>]\n# enable_commands = [<COMMAND_NAME>]\n# disable_commands = [<COMMAND_NAME>]\n```\n\n# Usage\n\nRun `delfino --help` to see all available commands and their usage.\n\n# Development\n\nDelfino is a simple wrapper around [Click commands](https://click.palletsprojects.com/quickstart/#basic-concepts-creating-a-command). Any Click command will be accepted by Delfino.\n\n## Commands discovery\n\nDelfino looks for any [`click.Command`](https://click.palletsprojects.com/en/8.0.x/api/#click.Command) sub-class in the following locations:\n\n- `commands` folder in the root of the project (next to the `pyproject.toml` file). This location is useful for commands that don\'t need to be replicated in multiple locations/projects.\n- python module import path (`<IMPORT_PATH>`) specified by `entry_point` of [a plugin](#minimal-plugin):\n  ```toml\n  [tool.poetry.plugins] # Optional super table\n\n  [tool.poetry.plugins."delfino.plugin"]\n  "delfino-<PLUGIN_NAME>" = "<IMPORT_PATH>"\n  ```\n\nAny files starting with an underscore, except for `__init__.py`, will be ignored.\n\n> **Warning**\n> Folders are NOT inspected recursively. If you place any commands into nested folders, they will not be loaded by Delfino.\n\n\n## Minimal command\n\n<!-- TODO(Radek): Delfino expects `pyproject.toml` configured. -->\n<!-- TODO(Radek): Delfino expects Poetry or Pipenv to be available. -->\n\n1. Create a `commands` folder:\n   ```shell script\n   mkdir commands\n   ```\n2. Create a `commands/__init__.py` file, with the following content:\n   ```python\n   import click\n   \n   @click.command()\n   def command_test():\n       """Tests commands placed in the `commands` folder are loaded."""\n       print("✨ This command works! ✨")\n   ```\n3. See if Delfino loads the command. Open a terminal and in the root of the project, call: `delfino --help`. You should see something like this:\n   ```text\n   Usage: delfino [OPTIONS] COMMAND [ARGS]...\n   \n   Options:\n     --help  Show this message and exit.\n   \n   Commands:\n     ...\n     command-test            Tests commands placed in the `commands` folder...\n     ...\n   ```\n4. Run the command with `delfino command-test`\n\n## Minimal plugin\n\nIf you\'d like to use one or more commands in multiple places, you can create a plugin. A plugin is just a regular Python package with specific entry point telling Delfino it should use it. It can also be distributed as any other Python packages, for example via Pypi.\n\nThe quickest way to create one is to use a [Delfino plugin cookiecutter template](https://github.com/radeklat/delfino-plugin-cookiecutter-template), which asks you several questions and sets up the whole project.\n\nAlternatively, you can get inspired by [the demo plugin](https://github.com/radeklat/delfino-demo) or any of the other [existing plugins](#plugins).\n\n# Advanced usage\n\n<!--\n## Advanced Command\n\nDelfino adds optional bits of functionality on top of Click. The following example demonstrates some of those:\n\n```python\n# commands/__init__.py\n\nimport click\n\nfrom delfino.contexts import pass_app_context, AppContext\nfrom delfino.validation import assert_pip_package_installed, pyproject_toml_key_missing\n\n@click.command()\n# The `pass_app_context` decorator adds `AppContext` as the first parameter.\n@pass_app_context\ndef command_test(app_context: AppContext):\n   """Tests commands placed in the `commands` folder are loaded."""\n   # Test optional dependencies. Any failing assertion will be printed as:\n   # Command \'<NAME>\' is misconfigured. <ASSERTION ERROR MESSAGE>\n   assert_pip_package_installed("delfino")\n\n   # AppContext contain a parsed `pyproject.toml` file.\n   # Commands can add their config under `[tool.delfino.commands.<COMMAND_NAME>]`.\n   assert "command_test" in app_context.pyproject_toml.tool.delfino.commands, \\\n       pyproject_toml_key_missing("tool.delfino.commands.command_test")\n\n   print(app_context.pyproject_toml.tool.delfino.commands["command-test"])\n```\n-->\n\n## Auto-completion\n\nYou can either attempt to install completions automatically with:\n\n```shell script\ndelfino --install-completion\n```\n\nor generate it with:\n\n```shell script\ndelfino --show-completion\n```\n\nand manually put it in the relevant RC file.\n\nThe auto-completion implementation is dynamic so that every time it is invoked, it uses the current project. Each project can have different commands or disable certain commands it doesn\'t use. And dynamic auto-completion makes sure only the currently available commands will be suggested.\n\nThe downside of this approach is that evaluating what is available each time is slower than a static list of commands.\n\n## Running external programs\n\nIt is up to you how you want to execute external processes as part of commands (if you need to at all). A common way in Python is to use `subprocess.run`. Delfino comes with its own [`run` implementation](https://github.com/radeklat/delfino/blob/main/src/delfino/execution.py#L94), which wraps and simplifies `subprocess.run` for the most common use cases:\n\n- Normalizing `subprocess.run` arguments - you can pass in either a string or a list. Either way, `subprocess.run` will be executed correctly.\n- Handling errors from the execution via the `on_error` argument. Giving the option to either ignore the errors and continue (`PASS`), not continue and clean exit (`EXIT`) or not continue and abort with error code (`ABORT`).\n- Setting environment variables.\n- Logging what is being executed in the debug level.\n\nExample:\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.execution import run, OnError\n\n@click.command()\ndef test():\n    run("pytest tests", on_error=OnError.ABORT)\n```\n\n## Optional dependencies\n\nIf you put several commands into one [plugin](#plugins), you can make some dependencies of some commands [optional](https://python-poetry.org/docs/pyproject#extras). This is useful when a command is not always used, and you don\'t want to install unnecessary dependencies. Instead, you can check if a dependency is installed only when the command is executed with `delfino.validation.assert_pip_package_installed`:\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.validation import assert_pip_package_installed\n\ntry:\n    from git import Repo\nexcept ImportError:\n    pass\n\n@click.command()\ndef git_active_branch():\n    assert_pip_package_installed("gitpython")\n    print(Repo(".").active_branch)\n```\n\nIn the example above, if `gitpython` is not installed, delfino will show the command but will fail with suggestion to install `gitpython` only when the command is executed. You can also add `git_active_branch` into [`disable_commands` config](#enablingdisabling-commands) in places where you don\'t intend to use it.\n\nThis way you can greatly reduce the number of dependencies a plugin brings into a project without a need to have many small plugins.\n\n## Project settings\n\nYou can store an arbitrary object in the Click context as [`click.Context.obj`](https://click.palletsprojects.com/api/#click.Context.obj). Delfino utilizes this object to store an instance of [`AppContext`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/app_context.py), which provides access to project related information. If you need to, you can still attach arbitrary attributes to this object later.\n\nYou can pass this object to your commands by decorating them with [`click.pass_obj`](https://click.palletsprojects.com/api/#click.pass_obj):\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.models.app_context import AppContext\n\n@click.command()\n@click.pass_obj\ndef print_app_version(obj: AppContext):\n    print(obj.pyproject_toml.tool.poetry.version)\n```\n\n## Plugin settings\n\nPlugin settings are expected to live in the `pyproject.toml` file. To prevent naming conflicts, each plugin must put its settings under `tool.delfino.plugins.<PLUGIN_NAME>`. It also allows Delfino to pass these settings directly to commands from these plugins.\n\nDelfino loads, parses, validates and stores plugin settings in [`AppContext.plugin_config`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/app_context.py). If not specified otherwise (see below), it will be an instance of [`PluginConfig`](https://github.com/radeklat/delfino/blob/main/src/delfino/models/pyproject_toml.py), with any extra keys unvalidated and in JSON-like Python objects.\n\nYou can add additional validation to your plugin settings by sub-classing the `PluginConfig` , defining expected keys, default values and/or validation. Delfino utilizes [`pydantic`](https://docs.pydantic.dev/) to create data classes.\n\nDelfino also needs to know, which class to use for the validation. To do that, switch to `delfino.decorators.pass_app_context` instead of [`click.pass_obj`](https://click.palletsprojects.com/api/#click.pass_obj):\n\n```toml\n# pyproject.toml\n\n[tool.delfino.plugins.delfino_login_plugin]\nusername = "user"\n```\n\n```python\n# commands/__init__.py\n\nimport click\nfrom delfino.models.pyproject_toml import PluginConfig\nfrom delfino.models.app_context import AppContext\nfrom delfino.decorators import pass_app_context\n\n\nclass LoginPluginConfig(PluginConfig):\n    login: str\n\n\n@click.command()\n@pass_app_context(LoginPluginConfig)\ndef login(app_context: AppContext[LoginPluginConfig]):\n    print(app_context.plugin_config.login)\n```\n\nThe `AppContext` class is generic. Defining the `PluginConfigType` (such as `AppContext[LoginPluginConfig]` in the example above) enables introspection and type checks.\n\n## Project specific overrides\n\nIt is likely your projects will require slight divergence to the defaults you encode in your scripts. The following sections cover the most common use cases.\n\n### Pass-through arguments\n\nYou can pass additional arguments to downstream tools by decorating commands with the [`decorators.pass_args`](https://github.com/radeklat/delfino/blob/main/src/delfino/decorators/pass_args.py) decorator:\n\n```python\n# commands/__init__.py\n\nfrom typing import Tuple\n\nimport click\nfrom delfino.decorators import pass_args\nfrom delfino.execution import run, OnError\n\n@click.command()\n@pass_args\ndef test(passed_args: Tuple[str, ...]):\n    run(["pytest", "tests", *passed_args], on_error=OnError.ABORT)\n```\n\nThen additional arguments can be passed either via command line after `--`:\n\n```shell script\ndelfino test -- --capture=no\n```\n\nOr via configuration in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN>.test]\npass_args = [\'--capture=no\']\n```\n\nEither way, both will result in executing `pytest tests --capture=no`.\n\n### Files override\n\nYou can override files passed to downstream tools by decorating commands with the [`decorators.files_folders_option`](https://github.com/radeklat/delfino/blob/main/src/delfino/decorators/files_folders.py) decorator:\n\n```python\n# commands/__init__.py\n\nfrom typing import Tuple\n\nimport click\nfrom delfino.decorators import files_folders_option\nfrom delfino.execution import run, OnError\n\n@click.command()\n@files_folders_option\ndef test(files_folders: Tuple[str, ...]):\n    if not files_folders:\n        files_folders = ("tests/unit", "tests/integration")\n    run(["pytest", *files_folders], on_error=OnError.ABORT)\n```\n\nThen the default `"tests/unit", "tests/integration"` folders can be overridden either via command line options `-f`/`--file`/`--folder`:\n\n```shell script\ndelfino test -f tests/other\n```\n\nOr via configuration in the `pyproject.toml` file:\n\n```toml\n[tool.delfino.plugins.<PLUGIN>.test]\nfiles_folders = [\'tests/other\']\n```\n\nEither way, both will result in executing `pytest tests/other`.\n\n## Grouping commands\n\nOften it is useful to run several commands as a group with a different command name. Click supports calling other commands with [`click.Context.forward`](https://click.palletsprojects.com/api/#click.Context.forward) or [`click.Context.invoke`](https://click.palletsprojects.com/api/#click.Context.invoke).\n\n<!-- TODO(Radek): Add description of `execute_commands_group` once migrated from `delfino-core`. -->\n',
     'author': 'Radek Lát',
     'author_email': 'radek.lat@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/radeklat/delfino',
     'package_dir': package_dir,
     'packages': packages,
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['delfino', 'delfino.click_utils', 'delfino.decorators',
 'delfino.internal_parameters', 'delfino.models'] package_data = \ {'': ['*']}
 install_requires = \ ['click>=8.0,<9.0', 'deprecation>=2.1,<3.0',
 'pydantic>=1.8,<2.0', 'toml>=0.10,<0.11'] extras_require = \ {':python_version
 < "3.10"': ['importlib-metadata']} entry_points = \ {'console_scripts':
 ['delfino = delfino.main:main', 'mike = delfino.main:main']} setup_kwargs =
-{ 'name': 'delfino', 'version': '1.1.1', 'description': 'A collection of
+{ 'name': 'delfino', 'version': '1.2.0', 'description': 'A collection of
 command line helper scripts wrapping tools used during Python development.',
 'long_description': '
                        ****** ð§°  Delfino  ð§° ******
 \n
            **** Plugable Click command finder/loader/executor. ****
 \n\n
   \n \n_[CircleCI]\n\n \n_[Codecov]\n\n \n_[GitHub_tag_(latest_SemVer)]\n\n
@@ -50,17 +50,22 @@
 day development (linting, testing, dependencies update). |\n| [delfino-docker]
 (https://github.com/radeklat/delfino-docker) | Docker build helper script.
 |\n\n# Installation\n\n- pip: `pip install delfino`\n- Poetry: `poetry add --
 group=dev delfino`\n- Pipenv: `pipenv install -d delfino`\n\nor \n\n- pip: `pip
 install delfino[completion]`\n- Poetry: `poetry add --group=dev delfino
 [completion]`\n- Pipenv: `pipenv install -d delfino[completion]`\n\nto enable
 [auto-completion](#auto-completion).\n\n# Configuration\n\nAll configuration is
-expected to live in the `pyproject.toml` file.\n\n## Enabling a plugin\n\nFor
-security reasons, plugins are disabled by default. To enable a plugin, you have
-to include it in the `pyproject.toml` file:\n\n```toml\n
+expected to live in one of the following files:\n\n- `pyproject.toml` in the
+project root\n- `.pylintrc` in the project root - to allow dev specific config,
+not source controlled or for non-Python projects\n- `.pylintrc` in the user
+home directory - for user tools available in the system\n\nIf multiple files
+are discovered, only the highest one in the list will be used.\n\nThe format
+for `.pylintrc` is the same as for `pyproject.toml`.\n\n## Enabling a
+plugin\n\nFor security reasons, plugins are disabled by default. To enable a
+plugin, you have to include it in the `pyproject.toml` file:\n\n```toml\n
 [tool.delfino.plugins.]\n```\n\n## Enabling/disabling commands\n\nBy default,
 all commands are enabled. Use `enable_commands` or `disable_commands` to show
 only a subset of commands. If both used, disabled commands are subtracted from
 the set of enabled commands.\n\n```toml\n# [tool.delfino.plugins.]\n#
 enable_commands = []\n# disable_commands = []\n\n# [tool.delfino.plugins.]\n#
 enable_commands = []\n# disable_commands = []\n```\n\n# Usage\n\nRun `delfino -
 -help` to see all available commands and their usage.\n\n#
```

### Comparing `delfino-1.1.1/PKG-INFO` & `delfino-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6465 6c66  : 2.1.Name: delf
-00000020: 696e 6f0a 5665 7273 696f 6e3a 2031 2e31  ino.Version: 1.1
-00000030: 2e31 0a53 756d 6d61 7279 3a20 4120 636f  .1.Summary: A co
+00000020: 696e 6f0a 5665 7273 696f 6e3a 2031 2e32  ino.Version: 1.2
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4120 636f  .0.Summary: A co
 00000040: 6c6c 6563 7469 6f6e 206f 6620 636f 6d6d  llection of comm
 00000050: 616e 6420 6c69 6e65 2068 656c 7065 7220  and line helper 
 00000060: 7363 7269 7074 7320 7772 6170 7069 6e67  scripts wrapping
 00000070: 2074 6f6f 6c73 2075 7365 6420 6475 7269   tools used duri
 00000080: 6e67 2050 7974 686f 6e20 6465 7665 6c6f  ng Python develo
 00000090: 706d 656e 742e 0a48 6f6d 652d 7061 6765  pment..Home-page
 000000a0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
@@ -369,792 +369,816 @@
 00001700: 6c66 696e 6f5b 636f 6d70 6c65 7469 6f6e  lfino[completion
 00001710: 5d60 0a0a 746f 2065 6e61 626c 6520 5b61  ]`..to enable [a
 00001720: 7574 6f2d 636f 6d70 6c65 7469 6f6e 5d28  uto-completion](
 00001730: 2361 7574 6f2d 636f 6d70 6c65 7469 6f6e  #auto-completion
 00001740: 292e 0a0a 2320 436f 6e66 6967 7572 6174  )...# Configurat
 00001750: 696f 6e0a 0a41 6c6c 2063 6f6e 6669 6775  ion..All configu
 00001760: 7261 7469 6f6e 2069 7320 6578 7065 6374  ration is expect
-00001770: 6564 2074 6f20 6c69 7665 2069 6e20 7468  ed to live in th
-00001780: 6520 6070 7970 726f 6a65 6374 2e74 6f6d  e `pyproject.tom
-00001790: 6c60 2066 696c 652e 0a0a 2323 2045 6e61  l` file...## Ena
-000017a0: 626c 696e 6720 6120 706c 7567 696e 0a0a  bling a plugin..
-000017b0: 466f 7220 7365 6375 7269 7479 2072 6561  For security rea
-000017c0: 736f 6e73 2c20 706c 7567 696e 7320 6172  sons, plugins ar
-000017d0: 6520 6469 7361 626c 6564 2062 7920 6465  e disabled by de
-000017e0: 6661 756c 742e 2054 6f20 656e 6162 6c65  fault. To enable
-000017f0: 2061 2070 6c75 6769 6e2c 2079 6f75 2068   a plugin, you h
-00001800: 6176 6520 746f 2069 6e63 6c75 6465 2069  ave to include i
-00001810: 7420 696e 2074 6865 2060 7079 7072 6f6a  t in the `pyproj
-00001820: 6563 742e 746f 6d6c 6020 6669 6c65 3a0a  ect.toml` file:.
-00001830: 0a60 6060 746f 6d6c 0a5b 746f 6f6c 2e64  .```toml.[tool.d
-00001840: 656c 6669 6e6f 2e70 6c75 6769 6e73 2e3c  elfino.plugins.<
-00001850: 504c 5547 494e 5f4e 414d 453e 5d0a 6060  PLUGIN_NAME>].``
-00001860: 600a 0a23 2320 456e 6162 6c69 6e67 2f64  `..## Enabling/d
-00001870: 6973 6162 6c69 6e67 2063 6f6d 6d61 6e64  isabling command
-00001880: 730a 0a42 7920 6465 6661 756c 742c 2061  s..By default, a
-00001890: 6c6c 2063 6f6d 6d61 6e64 7320 6172 6520  ll commands are 
-000018a0: 656e 6162 6c65 642e 2055 7365 2060 656e  enabled. Use `en
-000018b0: 6162 6c65 5f63 6f6d 6d61 6e64 7360 206f  able_commands` o
-000018c0: 7220 6064 6973 6162 6c65 5f63 6f6d 6d61  r `disable_comma
-000018d0: 6e64 7360 2020 746f 2073 686f 7720 6f6e  nds`  to show on
-000018e0: 6c79 2061 2073 7562 7365 7420 6f66 2063  ly a subset of c
-000018f0: 6f6d 6d61 6e64 732e 2049 6620 626f 7468  ommands. If both
-00001900: 2075 7365 642c 2064 6973 6162 6c65 6420   used, disabled 
-00001910: 636f 6d6d 616e 6473 2061 7265 2073 7562  commands are sub
-00001920: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
-00001930: 2073 6574 206f 6620 656e 6162 6c65 6420   set of enabled 
-00001940: 636f 6d6d 616e 6473 2e0a 0a60 6060 746f  commands...```to
-00001950: 6d6c 0a23 205b 746f 6f6c 2e64 656c 6669  ml.# [tool.delfi
-00001960: 6e6f 2e70 6c75 6769 6e73 2e3c 504c 5547  no.plugins.<PLUG
-00001970: 494e 5f4e 414d 455f 413e 5d0a 2320 656e  IN_NAME_A>].# en
-00001980: 6162 6c65 5f63 6f6d 6d61 6e64 7320 3d20  able_commands = 
-00001990: 5b3c 434f 4d4d 414e 445f 4e41 4d45 3e5d  [<COMMAND_NAME>]
-000019a0: 0a23 2064 6973 6162 6c65 5f63 6f6d 6d61  .# disable_comma
-000019b0: 6e64 7320 3d20 5b3c 434f 4d4d 414e 445f  nds = [<COMMAND_
-000019c0: 4e41 4d45 3e5d 0a0a 2320 5b74 6f6f 6c2e  NAME>]..# [tool.
-000019d0: 6465 6c66 696e 6f2e 706c 7567 696e 732e  delfino.plugins.
-000019e0: 3c50 4c55 4749 4e5f 4e41 4d45 5f42 3e5d  <PLUGIN_NAME_B>]
-000019f0: 0a23 2065 6e61 626c 655f 636f 6d6d 616e  .# enable_comman
-00001a00: 6473 203d 205b 3c43 4f4d 4d41 4e44 5f4e  ds = [<COMMAND_N
-00001a10: 414d 453e 5d0a 2320 6469 7361 626c 655f  AME>].# disable_
-00001a20: 636f 6d6d 616e 6473 203d 205b 3c43 4f4d  commands = [<COM
-00001a30: 4d41 4e44 5f4e 414d 453e 5d0a 6060 600a  MAND_NAME>].```.
-00001a40: 0a23 2055 7361 6765 0a0a 5275 6e20 6064  .# Usage..Run `d
-00001a50: 656c 6669 6e6f 202d 2d68 656c 7060 2074  elfino --help` t
-00001a60: 6f20 7365 6520 616c 6c20 6176 6169 6c61  o see all availa
-00001a70: 626c 6520 636f 6d6d 616e 6473 2061 6e64  ble commands and
-00001a80: 2074 6865 6972 2075 7361 6765 2e0a 0a23   their usage...#
-00001a90: 2044 6576 656c 6f70 6d65 6e74 0a0a 4465   Development..De
-00001aa0: 6c66 696e 6f20 6973 2061 2073 696d 706c  lfino is a simpl
-00001ab0: 6520 7772 6170 7065 7220 6172 6f75 6e64  e wrapper around
-00001ac0: 205b 436c 6963 6b20 636f 6d6d 616e 6473   [Click commands
-00001ad0: 5d28 6874 7470 733a 2f2f 636c 6963 6b2e  ](https://click.
-00001ae0: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
-00001af0: 636f 6d2f 7175 6963 6b73 7461 7274 2f23  com/quickstart/#
-00001b00: 6261 7369 632d 636f 6e63 6570 7473 2d63  basic-concepts-c
-00001b10: 7265 6174 696e 672d 612d 636f 6d6d 616e  reating-a-comman
-00001b20: 6429 2e20 416e 7920 436c 6963 6b20 636f  d). Any Click co
-00001b30: 6d6d 616e 6420 7769 6c6c 2062 6520 6163  mmand will be ac
-00001b40: 6365 7074 6564 2062 7920 4465 6c66 696e  cepted by Delfin
-00001b50: 6f2e 0a0a 2323 2043 6f6d 6d61 6e64 7320  o...## Commands 
-00001b60: 6469 7363 6f76 6572 790a 0a44 656c 6669  discovery..Delfi
-00001b70: 6e6f 206c 6f6f 6b73 2066 6f72 2061 6e79  no looks for any
-00001b80: 205b 6063 6c69 636b 2e43 6f6d 6d61 6e64   [`click.Command
-00001b90: 605d 2868 7474 7073 3a2f 2f63 6c69 636b  `](https://click
-00001ba0: 2e70 616c 6c65 7473 7072 6f6a 6563 7473  .palletsprojects
-00001bb0: 2e63 6f6d 2f65 6e2f 382e 302e 782f 6170  .com/en/8.0.x/ap
-00001bc0: 692f 2363 6c69 636b 2e43 6f6d 6d61 6e64  i/#click.Command
-00001bd0: 2920 7375 622d 636c 6173 7320 696e 2074  ) sub-class in t
-00001be0: 6865 2066 6f6c 6c6f 7769 6e67 206c 6f63  he following loc
-00001bf0: 6174 696f 6e73 3a0a 0a2d 2060 636f 6d6d  ations:..- `comm
-00001c00: 616e 6473 6020 666f 6c64 6572 2069 6e20  ands` folder in 
-00001c10: 7468 6520 726f 6f74 206f 6620 7468 6520  the root of the 
-00001c20: 7072 6f6a 6563 7420 286e 6578 7420 746f  project (next to
-00001c30: 2074 6865 2060 7079 7072 6f6a 6563 742e   the `pyproject.
-00001c40: 746f 6d6c 6020 6669 6c65 292e 2054 6869  toml` file). Thi
-00001c50: 7320 6c6f 6361 7469 6f6e 2069 7320 7573  s location is us
-00001c60: 6566 756c 2066 6f72 2063 6f6d 6d61 6e64  eful for command
-00001c70: 7320 7468 6174 2064 6f6e 2774 206e 6565  s that don't nee
-00001c80: 6420 746f 2062 6520 7265 706c 6963 6174  d to be replicat
-00001c90: 6564 2069 6e20 6d75 6c74 6970 6c65 206c  ed in multiple l
-00001ca0: 6f63 6174 696f 6e73 2f70 726f 6a65 6374  ocations/project
-00001cb0: 732e 0a2d 2070 7974 686f 6e20 6d6f 6475  s..- python modu
-00001cc0: 6c65 2069 6d70 6f72 7420 7061 7468 2028  le import path (
-00001cd0: 603c 494d 504f 5254 5f50 4154 483e 6029  `<IMPORT_PATH>`)
-00001ce0: 2073 7065 6369 6669 6564 2062 7920 6065   specified by `e
-00001cf0: 6e74 7279 5f70 6f69 6e74 6020 6f66 205b  ntry_point` of [
-00001d00: 6120 706c 7567 696e 5d28 236d 696e 696d  a plugin](#minim
-00001d10: 616c 2d70 6c75 6769 6e29 3a0a 2020 6060  al-plugin):.  ``
-00001d20: 6074 6f6d 6c0a 2020 5b74 6f6f 6c2e 706f  `toml.  [tool.po
-00001d30: 6574 7279 2e70 6c75 6769 6e73 5d20 2320  etry.plugins] # 
-00001d40: 4f70 7469 6f6e 616c 2073 7570 6572 2074  Optional super t
-00001d50: 6162 6c65 0a0a 2020 5b74 6f6f 6c2e 706f  able..  [tool.po
-00001d60: 6574 7279 2e70 6c75 6769 6e73 2e22 6465  etry.plugins."de
-00001d70: 6c66 696e 6f2e 706c 7567 696e 225d 0a20  lfino.plugin"]. 
-00001d80: 2022 6465 6c66 696e 6f2d 3c50 4c55 4749   "delfino-<PLUGI
-00001d90: 4e5f 4e41 4d45 3e22 203d 2022 3c49 4d50  N_NAME>" = "<IMP
-00001da0: 4f52 545f 5041 5448 3e22 0a20 2060 6060  ORT_PATH>".  ```
-00001db0: 0a0a 416e 7920 6669 6c65 7320 7374 6172  ..Any files star
-00001dc0: 7469 6e67 2077 6974 6820 616e 2075 6e64  ting with an und
-00001dd0: 6572 7363 6f72 652c 2065 7863 6570 7420  erscore, except 
-00001de0: 666f 7220 605f 5f69 6e69 745f 5f2e 7079  for `__init__.py
-00001df0: 602c 2077 696c 6c20 6265 2069 676e 6f72  `, will be ignor
-00001e00: 6564 2e0a 0a3e 202a 2a57 6172 6e69 6e67  ed...> **Warning
-00001e10: 2a2a 0a3e 2046 6f6c 6465 7273 2061 7265  **.> Folders are
-00001e20: 204e 4f54 2069 6e73 7065 6374 6564 2072   NOT inspected r
-00001e30: 6563 7572 7369 7665 6c79 2e20 4966 2079  ecursively. If y
-00001e40: 6f75 2070 6c61 6365 2061 6e79 2063 6f6d  ou place any com
-00001e50: 6d61 6e64 7320 696e 746f 206e 6573 7465  mands into neste
-00001e60: 6420 666f 6c64 6572 732c 2074 6865 7920  d folders, they 
-00001e70: 7769 6c6c 206e 6f74 2062 6520 6c6f 6164  will not be load
-00001e80: 6564 2062 7920 4465 6c66 696e 6f2e 0a0a  ed by Delfino...
-00001e90: 0a23 2320 4d69 6e69 6d61 6c20 636f 6d6d  .## Minimal comm
-00001ea0: 616e 640a 0a3c 212d 2d20 544f 444f 2852  and..<!-- TODO(R
-00001eb0: 6164 656b 293a 2044 656c 6669 6e6f 2065  adek): Delfino e
-00001ec0: 7870 6563 7473 2060 7079 7072 6f6a 6563  xpects `pyprojec
-00001ed0: 742e 746f 6d6c 6020 636f 6e66 6967 7572  t.toml` configur
-00001ee0: 6564 2e20 2d2d 3e0a 3c21 2d2d 2054 4f44  ed. -->.<!-- TOD
-00001ef0: 4f28 5261 6465 6b29 3a20 4465 6c66 696e  O(Radek): Delfin
-00001f00: 6f20 6578 7065 6374 7320 506f 6574 7279  o expects Poetry
-00001f10: 206f 7220 5069 7065 6e76 2074 6f20 6265   or Pipenv to be
-00001f20: 2061 7661 696c 6162 6c65 2e20 2d2d 3e0a   available. -->.
-00001f30: 0a31 2e20 4372 6561 7465 2061 2060 636f  .1. Create a `co
-00001f40: 6d6d 616e 6473 6020 666f 6c64 6572 3a0a  mmands` folder:.
-00001f50: 2020 2060 6060 7368 656c 6c20 7363 7269     ```shell scri
-00001f60: 7074 0a20 2020 6d6b 6469 7220 636f 6d6d  pt.   mkdir comm
-00001f70: 616e 6473 0a20 2020 6060 600a 322e 2043  ands.   ```.2. C
-00001f80: 7265 6174 6520 6120 6063 6f6d 6d61 6e64  reate a `command
-00001f90: 732f 5f5f 696e 6974 5f5f 2e70 7960 2066  s/__init__.py` f
-00001fa0: 696c 652c 2077 6974 6820 7468 6520 666f  ile, with the fo
-00001fb0: 6c6c 6f77 696e 6720 636f 6e74 656e 743a  llowing content:
-00001fc0: 0a20 2020 6060 6070 7974 686f 6e0a 2020  .   ```python.  
-00001fd0: 2069 6d70 6f72 7420 636c 6963 6b0a 2020   import click.  
-00001fe0: 200a 2020 2040 636c 6963 6b2e 636f 6d6d   .   @click.comm
-00001ff0: 616e 6428 290a 2020 2064 6566 2063 6f6d  and().   def com
-00002000: 6d61 6e64 5f74 6573 7428 293a 0a20 2020  mand_test():.   
-00002010: 2020 2020 2222 2254 6573 7473 2063 6f6d      """Tests com
-00002020: 6d61 6e64 7320 706c 6163 6564 2069 6e20  mands placed in 
-00002030: 7468 6520 6063 6f6d 6d61 6e64 7360 2066  the `commands` f
-00002040: 6f6c 6465 7220 6172 6520 6c6f 6164 6564  older are loaded
-00002050: 2e22 2222 0a20 2020 2020 2020 7072 696e  .""".       prin
-00002060: 7428 22e2 9ca8 2054 6869 7320 636f 6d6d  t("... This comm
-00002070: 616e 6420 776f 726b 7321 20e2 9ca8 2229  and works! ...")
-00002080: 0a20 2020 6060 600a 332e 2053 6565 2069  .   ```.3. See i
-00002090: 6620 4465 6c66 696e 6f20 6c6f 6164 7320  f Delfino loads 
-000020a0: 7468 6520 636f 6d6d 616e 642e 204f 7065  the command. Ope
-000020b0: 6e20 6120 7465 726d 696e 616c 2061 6e64  n a terminal and
-000020c0: 2069 6e20 7468 6520 726f 6f74 206f 6620   in the root of 
-000020d0: 7468 6520 7072 6f6a 6563 742c 2063 616c  the project, cal
-000020e0: 6c3a 2060 6465 6c66 696e 6f20 2d2d 6865  l: `delfino --he
-000020f0: 6c70 602e 2059 6f75 2073 686f 756c 6420  lp`. You should 
-00002100: 7365 6520 736f 6d65 7468 696e 6720 6c69  see something li
-00002110: 6b65 2074 6869 733a 0a20 2020 6060 6074  ke this:.   ```t
-00002120: 6578 740a 2020 2055 7361 6765 3a20 6465  ext.   Usage: de
-00002130: 6c66 696e 6f20 5b4f 5054 494f 4e53 5d20  lfino [OPTIONS] 
-00002140: 434f 4d4d 414e 4420 5b41 5247 535d 2e2e  COMMAND [ARGS]..
-00002150: 2e0a 2020 200a 2020 204f 7074 696f 6e73  ..   .   Options
-00002160: 3a0a 2020 2020 202d 2d68 656c 7020 2053  :.     --help  S
-00002170: 686f 7720 7468 6973 206d 6573 7361 6765  how this message
-00002180: 2061 6e64 2065 7869 742e 0a20 2020 0a20   and exit..   . 
-00002190: 2020 436f 6d6d 616e 6473 3a0a 2020 2020    Commands:.    
-000021a0: 202e 2e2e 0a20 2020 2020 636f 6d6d 616e   ....     comman
-000021b0: 642d 7465 7374 2020 2020 2020 2020 2020  d-test          
-000021c0: 2020 5465 7374 7320 636f 6d6d 616e 6473    Tests commands
-000021d0: 2070 6c61 6365 6420 696e 2074 6865 2060   placed in the `
-000021e0: 636f 6d6d 616e 6473 6020 666f 6c64 6572  commands` folder
-000021f0: 2e2e 2e0a 2020 2020 202e 2e2e 0a20 2020  ....     ....   
-00002200: 6060 600a 342e 2052 756e 2074 6865 2063  ```.4. Run the c
-00002210: 6f6d 6d61 6e64 2077 6974 6820 6064 656c  ommand with `del
-00002220: 6669 6e6f 2063 6f6d 6d61 6e64 2d74 6573  fino command-tes
-00002230: 7460 0a0a 2323 204d 696e 696d 616c 2070  t`..## Minimal p
-00002240: 6c75 6769 6e0a 0a49 6620 796f 7527 6420  lugin..If you'd 
-00002250: 6c69 6b65 2074 6f20 7573 6520 6f6e 6520  like to use one 
-00002260: 6f72 206d 6f72 6520 636f 6d6d 616e 6473  or more commands
-00002270: 2069 6e20 6d75 6c74 6970 6c65 2070 6c61   in multiple pla
-00002280: 6365 732c 2079 6f75 2063 616e 2063 7265  ces, you can cre
-00002290: 6174 6520 6120 706c 7567 696e 2e20 4120  ate a plugin. A 
-000022a0: 706c 7567 696e 2069 7320 6a75 7374 2061  plugin is just a
-000022b0: 2072 6567 756c 6172 2050 7974 686f 6e20   regular Python 
-000022c0: 7061 636b 6167 6520 7769 7468 2073 7065  package with spe
-000022d0: 6369 6669 6320 656e 7472 7920 706f 696e  cific entry poin
-000022e0: 7420 7465 6c6c 696e 6720 4465 6c66 696e  t telling Delfin
-000022f0: 6f20 6974 2073 686f 756c 6420 7573 6520  o it should use 
-00002300: 6974 2e20 4974 2063 616e 2061 6c73 6f20  it. It can also 
-00002310: 6265 2064 6973 7472 6962 7574 6564 2061  be distributed a
-00002320: 7320 616e 7920 6f74 6865 7220 5079 7468  s any other Pyth
-00002330: 6f6e 2070 6163 6b61 6765 732c 2066 6f72  on packages, for
-00002340: 2065 7861 6d70 6c65 2076 6961 2050 7970   example via Pyp
-00002350: 692e 0a0a 5468 6520 7175 6963 6b65 7374  i...The quickest
-00002360: 2077 6179 2074 6f20 6372 6561 7465 206f   way to create o
-00002370: 6e65 2069 7320 746f 2075 7365 2061 205b  ne is to use a [
-00002380: 4465 6c66 696e 6f20 706c 7567 696e 2063  Delfino plugin c
-00002390: 6f6f 6b69 6563 7574 7465 7220 7465 6d70  ookiecutter temp
-000023a0: 6c61 7465 5d28 6874 7470 733a 2f2f 6769  late](https://gi
-000023b0: 7468 7562 2e63 6f6d 2f72 6164 656b 6c61  thub.com/radekla
-000023c0: 742f 6465 6c66 696e 6f2d 706c 7567 696e  t/delfino-plugin
-000023d0: 2d63 6f6f 6b69 6563 7574 7465 722d 7465  -cookiecutter-te
-000023e0: 6d70 6c61 7465 292c 2077 6869 6368 2061  mplate), which a
-000023f0: 736b 7320 796f 7520 7365 7665 7261 6c20  sks you several 
-00002400: 7175 6573 7469 6f6e 7320 616e 6420 7365  questions and se
-00002410: 7473 2075 7020 7468 6520 7768 6f6c 6520  ts up the whole 
-00002420: 7072 6f6a 6563 742e 0a0a 416c 7465 726e  project...Altern
-00002430: 6174 6976 656c 792c 2079 6f75 2063 616e  atively, you can
-00002440: 2067 6574 2069 6e73 7069 7265 6420 6279   get inspired by
-00002450: 205b 7468 6520 6465 6d6f 2070 6c75 6769   [the demo plugi
-00002460: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00002470: 622e 636f 6d2f 7261 6465 6b6c 6174 2f64  b.com/radeklat/d
-00002480: 656c 6669 6e6f 2d64 656d 6f29 206f 7220  elfino-demo) or 
-00002490: 616e 7920 6f66 2074 6865 206f 7468 6572  any of the other
-000024a0: 205b 6578 6973 7469 6e67 2070 6c75 6769   [existing plugi
-000024b0: 6e73 5d28 2370 6c75 6769 6e73 292e 0a0a  ns](#plugins)...
-000024c0: 2320 4164 7661 6e63 6564 2075 7361 6765  # Advanced usage
-000024d0: 0a0a 3c21 2d2d 0a23 2320 4164 7661 6e63  ..<!--.## Advanc
-000024e0: 6564 2043 6f6d 6d61 6e64 0a0a 4465 6c66  ed Command..Delf
-000024f0: 696e 6f20 6164 6473 206f 7074 696f 6e61  ino adds optiona
-00002500: 6c20 6269 7473 206f 6620 6675 6e63 7469  l bits of functi
-00002510: 6f6e 616c 6974 7920 6f6e 2074 6f70 206f  onality on top o
-00002520: 6620 436c 6963 6b2e 2054 6865 2066 6f6c  f Click. The fol
-00002530: 6c6f 7769 6e67 2065 7861 6d70 6c65 2064  lowing example d
-00002540: 656d 6f6e 7374 7261 7465 7320 736f 6d65  emonstrates some
-00002550: 206f 6620 7468 6f73 653a 0a0a 6060 6070   of those:..```p
-00002560: 7974 686f 6e0a 2320 636f 6d6d 616e 6473  ython.# commands
-00002570: 2f5f 5f69 6e69 745f 5f2e 7079 0a0a 696d  /__init__.py..im
-00002580: 706f 7274 2063 6c69 636b 0a0a 6672 6f6d  port click..from
-00002590: 2064 656c 6669 6e6f 2e63 6f6e 7465 7874   delfino.context
-000025a0: 7320 696d 706f 7274 2070 6173 735f 6170  s import pass_ap
-000025b0: 705f 636f 6e74 6578 742c 2041 7070 436f  p_context, AppCo
-000025c0: 6e74 6578 740a 6672 6f6d 2064 656c 6669  ntext.from delfi
-000025d0: 6e6f 2e76 616c 6964 6174 696f 6e20 696d  no.validation im
-000025e0: 706f 7274 2061 7373 6572 745f 7069 705f  port assert_pip_
-000025f0: 7061 636b 6167 655f 696e 7374 616c 6c65  package_installe
-00002600: 642c 2070 7970 726f 6a65 6374 5f74 6f6d  d, pyproject_tom
-00002610: 6c5f 6b65 795f 6d69 7373 696e 670a 0a40  l_key_missing..@
-00002620: 636c 6963 6b2e 636f 6d6d 616e 6428 290a  click.command().
-00002630: 2320 5468 6520 6070 6173 735f 6170 705f  # The `pass_app_
-00002640: 636f 6e74 6578 7460 2064 6563 6f72 6174  context` decorat
-00002650: 6f72 2061 6464 7320 6041 7070 436f 6e74  or adds `AppCont
-00002660: 6578 7460 2061 7320 7468 6520 6669 7273  ext` as the firs
-00002670: 7420 7061 7261 6d65 7465 722e 0a40 7061  t parameter..@pa
-00002680: 7373 5f61 7070 5f63 6f6e 7465 7874 0a64  ss_app_context.d
-00002690: 6566 2063 6f6d 6d61 6e64 5f74 6573 7428  ef command_test(
-000026a0: 6170 705f 636f 6e74 6578 743a 2041 7070  app_context: App
-000026b0: 436f 6e74 6578 7429 3a0a 2020 2022 2222  Context):.   """
-000026c0: 5465 7374 7320 636f 6d6d 616e 6473 2070  Tests commands p
-000026d0: 6c61 6365 6420 696e 2074 6865 2060 636f  laced in the `co
-000026e0: 6d6d 616e 6473 6020 666f 6c64 6572 2061  mmands` folder a
-000026f0: 7265 206c 6f61 6465 642e 2222 220a 2020  re loaded.""".  
-00002700: 2023 2054 6573 7420 6f70 7469 6f6e 616c   # Test optional
-00002710: 2064 6570 656e 6465 6e63 6965 732e 2041   dependencies. A
-00002720: 6e79 2066 6169 6c69 6e67 2061 7373 6572  ny failing asser
-00002730: 7469 6f6e 2077 696c 6c20 6265 2070 7269  tion will be pri
-00002740: 6e74 6564 2061 733a 0a20 2020 2320 436f  nted as:.   # Co
-00002750: 6d6d 616e 6420 273c 4e41 4d45 3e27 2069  mmand '<NAME>' i
-00002760: 7320 6d69 7363 6f6e 6669 6775 7265 642e  s misconfigured.
-00002770: 203c 4153 5345 5254 494f 4e20 4552 524f   <ASSERTION ERRO
-00002780: 5220 4d45 5353 4147 453e 0a20 2020 6173  R MESSAGE>.   as
-00002790: 7365 7274 5f70 6970 5f70 6163 6b61 6765  sert_pip_package
-000027a0: 5f69 6e73 7461 6c6c 6564 2822 6465 6c66  _installed("delf
-000027b0: 696e 6f22 290a 0a20 2020 2320 4170 7043  ino")..   # AppC
-000027c0: 6f6e 7465 7874 2063 6f6e 7461 696e 2061  ontext contain a
-000027d0: 2070 6172 7365 6420 6070 7970 726f 6a65   parsed `pyproje
-000027e0: 6374 2e74 6f6d 6c60 2066 696c 652e 0a20  ct.toml` file.. 
-000027f0: 2020 2320 436f 6d6d 616e 6473 2063 616e    # Commands can
-00002800: 2061 6464 2074 6865 6972 2063 6f6e 6669   add their confi
-00002810: 6720 756e 6465 7220 605b 746f 6f6c 2e64  g under `[tool.d
-00002820: 656c 6669 6e6f 2e63 6f6d 6d61 6e64 732e  elfino.commands.
-00002830: 3c43 4f4d 4d41 4e44 5f4e 414d 453e 5d60  <COMMAND_NAME>]`
-00002840: 2e0a 2020 2061 7373 6572 7420 2263 6f6d  ..   assert "com
-00002850: 6d61 6e64 5f74 6573 7422 2069 6e20 6170  mand_test" in ap
-00002860: 705f 636f 6e74 6578 742e 7079 7072 6f6a  p_context.pyproj
-00002870: 6563 745f 746f 6d6c 2e74 6f6f 6c2e 6465  ect_toml.tool.de
-00002880: 6c66 696e 6f2e 636f 6d6d 616e 6473 2c20  lfino.commands, 
-00002890: 5c0a 2020 2020 2020 2070 7970 726f 6a65  \.       pyproje
-000028a0: 6374 5f74 6f6d 6c5f 6b65 795f 6d69 7373  ct_toml_key_miss
-000028b0: 696e 6728 2274 6f6f 6c2e 6465 6c66 696e  ing("tool.delfin
-000028c0: 6f2e 636f 6d6d 616e 6473 2e63 6f6d 6d61  o.commands.comma
-000028d0: 6e64 5f74 6573 7422 290a 0a20 2020 7072  nd_test")..   pr
-000028e0: 696e 7428 6170 705f 636f 6e74 6578 742e  int(app_context.
-000028f0: 7079 7072 6f6a 6563 745f 746f 6d6c 2e74  pyproject_toml.t
-00002900: 6f6f 6c2e 6465 6c66 696e 6f2e 636f 6d6d  ool.delfino.comm
-00002910: 616e 6473 5b22 636f 6d6d 616e 642d 7465  ands["command-te
-00002920: 7374 225d 290a 6060 600a 2d2d 3e0a 0a23  st"]).```.-->..#
-00002930: 2320 4175 746f 2d63 6f6d 706c 6574 696f  # Auto-completio
-00002940: 6e0a 0a59 6f75 2063 616e 2065 6974 6865  n..You can eithe
-00002950: 7220 6174 7465 6d70 7420 746f 2069 6e73  r attempt to ins
-00002960: 7461 6c6c 2063 6f6d 706c 6574 696f 6e73  tall completions
-00002970: 2061 7574 6f6d 6174 6963 616c 6c79 2077   automatically w
-00002980: 6974 683a 0a0a 6060 6073 6865 6c6c 2073  ith:..```shell s
-00002990: 6372 6970 740a 6465 6c66 696e 6f20 2d2d  cript.delfino --
-000029a0: 696e 7374 616c 6c2d 636f 6d70 6c65 7469  install-completi
-000029b0: 6f6e 0a60 6060 0a0a 6f72 2067 656e 6572  on.```..or gener
-000029c0: 6174 6520 6974 2077 6974 683a 0a0a 6060  ate it with:..``
-000029d0: 6073 6865 6c6c 2073 6372 6970 740a 6465  `shell script.de
-000029e0: 6c66 696e 6f20 2d2d 7368 6f77 2d63 6f6d  lfino --show-com
-000029f0: 706c 6574 696f 6e0a 6060 600a 0a61 6e64  pletion.```..and
-00002a00: 206d 616e 7561 6c6c 7920 7075 7420 6974   manually put it
-00002a10: 2069 6e20 7468 6520 7265 6c65 7661 6e74   in the relevant
-00002a20: 2052 4320 6669 6c65 2e0a 0a54 6865 2061   RC file...The a
-00002a30: 7574 6f2d 636f 6d70 6c65 7469 6f6e 2069  uto-completion i
-00002a40: 6d70 6c65 6d65 6e74 6174 696f 6e20 6973  mplementation is
-00002a50: 2064 796e 616d 6963 2073 6f20 7468 6174   dynamic so that
-00002a60: 2065 7665 7279 2074 696d 6520 6974 2069   every time it i
-00002a70: 7320 696e 766f 6b65 642c 2069 7420 7573  s invoked, it us
-00002a80: 6573 2074 6865 2063 7572 7265 6e74 2070  es the current p
-00002a90: 726f 6a65 6374 2e20 4561 6368 2070 726f  roject. Each pro
-00002aa0: 6a65 6374 2063 616e 2068 6176 6520 6469  ject can have di
-00002ab0: 6666 6572 656e 7420 636f 6d6d 616e 6473  fferent commands
-00002ac0: 206f 7220 6469 7361 626c 6520 6365 7274   or disable cert
-00002ad0: 6169 6e20 636f 6d6d 616e 6473 2069 7420  ain commands it 
-00002ae0: 646f 6573 6e27 7420 7573 652e 2041 6e64  doesn't use. And
-00002af0: 2064 796e 616d 6963 2061 7574 6f2d 636f   dynamic auto-co
-00002b00: 6d70 6c65 7469 6f6e 206d 616b 6573 2073  mpletion makes s
-00002b10: 7572 6520 6f6e 6c79 2074 6865 2063 7572  ure only the cur
-00002b20: 7265 6e74 6c79 2061 7661 696c 6162 6c65  rently available
-00002b30: 2063 6f6d 6d61 6e64 7320 7769 6c6c 2062   commands will b
-00002b40: 6520 7375 6767 6573 7465 642e 0a0a 5468  e suggested...Th
-00002b50: 6520 646f 776e 7369 6465 206f 6620 7468  e downside of th
-00002b60: 6973 2061 7070 726f 6163 6820 6973 2074  is approach is t
-00002b70: 6861 7420 6576 616c 7561 7469 6e67 2077  hat evaluating w
-00002b80: 6861 7420 6973 2061 7661 696c 6162 6c65  hat is available
-00002b90: 2065 6163 6820 7469 6d65 2069 7320 736c   each time is sl
-00002ba0: 6f77 6572 2074 6861 6e20 6120 7374 6174  ower than a stat
-00002bb0: 6963 206c 6973 7420 6f66 2063 6f6d 6d61  ic list of comma
-00002bc0: 6e64 732e 0a0a 2323 2052 756e 6e69 6e67  nds...## Running
-00002bd0: 2065 7874 6572 6e61 6c20 7072 6f67 7261   external progra
-00002be0: 6d73 0a0a 4974 2069 7320 7570 2074 6f20  ms..It is up to 
-00002bf0: 796f 7520 686f 7720 796f 7520 7761 6e74  you how you want
-00002c00: 2074 6f20 6578 6563 7574 6520 6578 7465   to execute exte
-00002c10: 726e 616c 2070 726f 6365 7373 6573 2061  rnal processes a
-00002c20: 7320 7061 7274 206f 6620 636f 6d6d 616e  s part of comman
-00002c30: 6473 2028 6966 2079 6f75 206e 6565 6420  ds (if you need 
-00002c40: 746f 2061 7420 616c 6c29 2e20 4120 636f  to at all). A co
-00002c50: 6d6d 6f6e 2077 6179 2069 6e20 5079 7468  mmon way in Pyth
-00002c60: 6f6e 2069 7320 746f 2075 7365 2060 7375  on is to use `su
-00002c70: 6270 726f 6365 7373 2e72 756e 602e 2044  bprocess.run`. D
-00002c80: 656c 6669 6e6f 2063 6f6d 6573 2077 6974  elfino comes wit
-00002c90: 6820 6974 7320 6f77 6e20 5b60 7275 6e60  h its own [`run`
-00002ca0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e5d   implementation]
-00002cb0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00002cc0: 636f 6d2f 7261 6465 6b6c 6174 2f64 656c  com/radeklat/del
-00002cd0: 6669 6e6f 2f62 6c6f 622f 6d61 696e 2f73  fino/blob/main/s
-00002ce0: 7263 2f64 656c 6669 6e6f 2f65 7865 6375  rc/delfino/execu
-00002cf0: 7469 6f6e 2e70 7923 4c39 3429 2c20 7768  tion.py#L94), wh
-00002d00: 6963 6820 7772 6170 7320 616e 6420 7369  ich wraps and si
-00002d10: 6d70 6c69 6669 6573 2060 7375 6270 726f  mplifies `subpro
-00002d20: 6365 7373 2e72 756e 6020 666f 7220 7468  cess.run` for th
-00002d30: 6520 6d6f 7374 2063 6f6d 6d6f 6e20 7573  e most common us
-00002d40: 6520 6361 7365 733a 0a0a 2d20 4e6f 726d  e cases:..- Norm
-00002d50: 616c 697a 696e 6720 6073 7562 7072 6f63  alizing `subproc
-00002d60: 6573 732e 7275 6e60 2061 7267 756d 656e  ess.run` argumen
-00002d70: 7473 202d 2079 6f75 2063 616e 2070 6173  ts - you can pas
-00002d80: 7320 696e 2065 6974 6865 7220 6120 7374  s in either a st
-00002d90: 7269 6e67 206f 7220 6120 6c69 7374 2e20  ring or a list. 
-00002da0: 4569 7468 6572 2077 6179 2c20 6073 7562  Either way, `sub
-00002db0: 7072 6f63 6573 732e 7275 6e60 2077 696c  process.run` wil
-00002dc0: 6c20 6265 2065 7865 6375 7465 6420 636f  l be executed co
-00002dd0: 7272 6563 746c 792e 0a2d 2048 616e 646c  rrectly..- Handl
-00002de0: 696e 6720 6572 726f 7273 2066 726f 6d20  ing errors from 
-00002df0: 7468 6520 6578 6563 7574 696f 6e20 7669  the execution vi
-00002e00: 6120 7468 6520 606f 6e5f 6572 726f 7260  a the `on_error`
-00002e10: 2061 7267 756d 656e 742e 2047 6976 696e   argument. Givin
-00002e20: 6720 7468 6520 6f70 7469 6f6e 2074 6f20  g the option to 
-00002e30: 6569 7468 6572 2069 676e 6f72 6520 7468  either ignore th
-00002e40: 6520 6572 726f 7273 2061 6e64 2063 6f6e  e errors and con
-00002e50: 7469 6e75 6520 2860 5041 5353 6029 2c20  tinue (`PASS`), 
-00002e60: 6e6f 7420 636f 6e74 696e 7565 2061 6e64  not continue and
-00002e70: 2063 6c65 616e 2065 7869 7420 2860 4558   clean exit (`EX
-00002e80: 4954 6029 206f 7220 6e6f 7420 636f 6e74  IT`) or not cont
-00002e90: 696e 7565 2061 6e64 2061 626f 7274 2077  inue and abort w
-00002ea0: 6974 6820 6572 726f 7220 636f 6465 2028  ith error code (
-00002eb0: 6041 424f 5254 6029 2e0a 2d20 5365 7474  `ABORT`)..- Sett
-00002ec0: 696e 6720 656e 7669 726f 6e6d 656e 7420  ing environment 
-00002ed0: 7661 7269 6162 6c65 732e 0a2d 204c 6f67  variables..- Log
-00002ee0: 6769 6e67 2077 6861 7420 6973 2062 6569  ging what is bei
-00002ef0: 6e67 2065 7865 6375 7465 6420 696e 2074  ng executed in t
-00002f00: 6865 2064 6562 7567 206c 6576 656c 2e0a  he debug level..
-00002f10: 0a45 7861 6d70 6c65 3a0a 0a60 6060 7079  .Example:..```py
-00002f20: 7468 6f6e 0a23 2063 6f6d 6d61 6e64 732f  thon.# commands/
-00002f30: 5f5f 696e 6974 5f5f 2e70 790a 0a69 6d70  __init__.py..imp
-00002f40: 6f72 7420 636c 6963 6b0a 6672 6f6d 2064  ort click.from d
-00002f50: 656c 6669 6e6f 2e65 7865 6375 7469 6f6e  elfino.execution
-00002f60: 2069 6d70 6f72 7420 7275 6e2c 204f 6e45   import run, OnE
-00002f70: 7272 6f72 0a0a 4063 6c69 636b 2e63 6f6d  rror..@click.com
-00002f80: 6d61 6e64 2829 0a64 6566 2074 6573 7428  mand().def test(
-00002f90: 293a 0a20 2020 2072 756e 2822 7079 7465  ):.    run("pyte
-00002fa0: 7374 2074 6573 7473 222c 206f 6e5f 6572  st tests", on_er
-00002fb0: 726f 723d 4f6e 4572 726f 722e 4142 4f52  ror=OnError.ABOR
-00002fc0: 5429 0a60 6060 0a0a 2323 204f 7074 696f  T).```..## Optio
-00002fd0: 6e61 6c20 6465 7065 6e64 656e 6369 6573  nal dependencies
-00002fe0: 0a0a 4966 2079 6f75 2070 7574 2073 6576  ..If you put sev
-00002ff0: 6572 616c 2063 6f6d 6d61 6e64 7320 696e  eral commands in
-00003000: 746f 206f 6e65 205b 706c 7567 696e 5d28  to one [plugin](
-00003010: 2370 6c75 6769 6e73 292c 2079 6f75 2063  #plugins), you c
-00003020: 616e 206d 616b 6520 736f 6d65 2064 6570  an make some dep
-00003030: 656e 6465 6e63 6965 7320 6f66 2073 6f6d  endencies of som
-00003040: 6520 636f 6d6d 616e 6473 205b 6f70 7469  e commands [opti
-00003050: 6f6e 616c 5d28 6874 7470 733a 2f2f 7079  onal](https://py
-00003060: 7468 6f6e 2d70 6f65 7472 792e 6f72 672f  thon-poetry.org/
-00003070: 646f 6373 2f70 7970 726f 6a65 6374 2365  docs/pyproject#e
-00003080: 7874 7261 7329 2e20 5468 6973 2069 7320  xtras). This is 
-00003090: 7573 6566 756c 2077 6865 6e20 6120 636f  useful when a co
-000030a0: 6d6d 616e 6420 6973 206e 6f74 2061 6c77  mmand is not alw
-000030b0: 6179 7320 7573 6564 2c20 616e 6420 796f  ays used, and yo
-000030c0: 7520 646f 6e27 7420 7761 6e74 2074 6f20  u don't want to 
-000030d0: 696e 7374 616c 6c20 756e 6e65 6365 7373  install unnecess
-000030e0: 6172 7920 6465 7065 6e64 656e 6369 6573  ary dependencies
-000030f0: 2e20 496e 7374 6561 642c 2079 6f75 2063  . Instead, you c
-00003100: 616e 2063 6865 636b 2069 6620 6120 6465  an check if a de
-00003110: 7065 6e64 656e 6379 2069 7320 696e 7374  pendency is inst
-00003120: 616c 6c65 6420 6f6e 6c79 2077 6865 6e20  alled only when 
-00003130: 7468 6520 636f 6d6d 616e 6420 6973 2065  the command is e
-00003140: 7865 6375 7465 6420 7769 7468 2060 6465  xecuted with `de
-00003150: 6c66 696e 6f2e 7661 6c69 6461 7469 6f6e  lfino.validation
-00003160: 2e61 7373 6572 745f 7069 705f 7061 636b  .assert_pip_pack
-00003170: 6167 655f 696e 7374 616c 6c65 6460 3a0a  age_installed`:.
-00003180: 0a60 6060 7079 7468 6f6e 0a23 2063 6f6d  .```python.# com
-00003190: 6d61 6e64 732f 5f5f 696e 6974 5f5f 2e70  mands/__init__.p
-000031a0: 790a 0a69 6d70 6f72 7420 636c 6963 6b0a  y..import click.
-000031b0: 6672 6f6d 2064 656c 6669 6e6f 2e76 616c  from delfino.val
-000031c0: 6964 6174 696f 6e20 696d 706f 7274 2061  idation import a
-000031d0: 7373 6572 745f 7069 705f 7061 636b 6167  ssert_pip_packag
-000031e0: 655f 696e 7374 616c 6c65 640a 0a74 7279  e_installed..try
-000031f0: 3a0a 2020 2020 6672 6f6d 2067 6974 2069  :.    from git i
-00003200: 6d70 6f72 7420 5265 706f 0a65 7863 6570  mport Repo.excep
-00003210: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
-00003220: 2020 2070 6173 730a 0a40 636c 6963 6b2e     pass..@click.
-00003230: 636f 6d6d 616e 6428 290a 6465 6620 6769  command().def gi
-00003240: 745f 6163 7469 7665 5f62 7261 6e63 6828  t_active_branch(
-00003250: 293a 0a20 2020 2061 7373 6572 745f 7069  ):.    assert_pi
-00003260: 705f 7061 636b 6167 655f 696e 7374 616c  p_package_instal
-00003270: 6c65 6428 2267 6974 7079 7468 6f6e 2229  led("gitpython")
-00003280: 0a20 2020 2070 7269 6e74 2852 6570 6f28  .    print(Repo(
-00003290: 222e 2229 2e61 6374 6976 655f 6272 616e  ".").active_bran
-000032a0: 6368 290a 6060 600a 0a49 6e20 7468 6520  ch).```..In the 
-000032b0: 6578 616d 706c 6520 6162 6f76 652c 2069  example above, i
-000032c0: 6620 6067 6974 7079 7468 6f6e 6020 6973  f `gitpython` is
-000032d0: 206e 6f74 2069 6e73 7461 6c6c 6564 2c20   not installed, 
-000032e0: 6465 6c66 696e 6f20 7769 6c6c 2073 686f  delfino will sho
-000032f0: 7720 7468 6520 636f 6d6d 616e 6420 6275  w the command bu
-00003300: 7420 7769 6c6c 2066 6169 6c20 7769 7468  t will fail with
-00003310: 2073 7567 6765 7374 696f 6e20 746f 2069   suggestion to i
-00003320: 6e73 7461 6c6c 2060 6769 7470 7974 686f  nstall `gitpytho
-00003330: 6e60 206f 6e6c 7920 7768 656e 2074 6865  n` only when the
-00003340: 2063 6f6d 6d61 6e64 2069 7320 6578 6563   command is exec
-00003350: 7574 6564 2e20 596f 7520 6361 6e20 616c  uted. You can al
-00003360: 736f 2061 6464 2060 6769 745f 6163 7469  so add `git_acti
-00003370: 7665 5f62 7261 6e63 6860 2069 6e74 6f20  ve_branch` into 
-00003380: 5b60 6469 7361 626c 655f 636f 6d6d 616e  [`disable_comman
-00003390: 6473 6020 636f 6e66 6967 5d28 2365 6e61  ds` config](#ena
-000033a0: 626c 696e 6764 6973 6162 6c69 6e67 2d63  blingdisabling-c
-000033b0: 6f6d 6d61 6e64 7329 2069 6e20 706c 6163  ommands) in plac
-000033c0: 6573 2077 6865 7265 2079 6f75 2064 6f6e  es where you don
-000033d0: 2774 2069 6e74 656e 6420 746f 2075 7365  't intend to use
-000033e0: 2069 742e 0a0a 5468 6973 2077 6179 2079   it...This way y
-000033f0: 6f75 2063 616e 2067 7265 6174 6c79 2072  ou can greatly r
-00003400: 6564 7563 6520 7468 6520 6e75 6d62 6572  educe the number
-00003410: 206f 6620 6465 7065 6e64 656e 6369 6573   of dependencies
-00003420: 2061 2070 6c75 6769 6e20 6272 696e 6773   a plugin brings
-00003430: 2069 6e74 6f20 6120 7072 6f6a 6563 7420   into a project 
-00003440: 7769 7468 6f75 7420 6120 6e65 6564 2074  without a need t
-00003450: 6f20 6861 7665 206d 616e 7920 736d 616c  o have many smal
-00003460: 6c20 706c 7567 696e 732e 0a0a 2323 2050  l plugins...## P
-00003470: 726f 6a65 6374 2073 6574 7469 6e67 730a  roject settings.
-00003480: 0a59 6f75 2063 616e 2073 746f 7265 2061  .You can store a
-00003490: 6e20 6172 6269 7472 6172 7920 6f62 6a65  n arbitrary obje
-000034a0: 6374 2069 6e20 7468 6520 436c 6963 6b20  ct in the Click 
-000034b0: 636f 6e74 6578 7420 6173 205b 6063 6c69  context as [`cli
-000034c0: 636b 2e43 6f6e 7465 7874 2e6f 626a 605d  ck.Context.obj`]
-000034d0: 2868 7474 7073 3a2f 2f63 6c69 636b 2e70  (https://click.p
-000034e0: 616c 6c65 7473 7072 6f6a 6563 7473 2e63  alletsprojects.c
-000034f0: 6f6d 2f61 7069 2f23 636c 6963 6b2e 436f  om/api/#click.Co
-00003500: 6e74 6578 742e 6f62 6a29 2e20 4465 6c66  ntext.obj). Delf
-00003510: 696e 6f20 7574 696c 697a 6573 2074 6869  ino utilizes thi
-00003520: 7320 6f62 6a65 6374 2074 6f20 7374 6f72  s object to stor
-00003530: 6520 616e 2069 6e73 7461 6e63 6520 6f66  e an instance of
-00003540: 205b 6041 7070 436f 6e74 6578 7460 5d28   [`AppContext`](
-00003550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00003560: 6f6d 2f72 6164 656b 6c61 742f 6465 6c66  om/radeklat/delf
-00003570: 696e 6f2f 626c 6f62 2f6d 6169 6e2f 7372  ino/blob/main/sr
-00003580: 632f 6465 6c66 696e 6f2f 6d6f 6465 6c73  c/delfino/models
-00003590: 2f61 7070 5f63 6f6e 7465 7874 2e70 7929  /app_context.py)
-000035a0: 2c20 7768 6963 6820 7072 6f76 6964 6573  , which provides
-000035b0: 2061 6363 6573 7320 746f 2070 726f 6a65   access to proje
-000035c0: 6374 2072 656c 6174 6564 2069 6e66 6f72  ct related infor
-000035d0: 6d61 7469 6f6e 2e20 4966 2079 6f75 206e  mation. If you n
-000035e0: 6565 6420 746f 2c20 796f 7520 6361 6e20  eed to, you can 
-000035f0: 7374 696c 6c20 6174 7461 6368 2061 7262  still attach arb
-00003600: 6974 7261 7279 2061 7474 7269 6275 7465  itrary attribute
-00003610: 7320 746f 2074 6869 7320 6f62 6a65 6374  s to this object
-00003620: 206c 6174 6572 2e0a 0a59 6f75 2063 616e   later...You can
-00003630: 2070 6173 7320 7468 6973 206f 626a 6563   pass this objec
-00003640: 7420 746f 2079 6f75 7220 636f 6d6d 616e  t to your comman
-00003650: 6473 2062 7920 6465 636f 7261 7469 6e67  ds by decorating
-00003660: 2074 6865 6d20 7769 7468 205b 6063 6c69   them with [`cli
-00003670: 636b 2e70 6173 735f 6f62 6a60 5d28 6874  ck.pass_obj`](ht
-00003680: 7470 733a 2f2f 636c 6963 6b2e 7061 6c6c  tps://click.pall
-00003690: 6574 7370 726f 6a65 6374 732e 636f 6d2f  etsprojects.com/
-000036a0: 6170 692f 2363 6c69 636b 2e70 6173 735f  api/#click.pass_
-000036b0: 6f62 6a29 3a0a 0a60 6060 7079 7468 6f6e  obj):..```python
-000036c0: 0a23 2063 6f6d 6d61 6e64 732f 5f5f 696e  .# commands/__in
-000036d0: 6974 5f5f 2e70 790a 0a69 6d70 6f72 7420  it__.py..import 
-000036e0: 636c 6963 6b0a 6672 6f6d 2064 656c 6669  click.from delfi
-000036f0: 6e6f 2e6d 6f64 656c 732e 6170 705f 636f  no.models.app_co
-00003700: 6e74 6578 7420 696d 706f 7274 2041 7070  ntext import App
-00003710: 436f 6e74 6578 740a 0a40 636c 6963 6b2e  Context..@click.
-00003720: 636f 6d6d 616e 6428 290a 4063 6c69 636b  command().@click
-00003730: 2e70 6173 735f 6f62 6a0a 6465 6620 7072  .pass_obj.def pr
-00003740: 696e 745f 6170 705f 7665 7273 696f 6e28  int_app_version(
-00003750: 6f62 6a3a 2041 7070 436f 6e74 6578 7429  obj: AppContext)
-00003760: 3a0a 2020 2020 7072 696e 7428 6f62 6a2e  :.    print(obj.
-00003770: 7079 7072 6f6a 6563 745f 746f 6d6c 2e74  pyproject_toml.t
-00003780: 6f6f 6c2e 706f 6574 7279 2e76 6572 7369  ool.poetry.versi
-00003790: 6f6e 290a 6060 600a 0a23 2320 506c 7567  on).```..## Plug
-000037a0: 696e 2073 6574 7469 6e67 730a 0a50 6c75  in settings..Plu
-000037b0: 6769 6e20 7365 7474 696e 6773 2061 7265  gin settings are
-000037c0: 2065 7870 6563 7465 6420 746f 206c 6976   expected to liv
-000037d0: 6520 696e 2074 6865 2060 7079 7072 6f6a  e in the `pyproj
-000037e0: 6563 742e 746f 6d6c 6020 6669 6c65 2e20  ect.toml` file. 
-000037f0: 546f 2070 7265 7665 6e74 206e 616d 696e  To prevent namin
-00003800: 6720 636f 6e66 6c69 6374 732c 2065 6163  g conflicts, eac
-00003810: 6820 706c 7567 696e 206d 7573 7420 7075  h plugin must pu
-00003820: 7420 6974 7320 7365 7474 696e 6773 2075  t its settings u
-00003830: 6e64 6572 2060 746f 6f6c 2e64 656c 6669  nder `tool.delfi
-00003840: 6e6f 2e70 6c75 6769 6e73 2e3c 504c 5547  no.plugins.<PLUG
-00003850: 494e 5f4e 414d 453e 602e 2049 7420 616c  IN_NAME>`. It al
-00003860: 736f 2061 6c6c 6f77 7320 4465 6c66 696e  so allows Delfin
-00003870: 6f20 746f 2070 6173 7320 7468 6573 6520  o to pass these 
-00003880: 7365 7474 696e 6773 2064 6972 6563 746c  settings directl
-00003890: 7920 746f 2063 6f6d 6d61 6e64 7320 6672  y to commands fr
-000038a0: 6f6d 2074 6865 7365 2070 6c75 6769 6e73  om these plugins
-000038b0: 2e0a 0a44 656c 6669 6e6f 206c 6f61 6473  ...Delfino loads
-000038c0: 2c20 7061 7273 6573 2c20 7661 6c69 6461  , parses, valida
-000038d0: 7465 7320 616e 6420 7374 6f72 6573 2070  tes and stores p
-000038e0: 6c75 6769 6e20 7365 7474 696e 6773 2069  lugin settings i
-000038f0: 6e20 5b60 4170 7043 6f6e 7465 7874 2e70  n [`AppContext.p
-00003900: 6c75 6769 6e5f 636f 6e66 6967 605d 2868  lugin_config`](h
-00003910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00003920: 6d2f 7261 6465 6b6c 6174 2f64 656c 6669  m/radeklat/delfi
-00003930: 6e6f 2f62 6c6f 622f 6d61 696e 2f73 7263  no/blob/main/src
-00003940: 2f64 656c 6669 6e6f 2f6d 6f64 656c 732f  /delfino/models/
-00003950: 6170 705f 636f 6e74 6578 742e 7079 292e  app_context.py).
-00003960: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
-00003970: 6420 6f74 6865 7277 6973 6520 2873 6565  d otherwise (see
-00003980: 2062 656c 6f77 292c 2069 7420 7769 6c6c   below), it will
-00003990: 2062 6520 616e 2069 6e73 7461 6e63 6520   be an instance 
-000039a0: 6f66 205b 6050 6c75 6769 6e43 6f6e 6669  of [`PluginConfi
-000039b0: 6760 5d28 6874 7470 733a 2f2f 6769 7468  g`](https://gith
-000039c0: 7562 2e63 6f6d 2f72 6164 656b 6c61 742f  ub.com/radeklat/
-000039d0: 6465 6c66 696e 6f2f 626c 6f62 2f6d 6169  delfino/blob/mai
-000039e0: 6e2f 7372 632f 6465 6c66 696e 6f2f 6d6f  n/src/delfino/mo
-000039f0: 6465 6c73 2f70 7970 726f 6a65 6374 5f74  dels/pyproject_t
-00003a00: 6f6d 6c2e 7079 292c 2077 6974 6820 616e  oml.py), with an
-00003a10: 7920 6578 7472 6120 6b65 7973 2075 6e76  y extra keys unv
-00003a20: 616c 6964 6174 6564 2061 6e64 2069 6e20  alidated and in 
-00003a30: 4a53 4f4e 2d6c 696b 6520 5079 7468 6f6e  JSON-like Python
-00003a40: 206f 626a 6563 7473 2e0a 0a59 6f75 2063   objects...You c
-00003a50: 616e 2061 6464 2061 6464 6974 696f 6e61  an add additiona
-00003a60: 6c20 7661 6c69 6461 7469 6f6e 2074 6f20  l validation to 
-00003a70: 796f 7572 2070 6c75 6769 6e20 7365 7474  your plugin sett
-00003a80: 696e 6773 2062 7920 7375 622d 636c 6173  ings by sub-clas
-00003a90: 7369 6e67 2074 6865 2060 506c 7567 696e  sing the `Plugin
-00003aa0: 436f 6e66 6967 6020 2c20 6465 6669 6e69  Config` , defini
-00003ab0: 6e67 2065 7870 6563 7465 6420 6b65 7973  ng expected keys
-00003ac0: 2c20 6465 6661 756c 7420 7661 6c75 6573  , default values
-00003ad0: 2061 6e64 2f6f 7220 7661 6c69 6461 7469   and/or validati
-00003ae0: 6f6e 2e20 4465 6c66 696e 6f20 7574 696c  on. Delfino util
-00003af0: 697a 6573 205b 6070 7964 616e 7469 6360  izes [`pydantic`
-00003b00: 5d28 6874 7470 733a 2f2f 646f 6373 2e70  ](https://docs.p
-00003b10: 7964 616e 7469 632e 6465 762f 2920 746f  ydantic.dev/) to
-00003b20: 2063 7265 6174 6520 6461 7461 2063 6c61   create data cla
-00003b30: 7373 6573 2e0a 0a44 656c 6669 6e6f 2061  sses...Delfino a
-00003b40: 6c73 6f20 6e65 6564 7320 746f 206b 6e6f  lso needs to kno
-00003b50: 772c 2077 6869 6368 2063 6c61 7373 2074  w, which class t
-00003b60: 6f20 7573 6520 666f 7220 7468 6520 7661  o use for the va
-00003b70: 6c69 6461 7469 6f6e 2e20 546f 2064 6f20  lidation. To do 
-00003b80: 7468 6174 2c20 7377 6974 6368 2074 6f20  that, switch to 
-00003b90: 6064 656c 6669 6e6f 2e64 6563 6f72 6174  `delfino.decorat
-00003ba0: 6f72 732e 7061 7373 5f61 7070 5f63 6f6e  ors.pass_app_con
-00003bb0: 7465 7874 6020 696e 7374 6561 6420 6f66  text` instead of
-00003bc0: 205b 6063 6c69 636b 2e70 6173 735f 6f62   [`click.pass_ob
-00003bd0: 6a60 5d28 6874 7470 733a 2f2f 636c 6963  j`](https://clic
-00003be0: 6b2e 7061 6c6c 6574 7370 726f 6a65 6374  k.palletsproject
-00003bf0: 732e 636f 6d2f 6170 692f 2363 6c69 636b  s.com/api/#click
-00003c00: 2e70 6173 735f 6f62 6a29 3a0a 0a60 6060  .pass_obj):..```
-00003c10: 746f 6d6c 0a23 2070 7970 726f 6a65 6374  toml.# pyproject
-00003c20: 2e74 6f6d 6c0a 0a5b 746f 6f6c 2e64 656c  .toml..[tool.del
-00003c30: 6669 6e6f 2e70 6c75 6769 6e73 2e64 656c  fino.plugins.del
-00003c40: 6669 6e6f 5f6c 6f67 696e 5f70 6c75 6769  fino_login_plugi
-00003c50: 6e5d 0a75 7365 726e 616d 6520 3d20 2275  n].username = "u
-00003c60: 7365 7222 0a60 6060 0a0a 6060 6070 7974  ser".```..```pyt
-00003c70: 686f 6e0a 2320 636f 6d6d 616e 6473 2f5f  hon.# commands/_
-00003c80: 5f69 6e69 745f 5f2e 7079 0a0a 696d 706f  _init__.py..impo
-00003c90: 7274 2063 6c69 636b 0a66 726f 6d20 6465  rt click.from de
-00003ca0: 6c66 696e 6f2e 6d6f 6465 6c73 2e70 7970  lfino.models.pyp
-00003cb0: 726f 6a65 6374 5f74 6f6d 6c20 696d 706f  roject_toml impo
-00003cc0: 7274 2050 6c75 6769 6e43 6f6e 6669 670a  rt PluginConfig.
-00003cd0: 6672 6f6d 2064 656c 6669 6e6f 2e6d 6f64  from delfino.mod
-00003ce0: 656c 732e 6170 705f 636f 6e74 6578 7420  els.app_context 
-00003cf0: 696d 706f 7274 2041 7070 436f 6e74 6578  import AppContex
-00003d00: 740a 6672 6f6d 2064 656c 6669 6e6f 2e64  t.from delfino.d
-00003d10: 6563 6f72 6174 6f72 7320 696d 706f 7274  ecorators import
-00003d20: 2070 6173 735f 6170 705f 636f 6e74 6578   pass_app_contex
-00003d30: 740a 0a0a 636c 6173 7320 4c6f 6769 6e50  t...class LoginP
-00003d40: 6c75 6769 6e43 6f6e 6669 6728 506c 7567  luginConfig(Plug
-00003d50: 696e 436f 6e66 6967 293a 0a20 2020 206c  inConfig):.    l
-00003d60: 6f67 696e 3a20 7374 720a 0a0a 4063 6c69  ogin: str...@cli
-00003d70: 636b 2e63 6f6d 6d61 6e64 2829 0a40 7061  ck.command().@pa
-00003d80: 7373 5f61 7070 5f63 6f6e 7465 7874 284c  ss_app_context(L
-00003d90: 6f67 696e 506c 7567 696e 436f 6e66 6967  oginPluginConfig
-00003da0: 290a 6465 6620 6c6f 6769 6e28 6170 705f  ).def login(app_
-00003db0: 636f 6e74 6578 743a 2041 7070 436f 6e74  context: AppCont
-00003dc0: 6578 745b 4c6f 6769 6e50 6c75 6769 6e43  ext[LoginPluginC
-00003dd0: 6f6e 6669 675d 293a 0a20 2020 2070 7269  onfig]):.    pri
-00003de0: 6e74 2861 7070 5f63 6f6e 7465 7874 2e70  nt(app_context.p
-00003df0: 6c75 6769 6e5f 636f 6e66 6967 2e6c 6f67  lugin_config.log
-00003e00: 696e 290a 6060 600a 0a54 6865 2060 4170  in).```..The `Ap
-00003e10: 7043 6f6e 7465 7874 6020 636c 6173 7320  pContext` class 
-00003e20: 6973 2067 656e 6572 6963 2e20 4465 6669  is generic. Defi
-00003e30: 6e69 6e67 2074 6865 2060 506c 7567 696e  ning the `Plugin
-00003e40: 436f 6e66 6967 5479 7065 6020 2873 7563  ConfigType` (suc
-00003e50: 6820 6173 2060 4170 7043 6f6e 7465 7874  h as `AppContext
-00003e60: 5b4c 6f67 696e 506c 7567 696e 436f 6e66  [LoginPluginConf
-00003e70: 6967 5d60 2069 6e20 7468 6520 6578 616d  ig]` in the exam
-00003e80: 706c 6520 6162 6f76 6529 2065 6e61 626c  ple above) enabl
-00003e90: 6573 2069 6e74 726f 7370 6563 7469 6f6e  es introspection
-00003ea0: 2061 6e64 2074 7970 6520 6368 6563 6b73   and type checks
-00003eb0: 2e0a 0a23 2320 5072 6f6a 6563 7420 7370  ...## Project sp
-00003ec0: 6563 6966 6963 206f 7665 7272 6964 6573  ecific overrides
-00003ed0: 0a0a 4974 2069 7320 6c69 6b65 6c79 2079  ..It is likely y
-00003ee0: 6f75 7220 7072 6f6a 6563 7473 2077 696c  our projects wil
-00003ef0: 6c20 7265 7175 6972 6520 736c 6967 6874  l require slight
-00003f00: 2064 6976 6572 6765 6e63 6520 746f 2074   divergence to t
-00003f10: 6865 2064 6566 6175 6c74 7320 796f 7520  he defaults you 
-00003f20: 656e 636f 6465 2069 6e20 796f 7572 2073  encode in your s
-00003f30: 6372 6970 7473 2e20 5468 6520 666f 6c6c  cripts. The foll
-00003f40: 6f77 696e 6720 7365 6374 696f 6e73 2063  owing sections c
-00003f50: 6f76 6572 2074 6865 206d 6f73 7420 636f  over the most co
-00003f60: 6d6d 6f6e 2075 7365 2063 6173 6573 2e0a  mmon use cases..
-00003f70: 0a23 2323 2050 6173 732d 7468 726f 7567  .### Pass-throug
-00003f80: 6820 6172 6775 6d65 6e74 730a 0a59 6f75  h arguments..You
-00003f90: 2063 616e 2070 6173 7320 6164 6469 7469   can pass additi
-00003fa0: 6f6e 616c 2061 7267 756d 656e 7473 2074  onal arguments t
-00003fb0: 6f20 646f 776e 7374 7265 616d 2074 6f6f  o downstream too
-00003fc0: 6c73 2062 7920 6465 636f 7261 7469 6e67  ls by decorating
-00003fd0: 2063 6f6d 6d61 6e64 7320 7769 7468 2074   commands with t
-00003fe0: 6865 205b 6064 6563 6f72 6174 6f72 732e  he [`decorators.
-00003ff0: 7061 7373 5f61 7267 7360 5d28 6874 7470  pass_args`](http
-00004000: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-00004010: 6164 656b 6c61 742f 6465 6c66 696e 6f2f  adeklat/delfino/
-00004020: 626c 6f62 2f6d 6169 6e2f 7372 632f 6465  blob/main/src/de
-00004030: 6c66 696e 6f2f 6465 636f 7261 746f 7273  lfino/decorators
-00004040: 2f70 6173 735f 6172 6773 2e70 7929 2064  /pass_args.py) d
-00004050: 6563 6f72 6174 6f72 3a0a 0a60 6060 7079  ecorator:..```py
-00004060: 7468 6f6e 0a23 2063 6f6d 6d61 6e64 732f  thon.# commands/
-00004070: 5f5f 696e 6974 5f5f 2e70 790a 0a66 726f  __init__.py..fro
-00004080: 6d20 7479 7069 6e67 2069 6d70 6f72 7420  m typing import 
-00004090: 5475 706c 650a 0a69 6d70 6f72 7420 636c  Tuple..import cl
-000040a0: 6963 6b0a 6672 6f6d 2064 656c 6669 6e6f  ick.from delfino
-000040b0: 2e64 6563 6f72 6174 6f72 7320 696d 706f  .decorators impo
-000040c0: 7274 2070 6173 735f 6172 6773 0a66 726f  rt pass_args.fro
-000040d0: 6d20 6465 6c66 696e 6f2e 6578 6563 7574  m delfino.execut
-000040e0: 696f 6e20 696d 706f 7274 2072 756e 2c20  ion import run, 
-000040f0: 4f6e 4572 726f 720a 0a40 636c 6963 6b2e  OnError..@click.
-00004100: 636f 6d6d 616e 6428 290a 4070 6173 735f  command().@pass_
-00004110: 6172 6773 0a64 6566 2074 6573 7428 7061  args.def test(pa
-00004120: 7373 6564 5f61 7267 733a 2054 7570 6c65  ssed_args: Tuple
-00004130: 5b73 7472 2c20 2e2e 2e5d 293a 0a20 2020  [str, ...]):.   
-00004140: 2072 756e 285b 2270 7974 6573 7422 2c20   run(["pytest", 
-00004150: 2274 6573 7473 222c 202a 7061 7373 6564  "tests", *passed
-00004160: 5f61 7267 735d 2c20 6f6e 5f65 7272 6f72  _args], on_error
-00004170: 3d4f 6e45 7272 6f72 2e41 424f 5254 290a  =OnError.ABORT).
-00004180: 6060 600a 0a54 6865 6e20 6164 6469 7469  ```..Then additi
-00004190: 6f6e 616c 2061 7267 756d 656e 7473 2063  onal arguments c
-000041a0: 616e 2062 6520 7061 7373 6564 2065 6974  an be passed eit
-000041b0: 6865 7220 7669 6120 636f 6d6d 616e 6420  her via command 
-000041c0: 6c69 6e65 2061 6674 6572 2060 2d2d 603a  line after `--`:
-000041d0: 0a0a 6060 6073 6865 6c6c 2073 6372 6970  ..```shell scrip
-000041e0: 740a 6465 6c66 696e 6f20 7465 7374 202d  t.delfino test -
-000041f0: 2d20 2d2d 6361 7074 7572 653d 6e6f 0a60  - --capture=no.`
-00004200: 6060 0a0a 4f72 2076 6961 2063 6f6e 6669  ``..Or via confi
-00004210: 6775 7261 7469 6f6e 2069 6e20 7468 6520  guration in the 
-00004220: 6070 7970 726f 6a65 6374 2e74 6f6d 6c60  `pyproject.toml`
-00004230: 2066 696c 653a 0a0a 6060 6074 6f6d 6c0a   file:..```toml.
-00004240: 5b74 6f6f 6c2e 6465 6c66 696e 6f2e 706c  [tool.delfino.pl
-00004250: 7567 696e 732e 3c50 4c55 4749 4e3e 2e74  ugins.<PLUGIN>.t
-00004260: 6573 745d 0a70 6173 735f 6172 6773 203d  est].pass_args =
-00004270: 205b 272d 2d63 6170 7475 7265 3d6e 6f27   ['--capture=no'
-00004280: 5d0a 6060 600a 0a45 6974 6865 7220 7761  ].```..Either wa
-00004290: 792c 2062 6f74 6820 7769 6c6c 2072 6573  y, both will res
-000042a0: 756c 7420 696e 2065 7865 6375 7469 6e67  ult in executing
-000042b0: 2060 7079 7465 7374 2074 6573 7473 202d   `pytest tests -
-000042c0: 2d63 6170 7475 7265 3d6e 6f60 2e0a 0a23  -capture=no`...#
-000042d0: 2323 2046 696c 6573 206f 7665 7272 6964  ## Files overrid
-000042e0: 650a 0a59 6f75 2063 616e 206f 7665 7272  e..You can overr
-000042f0: 6964 6520 6669 6c65 7320 7061 7373 6564  ide files passed
-00004300: 2074 6f20 646f 776e 7374 7265 616d 2074   to downstream t
-00004310: 6f6f 6c73 2062 7920 6465 636f 7261 7469  ools by decorati
-00004320: 6e67 2063 6f6d 6d61 6e64 7320 7769 7468  ng commands with
-00004330: 2074 6865 205b 6064 6563 6f72 6174 6f72   the [`decorator
-00004340: 732e 6669 6c65 735f 666f 6c64 6572 735f  s.files_folders_
-00004350: 6f70 7469 6f6e 605d 2868 7474 7073 3a2f  option`](https:/
-00004360: 2f67 6974 6875 622e 636f 6d2f 7261 6465  /github.com/rade
-00004370: 6b6c 6174 2f64 656c 6669 6e6f 2f62 6c6f  klat/delfino/blo
-00004380: 622f 6d61 696e 2f73 7263 2f64 656c 6669  b/main/src/delfi
-00004390: 6e6f 2f64 6563 6f72 6174 6f72 732f 6669  no/decorators/fi
-000043a0: 6c65 735f 666f 6c64 6572 732e 7079 2920  les_folders.py) 
-000043b0: 6465 636f 7261 746f 723a 0a0a 6060 6070  decorator:..```p
-000043c0: 7974 686f 6e0a 2320 636f 6d6d 616e 6473  ython.# commands
-000043d0: 2f5f 5f69 6e69 745f 5f2e 7079 0a0a 6672  /__init__.py..fr
-000043e0: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
-000043f0: 2054 7570 6c65 0a0a 696d 706f 7274 2063   Tuple..import c
-00004400: 6c69 636b 0a66 726f 6d20 6465 6c66 696e  lick.from delfin
-00004410: 6f2e 6465 636f 7261 746f 7273 2069 6d70  o.decorators imp
-00004420: 6f72 7420 6669 6c65 735f 666f 6c64 6572  ort files_folder
-00004430: 735f 6f70 7469 6f6e 0a66 726f 6d20 6465  s_option.from de
-00004440: 6c66 696e 6f2e 6578 6563 7574 696f 6e20  lfino.execution 
-00004450: 696d 706f 7274 2072 756e 2c20 4f6e 4572  import run, OnEr
-00004460: 726f 720a 0a40 636c 6963 6b2e 636f 6d6d  ror..@click.comm
-00004470: 616e 6428 290a 4066 696c 6573 5f66 6f6c  and().@files_fol
-00004480: 6465 7273 5f6f 7074 696f 6e0a 6465 6620  ders_option.def 
-00004490: 7465 7374 2866 696c 6573 5f66 6f6c 6465  test(files_folde
-000044a0: 7273 3a20 5475 706c 655b 7374 722c 202e  rs: Tuple[str, .
-000044b0: 2e2e 5d29 3a0a 2020 2020 6966 206e 6f74  ..]):.    if not
-000044c0: 2066 696c 6573 5f66 6f6c 6465 7273 3a0a   files_folders:.
-000044d0: 2020 2020 2020 2020 6669 6c65 735f 666f          files_fo
-000044e0: 6c64 6572 7320 3d20 2822 7465 7374 732f  lders = ("tests/
-000044f0: 756e 6974 222c 2022 7465 7374 732f 696e  unit", "tests/in
-00004500: 7465 6772 6174 696f 6e22 290a 2020 2020  tegration").    
-00004510: 7275 6e28 5b22 7079 7465 7374 222c 202a  run(["pytest", *
-00004520: 6669 6c65 735f 666f 6c64 6572 735d 2c20  files_folders], 
-00004530: 6f6e 5f65 7272 6f72 3d4f 6e45 7272 6f72  on_error=OnError
-00004540: 2e41 424f 5254 290a 6060 600a 0a54 6865  .ABORT).```..The
-00004550: 6e20 7468 6520 6465 6661 756c 7420 6022  n the default `"
-00004560: 7465 7374 732f 756e 6974 222c 2022 7465  tests/unit", "te
-00004570: 7374 732f 696e 7465 6772 6174 696f 6e22  sts/integration"
-00004580: 6020 666f 6c64 6572 7320 6361 6e20 6265  ` folders can be
-00004590: 206f 7665 7272 6964 6465 6e20 6569 7468   overridden eith
-000045a0: 6572 2076 6961 2063 6f6d 6d61 6e64 206c  er via command l
-000045b0: 696e 6520 6f70 7469 6f6e 7320 602d 6660  ine options `-f`
-000045c0: 2f60 2d2d 6669 6c65 602f 602d 2d66 6f6c  /`--file`/`--fol
-000045d0: 6465 7260 3a0a 0a60 6060 7368 656c 6c20  der`:..```shell 
-000045e0: 7363 7269 7074 0a64 656c 6669 6e6f 2074  script.delfino t
-000045f0: 6573 7420 2d66 2074 6573 7473 2f6f 7468  est -f tests/oth
-00004600: 6572 0a60 6060 0a0a 4f72 2076 6961 2063  er.```..Or via c
-00004610: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
-00004620: 7468 6520 6070 7970 726f 6a65 6374 2e74  the `pyproject.t
-00004630: 6f6d 6c60 2066 696c 653a 0a0a 6060 6074  oml` file:..```t
-00004640: 6f6d 6c0a 5b74 6f6f 6c2e 6465 6c66 696e  oml.[tool.delfin
-00004650: 6f2e 706c 7567 696e 732e 3c50 4c55 4749  o.plugins.<PLUGI
-00004660: 4e3e 2e74 6573 745d 0a66 696c 6573 5f66  N>.test].files_f
-00004670: 6f6c 6465 7273 203d 205b 2774 6573 7473  olders = ['tests
-00004680: 2f6f 7468 6572 275d 0a60 6060 0a0a 4569  /other'].```..Ei
-00004690: 7468 6572 2077 6179 2c20 626f 7468 2077  ther way, both w
-000046a0: 696c 6c20 7265 7375 6c74 2069 6e20 6578  ill result in ex
-000046b0: 6563 7574 696e 6720 6070 7974 6573 7420  ecuting `pytest 
-000046c0: 7465 7374 732f 6f74 6865 7260 2e0a 0a23  tests/other`...#
-000046d0: 2320 4772 6f75 7069 6e67 2063 6f6d 6d61  # Grouping comma
-000046e0: 6e64 730a 0a4f 6674 656e 2069 7420 6973  nds..Often it is
-000046f0: 2075 7365 6675 6c20 746f 2072 756e 2073   useful to run s
-00004700: 6576 6572 616c 2063 6f6d 6d61 6e64 7320  everal commands 
-00004710: 6173 2061 2067 726f 7570 2077 6974 6820  as a group with 
-00004720: 6120 6469 6666 6572 656e 7420 636f 6d6d  a different comm
-00004730: 616e 6420 6e61 6d65 2e20 436c 6963 6b20  and name. Click 
-00004740: 7375 7070 6f72 7473 2063 616c 6c69 6e67  supports calling
-00004750: 206f 7468 6572 2063 6f6d 6d61 6e64 7320   other commands 
-00004760: 7769 7468 205b 6063 6c69 636b 2e43 6f6e  with [`click.Con
-00004770: 7465 7874 2e66 6f72 7761 7264 605d 2868  text.forward`](h
-00004780: 7474 7073 3a2f 2f63 6c69 636b 2e70 616c  ttps://click.pal
-00004790: 6c65 7473 7072 6f6a 6563 7473 2e63 6f6d  letsprojects.com
-000047a0: 2f61 7069 2f23 636c 6963 6b2e 436f 6e74  /api/#click.Cont
-000047b0: 6578 742e 666f 7277 6172 6429 206f 7220  ext.forward) or 
-000047c0: 5b60 636c 6963 6b2e 436f 6e74 6578 742e  [`click.Context.
-000047d0: 696e 766f 6b65 605d 2868 7474 7073 3a2f  invoke`](https:/
-000047e0: 2f63 6c69 636b 2e70 616c 6c65 7473 7072  /click.palletspr
-000047f0: 6f6a 6563 7473 2e63 6f6d 2f61 7069 2f23  ojects.com/api/#
-00004800: 636c 6963 6b2e 436f 6e74 6578 742e 696e  click.Context.in
-00004810: 766f 6b65 292e 0a0a 3c21 2d2d 2054 4f44  voke)...<!-- TOD
-00004820: 4f28 5261 6465 6b29 3a20 4164 6420 6465  O(Radek): Add de
-00004830: 7363 7269 7074 696f 6e20 6f66 2060 6578  scription of `ex
-00004840: 6563 7574 655f 636f 6d6d 616e 6473 5f67  ecute_commands_g
-00004850: 726f 7570 6020 6f6e 6365 206d 6967 7261  roup` once migra
-00004860: 7465 6420 6672 6f6d 2060 6465 6c66 696e  ted from `delfin
-00004870: 6f2d 636f 7265 602e 202d 2d3e 0a0a       o-core`. -->..
+00001770: 6564 2074 6f20 6c69 7665 2069 6e20 6f6e  ed to live in on
+00001780: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+00001790: 6e67 2066 696c 6573 3a0a 0a2d 2060 7079  ng files:..- `py
+000017a0: 7072 6f6a 6563 742e 746f 6d6c 6020 696e  project.toml` in
+000017b0: 2074 6865 2070 726f 6a65 6374 2072 6f6f   the project roo
+000017c0: 740a 2d20 602e 7079 6c69 6e74 7263 6020  t.- `.pylintrc` 
+000017d0: 696e 2074 6865 2070 726f 6a65 6374 2072  in the project r
+000017e0: 6f6f 7420 2d20 746f 2061 6c6c 6f77 2064  oot - to allow d
+000017f0: 6576 2073 7065 6369 6669 6320 636f 6e66  ev specific conf
+00001800: 6967 2c20 6e6f 7420 736f 7572 6365 2063  ig, not source c
+00001810: 6f6e 7472 6f6c 6c65 6420 6f72 2066 6f72  ontrolled or for
+00001820: 206e 6f6e 2d50 7974 686f 6e20 7072 6f6a   non-Python proj
+00001830: 6563 7473 0a2d 2060 2e70 796c 696e 7472  ects.- `.pylintr
+00001840: 6360 2069 6e20 7468 6520 7573 6572 2068  c` in the user h
+00001850: 6f6d 6520 6469 7265 6374 6f72 7920 2d20  ome directory - 
+00001860: 666f 7220 7573 6572 2074 6f6f 6c73 2061  for user tools a
+00001870: 7661 696c 6162 6c65 2069 6e20 7468 6520  vailable in the 
+00001880: 7379 7374 656d 0a0a 4966 206d 756c 7469  system..If multi
+00001890: 706c 6520 6669 6c65 7320 6172 6520 6469  ple files are di
+000018a0: 7363 6f76 6572 6564 2c20 6f6e 6c79 2074  scovered, only t
+000018b0: 6865 2068 6967 6865 7374 206f 6e65 2069  he highest one i
+000018c0: 6e20 7468 6520 6c69 7374 2077 696c 6c20  n the list will 
+000018d0: 6265 2075 7365 642e 0a0a 5468 6520 666f  be used...The fo
+000018e0: 726d 6174 2066 6f72 2060 2e70 796c 696e  rmat for `.pylin
+000018f0: 7472 6360 2069 7320 7468 6520 7361 6d65  trc` is the same
+00001900: 2061 7320 666f 7220 6070 7970 726f 6a65   as for `pyproje
+00001910: 6374 2e74 6f6d 6c60 2e0a 0a23 2320 456e  ct.toml`...## En
+00001920: 6162 6c69 6e67 2061 2070 6c75 6769 6e0a  abling a plugin.
+00001930: 0a46 6f72 2073 6563 7572 6974 7920 7265  .For security re
+00001940: 6173 6f6e 732c 2070 6c75 6769 6e73 2061  asons, plugins a
+00001950: 7265 2064 6973 6162 6c65 6420 6279 2064  re disabled by d
+00001960: 6566 6175 6c74 2e20 546f 2065 6e61 626c  efault. To enabl
+00001970: 6520 6120 706c 7567 696e 2c20 796f 7520  e a plugin, you 
+00001980: 6861 7665 2074 6f20 696e 636c 7564 6520  have to include 
+00001990: 6974 2069 6e20 7468 6520 6070 7970 726f  it in the `pypro
+000019a0: 6a65 6374 2e74 6f6d 6c60 2066 696c 653a  ject.toml` file:
+000019b0: 0a0a 6060 6074 6f6d 6c0a 5b74 6f6f 6c2e  ..```toml.[tool.
+000019c0: 6465 6c66 696e 6f2e 706c 7567 696e 732e  delfino.plugins.
+000019d0: 3c50 4c55 4749 4e5f 4e41 4d45 3e5d 0a60  <PLUGIN_NAME>].`
+000019e0: 6060 0a0a 2323 2045 6e61 626c 696e 672f  ``..## Enabling/
+000019f0: 6469 7361 626c 696e 6720 636f 6d6d 616e  disabling comman
+00001a00: 6473 0a0a 4279 2064 6566 6175 6c74 2c20  ds..By default, 
+00001a10: 616c 6c20 636f 6d6d 616e 6473 2061 7265  all commands are
+00001a20: 2065 6e61 626c 6564 2e20 5573 6520 6065   enabled. Use `e
+00001a30: 6e61 626c 655f 636f 6d6d 616e 6473 6020  nable_commands` 
+00001a40: 6f72 2060 6469 7361 626c 655f 636f 6d6d  or `disable_comm
+00001a50: 616e 6473 6020 2074 6f20 7368 6f77 206f  ands`  to show o
+00001a60: 6e6c 7920 6120 7375 6273 6574 206f 6620  nly a subset of 
+00001a70: 636f 6d6d 616e 6473 2e20 4966 2062 6f74  commands. If bot
+00001a80: 6820 7573 6564 2c20 6469 7361 626c 6564  h used, disabled
+00001a90: 2063 6f6d 6d61 6e64 7320 6172 6520 7375   commands are su
+00001aa0: 6274 7261 6374 6564 2066 726f 6d20 7468  btracted from th
+00001ab0: 6520 7365 7420 6f66 2065 6e61 626c 6564  e set of enabled
+00001ac0: 2063 6f6d 6d61 6e64 732e 0a0a 6060 6074   commands...```t
+00001ad0: 6f6d 6c0a 2320 5b74 6f6f 6c2e 6465 6c66  oml.# [tool.delf
+00001ae0: 696e 6f2e 706c 7567 696e 732e 3c50 4c55  ino.plugins.<PLU
+00001af0: 4749 4e5f 4e41 4d45 5f41 3e5d 0a23 2065  GIN_NAME_A>].# e
+00001b00: 6e61 626c 655f 636f 6d6d 616e 6473 203d  nable_commands =
+00001b10: 205b 3c43 4f4d 4d41 4e44 5f4e 414d 453e   [<COMMAND_NAME>
+00001b20: 5d0a 2320 6469 7361 626c 655f 636f 6d6d  ].# disable_comm
+00001b30: 616e 6473 203d 205b 3c43 4f4d 4d41 4e44  ands = [<COMMAND
+00001b40: 5f4e 414d 453e 5d0a 0a23 205b 746f 6f6c  _NAME>]..# [tool
+00001b50: 2e64 656c 6669 6e6f 2e70 6c75 6769 6e73  .delfino.plugins
+00001b60: 2e3c 504c 5547 494e 5f4e 414d 455f 423e  .<PLUGIN_NAME_B>
+00001b70: 5d0a 2320 656e 6162 6c65 5f63 6f6d 6d61  ].# enable_comma
+00001b80: 6e64 7320 3d20 5b3c 434f 4d4d 414e 445f  nds = [<COMMAND_
+00001b90: 4e41 4d45 3e5d 0a23 2064 6973 6162 6c65  NAME>].# disable
+00001ba0: 5f63 6f6d 6d61 6e64 7320 3d20 5b3c 434f  _commands = [<CO
+00001bb0: 4d4d 414e 445f 4e41 4d45 3e5d 0a60 6060  MMAND_NAME>].```
+00001bc0: 0a0a 2320 5573 6167 650a 0a52 756e 2060  ..# Usage..Run `
+00001bd0: 6465 6c66 696e 6f20 2d2d 6865 6c70 6020  delfino --help` 
+00001be0: 746f 2073 6565 2061 6c6c 2061 7661 696c  to see all avail
+00001bf0: 6162 6c65 2063 6f6d 6d61 6e64 7320 616e  able commands an
+00001c00: 6420 7468 6569 7220 7573 6167 652e 0a0a  d their usage...
+00001c10: 2320 4465 7665 6c6f 706d 656e 740a 0a44  # Development..D
+00001c20: 656c 6669 6e6f 2069 7320 6120 7369 6d70  elfino is a simp
+00001c30: 6c65 2077 7261 7070 6572 2061 726f 756e  le wrapper aroun
+00001c40: 6420 5b43 6c69 636b 2063 6f6d 6d61 6e64  d [Click command
+00001c50: 735d 2868 7474 7073 3a2f 2f63 6c69 636b  s](https://click
+00001c60: 2e70 616c 6c65 7473 7072 6f6a 6563 7473  .palletsprojects
+00001c70: 2e63 6f6d 2f71 7569 636b 7374 6172 742f  .com/quickstart/
+00001c80: 2362 6173 6963 2d63 6f6e 6365 7074 732d  #basic-concepts-
+00001c90: 6372 6561 7469 6e67 2d61 2d63 6f6d 6d61  creating-a-comma
+00001ca0: 6e64 292e 2041 6e79 2043 6c69 636b 2063  nd). Any Click c
+00001cb0: 6f6d 6d61 6e64 2077 696c 6c20 6265 2061  ommand will be a
+00001cc0: 6363 6570 7465 6420 6279 2044 656c 6669  ccepted by Delfi
+00001cd0: 6e6f 2e0a 0a23 2320 436f 6d6d 616e 6473  no...## Commands
+00001ce0: 2064 6973 636f 7665 7279 0a0a 4465 6c66   discovery..Delf
+00001cf0: 696e 6f20 6c6f 6f6b 7320 666f 7220 616e  ino looks for an
+00001d00: 7920 5b60 636c 6963 6b2e 436f 6d6d 616e  y [`click.Comman
+00001d10: 6460 5d28 6874 7470 733a 2f2f 636c 6963  d`](https://clic
+00001d20: 6b2e 7061 6c6c 6574 7370 726f 6a65 6374  k.palletsproject
+00001d30: 732e 636f 6d2f 656e 2f38 2e30 2e78 2f61  s.com/en/8.0.x/a
+00001d40: 7069 2f23 636c 6963 6b2e 436f 6d6d 616e  pi/#click.Comman
+00001d50: 6429 2073 7562 2d63 6c61 7373 2069 6e20  d) sub-class in 
+00001d60: 7468 6520 666f 6c6c 6f77 696e 6720 6c6f  the following lo
+00001d70: 6361 7469 6f6e 733a 0a0a 2d20 6063 6f6d  cations:..- `com
+00001d80: 6d61 6e64 7360 2066 6f6c 6465 7220 696e  mands` folder in
+00001d90: 2074 6865 2072 6f6f 7420 6f66 2074 6865   the root of the
+00001da0: 2070 726f 6a65 6374 2028 6e65 7874 2074   project (next t
+00001db0: 6f20 7468 6520 6070 7970 726f 6a65 6374  o the `pyproject
+00001dc0: 2e74 6f6d 6c60 2066 696c 6529 2e20 5468  .toml` file). Th
+00001dd0: 6973 206c 6f63 6174 696f 6e20 6973 2075  is location is u
+00001de0: 7365 6675 6c20 666f 7220 636f 6d6d 616e  seful for comman
+00001df0: 6473 2074 6861 7420 646f 6e27 7420 6e65  ds that don't ne
+00001e00: 6564 2074 6f20 6265 2072 6570 6c69 6361  ed to be replica
+00001e10: 7465 6420 696e 206d 756c 7469 706c 6520  ted in multiple 
+00001e20: 6c6f 6361 7469 6f6e 732f 7072 6f6a 6563  locations/projec
+00001e30: 7473 2e0a 2d20 7079 7468 6f6e 206d 6f64  ts..- python mod
+00001e40: 756c 6520 696d 706f 7274 2070 6174 6820  ule import path 
+00001e50: 2860 3c49 4d50 4f52 545f 5041 5448 3e60  (`<IMPORT_PATH>`
+00001e60: 2920 7370 6563 6966 6965 6420 6279 2060  ) specified by `
+00001e70: 656e 7472 795f 706f 696e 7460 206f 6620  entry_point` of 
+00001e80: 5b61 2070 6c75 6769 6e5d 2823 6d69 6e69  [a plugin](#mini
+00001e90: 6d61 6c2d 706c 7567 696e 293a 0a20 2060  mal-plugin):.  `
+00001ea0: 6060 746f 6d6c 0a20 205b 746f 6f6c 2e70  ``toml.  [tool.p
+00001eb0: 6f65 7472 792e 706c 7567 696e 735d 2023  oetry.plugins] #
+00001ec0: 204f 7074 696f 6e61 6c20 7375 7065 7220   Optional super 
+00001ed0: 7461 626c 650a 0a20 205b 746f 6f6c 2e70  table..  [tool.p
+00001ee0: 6f65 7472 792e 706c 7567 696e 732e 2264  oetry.plugins."d
+00001ef0: 656c 6669 6e6f 2e70 6c75 6769 6e22 5d0a  elfino.plugin"].
+00001f00: 2020 2264 656c 6669 6e6f 2d3c 504c 5547    "delfino-<PLUG
+00001f10: 494e 5f4e 414d 453e 2220 3d20 223c 494d  IN_NAME>" = "<IM
+00001f20: 504f 5254 5f50 4154 483e 220a 2020 6060  PORT_PATH>".  ``
+00001f30: 600a 0a41 6e79 2066 696c 6573 2073 7461  `..Any files sta
+00001f40: 7274 696e 6720 7769 7468 2061 6e20 756e  rting with an un
+00001f50: 6465 7273 636f 7265 2c20 6578 6365 7074  derscore, except
+00001f60: 2066 6f72 2060 5f5f 696e 6974 5f5f 2e70   for `__init__.p
+00001f70: 7960 2c20 7769 6c6c 2062 6520 6967 6e6f  y`, will be igno
+00001f80: 7265 642e 0a0a 3e20 2a2a 5761 726e 696e  red...> **Warnin
+00001f90: 672a 2a0a 3e20 466f 6c64 6572 7320 6172  g**.> Folders ar
+00001fa0: 6520 4e4f 5420 696e 7370 6563 7465 6420  e NOT inspected 
+00001fb0: 7265 6375 7273 6976 656c 792e 2049 6620  recursively. If 
+00001fc0: 796f 7520 706c 6163 6520 616e 7920 636f  you place any co
+00001fd0: 6d6d 616e 6473 2069 6e74 6f20 6e65 7374  mmands into nest
+00001fe0: 6564 2066 6f6c 6465 7273 2c20 7468 6579  ed folders, they
+00001ff0: 2077 696c 6c20 6e6f 7420 6265 206c 6f61   will not be loa
+00002000: 6465 6420 6279 2044 656c 6669 6e6f 2e0a  ded by Delfino..
+00002010: 0a0a 2323 204d 696e 696d 616c 2063 6f6d  ..## Minimal com
+00002020: 6d61 6e64 0a0a 3c21 2d2d 2054 4f44 4f28  mand..<!-- TODO(
+00002030: 5261 6465 6b29 3a20 4465 6c66 696e 6f20  Radek): Delfino 
+00002040: 6578 7065 6374 7320 6070 7970 726f 6a65  expects `pyproje
+00002050: 6374 2e74 6f6d 6c60 2063 6f6e 6669 6775  ct.toml` configu
+00002060: 7265 642e 202d 2d3e 0a3c 212d 2d20 544f  red. -->.<!-- TO
+00002070: 444f 2852 6164 656b 293a 2044 656c 6669  DO(Radek): Delfi
+00002080: 6e6f 2065 7870 6563 7473 2050 6f65 7472  no expects Poetr
+00002090: 7920 6f72 2050 6970 656e 7620 746f 2062  y or Pipenv to b
+000020a0: 6520 6176 6169 6c61 626c 652e 202d 2d3e  e available. -->
+000020b0: 0a0a 312e 2043 7265 6174 6520 6120 6063  ..1. Create a `c
+000020c0: 6f6d 6d61 6e64 7360 2066 6f6c 6465 723a  ommands` folder:
+000020d0: 0a20 2020 6060 6073 6865 6c6c 2073 6372  .   ```shell scr
+000020e0: 6970 740a 2020 206d 6b64 6972 2063 6f6d  ipt.   mkdir com
+000020f0: 6d61 6e64 730a 2020 2060 6060 0a32 2e20  mands.   ```.2. 
+00002100: 4372 6561 7465 2061 2060 636f 6d6d 616e  Create a `comman
+00002110: 6473 2f5f 5f69 6e69 745f 5f2e 7079 6020  ds/__init__.py` 
+00002120: 6669 6c65 2c20 7769 7468 2074 6865 2066  file, with the f
+00002130: 6f6c 6c6f 7769 6e67 2063 6f6e 7465 6e74  ollowing content
+00002140: 3a0a 2020 2060 6060 7079 7468 6f6e 0a20  :.   ```python. 
+00002150: 2020 696d 706f 7274 2063 6c69 636b 0a20    import click. 
+00002160: 2020 0a20 2020 4063 6c69 636b 2e63 6f6d    .   @click.com
+00002170: 6d61 6e64 2829 0a20 2020 6465 6620 636f  mand().   def co
+00002180: 6d6d 616e 645f 7465 7374 2829 3a0a 2020  mmand_test():.  
+00002190: 2020 2020 2022 2222 5465 7374 7320 636f       """Tests co
+000021a0: 6d6d 616e 6473 2070 6c61 6365 6420 696e  mmands placed in
+000021b0: 2074 6865 2060 636f 6d6d 616e 6473 6020   the `commands` 
+000021c0: 666f 6c64 6572 2061 7265 206c 6f61 6465  folder are loade
+000021d0: 642e 2222 220a 2020 2020 2020 2070 7269  d.""".       pri
+000021e0: 6e74 2822 e29c a820 5468 6973 2063 6f6d  nt("... This com
+000021f0: 6d61 6e64 2077 6f72 6b73 2120 e29c a822  mand works! ..."
+00002200: 290a 2020 2060 6060 0a33 2e20 5365 6520  ).   ```.3. See 
+00002210: 6966 2044 656c 6669 6e6f 206c 6f61 6473  if Delfino loads
+00002220: 2074 6865 2063 6f6d 6d61 6e64 2e20 4f70   the command. Op
+00002230: 656e 2061 2074 6572 6d69 6e61 6c20 616e  en a terminal an
+00002240: 6420 696e 2074 6865 2072 6f6f 7420 6f66  d in the root of
+00002250: 2074 6865 2070 726f 6a65 6374 2c20 6361   the project, ca
+00002260: 6c6c 3a20 6064 656c 6669 6e6f 202d 2d68  ll: `delfino --h
+00002270: 656c 7060 2e20 596f 7520 7368 6f75 6c64  elp`. You should
+00002280: 2073 6565 2073 6f6d 6574 6869 6e67 206c   see something l
+00002290: 696b 6520 7468 6973 3a0a 2020 2060 6060  ike this:.   ```
+000022a0: 7465 7874 0a20 2020 5573 6167 653a 2064  text.   Usage: d
+000022b0: 656c 6669 6e6f 205b 4f50 5449 4f4e 535d  elfino [OPTIONS]
+000022c0: 2043 4f4d 4d41 4e44 205b 4152 4753 5d2e   COMMAND [ARGS].
+000022d0: 2e2e 0a20 2020 0a20 2020 4f70 7469 6f6e  ...   .   Option
+000022e0: 733a 0a20 2020 2020 2d2d 6865 6c70 2020  s:.     --help  
+000022f0: 5368 6f77 2074 6869 7320 6d65 7373 6167  Show this messag
+00002300: 6520 616e 6420 6578 6974 2e0a 2020 200a  e and exit..   .
+00002310: 2020 2043 6f6d 6d61 6e64 733a 0a20 2020     Commands:.   
+00002320: 2020 2e2e 2e0a 2020 2020 2063 6f6d 6d61    ....     comma
+00002330: 6e64 2d74 6573 7420 2020 2020 2020 2020  nd-test         
+00002340: 2020 2054 6573 7473 2063 6f6d 6d61 6e64     Tests command
+00002350: 7320 706c 6163 6564 2069 6e20 7468 6520  s placed in the 
+00002360: 6063 6f6d 6d61 6e64 7360 2066 6f6c 6465  `commands` folde
+00002370: 722e 2e2e 0a20 2020 2020 2e2e 2e0a 2020  r....     ....  
+00002380: 2060 6060 0a34 2e20 5275 6e20 7468 6520   ```.4. Run the 
+00002390: 636f 6d6d 616e 6420 7769 7468 2060 6465  command with `de
+000023a0: 6c66 696e 6f20 636f 6d6d 616e 642d 7465  lfino command-te
+000023b0: 7374 600a 0a23 2320 4d69 6e69 6d61 6c20  st`..## Minimal 
+000023c0: 706c 7567 696e 0a0a 4966 2079 6f75 2764  plugin..If you'd
+000023d0: 206c 696b 6520 746f 2075 7365 206f 6e65   like to use one
+000023e0: 206f 7220 6d6f 7265 2063 6f6d 6d61 6e64   or more command
+000023f0: 7320 696e 206d 756c 7469 706c 6520 706c  s in multiple pl
+00002400: 6163 6573 2c20 796f 7520 6361 6e20 6372  aces, you can cr
+00002410: 6561 7465 2061 2070 6c75 6769 6e2e 2041  eate a plugin. A
+00002420: 2070 6c75 6769 6e20 6973 206a 7573 7420   plugin is just 
+00002430: 6120 7265 6775 6c61 7220 5079 7468 6f6e  a regular Python
+00002440: 2070 6163 6b61 6765 2077 6974 6820 7370   package with sp
+00002450: 6563 6966 6963 2065 6e74 7279 2070 6f69  ecific entry poi
+00002460: 6e74 2074 656c 6c69 6e67 2044 656c 6669  nt telling Delfi
+00002470: 6e6f 2069 7420 7368 6f75 6c64 2075 7365  no it should use
+00002480: 2069 742e 2049 7420 6361 6e20 616c 736f   it. It can also
+00002490: 2062 6520 6469 7374 7269 6275 7465 6420   be distributed 
+000024a0: 6173 2061 6e79 206f 7468 6572 2050 7974  as any other Pyt
+000024b0: 686f 6e20 7061 636b 6167 6573 2c20 666f  hon packages, fo
+000024c0: 7220 6578 616d 706c 6520 7669 6120 5079  r example via Py
+000024d0: 7069 2e0a 0a54 6865 2071 7569 636b 6573  pi...The quickes
+000024e0: 7420 7761 7920 746f 2063 7265 6174 6520  t way to create 
+000024f0: 6f6e 6520 6973 2074 6f20 7573 6520 6120  one is to use a 
+00002500: 5b44 656c 6669 6e6f 2070 6c75 6769 6e20  [Delfino plugin 
+00002510: 636f 6f6b 6965 6375 7474 6572 2074 656d  cookiecutter tem
+00002520: 706c 6174 655d 2868 7474 7073 3a2f 2f67  plate](https://g
+00002530: 6974 6875 622e 636f 6d2f 7261 6465 6b6c  ithub.com/radekl
+00002540: 6174 2f64 656c 6669 6e6f 2d70 6c75 6769  at/delfino-plugi
+00002550: 6e2d 636f 6f6b 6965 6375 7474 6572 2d74  n-cookiecutter-t
+00002560: 656d 706c 6174 6529 2c20 7768 6963 6820  emplate), which 
+00002570: 6173 6b73 2079 6f75 2073 6576 6572 616c  asks you several
+00002580: 2071 7565 7374 696f 6e73 2061 6e64 2073   questions and s
+00002590: 6574 7320 7570 2074 6865 2077 686f 6c65  ets up the whole
+000025a0: 2070 726f 6a65 6374 2e0a 0a41 6c74 6572   project...Alter
+000025b0: 6e61 7469 7665 6c79 2c20 796f 7520 6361  natively, you ca
+000025c0: 6e20 6765 7420 696e 7370 6972 6564 2062  n get inspired b
+000025d0: 7920 5b74 6865 2064 656d 6f20 706c 7567  y [the demo plug
+000025e0: 696e 5d28 6874 7470 733a 2f2f 6769 7468  in](https://gith
+000025f0: 7562 2e63 6f6d 2f72 6164 656b 6c61 742f  ub.com/radeklat/
+00002600: 6465 6c66 696e 6f2d 6465 6d6f 2920 6f72  delfino-demo) or
+00002610: 2061 6e79 206f 6620 7468 6520 6f74 6865   any of the othe
+00002620: 7220 5b65 7869 7374 696e 6720 706c 7567  r [existing plug
+00002630: 696e 735d 2823 706c 7567 696e 7329 2e0a  ins](#plugins)..
+00002640: 0a23 2041 6476 616e 6365 6420 7573 6167  .# Advanced usag
+00002650: 650a 0a3c 212d 2d0a 2323 2041 6476 616e  e..<!--.## Advan
+00002660: 6365 6420 436f 6d6d 616e 640a 0a44 656c  ced Command..Del
+00002670: 6669 6e6f 2061 6464 7320 6f70 7469 6f6e  fino adds option
+00002680: 616c 2062 6974 7320 6f66 2066 756e 6374  al bits of funct
+00002690: 696f 6e61 6c69 7479 206f 6e20 746f 7020  ionality on top 
+000026a0: 6f66 2043 6c69 636b 2e20 5468 6520 666f  of Click. The fo
+000026b0: 6c6c 6f77 696e 6720 6578 616d 706c 6520  llowing example 
+000026c0: 6465 6d6f 6e73 7472 6174 6573 2073 6f6d  demonstrates som
+000026d0: 6520 6f66 2074 686f 7365 3a0a 0a60 6060  e of those:..```
+000026e0: 7079 7468 6f6e 0a23 2063 6f6d 6d61 6e64  python.# command
+000026f0: 732f 5f5f 696e 6974 5f5f 2e70 790a 0a69  s/__init__.py..i
+00002700: 6d70 6f72 7420 636c 6963 6b0a 0a66 726f  mport click..fro
+00002710: 6d20 6465 6c66 696e 6f2e 636f 6e74 6578  m delfino.contex
+00002720: 7473 2069 6d70 6f72 7420 7061 7373 5f61  ts import pass_a
+00002730: 7070 5f63 6f6e 7465 7874 2c20 4170 7043  pp_context, AppC
+00002740: 6f6e 7465 7874 0a66 726f 6d20 6465 6c66  ontext.from delf
+00002750: 696e 6f2e 7661 6c69 6461 7469 6f6e 2069  ino.validation i
+00002760: 6d70 6f72 7420 6173 7365 7274 5f70 6970  mport assert_pip
+00002770: 5f70 6163 6b61 6765 5f69 6e73 7461 6c6c  _package_install
+00002780: 6564 2c20 7079 7072 6f6a 6563 745f 746f  ed, pyproject_to
+00002790: 6d6c 5f6b 6579 5f6d 6973 7369 6e67 0a0a  ml_key_missing..
+000027a0: 4063 6c69 636b 2e63 6f6d 6d61 6e64 2829  @click.command()
+000027b0: 0a23 2054 6865 2060 7061 7373 5f61 7070  .# The `pass_app
+000027c0: 5f63 6f6e 7465 7874 6020 6465 636f 7261  _context` decora
+000027d0: 746f 7220 6164 6473 2060 4170 7043 6f6e  tor adds `AppCon
+000027e0: 7465 7874 6020 6173 2074 6865 2066 6972  text` as the fir
+000027f0: 7374 2070 6172 616d 6574 6572 2e0a 4070  st parameter..@p
+00002800: 6173 735f 6170 705f 636f 6e74 6578 740a  ass_app_context.
+00002810: 6465 6620 636f 6d6d 616e 645f 7465 7374  def command_test
+00002820: 2861 7070 5f63 6f6e 7465 7874 3a20 4170  (app_context: Ap
+00002830: 7043 6f6e 7465 7874 293a 0a20 2020 2222  pContext):.   ""
+00002840: 2254 6573 7473 2063 6f6d 6d61 6e64 7320  "Tests commands 
+00002850: 706c 6163 6564 2069 6e20 7468 6520 6063  placed in the `c
+00002860: 6f6d 6d61 6e64 7360 2066 6f6c 6465 7220  ommands` folder 
+00002870: 6172 6520 6c6f 6164 6564 2e22 2222 0a20  are loaded.""". 
+00002880: 2020 2320 5465 7374 206f 7074 696f 6e61    # Test optiona
+00002890: 6c20 6465 7065 6e64 656e 6369 6573 2e20  l dependencies. 
+000028a0: 416e 7920 6661 696c 696e 6720 6173 7365  Any failing asse
+000028b0: 7274 696f 6e20 7769 6c6c 2062 6520 7072  rtion will be pr
+000028c0: 696e 7465 6420 6173 3a0a 2020 2023 2043  inted as:.   # C
+000028d0: 6f6d 6d61 6e64 2027 3c4e 414d 453e 2720  ommand '<NAME>' 
+000028e0: 6973 206d 6973 636f 6e66 6967 7572 6564  is misconfigured
+000028f0: 2e20 3c41 5353 4552 5449 4f4e 2045 5252  . <ASSERTION ERR
+00002900: 4f52 204d 4553 5341 4745 3e0a 2020 2061  OR MESSAGE>.   a
+00002910: 7373 6572 745f 7069 705f 7061 636b 6167  ssert_pip_packag
+00002920: 655f 696e 7374 616c 6c65 6428 2264 656c  e_installed("del
+00002930: 6669 6e6f 2229 0a0a 2020 2023 2041 7070  fino")..   # App
+00002940: 436f 6e74 6578 7420 636f 6e74 6169 6e20  Context contain 
+00002950: 6120 7061 7273 6564 2060 7079 7072 6f6a  a parsed `pyproj
+00002960: 6563 742e 746f 6d6c 6020 6669 6c65 2e0a  ect.toml` file..
+00002970: 2020 2023 2043 6f6d 6d61 6e64 7320 6361     # Commands ca
+00002980: 6e20 6164 6420 7468 6569 7220 636f 6e66  n add their conf
+00002990: 6967 2075 6e64 6572 2060 5b74 6f6f 6c2e  ig under `[tool.
+000029a0: 6465 6c66 696e 6f2e 636f 6d6d 616e 6473  delfino.commands
+000029b0: 2e3c 434f 4d4d 414e 445f 4e41 4d45 3e5d  .<COMMAND_NAME>]
+000029c0: 602e 0a20 2020 6173 7365 7274 2022 636f  `..   assert "co
+000029d0: 6d6d 616e 645f 7465 7374 2220 696e 2061  mmand_test" in a
+000029e0: 7070 5f63 6f6e 7465 7874 2e70 7970 726f  pp_context.pypro
+000029f0: 6a65 6374 5f74 6f6d 6c2e 746f 6f6c 2e64  ject_toml.tool.d
+00002a00: 656c 6669 6e6f 2e63 6f6d 6d61 6e64 732c  elfino.commands,
+00002a10: 205c 0a20 2020 2020 2020 7079 7072 6f6a   \.       pyproj
+00002a20: 6563 745f 746f 6d6c 5f6b 6579 5f6d 6973  ect_toml_key_mis
+00002a30: 7369 6e67 2822 746f 6f6c 2e64 656c 6669  sing("tool.delfi
+00002a40: 6e6f 2e63 6f6d 6d61 6e64 732e 636f 6d6d  no.commands.comm
+00002a50: 616e 645f 7465 7374 2229 0a0a 2020 2070  and_test")..   p
+00002a60: 7269 6e74 2861 7070 5f63 6f6e 7465 7874  rint(app_context
+00002a70: 2e70 7970 726f 6a65 6374 5f74 6f6d 6c2e  .pyproject_toml.
+00002a80: 746f 6f6c 2e64 656c 6669 6e6f 2e63 6f6d  tool.delfino.com
+00002a90: 6d61 6e64 735b 2263 6f6d 6d61 6e64 2d74  mands["command-t
+00002aa0: 6573 7422 5d29 0a60 6060 0a2d 2d3e 0a0a  est"]).```.-->..
+00002ab0: 2323 2041 7574 6f2d 636f 6d70 6c65 7469  ## Auto-completi
+00002ac0: 6f6e 0a0a 596f 7520 6361 6e20 6569 7468  on..You can eith
+00002ad0: 6572 2061 7474 656d 7074 2074 6f20 696e  er attempt to in
+00002ae0: 7374 616c 6c20 636f 6d70 6c65 7469 6f6e  stall completion
+00002af0: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
+00002b00: 7769 7468 3a0a 0a60 6060 7368 656c 6c20  with:..```shell 
+00002b10: 7363 7269 7074 0a64 656c 6669 6e6f 202d  script.delfino -
+00002b20: 2d69 6e73 7461 6c6c 2d63 6f6d 706c 6574  -install-complet
+00002b30: 696f 6e0a 6060 600a 0a6f 7220 6765 6e65  ion.```..or gene
+00002b40: 7261 7465 2069 7420 7769 7468 3a0a 0a60  rate it with:..`
+00002b50: 6060 7368 656c 6c20 7363 7269 7074 0a64  ``shell script.d
+00002b60: 656c 6669 6e6f 202d 2d73 686f 772d 636f  elfino --show-co
+00002b70: 6d70 6c65 7469 6f6e 0a60 6060 0a0a 616e  mpletion.```..an
+00002b80: 6420 6d61 6e75 616c 6c79 2070 7574 2069  d manually put i
+00002b90: 7420 696e 2074 6865 2072 656c 6576 616e  t in the relevan
+00002ba0: 7420 5243 2066 696c 652e 0a0a 5468 6520  t RC file...The 
+00002bb0: 6175 746f 2d63 6f6d 706c 6574 696f 6e20  auto-completion 
+00002bc0: 696d 706c 656d 656e 7461 7469 6f6e 2069  implementation i
+00002bd0: 7320 6479 6e61 6d69 6320 736f 2074 6861  s dynamic so tha
+00002be0: 7420 6576 6572 7920 7469 6d65 2069 7420  t every time it 
+00002bf0: 6973 2069 6e76 6f6b 6564 2c20 6974 2075  is invoked, it u
+00002c00: 7365 7320 7468 6520 6375 7272 656e 7420  ses the current 
+00002c10: 7072 6f6a 6563 742e 2045 6163 6820 7072  project. Each pr
+00002c20: 6f6a 6563 7420 6361 6e20 6861 7665 2064  oject can have d
+00002c30: 6966 6665 7265 6e74 2063 6f6d 6d61 6e64  ifferent command
+00002c40: 7320 6f72 2064 6973 6162 6c65 2063 6572  s or disable cer
+00002c50: 7461 696e 2063 6f6d 6d61 6e64 7320 6974  tain commands it
+00002c60: 2064 6f65 736e 2774 2075 7365 2e20 416e   doesn't use. An
+00002c70: 6420 6479 6e61 6d69 6320 6175 746f 2d63  d dynamic auto-c
+00002c80: 6f6d 706c 6574 696f 6e20 6d61 6b65 7320  ompletion makes 
+00002c90: 7375 7265 206f 6e6c 7920 7468 6520 6375  sure only the cu
+00002ca0: 7272 656e 746c 7920 6176 6169 6c61 626c  rrently availabl
+00002cb0: 6520 636f 6d6d 616e 6473 2077 696c 6c20  e commands will 
+00002cc0: 6265 2073 7567 6765 7374 6564 2e0a 0a54  be suggested...T
+00002cd0: 6865 2064 6f77 6e73 6964 6520 6f66 2074  he downside of t
+00002ce0: 6869 7320 6170 7072 6f61 6368 2069 7320  his approach is 
+00002cf0: 7468 6174 2065 7661 6c75 6174 696e 6720  that evaluating 
+00002d00: 7768 6174 2069 7320 6176 6169 6c61 626c  what is availabl
+00002d10: 6520 6561 6368 2074 696d 6520 6973 2073  e each time is s
+00002d20: 6c6f 7765 7220 7468 616e 2061 2073 7461  lower than a sta
+00002d30: 7469 6320 6c69 7374 206f 6620 636f 6d6d  tic list of comm
+00002d40: 616e 6473 2e0a 0a23 2320 5275 6e6e 696e  ands...## Runnin
+00002d50: 6720 6578 7465 726e 616c 2070 726f 6772  g external progr
+00002d60: 616d 730a 0a49 7420 6973 2075 7020 746f  ams..It is up to
+00002d70: 2079 6f75 2068 6f77 2079 6f75 2077 616e   you how you wan
+00002d80: 7420 746f 2065 7865 6375 7465 2065 7874  t to execute ext
+00002d90: 6572 6e61 6c20 7072 6f63 6573 7365 7320  ernal processes 
+00002da0: 6173 2070 6172 7420 6f66 2063 6f6d 6d61  as part of comma
+00002db0: 6e64 7320 2869 6620 796f 7520 6e65 6564  nds (if you need
+00002dc0: 2074 6f20 6174 2061 6c6c 292e 2041 2063   to at all). A c
+00002dd0: 6f6d 6d6f 6e20 7761 7920 696e 2050 7974  ommon way in Pyt
+00002de0: 686f 6e20 6973 2074 6f20 7573 6520 6073  hon is to use `s
+00002df0: 7562 7072 6f63 6573 732e 7275 6e60 2e20  ubprocess.run`. 
+00002e00: 4465 6c66 696e 6f20 636f 6d65 7320 7769  Delfino comes wi
+00002e10: 7468 2069 7473 206f 776e 205b 6072 756e  th its own [`run
+00002e20: 6020 696d 706c 656d 656e 7461 7469 6f6e  ` implementation
+00002e30: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00002e40: 2e63 6f6d 2f72 6164 656b 6c61 742f 6465  .com/radeklat/de
+00002e50: 6c66 696e 6f2f 626c 6f62 2f6d 6169 6e2f  lfino/blob/main/
+00002e60: 7372 632f 6465 6c66 696e 6f2f 6578 6563  src/delfino/exec
+00002e70: 7574 696f 6e2e 7079 234c 3934 292c 2077  ution.py#L94), w
+00002e80: 6869 6368 2077 7261 7073 2061 6e64 2073  hich wraps and s
+00002e90: 696d 706c 6966 6965 7320 6073 7562 7072  implifies `subpr
+00002ea0: 6f63 6573 732e 7275 6e60 2066 6f72 2074  ocess.run` for t
+00002eb0: 6865 206d 6f73 7420 636f 6d6d 6f6e 2075  he most common u
+00002ec0: 7365 2063 6173 6573 3a0a 0a2d 204e 6f72  se cases:..- Nor
+00002ed0: 6d61 6c69 7a69 6e67 2060 7375 6270 726f  malizing `subpro
+00002ee0: 6365 7373 2e72 756e 6020 6172 6775 6d65  cess.run` argume
+00002ef0: 6e74 7320 2d20 796f 7520 6361 6e20 7061  nts - you can pa
+00002f00: 7373 2069 6e20 6569 7468 6572 2061 2073  ss in either a s
+00002f10: 7472 696e 6720 6f72 2061 206c 6973 742e  tring or a list.
+00002f20: 2045 6974 6865 7220 7761 792c 2060 7375   Either way, `su
+00002f30: 6270 726f 6365 7373 2e72 756e 6020 7769  bprocess.run` wi
+00002f40: 6c6c 2062 6520 6578 6563 7574 6564 2063  ll be executed c
+00002f50: 6f72 7265 6374 6c79 2e0a 2d20 4861 6e64  orrectly..- Hand
+00002f60: 6c69 6e67 2065 7272 6f72 7320 6672 6f6d  ling errors from
+00002f70: 2074 6865 2065 7865 6375 7469 6f6e 2076   the execution v
+00002f80: 6961 2074 6865 2060 6f6e 5f65 7272 6f72  ia the `on_error
+00002f90: 6020 6172 6775 6d65 6e74 2e20 4769 7669  ` argument. Givi
+00002fa0: 6e67 2074 6865 206f 7074 696f 6e20 746f  ng the option to
+00002fb0: 2065 6974 6865 7220 6967 6e6f 7265 2074   either ignore t
+00002fc0: 6865 2065 7272 6f72 7320 616e 6420 636f  he errors and co
+00002fd0: 6e74 696e 7565 2028 6050 4153 5360 292c  ntinue (`PASS`),
+00002fe0: 206e 6f74 2063 6f6e 7469 6e75 6520 616e   not continue an
+00002ff0: 6420 636c 6561 6e20 6578 6974 2028 6045  d clean exit (`E
+00003000: 5849 5460 2920 6f72 206e 6f74 2063 6f6e  XIT`) or not con
+00003010: 7469 6e75 6520 616e 6420 6162 6f72 7420  tinue and abort 
+00003020: 7769 7468 2065 7272 6f72 2063 6f64 6520  with error code 
+00003030: 2860 4142 4f52 5460 292e 0a2d 2053 6574  (`ABORT`)..- Set
+00003040: 7469 6e67 2065 6e76 6972 6f6e 6d65 6e74  ting environment
+00003050: 2076 6172 6961 626c 6573 2e0a 2d20 4c6f   variables..- Lo
+00003060: 6767 696e 6720 7768 6174 2069 7320 6265  gging what is be
+00003070: 696e 6720 6578 6563 7574 6564 2069 6e20  ing executed in 
+00003080: 7468 6520 6465 6275 6720 6c65 7665 6c2e  the debug level.
+00003090: 0a0a 4578 616d 706c 653a 0a0a 6060 6070  ..Example:..```p
+000030a0: 7974 686f 6e0a 2320 636f 6d6d 616e 6473  ython.# commands
+000030b0: 2f5f 5f69 6e69 745f 5f2e 7079 0a0a 696d  /__init__.py..im
+000030c0: 706f 7274 2063 6c69 636b 0a66 726f 6d20  port click.from 
+000030d0: 6465 6c66 696e 6f2e 6578 6563 7574 696f  delfino.executio
+000030e0: 6e20 696d 706f 7274 2072 756e 2c20 4f6e  n import run, On
+000030f0: 4572 726f 720a 0a40 636c 6963 6b2e 636f  Error..@click.co
+00003100: 6d6d 616e 6428 290a 6465 6620 7465 7374  mmand().def test
+00003110: 2829 3a0a 2020 2020 7275 6e28 2270 7974  ():.    run("pyt
+00003120: 6573 7420 7465 7374 7322 2c20 6f6e 5f65  est tests", on_e
+00003130: 7272 6f72 3d4f 6e45 7272 6f72 2e41 424f  rror=OnError.ABO
+00003140: 5254 290a 6060 600a 0a23 2320 4f70 7469  RT).```..## Opti
+00003150: 6f6e 616c 2064 6570 656e 6465 6e63 6965  onal dependencie
+00003160: 730a 0a49 6620 796f 7520 7075 7420 7365  s..If you put se
+00003170: 7665 7261 6c20 636f 6d6d 616e 6473 2069  veral commands i
+00003180: 6e74 6f20 6f6e 6520 5b70 6c75 6769 6e5d  nto one [plugin]
+00003190: 2823 706c 7567 696e 7329 2c20 796f 7520  (#plugins), you 
+000031a0: 6361 6e20 6d61 6b65 2073 6f6d 6520 6465  can make some de
+000031b0: 7065 6e64 656e 6369 6573 206f 6620 736f  pendencies of so
+000031c0: 6d65 2063 6f6d 6d61 6e64 7320 5b6f 7074  me commands [opt
+000031d0: 696f 6e61 6c5d 2868 7474 7073 3a2f 2f70  ional](https://p
+000031e0: 7974 686f 6e2d 706f 6574 7279 2e6f 7267  ython-poetry.org
+000031f0: 2f64 6f63 732f 7079 7072 6f6a 6563 7423  /docs/pyproject#
+00003200: 6578 7472 6173 292e 2054 6869 7320 6973  extras). This is
+00003210: 2075 7365 6675 6c20 7768 656e 2061 2063   useful when a c
+00003220: 6f6d 6d61 6e64 2069 7320 6e6f 7420 616c  ommand is not al
+00003230: 7761 7973 2075 7365 642c 2061 6e64 2079  ways used, and y
+00003240: 6f75 2064 6f6e 2774 2077 616e 7420 746f  ou don't want to
+00003250: 2069 6e73 7461 6c6c 2075 6e6e 6563 6573   install unneces
+00003260: 7361 7279 2064 6570 656e 6465 6e63 6965  sary dependencie
+00003270: 732e 2049 6e73 7465 6164 2c20 796f 7520  s. Instead, you 
+00003280: 6361 6e20 6368 6563 6b20 6966 2061 2064  can check if a d
+00003290: 6570 656e 6465 6e63 7920 6973 2069 6e73  ependency is ins
+000032a0: 7461 6c6c 6564 206f 6e6c 7920 7768 656e  talled only when
+000032b0: 2074 6865 2063 6f6d 6d61 6e64 2069 7320   the command is 
+000032c0: 6578 6563 7574 6564 2077 6974 6820 6064  executed with `d
+000032d0: 656c 6669 6e6f 2e76 616c 6964 6174 696f  elfino.validatio
+000032e0: 6e2e 6173 7365 7274 5f70 6970 5f70 6163  n.assert_pip_pac
+000032f0: 6b61 6765 5f69 6e73 7461 6c6c 6564 603a  kage_installed`:
+00003300: 0a0a 6060 6070 7974 686f 6e0a 2320 636f  ..```python.# co
+00003310: 6d6d 616e 6473 2f5f 5f69 6e69 745f 5f2e  mmands/__init__.
+00003320: 7079 0a0a 696d 706f 7274 2063 6c69 636b  py..import click
+00003330: 0a66 726f 6d20 6465 6c66 696e 6f2e 7661  .from delfino.va
+00003340: 6c69 6461 7469 6f6e 2069 6d70 6f72 7420  lidation import 
+00003350: 6173 7365 7274 5f70 6970 5f70 6163 6b61  assert_pip_packa
+00003360: 6765 5f69 6e73 7461 6c6c 6564 0a0a 7472  ge_installed..tr
+00003370: 793a 0a20 2020 2066 726f 6d20 6769 7420  y:.    from git 
+00003380: 696d 706f 7274 2052 6570 6f0a 6578 6365  import Repo.exce
+00003390: 7074 2049 6d70 6f72 7445 7272 6f72 3a0a  pt ImportError:.
+000033a0: 2020 2020 7061 7373 0a0a 4063 6c69 636b      pass..@click
+000033b0: 2e63 6f6d 6d61 6e64 2829 0a64 6566 2067  .command().def g
+000033c0: 6974 5f61 6374 6976 655f 6272 616e 6368  it_active_branch
+000033d0: 2829 3a0a 2020 2020 6173 7365 7274 5f70  ():.    assert_p
+000033e0: 6970 5f70 6163 6b61 6765 5f69 6e73 7461  ip_package_insta
+000033f0: 6c6c 6564 2822 6769 7470 7974 686f 6e22  lled("gitpython"
+00003400: 290a 2020 2020 7072 696e 7428 5265 706f  ).    print(Repo
+00003410: 2822 2e22 292e 6163 7469 7665 5f62 7261  (".").active_bra
+00003420: 6e63 6829 0a60 6060 0a0a 496e 2074 6865  nch).```..In the
+00003430: 2065 7861 6d70 6c65 2061 626f 7665 2c20   example above, 
+00003440: 6966 2060 6769 7470 7974 686f 6e60 2069  if `gitpython` i
+00003450: 7320 6e6f 7420 696e 7374 616c 6c65 642c  s not installed,
+00003460: 2064 656c 6669 6e6f 2077 696c 6c20 7368   delfino will sh
+00003470: 6f77 2074 6865 2063 6f6d 6d61 6e64 2062  ow the command b
+00003480: 7574 2077 696c 6c20 6661 696c 2077 6974  ut will fail wit
+00003490: 6820 7375 6767 6573 7469 6f6e 2074 6f20  h suggestion to 
+000034a0: 696e 7374 616c 6c20 6067 6974 7079 7468  install `gitpyth
+000034b0: 6f6e 6020 6f6e 6c79 2077 6865 6e20 7468  on` only when th
+000034c0: 6520 636f 6d6d 616e 6420 6973 2065 7865  e command is exe
+000034d0: 6375 7465 642e 2059 6f75 2063 616e 2061  cuted. You can a
+000034e0: 6c73 6f20 6164 6420 6067 6974 5f61 6374  lso add `git_act
+000034f0: 6976 655f 6272 616e 6368 6020 696e 746f  ive_branch` into
+00003500: 205b 6064 6973 6162 6c65 5f63 6f6d 6d61   [`disable_comma
+00003510: 6e64 7360 2063 6f6e 6669 675d 2823 656e  nds` config](#en
+00003520: 6162 6c69 6e67 6469 7361 626c 696e 672d  ablingdisabling-
+00003530: 636f 6d6d 616e 6473 2920 696e 2070 6c61  commands) in pla
+00003540: 6365 7320 7768 6572 6520 796f 7520 646f  ces where you do
+00003550: 6e27 7420 696e 7465 6e64 2074 6f20 7573  n't intend to us
+00003560: 6520 6974 2e0a 0a54 6869 7320 7761 7920  e it...This way 
+00003570: 796f 7520 6361 6e20 6772 6561 746c 7920  you can greatly 
+00003580: 7265 6475 6365 2074 6865 206e 756d 6265  reduce the numbe
+00003590: 7220 6f66 2064 6570 656e 6465 6e63 6965  r of dependencie
+000035a0: 7320 6120 706c 7567 696e 2062 7269 6e67  s a plugin bring
+000035b0: 7320 696e 746f 2061 2070 726f 6a65 6374  s into a project
+000035c0: 2077 6974 686f 7574 2061 206e 6565 6420   without a need 
+000035d0: 746f 2068 6176 6520 6d61 6e79 2073 6d61  to have many sma
+000035e0: 6c6c 2070 6c75 6769 6e73 2e0a 0a23 2320  ll plugins...## 
+000035f0: 5072 6f6a 6563 7420 7365 7474 696e 6773  Project settings
+00003600: 0a0a 596f 7520 6361 6e20 7374 6f72 6520  ..You can store 
+00003610: 616e 2061 7262 6974 7261 7279 206f 626a  an arbitrary obj
+00003620: 6563 7420 696e 2074 6865 2043 6c69 636b  ect in the Click
+00003630: 2063 6f6e 7465 7874 2061 7320 5b60 636c   context as [`cl
+00003640: 6963 6b2e 436f 6e74 6578 742e 6f62 6a60  ick.Context.obj`
+00003650: 5d28 6874 7470 733a 2f2f 636c 6963 6b2e  ](https://click.
+00003660: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
+00003670: 636f 6d2f 6170 692f 2363 6c69 636b 2e43  com/api/#click.C
+00003680: 6f6e 7465 7874 2e6f 626a 292e 2044 656c  ontext.obj). Del
+00003690: 6669 6e6f 2075 7469 6c69 7a65 7320 7468  fino utilizes th
+000036a0: 6973 206f 626a 6563 7420 746f 2073 746f  is object to sto
+000036b0: 7265 2061 6e20 696e 7374 616e 6365 206f  re an instance o
+000036c0: 6620 5b60 4170 7043 6f6e 7465 7874 605d  f [`AppContext`]
+000036d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000036e0: 636f 6d2f 7261 6465 6b6c 6174 2f64 656c  com/radeklat/del
+000036f0: 6669 6e6f 2f62 6c6f 622f 6d61 696e 2f73  fino/blob/main/s
+00003700: 7263 2f64 656c 6669 6e6f 2f6d 6f64 656c  rc/delfino/model
+00003710: 732f 6170 705f 636f 6e74 6578 742e 7079  s/app_context.py
+00003720: 292c 2077 6869 6368 2070 726f 7669 6465  ), which provide
+00003730: 7320 6163 6365 7373 2074 6f20 7072 6f6a  s access to proj
+00003740: 6563 7420 7265 6c61 7465 6420 696e 666f  ect related info
+00003750: 726d 6174 696f 6e2e 2049 6620 796f 7520  rmation. If you 
+00003760: 6e65 6564 2074 6f2c 2079 6f75 2063 616e  need to, you can
+00003770: 2073 7469 6c6c 2061 7474 6163 6820 6172   still attach ar
+00003780: 6269 7472 6172 7920 6174 7472 6962 7574  bitrary attribut
+00003790: 6573 2074 6f20 7468 6973 206f 626a 6563  es to this objec
+000037a0: 7420 6c61 7465 722e 0a0a 596f 7520 6361  t later...You ca
+000037b0: 6e20 7061 7373 2074 6869 7320 6f62 6a65  n pass this obje
+000037c0: 6374 2074 6f20 796f 7572 2063 6f6d 6d61  ct to your comma
+000037d0: 6e64 7320 6279 2064 6563 6f72 6174 696e  nds by decoratin
+000037e0: 6720 7468 656d 2077 6974 6820 5b60 636c  g them with [`cl
+000037f0: 6963 6b2e 7061 7373 5f6f 626a 605d 2868  ick.pass_obj`](h
+00003800: 7474 7073 3a2f 2f63 6c69 636b 2e70 616c  ttps://click.pal
+00003810: 6c65 7473 7072 6f6a 6563 7473 2e63 6f6d  letsprojects.com
+00003820: 2f61 7069 2f23 636c 6963 6b2e 7061 7373  /api/#click.pass
+00003830: 5f6f 626a 293a 0a0a 6060 6070 7974 686f  _obj):..```pytho
+00003840: 6e0a 2320 636f 6d6d 616e 6473 2f5f 5f69  n.# commands/__i
+00003850: 6e69 745f 5f2e 7079 0a0a 696d 706f 7274  nit__.py..import
+00003860: 2063 6c69 636b 0a66 726f 6d20 6465 6c66   click.from delf
+00003870: 696e 6f2e 6d6f 6465 6c73 2e61 7070 5f63  ino.models.app_c
+00003880: 6f6e 7465 7874 2069 6d70 6f72 7420 4170  ontext import Ap
+00003890: 7043 6f6e 7465 7874 0a0a 4063 6c69 636b  pContext..@click
+000038a0: 2e63 6f6d 6d61 6e64 2829 0a40 636c 6963  .command().@clic
+000038b0: 6b2e 7061 7373 5f6f 626a 0a64 6566 2070  k.pass_obj.def p
+000038c0: 7269 6e74 5f61 7070 5f76 6572 7369 6f6e  rint_app_version
+000038d0: 286f 626a 3a20 4170 7043 6f6e 7465 7874  (obj: AppContext
+000038e0: 293a 0a20 2020 2070 7269 6e74 286f 626a  ):.    print(obj
+000038f0: 2e70 7970 726f 6a65 6374 5f74 6f6d 6c2e  .pyproject_toml.
+00003900: 746f 6f6c 2e70 6f65 7472 792e 7665 7273  tool.poetry.vers
+00003910: 696f 6e29 0a60 6060 0a0a 2323 2050 6c75  ion).```..## Plu
+00003920: 6769 6e20 7365 7474 696e 6773 0a0a 506c  gin settings..Pl
+00003930: 7567 696e 2073 6574 7469 6e67 7320 6172  ugin settings ar
+00003940: 6520 6578 7065 6374 6564 2074 6f20 6c69  e expected to li
+00003950: 7665 2069 6e20 7468 6520 6070 7970 726f  ve in the `pypro
+00003960: 6a65 6374 2e74 6f6d 6c60 2066 696c 652e  ject.toml` file.
+00003970: 2054 6f20 7072 6576 656e 7420 6e61 6d69   To prevent nami
+00003980: 6e67 2063 6f6e 666c 6963 7473 2c20 6561  ng conflicts, ea
+00003990: 6368 2070 6c75 6769 6e20 6d75 7374 2070  ch plugin must p
+000039a0: 7574 2069 7473 2073 6574 7469 6e67 7320  ut its settings 
+000039b0: 756e 6465 7220 6074 6f6f 6c2e 6465 6c66  under `tool.delf
+000039c0: 696e 6f2e 706c 7567 696e 732e 3c50 4c55  ino.plugins.<PLU
+000039d0: 4749 4e5f 4e41 4d45 3e60 2e20 4974 2061  GIN_NAME>`. It a
+000039e0: 6c73 6f20 616c 6c6f 7773 2044 656c 6669  lso allows Delfi
+000039f0: 6e6f 2074 6f20 7061 7373 2074 6865 7365  no to pass these
+00003a00: 2073 6574 7469 6e67 7320 6469 7265 6374   settings direct
+00003a10: 6c79 2074 6f20 636f 6d6d 616e 6473 2066  ly to commands f
+00003a20: 726f 6d20 7468 6573 6520 706c 7567 696e  rom these plugin
+00003a30: 732e 0a0a 4465 6c66 696e 6f20 6c6f 6164  s...Delfino load
+00003a40: 732c 2070 6172 7365 732c 2076 616c 6964  s, parses, valid
+00003a50: 6174 6573 2061 6e64 2073 746f 7265 7320  ates and stores 
+00003a60: 706c 7567 696e 2073 6574 7469 6e67 7320  plugin settings 
+00003a70: 696e 205b 6041 7070 436f 6e74 6578 742e  in [`AppContext.
+00003a80: 706c 7567 696e 5f63 6f6e 6669 6760 5d28  plugin_config`](
+00003a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003aa0: 6f6d 2f72 6164 656b 6c61 742f 6465 6c66  om/radeklat/delf
+00003ab0: 696e 6f2f 626c 6f62 2f6d 6169 6e2f 7372  ino/blob/main/sr
+00003ac0: 632f 6465 6c66 696e 6f2f 6d6f 6465 6c73  c/delfino/models
+00003ad0: 2f61 7070 5f63 6f6e 7465 7874 2e70 7929  /app_context.py)
+00003ae0: 2e20 4966 206e 6f74 2073 7065 6369 6669  . If not specifi
+00003af0: 6564 206f 7468 6572 7769 7365 2028 7365  ed otherwise (se
+00003b00: 6520 6265 6c6f 7729 2c20 6974 2077 696c  e below), it wil
+00003b10: 6c20 6265 2061 6e20 696e 7374 616e 6365  l be an instance
+00003b20: 206f 6620 5b60 506c 7567 696e 436f 6e66   of [`PluginConf
+00003b30: 6967 605d 2868 7474 7073 3a2f 2f67 6974  ig`](https://git
+00003b40: 6875 622e 636f 6d2f 7261 6465 6b6c 6174  hub.com/radeklat
+00003b50: 2f64 656c 6669 6e6f 2f62 6c6f 622f 6d61  /delfino/blob/ma
+00003b60: 696e 2f73 7263 2f64 656c 6669 6e6f 2f6d  in/src/delfino/m
+00003b70: 6f64 656c 732f 7079 7072 6f6a 6563 745f  odels/pyproject_
+00003b80: 746f 6d6c 2e70 7929 2c20 7769 7468 2061  toml.py), with a
+00003b90: 6e79 2065 7874 7261 206b 6579 7320 756e  ny extra keys un
+00003ba0: 7661 6c69 6461 7465 6420 616e 6420 696e  validated and in
+00003bb0: 204a 534f 4e2d 6c69 6b65 2050 7974 686f   JSON-like Pytho
+00003bc0: 6e20 6f62 6a65 6374 732e 0a0a 596f 7520  n objects...You 
+00003bd0: 6361 6e20 6164 6420 6164 6469 7469 6f6e  can add addition
+00003be0: 616c 2076 616c 6964 6174 696f 6e20 746f  al validation to
+00003bf0: 2079 6f75 7220 706c 7567 696e 2073 6574   your plugin set
+00003c00: 7469 6e67 7320 6279 2073 7562 2d63 6c61  tings by sub-cla
+00003c10: 7373 696e 6720 7468 6520 6050 6c75 6769  ssing the `Plugi
+00003c20: 6e43 6f6e 6669 6760 202c 2064 6566 696e  nConfig` , defin
+00003c30: 696e 6720 6578 7065 6374 6564 206b 6579  ing expected key
+00003c40: 732c 2064 6566 6175 6c74 2076 616c 7565  s, default value
+00003c50: 7320 616e 642f 6f72 2076 616c 6964 6174  s and/or validat
+00003c60: 696f 6e2e 2044 656c 6669 6e6f 2075 7469  ion. Delfino uti
+00003c70: 6c69 7a65 7320 5b60 7079 6461 6e74 6963  lizes [`pydantic
+00003c80: 605d 2868 7474 7073 3a2f 2f64 6f63 732e  `](https://docs.
+00003c90: 7079 6461 6e74 6963 2e64 6576 2f29 2074  pydantic.dev/) t
+00003ca0: 6f20 6372 6561 7465 2064 6174 6120 636c  o create data cl
+00003cb0: 6173 7365 732e 0a0a 4465 6c66 696e 6f20  asses...Delfino 
+00003cc0: 616c 736f 206e 6565 6473 2074 6f20 6b6e  also needs to kn
+00003cd0: 6f77 2c20 7768 6963 6820 636c 6173 7320  ow, which class 
+00003ce0: 746f 2075 7365 2066 6f72 2074 6865 2076  to use for the v
+00003cf0: 616c 6964 6174 696f 6e2e 2054 6f20 646f  alidation. To do
+00003d00: 2074 6861 742c 2073 7769 7463 6820 746f   that, switch to
+00003d10: 2060 6465 6c66 696e 6f2e 6465 636f 7261   `delfino.decora
+00003d20: 746f 7273 2e70 6173 735f 6170 705f 636f  tors.pass_app_co
+00003d30: 6e74 6578 7460 2069 6e73 7465 6164 206f  ntext` instead o
+00003d40: 6620 5b60 636c 6963 6b2e 7061 7373 5f6f  f [`click.pass_o
+00003d50: 626a 605d 2868 7474 7073 3a2f 2f63 6c69  bj`](https://cli
+00003d60: 636b 2e70 616c 6c65 7473 7072 6f6a 6563  ck.palletsprojec
+00003d70: 7473 2e63 6f6d 2f61 7069 2f23 636c 6963  ts.com/api/#clic
+00003d80: 6b2e 7061 7373 5f6f 626a 293a 0a0a 6060  k.pass_obj):..``
+00003d90: 6074 6f6d 6c0a 2320 7079 7072 6f6a 6563  `toml.# pyprojec
+00003da0: 742e 746f 6d6c 0a0a 5b74 6f6f 6c2e 6465  t.toml..[tool.de
+00003db0: 6c66 696e 6f2e 706c 7567 696e 732e 6465  lfino.plugins.de
+00003dc0: 6c66 696e 6f5f 6c6f 6769 6e5f 706c 7567  lfino_login_plug
+00003dd0: 696e 5d0a 7573 6572 6e61 6d65 203d 2022  in].username = "
+00003de0: 7573 6572 220a 6060 600a 0a60 6060 7079  user".```..```py
+00003df0: 7468 6f6e 0a23 2063 6f6d 6d61 6e64 732f  thon.# commands/
+00003e00: 5f5f 696e 6974 5f5f 2e70 790a 0a69 6d70  __init__.py..imp
+00003e10: 6f72 7420 636c 6963 6b0a 6672 6f6d 2064  ort click.from d
+00003e20: 656c 6669 6e6f 2e6d 6f64 656c 732e 7079  elfino.models.py
+00003e30: 7072 6f6a 6563 745f 746f 6d6c 2069 6d70  project_toml imp
+00003e40: 6f72 7420 506c 7567 696e 436f 6e66 6967  ort PluginConfig
+00003e50: 0a66 726f 6d20 6465 6c66 696e 6f2e 6d6f  .from delfino.mo
+00003e60: 6465 6c73 2e61 7070 5f63 6f6e 7465 7874  dels.app_context
+00003e70: 2069 6d70 6f72 7420 4170 7043 6f6e 7465   import AppConte
+00003e80: 7874 0a66 726f 6d20 6465 6c66 696e 6f2e  xt.from delfino.
+00003e90: 6465 636f 7261 746f 7273 2069 6d70 6f72  decorators impor
+00003ea0: 7420 7061 7373 5f61 7070 5f63 6f6e 7465  t pass_app_conte
+00003eb0: 7874 0a0a 0a63 6c61 7373 204c 6f67 696e  xt...class Login
+00003ec0: 506c 7567 696e 436f 6e66 6967 2850 6c75  PluginConfig(Plu
+00003ed0: 6769 6e43 6f6e 6669 6729 3a0a 2020 2020  ginConfig):.    
+00003ee0: 6c6f 6769 6e3a 2073 7472 0a0a 0a40 636c  login: str...@cl
+00003ef0: 6963 6b2e 636f 6d6d 616e 6428 290a 4070  ick.command().@p
+00003f00: 6173 735f 6170 705f 636f 6e74 6578 7428  ass_app_context(
+00003f10: 4c6f 6769 6e50 6c75 6769 6e43 6f6e 6669  LoginPluginConfi
+00003f20: 6729 0a64 6566 206c 6f67 696e 2861 7070  g).def login(app
+00003f30: 5f63 6f6e 7465 7874 3a20 4170 7043 6f6e  _context: AppCon
+00003f40: 7465 7874 5b4c 6f67 696e 506c 7567 696e  text[LoginPlugin
+00003f50: 436f 6e66 6967 5d29 3a0a 2020 2020 7072  Config]):.    pr
+00003f60: 696e 7428 6170 705f 636f 6e74 6578 742e  int(app_context.
+00003f70: 706c 7567 696e 5f63 6f6e 6669 672e 6c6f  plugin_config.lo
+00003f80: 6769 6e29 0a60 6060 0a0a 5468 6520 6041  gin).```..The `A
+00003f90: 7070 436f 6e74 6578 7460 2063 6c61 7373  ppContext` class
+00003fa0: 2069 7320 6765 6e65 7269 632e 2044 6566   is generic. Def
+00003fb0: 696e 696e 6720 7468 6520 6050 6c75 6769  ining the `Plugi
+00003fc0: 6e43 6f6e 6669 6754 7970 6560 2028 7375  nConfigType` (su
+00003fd0: 6368 2061 7320 6041 7070 436f 6e74 6578  ch as `AppContex
+00003fe0: 745b 4c6f 6769 6e50 6c75 6769 6e43 6f6e  t[LoginPluginCon
+00003ff0: 6669 675d 6020 696e 2074 6865 2065 7861  fig]` in the exa
+00004000: 6d70 6c65 2061 626f 7665 2920 656e 6162  mple above) enab
+00004010: 6c65 7320 696e 7472 6f73 7065 6374 696f  les introspectio
+00004020: 6e20 616e 6420 7479 7065 2063 6865 636b  n and type check
+00004030: 732e 0a0a 2323 2050 726f 6a65 6374 2073  s...## Project s
+00004040: 7065 6369 6669 6320 6f76 6572 7269 6465  pecific override
+00004050: 730a 0a49 7420 6973 206c 696b 656c 7920  s..It is likely 
+00004060: 796f 7572 2070 726f 6a65 6374 7320 7769  your projects wi
+00004070: 6c6c 2072 6571 7569 7265 2073 6c69 6768  ll require sligh
+00004080: 7420 6469 7665 7267 656e 6365 2074 6f20  t divergence to 
+00004090: 7468 6520 6465 6661 756c 7473 2079 6f75  the defaults you
+000040a0: 2065 6e63 6f64 6520 696e 2079 6f75 7220   encode in your 
+000040b0: 7363 7269 7074 732e 2054 6865 2066 6f6c  scripts. The fol
+000040c0: 6c6f 7769 6e67 2073 6563 7469 6f6e 7320  lowing sections 
+000040d0: 636f 7665 7220 7468 6520 6d6f 7374 2063  cover the most c
+000040e0: 6f6d 6d6f 6e20 7573 6520 6361 7365 732e  ommon use cases.
+000040f0: 0a0a 2323 2320 5061 7373 2d74 6872 6f75  ..### Pass-throu
+00004100: 6768 2061 7267 756d 656e 7473 0a0a 596f  gh arguments..Yo
+00004110: 7520 6361 6e20 7061 7373 2061 6464 6974  u can pass addit
+00004120: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
+00004130: 746f 2064 6f77 6e73 7472 6561 6d20 746f  to downstream to
+00004140: 6f6c 7320 6279 2064 6563 6f72 6174 696e  ols by decoratin
+00004150: 6720 636f 6d6d 616e 6473 2077 6974 6820  g commands with 
+00004160: 7468 6520 5b60 6465 636f 7261 746f 7273  the [`decorators
+00004170: 2e70 6173 735f 6172 6773 605d 2868 7474  .pass_args`](htt
+00004180: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00004190: 7261 6465 6b6c 6174 2f64 656c 6669 6e6f  radeklat/delfino
+000041a0: 2f62 6c6f 622f 6d61 696e 2f73 7263 2f64  /blob/main/src/d
+000041b0: 656c 6669 6e6f 2f64 6563 6f72 6174 6f72  elfino/decorator
+000041c0: 732f 7061 7373 5f61 7267 732e 7079 2920  s/pass_args.py) 
+000041d0: 6465 636f 7261 746f 723a 0a0a 6060 6070  decorator:..```p
+000041e0: 7974 686f 6e0a 2320 636f 6d6d 616e 6473  ython.# commands
+000041f0: 2f5f 5f69 6e69 745f 5f2e 7079 0a0a 6672  /__init__.py..fr
+00004200: 6f6d 2074 7970 696e 6720 696d 706f 7274  om typing import
+00004210: 2054 7570 6c65 0a0a 696d 706f 7274 2063   Tuple..import c
+00004220: 6c69 636b 0a66 726f 6d20 6465 6c66 696e  lick.from delfin
+00004230: 6f2e 6465 636f 7261 746f 7273 2069 6d70  o.decorators imp
+00004240: 6f72 7420 7061 7373 5f61 7267 730a 6672  ort pass_args.fr
+00004250: 6f6d 2064 656c 6669 6e6f 2e65 7865 6375  om delfino.execu
+00004260: 7469 6f6e 2069 6d70 6f72 7420 7275 6e2c  tion import run,
+00004270: 204f 6e45 7272 6f72 0a0a 4063 6c69 636b   OnError..@click
+00004280: 2e63 6f6d 6d61 6e64 2829 0a40 7061 7373  .command().@pass
+00004290: 5f61 7267 730a 6465 6620 7465 7374 2870  _args.def test(p
+000042a0: 6173 7365 645f 6172 6773 3a20 5475 706c  assed_args: Tupl
+000042b0: 655b 7374 722c 202e 2e2e 5d29 3a0a 2020  e[str, ...]):.  
+000042c0: 2020 7275 6e28 5b22 7079 7465 7374 222c    run(["pytest",
+000042d0: 2022 7465 7374 7322 2c20 2a70 6173 7365   "tests", *passe
+000042e0: 645f 6172 6773 5d2c 206f 6e5f 6572 726f  d_args], on_erro
+000042f0: 723d 4f6e 4572 726f 722e 4142 4f52 5429  r=OnError.ABORT)
+00004300: 0a60 6060 0a0a 5468 656e 2061 6464 6974  .```..Then addit
+00004310: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
+00004320: 6361 6e20 6265 2070 6173 7365 6420 6569  can be passed ei
+00004330: 7468 6572 2076 6961 2063 6f6d 6d61 6e64  ther via command
+00004340: 206c 696e 6520 6166 7465 7220 602d 2d60   line after `--`
+00004350: 3a0a 0a60 6060 7368 656c 6c20 7363 7269  :..```shell scri
+00004360: 7074 0a64 656c 6669 6e6f 2074 6573 7420  pt.delfino test 
+00004370: 2d2d 202d 2d63 6170 7475 7265 3d6e 6f0a  -- --capture=no.
+00004380: 6060 600a 0a4f 7220 7669 6120 636f 6e66  ```..Or via conf
+00004390: 6967 7572 6174 696f 6e20 696e 2074 6865  iguration in the
+000043a0: 2060 7079 7072 6f6a 6563 742e 746f 6d6c   `pyproject.toml
+000043b0: 6020 6669 6c65 3a0a 0a60 6060 746f 6d6c  ` file:..```toml
+000043c0: 0a5b 746f 6f6c 2e64 656c 6669 6e6f 2e70  .[tool.delfino.p
+000043d0: 6c75 6769 6e73 2e3c 504c 5547 494e 3e2e  lugins.<PLUGIN>.
+000043e0: 7465 7374 5d0a 7061 7373 5f61 7267 7320  test].pass_args 
+000043f0: 3d20 5b27 2d2d 6361 7074 7572 653d 6e6f  = ['--capture=no
+00004400: 275d 0a60 6060 0a0a 4569 7468 6572 2077  '].```..Either w
+00004410: 6179 2c20 626f 7468 2077 696c 6c20 7265  ay, both will re
+00004420: 7375 6c74 2069 6e20 6578 6563 7574 696e  sult in executin
+00004430: 6720 6070 7974 6573 7420 7465 7374 7320  g `pytest tests 
+00004440: 2d2d 6361 7074 7572 653d 6e6f 602e 0a0a  --capture=no`...
+00004450: 2323 2320 4669 6c65 7320 6f76 6572 7269  ### Files overri
+00004460: 6465 0a0a 596f 7520 6361 6e20 6f76 6572  de..You can over
+00004470: 7269 6465 2066 696c 6573 2070 6173 7365  ride files passe
+00004480: 6420 746f 2064 6f77 6e73 7472 6561 6d20  d to downstream 
+00004490: 746f 6f6c 7320 6279 2064 6563 6f72 6174  tools by decorat
+000044a0: 696e 6720 636f 6d6d 616e 6473 2077 6974  ing commands wit
+000044b0: 6820 7468 6520 5b60 6465 636f 7261 746f  h the [`decorato
+000044c0: 7273 2e66 696c 6573 5f66 6f6c 6465 7273  rs.files_folders
+000044d0: 5f6f 7074 696f 6e60 5d28 6874 7470 733a  _option`](https:
+000044e0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6164  //github.com/rad
+000044f0: 656b 6c61 742f 6465 6c66 696e 6f2f 626c  eklat/delfino/bl
+00004500: 6f62 2f6d 6169 6e2f 7372 632f 6465 6c66  ob/main/src/delf
+00004510: 696e 6f2f 6465 636f 7261 746f 7273 2f66  ino/decorators/f
+00004520: 696c 6573 5f66 6f6c 6465 7273 2e70 7929  iles_folders.py)
+00004530: 2064 6563 6f72 6174 6f72 3a0a 0a60 6060   decorator:..```
+00004540: 7079 7468 6f6e 0a23 2063 6f6d 6d61 6e64  python.# command
+00004550: 732f 5f5f 696e 6974 5f5f 2e70 790a 0a66  s/__init__.py..f
+00004560: 726f 6d20 7479 7069 6e67 2069 6d70 6f72  rom typing impor
+00004570: 7420 5475 706c 650a 0a69 6d70 6f72 7420  t Tuple..import 
+00004580: 636c 6963 6b0a 6672 6f6d 2064 656c 6669  click.from delfi
+00004590: 6e6f 2e64 6563 6f72 6174 6f72 7320 696d  no.decorators im
+000045a0: 706f 7274 2066 696c 6573 5f66 6f6c 6465  port files_folde
+000045b0: 7273 5f6f 7074 696f 6e0a 6672 6f6d 2064  rs_option.from d
+000045c0: 656c 6669 6e6f 2e65 7865 6375 7469 6f6e  elfino.execution
+000045d0: 2069 6d70 6f72 7420 7275 6e2c 204f 6e45   import run, OnE
+000045e0: 7272 6f72 0a0a 4063 6c69 636b 2e63 6f6d  rror..@click.com
+000045f0: 6d61 6e64 2829 0a40 6669 6c65 735f 666f  mand().@files_fo
+00004600: 6c64 6572 735f 6f70 7469 6f6e 0a64 6566  lders_option.def
+00004610: 2074 6573 7428 6669 6c65 735f 666f 6c64   test(files_fold
+00004620: 6572 733a 2054 7570 6c65 5b73 7472 2c20  ers: Tuple[str, 
+00004630: 2e2e 2e5d 293a 0a20 2020 2069 6620 6e6f  ...]):.    if no
+00004640: 7420 6669 6c65 735f 666f 6c64 6572 733a  t files_folders:
+00004650: 0a20 2020 2020 2020 2066 696c 6573 5f66  .        files_f
+00004660: 6f6c 6465 7273 203d 2028 2274 6573 7473  olders = ("tests
+00004670: 2f75 6e69 7422 2c20 2274 6573 7473 2f69  /unit", "tests/i
+00004680: 6e74 6567 7261 7469 6f6e 2229 0a20 2020  ntegration").   
+00004690: 2072 756e 285b 2270 7974 6573 7422 2c20   run(["pytest", 
+000046a0: 2a66 696c 6573 5f66 6f6c 6465 7273 5d2c  *files_folders],
+000046b0: 206f 6e5f 6572 726f 723d 4f6e 4572 726f   on_error=OnErro
+000046c0: 722e 4142 4f52 5429 0a60 6060 0a0a 5468  r.ABORT).```..Th
+000046d0: 656e 2074 6865 2064 6566 6175 6c74 2060  en the default `
+000046e0: 2274 6573 7473 2f75 6e69 7422 2c20 2274  "tests/unit", "t
+000046f0: 6573 7473 2f69 6e74 6567 7261 7469 6f6e  ests/integration
+00004700: 2260 2066 6f6c 6465 7273 2063 616e 2062  "` folders can b
+00004710: 6520 6f76 6572 7269 6464 656e 2065 6974  e overridden eit
+00004720: 6865 7220 7669 6120 636f 6d6d 616e 6420  her via command 
+00004730: 6c69 6e65 206f 7074 696f 6e73 2060 2d66  line options `-f
+00004740: 602f 602d 2d66 696c 6560 2f60 2d2d 666f  `/`--file`/`--fo
+00004750: 6c64 6572 603a 0a0a 6060 6073 6865 6c6c  lder`:..```shell
+00004760: 2073 6372 6970 740a 6465 6c66 696e 6f20   script.delfino 
+00004770: 7465 7374 202d 6620 7465 7374 732f 6f74  test -f tests/ot
+00004780: 6865 720a 6060 600a 0a4f 7220 7669 6120  her.```..Or via 
+00004790: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
+000047a0: 2074 6865 2060 7079 7072 6f6a 6563 742e   the `pyproject.
+000047b0: 746f 6d6c 6020 6669 6c65 3a0a 0a60 6060  toml` file:..```
+000047c0: 746f 6d6c 0a5b 746f 6f6c 2e64 656c 6669  toml.[tool.delfi
+000047d0: 6e6f 2e70 6c75 6769 6e73 2e3c 504c 5547  no.plugins.<PLUG
+000047e0: 494e 3e2e 7465 7374 5d0a 6669 6c65 735f  IN>.test].files_
+000047f0: 666f 6c64 6572 7320 3d20 5b27 7465 7374  folders = ['test
+00004800: 732f 6f74 6865 7227 5d0a 6060 600a 0a45  s/other'].```..E
+00004810: 6974 6865 7220 7761 792c 2062 6f74 6820  ither way, both 
+00004820: 7769 6c6c 2072 6573 756c 7420 696e 2065  will result in e
+00004830: 7865 6375 7469 6e67 2060 7079 7465 7374  xecuting `pytest
+00004840: 2074 6573 7473 2f6f 7468 6572 602e 0a0a   tests/other`...
+00004850: 2323 2047 726f 7570 696e 6720 636f 6d6d  ## Grouping comm
+00004860: 616e 6473 0a0a 4f66 7465 6e20 6974 2069  ands..Often it i
+00004870: 7320 7573 6566 756c 2074 6f20 7275 6e20  s useful to run 
+00004880: 7365 7665 7261 6c20 636f 6d6d 616e 6473  several commands
+00004890: 2061 7320 6120 6772 6f75 7020 7769 7468   as a group with
+000048a0: 2061 2064 6966 6665 7265 6e74 2063 6f6d   a different com
+000048b0: 6d61 6e64 206e 616d 652e 2043 6c69 636b  mand name. Click
+000048c0: 2073 7570 706f 7274 7320 6361 6c6c 696e   supports callin
+000048d0: 6720 6f74 6865 7220 636f 6d6d 616e 6473  g other commands
+000048e0: 2077 6974 6820 5b60 636c 6963 6b2e 436f   with [`click.Co
+000048f0: 6e74 6578 742e 666f 7277 6172 6460 5d28  ntext.forward`](
+00004900: 6874 7470 733a 2f2f 636c 6963 6b2e 7061  https://click.pa
+00004910: 6c6c 6574 7370 726f 6a65 6374 732e 636f  lletsprojects.co
+00004920: 6d2f 6170 692f 2363 6c69 636b 2e43 6f6e  m/api/#click.Con
+00004930: 7465 7874 2e66 6f72 7761 7264 2920 6f72  text.forward) or
+00004940: 205b 6063 6c69 636b 2e43 6f6e 7465 7874   [`click.Context
+00004950: 2e69 6e76 6f6b 6560 5d28 6874 7470 733a  .invoke`](https:
+00004960: 2f2f 636c 6963 6b2e 7061 6c6c 6574 7370  //click.palletsp
+00004970: 726f 6a65 6374 732e 636f 6d2f 6170 692f  rojects.com/api/
+00004980: 2363 6c69 636b 2e43 6f6e 7465 7874 2e69  #click.Context.i
+00004990: 6e76 6f6b 6529 2e0a 0a3c 212d 2d20 544f  nvoke)...<!-- TO
+000049a0: 444f 2852 6164 656b 293a 2041 6464 2064  DO(Radek): Add d
+000049b0: 6573 6372 6970 7469 6f6e 206f 6620 6065  escription of `e
+000049c0: 7865 6375 7465 5f63 6f6d 6d61 6e64 735f  xecute_commands_
+000049d0: 6772 6f75 7060 206f 6e63 6520 6d69 6772  group` once migr
+000049e0: 6174 6564 2066 726f 6d20 6064 656c 6669  ated from `delfi
+000049f0: 6e6f 2d63 6f72 6560 2e20 2d2d 3e0a 0a    no-core`. -->..
```

