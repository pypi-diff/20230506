# Comparing `tmp/tt_terminal_translator-0.1.1.tar.gz` & `tmp/tt_terminal_translator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_terminal_translator-0.1.1.tar", max compression
+gzip compressed data, was "tt_terminal_translator-0.1.2.tar", max compression
```

## Comparing `tt_terminal_translator-0.1.1.tar` & `tt_terminal_translator-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1895 2023-04-01 04:28:41.641347 tt_terminal_translator-0.1.1/README.md
--rw-r--r--   0        0        0     1725 2023-04-14 02:59:49.209719 tt_terminal_translator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2214 2023-04-14 02:50:58.093918 tt_terminal_translator-0.1.1/src/terminal_translator/config.py
--rw-r--r--   0        0        0     2297 2023-04-14 02:58:35.636506 tt_terminal_translator-0.1.1/src/terminal_translator/main.py
--rw-r--r--   0        0        0     3070 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.1/setup.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1895 2023-05-06 02:57:49.810774 tt_terminal_translator-0.1.2/README.md
+-rw-r--r--   0        0        0     1725 2023-05-06 03:14:58.833218 tt_terminal_translator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2439 2023-05-06 03:14:32.129998 tt_terminal_translator-0.1.2/src/terminal_translator/config.py
+-rw-r--r--   0        0        0     2517 2023-05-06 03:14:41.539958 tt_terminal_translator-0.1.2/src/terminal_translator/main.py
+-rw-r--r--   0        0        0      452 2023-05-06 03:14:32.106665 tt_terminal_translator-0.1.2/src/terminal_translator/version.py
+-rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 tt_terminal_translator-0.1.2/PKG-INFO
```

### Comparing `tt_terminal_translator-0.1.1/README.md` & `tt_terminal_translator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tt_terminal_translator-0.1.1/pyproject.toml` & `tt_terminal_translator-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tt-terminal-translator"
-version = "0.1.1"
+version = "0.1.2"
 description = "Terminal Translator is a translation CLI that uses the Google Cloud API. "
 authors = ["gbPagano <guilhermebpagano@gmail.com>"]
 readme = "README.md"
 packages = [{include = "terminal_translator", from = "src"}]
 classifiers = [  
     "Environment :: Console",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `tt_terminal_translator-0.1.1/src/terminal_translator/config.py` & `tt_terminal_translator-0.1.2/src/terminal_translator/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import Path
 
 import toml
 from dynaconf import Dynaconf
 from rich.console import Console
-from typer import Argument, Typer
+from typer import Argument, Option, Typer
+
+from .version import get_version
 
 config_path = Path.home() / ".config" / "terminal_translator" / "credentials.toml"
 config_path.parent.parent.mkdir(exist_ok=True)  # create .config/
 config_path.parent.mkdir(exist_ok=True)  # create terminal_translator/
 config_path.touch()
 
 settings = Dynaconf(
@@ -23,14 +25,22 @@
 def configure_credentials(
     project_id: str = Argument(
         ..., help="Project ID of Google Cloud API", show_default=False
     ),
     google_api_credentials: str = Argument(
         ..., help="Path of the json API service key", show_default=False
     ),
+    _version: bool = Option(
+        None,
+        "--version",
+        "-V",
+        callback=get_version,
+        is_eager=True,
+        help="Display the current version.",
+    ),
 ):
     set_project_id(project_id)
     set_google_application_credentials(google_api_credentials)
 
 
 def set_project_id(credential: str) -> None:
     """Receives the project-id as a parameter and puts it in the configuration file
```

### Comparing `tt_terminal_translator-0.1.1/src/terminal_translator/main.py` & `tt_terminal_translator-0.1.2/src/terminal_translator/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pyperclip
 from google.cloud import translate
 from rich.console import Console
 from typer import Argument, Option, Typer
 
 from .config import settings
+from .version import get_version
 
 try:
     os.environ[
         "GOOGLE_APPLICATION_CREDENTIALS"
     ] = settings.google_application_credentials
     PROJECT_ID = settings.project_id
 except AttributeError:
@@ -23,24 +24,32 @@
 app = Typer(add_completion=False)
 
 
 @app.command()
 def terminal_translator(
     text: List[str] = Argument(..., help="Text to be translated", show_default=False),
     target_lang: str = Option(
-        "en-US", "--target", "-t", help="Target language text to be translated"
+        "en-US", "--target", "-t", help="Target language text to be translated."
     ),
     source_lang: str = Option(
-        "", "--source", "-s", help="Source language of text to be translated"
+        "", "--source", "-s", help="Source language of text to be translated."
     ),
     portuguese: bool = Option(
-        False, "--pt", "-p", help="Text will be translated into portuguese"
+        False, "--pt", "-p", help="Text will be translated into portuguese."
     ),
     copy: bool = Option(
-        False, "--copy", "-c", help="The output will be copied to clipboard"
+        False, "--copy", "-c", help="The output will be copied to clipboard."
+    ),
+    _version: bool = Option(
+        None,
+        "--version",
+        "-V",
+        callback=get_version,
+        is_eager=True,
+        help="Display the current version.",
     ),
 ):
     if portuguese:
         target_lang = "pt-BR"
 
     translated_text = translate_text(" ".join(text), target_lang, source_lang)
```

### Comparing `tt_terminal_translator-0.1.1/PKG-INFO` & `tt_terminal_translator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tt-terminal-translator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Terminal Translator is a translation CLI that uses the Google Cloud API. 
 Author: gbPagano
 Author-email: guilhermebpagano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

