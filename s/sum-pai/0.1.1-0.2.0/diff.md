# Comparing `tmp/sum_pai-0.1.1.tar.gz` & `tmp/sum_pai-0.2.0.tar.gz`

## Comparing `sum_pai-0.1.1.tar` & `sum_pai-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.isort.cfg
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_all.bat
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_all.sh
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_sumpai.py
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 sum_pai-0.1.1/publish.bat
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.1.1/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.1.1/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.1.1/qa.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.1.1/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.1.1/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.1.1/style.sh
--rw-r--r--   0        0        0    71055 2020-02-02 00:00:00.000000 sum_pai-0.1.1/test.ipynb
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/__main__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/code_extractor.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/constants.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/file_io.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/loguru_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/batch.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/convert.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/create.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/length_safe.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/__init__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/code_element.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/compare.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/directory.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/file.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/summary_embed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/summary/__init__.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/summary/text.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.1.1/LICENSE
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sum_pai-0.1.1/README.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sum_pai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.isort.cfg
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_all.bat
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_all.sh
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_sumpai.py
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 sum_pai-0.2.0/publish.bat
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.2.0/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.2.0/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.2.0/qa.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.2.0/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.2.0/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.2.0/style.sh
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sum_pai-0.2.0/test.ipynb
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/__init__.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/__main__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/code_extractor.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/constants.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/file_io.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/loguru_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/batch.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/convert.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/create.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/length_safe.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/__init__.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/classes.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/code_element.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/compare.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/directory.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/file.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/functions.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/global_level.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/summary_embed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/summary/__init__.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/summary/text.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 sum_pai-0.2.0/README.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sum_pai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sum_pai-0.2.0/PKG-INFO
```

### Comparing `sum_pai-0.1.1/.coveragerc` & `sum_pai-0.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/clean_sumpai.py` & `sum_pai-0.2.0/clean_sumpai.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/pylintrc` & `sum_pai-0.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/__main__.py` & `sum_pai-0.2.0/src/sum_pai/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,14 @@
             "Please set it to your OpenAI API key or pass the "
             "value to the --openai-api-key option."
         )
     openai.api_key = openai_api_key
     setup_logging(log_level)
     from loguru import logger
 
-    logger.info("SumPAI - v0.0.20\n" "================\n")
+    logger.info("SumPAI - v0.2.0")
     logger.info(f"Logging is configured for {log_level} level.")
     process_directory(directory_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sum_pai-0.1.1/src/sum_pai/code_extractor.py` & `sum_pai-0.2.0/src/sum_pai/code_extractor.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/embedding/batch.py` & `sum_pai-0.2.0/src/sum_pai/embedding/batch.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/embedding/create.py` & `sum_pai-0.2.0/src/sum_pai/embedding/create.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/embedding/length_safe.py` & `sum_pai-0.2.0/src/sum_pai/embedding/length_safe.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/process/file.py` & `sum_pai-0.2.0/src/sum_pai/process/file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,47 @@
-import os
-import pickle
 from pathlib import Path
+from typing import Optional
 
 import cityhash
 
 from sum_pai.file_io import load_sum, save_sum
 from sum_pai.process.code_element import process_code_elements
+from sum_pai.process.compare import same_hash
 from sum_pai.process.summary_embed import summarize_and_embed
 from sum_pai.summary.text import summarize_text
 
 
-def process_file(file_path):
+def process_file(file_path: str) -> Optional[str]:
+    """
+    Processes a Python file, generating summaries and embeddings for its elements.
+
+    Args:
+        file_path (str): Path to the Python file.
+
+    Returns:
+        Optional[str]: Summary of the file. Returns None if the file is empty.
+    """
     with open(file_path, "r") as file:
         code = file.read()
     if not len(code):
         return
     path = Path(file_path)
 
     city_hash = cityhash.CityHash64(code)
     path_no_ext = file_path[:-3]
     existing_output_name = f"{path_no_ext}.sumpai"
-    loaded_sum = load_sum(existing_output_name)
-    if loaded_sum:
-        loaded_hash = loaded_sum["hash"]
-        if city_hash == loaded_hash:
-            return
+    if loaded_sum := same_hash(
+        city_hash, "file", existing_output_name, path_is_full=True
+    ):
+        return loaded_sum["summary"]
     code_elements = process_code_elements(code, str(path))
     summaries = [element["summary"] for element in code_elements]
     file_summary = summarize_text("\n".join(summaries))
 
     save_sum(
         existing_output_name,
         summarize_and_embed(code, "file", path.name, path_no_ext, file_summary),
     )
     for element in code_elements:
         output_name = f"{path_no_ext}__{element['name']}.sumpai"
         save_sum(output_name, element)
+    return file_summary
```

### Comparing `sum_pai-0.1.1/src/sum_pai/process/summary_embed.py` & `sum_pai-0.2.0/src/sum_pai/process/summary_embed.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/src/sum_pai/summary/text.py` & `sum_pai-0.2.0/src/sum_pai/summary/text.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/.gitignore` & `sum_pai-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/LICENSE` & `sum_pai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.1/pyproject.toml` & `sum_pai-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sum-pai"
-version = "0.1.1"
+version = "0.2.0"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "A Python library for cataloging and searching python files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

