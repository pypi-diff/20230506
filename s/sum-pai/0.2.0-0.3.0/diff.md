# Comparing `tmp/sum_pai-0.2.0.tar.gz` & `tmp/sum_pai-0.3.0.tar.gz`

## Comparing `sum_pai-0.2.0.tar` & `sum_pai-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,50 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.isort.cfg
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_all.bat
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_all.sh
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.2.0/clean_sumpai.py
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 sum_pai-0.2.0/publish.bat
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.2.0/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.2.0/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.2.0/qa.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.2.0/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.2.0/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.2.0/style.sh
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sum_pai-0.2.0/test.ipynb
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/__init__.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/__main__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/code_extractor.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/constants.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/file_io.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/loguru_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/batch.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/convert.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/create.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/length_safe.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/embedding/loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/__init__.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/classes.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/code_element.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/compare.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/directory.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/file.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/functions.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/global_level.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/process/summary_embed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/summary/__init__.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.2.0/src/sum_pai/summary/text.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.2.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.2.0/LICENSE
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 sum_pai-0.2.0/README.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sum_pai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 sum_pai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.isort.cfg
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_all.bat
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_all.sh
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.3.0/clean_sumpai.py
+-rwxr-xr-x   0        0        0      135 2020-02-02 00:00:00.000000 sum_pai-0.3.0/publish.bat
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.3.0/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.3.0/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.3.0/qa.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.3.0/run_pylint.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sum_pai-0.3.0/search_embedding_1442409337828784761.pickle
+-rw-r--r--   0        0        0    19081 2020-02-02 00:00:00.000000 sum_pai-0.3.0/ss.png
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.3.0/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.3.0/style.sh
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 sum_pai-0.3.0/test.ipynb
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/__init__.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/__main__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/code_extractor.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/constants.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/create_search_embedding.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/file_io.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/loguru_config.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/batch.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/convert.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/create.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/length_safe.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/embedding/loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/__init__.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/classes.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/code_element.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/compare.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/directory.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/file.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/functions.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/global_level.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/process/summary_embed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/knn.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/search/svm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/summary/__init__.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.3.0/src/sum_pai/summary/text.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 sum_pai-0.3.0/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 sum_pai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 sum_pai-0.3.0/PKG-INFO
```

### Comparing `sum_pai-0.2.0/.coveragerc` & `sum_pai-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/clean_sumpai.py` & `sum_pai-0.3.0/clean_sumpai.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/pylintrc` & `sum_pai-0.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/test.ipynb` & `sum_pai-0.3.0/test.ipynb`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/__main__.py` & `sum_pai-0.3.0/src/sum_pai/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,14 @@
             "Please set it to your OpenAI API key or pass the "
             "value to the --openai-api-key option."
         )
     openai.api_key = openai_api_key
     setup_logging(log_level)
     from loguru import logger
 
-    logger.info("SumPAI - v0.2.0")
+    logger.info("SumPAI - v0.3.0")
     logger.info(f"Logging is configured for {log_level} level.")
     process_directory(directory_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `sum_pai-0.2.0/src/sum_pai/code_extractor.py` & `sum_pai-0.3.0/src/sum_pai/code_extractor.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/embedding/batch.py` & `sum_pai-0.3.0/src/sum_pai/embedding/batch.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/embedding/create.py` & `sum_pai-0.3.0/src/sum_pai/embedding/create.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/embedding/length_safe.py` & `sum_pai-0.3.0/src/sum_pai/embedding/length_safe.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/embedding/loading.py` & `sum_pai-0.3.0/src/sum_pai/embedding/loading.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/classes.py` & `sum_pai-0.3.0/src/sum_pai/process/classes.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/code_element.py` & `sum_pai-0.3.0/src/sum_pai/process/code_element.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/compare.py` & `sum_pai-0.3.0/src/sum_pai/process/compare.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/directory.py` & `sum_pai-0.3.0/src/sum_pai/process/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import cityhash
 from loguru import logger
+
 from sum_pai.file_io import save_sum
 from sum_pai.process.compare import same_hash
