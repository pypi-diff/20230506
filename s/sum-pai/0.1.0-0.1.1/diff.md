# Comparing `tmp/sum_pai-0.1.0.tar.gz` & `tmp/sum_pai-0.1.1.tar.gz`

## Comparing `sum_pai-0.1.0.tar` & `sum_pai-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.0/.coveragerc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.1.0/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.1.0/.flake8
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.1.0/.isort.cfg
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.1.0/clean_all.bat
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.1.0/clean_all.sh
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.1.0/clean_sumpai.py
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 sum_pai-0.1.0/publish.bat
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.1.0/pylintrc
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.1.0/qa.bat
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.1.0/qa.sh
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.1.0/run_pylint.py
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.1.0/style.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.1.0/style.sh
--rw-r--r--   0        0        0    71055 2020-02-02 00:00:00.000000 sum_pai-0.1.0/test.ipynb
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/__init__.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/__main__.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/code_extractor.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/constants.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/file_io.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/loguru_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/__init__.py
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/batch.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/convert.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/create.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/length_safe.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/embedding/loading.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/__init__.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/code_element.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/compare.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/directory.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/file.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/process/summary_embed.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/summary/__init__.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.1.0/src/sum_pai/summary/text.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.1.0/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.1.0/LICENSE
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sum_pai-0.1.0/README.md
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 sum_pai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.coveragerc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.flake8
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.isort.cfg
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_all.bat
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_all.sh
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 sum_pai-0.1.1/clean_sumpai.py
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 sum_pai-0.1.1/publish.bat
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 sum_pai-0.1.1/pylintrc
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 sum_pai-0.1.1/qa.bat
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sum_pai-0.1.1/qa.sh
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 sum_pai-0.1.1/run_pylint.py
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 sum_pai-0.1.1/style.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 sum_pai-0.1.1/style.sh
+-rw-r--r--   0        0        0    71055 2020-02-02 00:00:00.000000 sum_pai-0.1.1/test.ipynb
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/__main__.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/code_extractor.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/constants.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/file_io.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/loguru_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/__init__.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/batch.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/convert.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/create.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/length_safe.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/embedding/loading.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/__init__.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/code_element.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/compare.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/directory.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/file.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/process/summary_embed.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/summary/__init__.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 sum_pai-0.1.1/src/sum_pai/summary/text.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 sum_pai-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 sum_pai-0.1.1/LICENSE
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 sum_pai-0.1.1/README.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 sum_pai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sum_pai-0.1.1/PKG-INFO
```

### Comparing `sum_pai-0.1.0/.coveragerc` & `sum_pai-0.1.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/clean_sumpai.py` & `sum_pai-0.1.1/clean_sumpai.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/pylintrc` & `sum_pai-0.1.1/pylintrc`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/test.ipynb` & `sum_pai-0.1.1/test.ipynb`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/__main__.py` & `sum_pai-0.1.1/src/sum_pai/__main__.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/code_extractor.py` & `sum_pai-0.1.1/src/sum_pai/code_extractor.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/embedding/batch.py` & `sum_pai-0.1.1/src/sum_pai/embedding/batch.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/embedding/create.py` & `sum_pai-0.1.1/src/sum_pai/embedding/create.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/embedding/length_safe.py` & `sum_pai-0.1.1/src/sum_pai/embedding/length_safe.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/embedding/loading.py` & `sum_pai-0.1.1/src/sum_pai/embedding/loading.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/process/code_element.py` & `sum_pai-0.1.1/src/sum_pai/process/code_element.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/process/directory.py` & `sum_pai-0.1.1/src/sum_pai/process/directory.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/process/file.py` & `sum_pai-0.1.1/src/sum_pai/process/file.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/process/summary_embed.py` & `sum_pai-0.1.1/src/sum_pai/process/summary_embed.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/src/sum_pai/summary/text.py` & `sum_pai-0.1.1/src/sum_pai/summary/text.py`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/.gitignore` & `sum_pai-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/LICENSE` & `sum_pai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sum_pai-0.1.0/pyproject.toml` & `sum_pai-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sum-pai"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "A Python library for cataloging and searching python files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -16,15 +16,16 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["build", "setuptools", "twine", "wheel", "openai", "loguru", "click",
  "python-dotenv", "black", "isort", "pytest", "tenacity","tiktoken", "cityhash", "numpy"]
 
 [project.scripts]
-athena = "sum_pai.__main__:main"
+sum_pai = "sum_pai.__main__:main"
+
 [tool.hatch.build]
 exclude = [
   "*.txt",
   ".env",
   ".env*",
   "*.env",
   "*venv*",
@@ -37,15 +38,15 @@
   "**/node_modules/*",
   "**/*.sumpai",
 ]
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel.force-include]
-"bin/sum_pai.py" = "sum_pai/__main__.py"
+"bin/sum_pai.py" = "src/sum_pai/__main__.py"
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/SumPAI"
 "Bug Tracker" = "https://github.com/BillSchumacher/SumPAI"
 
 [tool.black]
 line-length = 88
```

### Comparing `sum_pai-0.1.0/PKG-INFO` & `sum_pai-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sum-pai
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for cataloging and searching python files.
 Project-URL: Homepage, https://github.com/BillSchumacher/SumPAI
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/SumPAI
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