-
 from sum_pai.process.file import process_file
 from sum_pai.process.summary_embed import summarize_and_embed
 from sum_pai.summary.text import summarize_text
 
 
 def process_directory(directory_path: str) -> None:
     """Processes all Python files within a directory and its subdirectories.
@@ -24,24 +24,26 @@
         for file in files:
             if file.endswith(".py"):
                 file_path = os.path.join(root, file)
                 file_summary = process_file(file_path)
                 if file_summary:
                     file_summaries[file_path] = file_summary
     logger.info(f"Processed {len(file_summaries)} files")
-    collated_summary = "\n".join([
-        f"{file_path}: {file_summary}\n"
-        for file_path, file_summary in file_summaries.items()
-    ])
+    collated_summary = "\n".join(
+        [
+            f"{file_path}: {file_summary}\n"
+            for file_path, file_summary in file_summaries.items()
+        ]
+    )
     logger.debug(f"Collated summary:\n{collated_summary}")
     city_hash = cityhash.CityHash64(collated_summary)
     existing_output_name = f"{directory_path}__dir_overview.sumpai"
-    if same_hash(
-        city_hash, "dir_overview", existing_output_name, path_is_full=True
-    ):
+    if same_hash(city_hash, "dir_overview", existing_output_name, path_is_full=True):
         return
     summary = summarize_text(collated_summary)
     logger.debug(f"Summary:\n{summary}")
     save_sum(
         existing_output_name,
-        summarize_and_embed(collated_summary, "directory", "dir_overview", directory_path, summary)
+        summarize_and_embed(
+            collated_summary, "directory", "dir_overview", directory_path, summary
+        ),
     )
```

### Comparing `sum_pai-0.2.0/src/sum_pai/process/file.py` & `sum_pai-0.3.0/src/sum_pai/process/file.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/functions.py` & `sum_pai-0.3.0/src/sum_pai/process/functions.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/global_level.py` & `sum_pai-0.3.0/src/sum_pai/process/global_level.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/process/summary_embed.py` & `sum_pai-0.3.0/src/sum_pai/process/summary_embed.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/src/sum_pai/summary/text.py` & `sum_pai-0.3.0/src/sum_pai/summary/text.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/.gitignore` & `sum_pai-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/LICENSE` & `sum_pai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_pai-0.2.0/README.md` & `sum_pai-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -50,7 +50,18 @@
 ```
 sum_pai <target>
 ```
 
 you can also set the logging level with LOG_LEVEL envvar or 
 
 `--log-level=DEBUG`
+
+
+### Searching
+
+There's a search embedding in the root of the project, will be used for testing.
+
+`search_project.exe --text "perform a knn search" --target src`
+
+Result:
+
+![SS](https://raw.githubusercontent.com/BillSchumacher/SumPAI/main/ss.png)
```

### Comparing `sum_pai-0.2.0/pyproject.toml` & `sum_pai-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sum-pai"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "A Python library for cataloging and searching python files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["build", "setuptools", "twine", "wheel", "openai", "loguru", "click",
- "python-dotenv", "black", "isort", "pytest", "tenacity","tiktoken", "cityhash", "numpy"]
+ "python-dotenv", "black", "isort", "pytest", "tenacity","tiktoken", "cityhash", "numpy",
+ "scikit-learn"]
 
 [project.scripts]
 sum_pai = "sum_pai.__main__:main"
+create_search_embedding = "sum_pai.create_search_embedding:main"
+search_project = "sum_pai.search_project:main"
 
 [tool.hatch.build]
 exclude = [
   "*.txt",
   ".env",
   ".env*",
   "*.env",
@@ -39,14 +42,16 @@
   "**/*.sumpai",
 ]
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel.force-include]
 "bin/sum_pai.py" = "src/sum_pai/__main__.py"
+"bin/create_search_embedding.py" = "src/sum_pai/create_search_embedding.py"
+"bin/search_project.py" = "src/sum_pai/search_project.py"
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/SumPAI"
 "Bug Tracker" = "https://github.com/BillSchumacher/SumPAI"
 
 [tool.black]
 line-length = 88
```

### Comparing `sum_pai-0.2.0/PKG-INFO` & `sum_pai-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum-pai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for cataloging and searching python files.
 Project-URL: Homepage, https://github.com/BillSchumacher/SumPAI
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/SumPAI
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 Requires-Dist: click
 Requires-Dist: isort
 Requires-Dist: loguru
 Requires-Dist: numpy
 Requires-Dist: openai
 Requires-Dist: pytest
 Requires-Dist: python-dotenv
+Requires-Dist: scikit-learn
 Requires-Dist: setuptools
 Requires-Dist: tenacity
 Requires-Dist: tiktoken
 Requires-Dist: twine
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
@@ -79,7 +80,18 @@
 ```
 sum_pai <target>
 ```
 
 you can also set the logging level with LOG_LEVEL envvar or 
 
 `--log-level=DEBUG`
+
+
+### Searching
+
+There's a search embedding in the root of the project, will be used for testing.
+
+`search_project.exe --text "perform a knn search" --target src`
+
+Result:
+
+![SS](https://raw.githubusercontent.com/BillSchumacher/SumPAI/main/ss.png)
```

